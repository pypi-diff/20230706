# Comparing `tmp/preset-cli-0.2.1.tar.gz` & `tmp/preset-cli-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preset-cli-0.2.1.tar", last modified: Wed May 31 02:14:06 2023, max compression
+gzip compressed data, was "preset-cli-0.2.2.tar", last modified: Wed Jul  5 22:23:30 2023, max compression
```

## Comparing `preset-cli-0.2.1.tar` & `preset-cli-0.2.2.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.775785 preset-cli-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.751784 preset-cli-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.759784 preset-cli-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.github/workflows/python-package-daily.yml
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-31 02:13:53.000000 preset-cli-0.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-31 02:13:53.000000 preset-cli-0.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-31 02:13:53.000000 preset-cli-0.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-05-31 02:13:53.000000 preset-cli-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-31 02:13:53.000000 preset-cli-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-31 02:13:53.000000 preset-cli-0.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    24095 2023-05-31 02:14:06.775785 preset-cli-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23284 2023-05-31 02:13:53.000000 preset-cli-0.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 02:13:53.000000 preset-cli-0.2.1/dev-requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-31 02:13:53.000000 preset-cli-0.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.759784 preset-cli-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.759784 preset-cli-0.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   271378 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/images/export_dashboards.png
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-31 02:13:53.000000 preset-cli-0.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.751784 preset-cli-0.2.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/examples/exports/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/examples/exports/charts/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-31 02:13:53.000000 preset-cli-0.2.1/examples/exports/charts/Total_count_134.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/examples/exports/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-31 02:13:53.000000 preset-cli-0.2.1/examples/exports/dashboards/White_label_test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/examples/exports/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-31 02:13:53.000000 preset-cli-0.2.1/examples/exports/databases/Google_Sheets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.751784 preset-cli-0.2.1/examples/exports/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/examples/exports/datasets/Google_Sheets/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-31 02:13:53.000000 preset-cli-0.2.1/examples/exports/datasets/Google_Sheets/country_cnt.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/examples/exports/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-31 02:13:53.000000 preset-cli-0.2.1/examples/exports/functions/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 02:13:53.000000 preset-cli-0.2.1/examples/exports/metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-31 02:13:53.000000 preset-cli-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 02:13:53.000000 preset-cli-0.2.1/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-31 02:13:53.000000 preset-cli-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-31 02:14:06.779785 preset-cli-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-31 02:13:53.000000 preset-cli-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.755784 preset-cli-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/src/preset_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/src/preset_cli/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.767785 preset-cli-0.2.1/src/preset_cli/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20169 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/api/clients/dbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/api/clients/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)    35569 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/api/clients/superset.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/api/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.767785 preset-cli-0.2.1/src/preset_cli/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/auth/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/auth/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/auth/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/auth/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/auth/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.767785 preset-cli-0.2.1/src/preset_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.767785 preset-cli-0.2.1/src/preset_cli/cli/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.767785 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.771785 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/exposures.py
--rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.771785 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/cli/superset/sync/native/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-31 02:13:53.000000 preset-cli-0.2.1/src/preset_cli/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.763785 preset-cli-0.2.1/src/preset_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24095 2023-05-31 02:14:06.000000 preset-cli-0.2.1/src/preset_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-31 02:14:06.000000 preset-cli-0.2.1/src/preset_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 02:14:06.000000 preset-cli-0.2.1/src/preset_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-31 02:14:06.000000 preset-cli-0.2.1/src/preset_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 02:14:06.000000 preset-cli-0.2.1/src/preset_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-31 02:14:06.000000 preset-cli-0.2.1/src/preset_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 02:14:06.000000 preset-cli-0.2.1/src/preset_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.771785 preset-cli-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.771785 preset-cli-0.2.1/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.771785 preset-cli-0.2.1/tests/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47038 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/api/clients/dbt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/api/clients/preset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    90501 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/api/clients/superset_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.771785 preset-cli-0.2.1/tests/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/auth/jwt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/auth/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/auth/main_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/auth/password_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/auth/preset_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.775785 preset-cli-0.2.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52383 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.775785 preset-cli-0.2.1/tests/cli/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/export_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/import_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/main_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sql_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.775785 preset-cli-0.2.1/tests/cli/superset/sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.775785 preset-cli-0.2.1/tests/cli/superset/sync/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32583 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/dbt/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/dbt/databases_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/dbt/datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23913 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/dbt/exposures_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/dbt/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/dbt/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/dbt/metrics_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:14:06.775785 preset-cli-0.2.1/tests/cli/superset/sync/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26997 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/cli/superset/sync/native/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tests/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-31 02:13:53.000000 preset-cli-0.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.719186 preset-cli-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.691186 preset-cli-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.695186 preset-cli-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.github/workflows/python-package-daily.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-05 22:23:19.000000 preset-cli-0.2.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-05 22:23:19.000000 preset-cli-0.2.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-07-05 22:23:19.000000 preset-cli-0.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-05 22:23:19.000000 preset-cli-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-05 22:23:19.000000 preset-cli-0.2.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-07-05 22:23:30.719186 preset-cli-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24105 2023-07-05 22:23:19.000000 preset-cli-0.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 22:23:19.000000 preset-cli-0.2.2/dev-requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-05 22:23:19.000000 preset-cli-0.2.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   271378 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/images/export_dashboards.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.691186 preset-cli-0.2.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/examples/exports/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/examples/exports/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-05 22:23:19.000000 preset-cli-0.2.2/examples/exports/charts/Total_count_134.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/examples/exports/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-05 22:23:19.000000 preset-cli-0.2.2/examples/exports/dashboards/White_label_test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/examples/exports/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-05 22:23:19.000000 preset-cli-0.2.2/examples/exports/databases/Google_Sheets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.691186 preset-cli-0.2.2/examples/exports/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/examples/exports/datasets/Google_Sheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-05 22:23:19.000000 preset-cli-0.2.2/examples/exports/datasets/Google_Sheets/country_cnt.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/examples/exports/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-05 22:23:19.000000 preset-cli-0.2.2/examples/exports/functions/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 22:23:19.000000 preset-cli-0.2.2/examples/exports/metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-05 22:23:19.000000 preset-cli-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 22:23:19.000000 preset-cli-0.2.2/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-05 22:23:19.000000 preset-cli-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-05 22:23:30.719186 preset-cli-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-05 22:23:19.000000 preset-cli-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.691186 preset-cli-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.703186 preset-cli-0.2.2/src/preset_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.703186 preset-cli-0.2.2/src/preset_cli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.703186 preset-cli-0.2.2/src/preset_cli/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20169 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/api/clients/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/api/clients/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35569 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/api/clients/superset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/api/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.703186 preset-cli-0.2.2/src/preset_cli/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/auth/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/auth/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/auth/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/auth/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/auth/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.703186 preset-cli-0.2.2/src/preset_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.707186 preset-cli-0.2.2/src/preset_cli/cli/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.707186 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.707186 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/exposures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.707186 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/native/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.703186 preset-cli-0.2.2/src/preset_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-07-05 22:23:30.000000 preset-cli-0.2.2/src/preset_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-05 22:23:30.000000 preset-cli-0.2.2/src/preset_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:23:30.000000 preset-cli-0.2.2/src/preset_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-05 22:23:30.000000 preset-cli-0.2.2/src/preset_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:23:30.000000 preset-cli-0.2.2/src/preset_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-05 22:23:30.000000 preset-cli-0.2.2/src/preset_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 22:23:30.000000 preset-cli-0.2.2/src/preset_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.711186 preset-cli-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.711186 preset-cli-0.2.2/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.711186 preset-cli-0.2.2/tests/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47038 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/api/clients/dbt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/api/clients/preset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90501 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/api/clients/superset_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.711186 preset-cli-0.2.2/tests/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/auth/jwt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/auth/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/auth/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/auth/password_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/auth/preset_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.711186 preset-cli-0.2.2/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52383 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.715186 preset-cli-0.2.2/tests/cli/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/export_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/import_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sql_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.715186 preset-cli-0.2.2/tests/cli/superset/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.715186 preset-cli-0.2.2/tests/cli/superset/sync/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/dbt/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/dbt/databases_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34788 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/dbt/datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28144 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/dbt/exposures_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/dbt/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/dbt/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/dbt/metrics_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.715186 preset-cli-0.2.2/tests/cli/superset/sync/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26997 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/native/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tox.ini
```

### Comparing `preset-cli-0.2.1/.coveragerc` & `preset-cli-0.2.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/.github/workflows/python-package-daily.yml` & `preset-cli-0.2.2/.github/workflows/python-package-daily.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/.github/workflows/python-package.yml` & `preset-cli-0.2.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/.github/workflows/python-publish.yml` & `preset-cli-0.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/.gitignore` & `preset-cli-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/.pre-commit-config.yaml` & `preset-cli-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/CHANGELOG.rst` & `preset-cli-0.2.2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
 Changelog
 =========
 
+Version 0.2.2 - 2023-07-05
+==========================
+
+- ``certification`` and additional ``extra`` information is now synced from dbt models (`#213 <https://github.com/preset-io/backend-sdk/pull/213>`_ and `#215 <https://github.com/preset-io/backend-sdk/pull/215>`_).
+- Improved the ``exposures`` sync (`#221 <https://github.com/preset-io/backend-sdk/pull/221>`_).
+- The ``--preserve-columns`` flag can now be used to preserve ``groupby`` and ``filterable`` values for existing columns during a dbt sync (`#221 <https://github.com/preset-io/backend-sdk/pull/221>`_).
+- The search for roles during the ``sync roles`` command now uses ``Equals`` comparison, instead of ``Starts with`` (`#222 <https://github.com/preset-io/backend-sdk/pull/222>`_).
+
 Version 0.2.1 - 2023-05-30
 ==========================
 
 - Fix for https://github.com/apache/superset/pull/24067 (`#211 <https://github.com/preset-io/backend-sdk/pull/211>`_).
 
 Version 0.2.0 - 2023-05-23
 ==========================
```

### Comparing `preset-cli-0.2.1/CONTRIBUTING.rst` & `preset-cli-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/Makefile` & `preset-cli-0.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/PKG-INFO` & `preset-cli-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preset-cli
-Version: 0.2.1
+Version: 0.2.2
 Summary: A CLI to interact with Preset (https://preset.io/) workspaces.
 Home-page: https://github.com/preset-io/backend-sdk
 Author: Beto Dealmeida
 Author-email: beto@preset.io
 License: Other/Proprietary License
 Project-URL: Documentation, https://github.com/preset-io/backend-sdk/blob/master/README.rst
 Platform: any
@@ -381,14 +381,39 @@
 
 1. Read the dbt profile and create the ``$target`` database for the specified project in the Preset workspace.
 2. Every source in the project will be created as a dataset in the Preset workspace.
 3. Every model in the project will be created as a dataset in the Preset workspace.
 4. Any `metrics <https://docs.getdbt.com/docs/building-a-dbt-project/metrics>`_ will be added to the corresponding datasets.
 5. Every dashboard built on top of the dbt sources and/or models will be synchronized back to dbt as an `exposure <https://docs.getdbt.com/docs/building-a-dbt-project/exposures>`_.
 
+Descriptions, labels and other metadata is also synced from dbt models to the corresponding fields in the dataset. It's also possible to specify values for Superset-only fields directly in the model definition, under ``model.meta.superset.{{field_name}}``. For example, to specify the cache timeout for a dataset:
+
+.. code-block:: yaml
+
+    models:
+      - name: my_dbt_model
+        meta:
+          superset:
+            cache_timeout: 250 # Setting the dataset cache timeout to 250. 
+
+The same is applied for metrics. For example, to specify the d3 format for a metric:
+
+.. code-block:: yaml
+
+    - name: avg_revenue
+      label: "AVG Revenue"
+      model: ref('my_dbt_model')
+      calculation_method: average
+      expression: price_each
+      timestamp: date
+      meta:
+        superset:
+          d3format: '%d'
+
+
 The ``--external-url-prefix`` should point to your dbt docs, so that the resources in the workspace can point to the source of truth where they are being managed. Similar to the native sync, the dbt sync also supports the ``--disallow-edits`` flag.
 
 By default, the CLI sync would create a new database on the destination workspace using below name structure:
 
 .. code-block:: python
 
     f"{project_name}_{target_name}"
```

### Comparing `preset-cli-0.2.1/README.rst` & `preset-cli-0.2.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -360,14 +360,39 @@
 
 1. Read the dbt profile and create the ``$target`` database for the specified project in the Preset workspace.
 2. Every source in the project will be created as a dataset in the Preset workspace.
 3. Every model in the project will be created as a dataset in the Preset workspace.
 4. Any `metrics <https://docs.getdbt.com/docs/building-a-dbt-project/metrics>`_ will be added to the corresponding datasets.
 5. Every dashboard built on top of the dbt sources and/or models will be synchronized back to dbt as an `exposure <https://docs.getdbt.com/docs/building-a-dbt-project/exposures>`_.
 
+Descriptions, labels and other metadata is also synced from dbt models to the corresponding fields in the dataset. It's also possible to specify values for Superset-only fields directly in the model definition, under ``model.meta.superset.{{field_name}}``. For example, to specify the cache timeout for a dataset:
+
+.. code-block:: yaml
+
+    models:
+      - name: my_dbt_model
+        meta:
+          superset:
+            cache_timeout: 250 # Setting the dataset cache timeout to 250. 
+
+The same is applied for metrics. For example, to specify the d3 format for a metric:
+
+.. code-block:: yaml
+
+    - name: avg_revenue
+      label: "AVG Revenue"
+      model: ref('my_dbt_model')
+      calculation_method: average
+      expression: price_each
+      timestamp: date
+      meta:
+        superset:
+          d3format: '%d'
+
+
 The ``--external-url-prefix`` should point to your dbt docs, so that the resources in the workspace can point to the source of truth where they are being managed. Similar to the native sync, the dbt sync also supports the ``--disallow-edits`` flag.
 
 By default, the CLI sync would create a new database on the destination workspace using below name structure:
 
 .. code-block:: python
 
     f"{project_name}_{target_name}"
```

### Comparing `preset-cli-0.2.1/dev-requirements.txt` & `preset-cli-0.2.2/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/docs/Makefile` & `preset-cli-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/docs/conf.py` & `preset-cli-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/docs/images/export_dashboards.png` & `preset-cli-0.2.2/docs/images/export_dashboards.png`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/docs/index.rst` & `preset-cli-0.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/examples/exports/charts/Total_count_134.yaml` & `preset-cli-0.2.2/examples/exports/charts/Total_count_134.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/examples/exports/dashboards/White_label_test.yaml` & `preset-cli-0.2.2/examples/exports/dashboards/White_label_test.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/examples/exports/datasets/Google_Sheets/country_cnt.yaml` & `preset-cli-0.2.2/examples/exports/datasets/Google_Sheets/country_cnt.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/requirements.txt` & `preset-cli-0.2.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/setup.cfg` & `preset-cli-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/setup.py` & `preset-cli-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/api/clients/dbt.py` & `preset-cli-0.2.2/src/preset_cli/api/clients/dbt.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/api/clients/preset.py` & `preset-cli-0.2.2/src/preset_cli/api/clients/preset.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/api/clients/superset.py` & `preset-cli-0.2.2/src/preset_cli/api/clients/superset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1002,15 +1002,15 @@
             if "selected" in option.attrs
         ]
 
     def get_role_id(self, role_name: str) -> int:
         """
         Return the ID of a given role.
         """
-        params = {"_flt_0_name": role_name}
+        params = {"_flt_3_name": role_name}
         url = self.baseurl / "roles/list/"
         _logger.debug("GET %s", url % params)
         response = self.session.get(url, params=params)
 
         soup = BeautifulSoup(response.text, features="html.parser")
         tables = soup.find_all("table")
         if len(tables) < 2:
```

### Comparing `preset-cli-0.2.1/src/preset_cli/auth/jwt.py` & `preset-cli-0.2.2/src/preset_cli/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/auth/lib.py` & `preset-cli-0.2.2/src/preset_cli/auth/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/auth/main.py` & `preset-cli-0.2.2/src/preset_cli/auth/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/auth/password.py` & `preset-cli-0.2.2/src/preset_cli/auth/password.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/auth/preset.py` & `preset-cli-0.2.2/src/preset_cli/auth/preset.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/cli/main.py` & `preset-cli-0.2.2/src/preset_cli/cli/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/cli/superset/export.py` & `preset-cli-0.2.2/src/preset_cli/cli/superset/export.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/cli/superset/import_.py` & `preset-cli-0.2.2/src/preset_cli/cli/superset/import_.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/cli/superset/main.py` & `preset-cli-0.2.2/src/preset_cli/cli/superset/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/cli/superset/sql.py` & `preset-cli-0.2.2/src/preset_cli/cli/superset/sql.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/command.py` & `preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,36 +63,45 @@
 )
 @click.option(
     "--exposures-only",
     is_flag=True,
     default=False,
     help="Do not sync models to datasets and only fetch exposures instead",
 )
+@click.option(
+    "--preserve-columns",
+    is_flag=True,
+    default=False,
+    help="Preserve column configurations",
+)
 @click.pass_context
 def dbt_core(  # pylint: disable=too-many-arguments, too-many-locals
     ctx: click.core.Context,
     file: str,
     project: Optional[str],
     target: Optional[str],
     select: Tuple[str, ...],
     exclude: Tuple[str, ...],
     profiles: Optional[str] = None,
     exposures: Optional[str] = None,
     import_db: bool = False,
     disallow_edits: bool = True,
     external_url_prefix: str = "",
     exposures_only: bool = False,
+    preserve_columns: bool = False,
 ) -> None:
     """
     Sync models/metrics from dbt Core to Superset and charts/dashboards to dbt exposures.
     """
     auth = ctx.obj["AUTH"]
     url = URL(ctx.obj["INSTANCE"])
     client = SupersetClient(url, auth)
 
+    reload_columns = not preserve_columns
+
     if profiles is None:
         profiles = os.path.expanduser("~/.dbt/profiles.yml")
 
     file_path = Path(file)
     if file_path.name == "manifest.json":
         warnings.warn(
             (
@@ -130,15 +139,15 @@
             # conform to the same schema that dbt Cloud uses for models
             unique_id = config["uniqueId"] = config["unique_id"]
             config["children"] = configs["child_map"][unique_id]
             config["columns"] = list(config["columns"].values())
             models.append(model_schema.load(config))
     models = apply_select(models, select, exclude)
     model_map = {
-        ModelKey(model["schema"], model["name"]): f'ref({model["name"]})'
+        ModelKey(model["schema"], model["name"]): f"ref('{model['name']}')"
         for model in models
     }
 
     if exposures_only:
         datasets = [
             dataset
             for dataset in client.get_datasets()
@@ -171,14 +180,15 @@
         datasets = sync_datasets(
             client,
             models,
             metrics,
             database,
             disallow_edits,
             external_url_prefix,
+            reload_columns=reload_columns,
         )
 
     if exposures:
         exposures = os.path.expanduser(exposures)
         sync_exposures(client, Path(exposures), datasets, model_map)
 
 
@@ -296,36 +306,45 @@
 )
 @click.option(
     "--exposures-only",
     is_flag=True,
     default=False,
     help="Do not sync models to datasets and only fetch exposures instead",
 )
+@click.option(
+    "--preserve-columns",
+    is_flag=True,
+    default=False,
+    help="Preserve column configurations",
+)
 @click.pass_context
 def dbt_cloud(  # pylint: disable=too-many-arguments, too-many-locals
     ctx: click.core.Context,
     token: str,
     select: Tuple[str, ...],
     exclude: Tuple[str, ...],
     exposures: Optional[str] = None,
     job_id: Optional[int] = None,
     disallow_edits: bool = True,
     external_url_prefix: str = "",
     exposures_only: bool = False,
+    preserve_columns: bool = False,
 ) -> None:
     """
     Sync models/metrics from dbt Cloud to Superset.
     """
     superset_auth = ctx.obj["AUTH"]
     url = URL(ctx.obj["INSTANCE"])
     superset_client = SupersetClient(url, superset_auth)
 
     dbt_auth = TokenAuth(token)
     dbt_client = DBTClient(dbt_auth)
 
+    reload_columns = not preserve_columns
+
     if job_id is None:
         job_id = get_job_id(dbt_client)
 
     # with dbt cloud the database must already exist
     database_name = dbt_client.get_database_name(job_id)
     databases = superset_client.get_databases(database_name=database_name)
     if not databases:
@@ -336,15 +355,15 @@
 
     # need to get the database by itself so the response has the SQLAlchemy URI
     database = superset_client.get_database(databases[0]["id"])
 
     models = dbt_client.get_models(job_id)
     models = apply_select(models, select, exclude)
     model_map = {
-        ModelKey(model["schema"], model["name"]): f'ref({model["name"]})'
+        ModelKey(model["schema"], model["name"]): f"ref('{model['name']}')"
         for model in models
     }
     metrics = dbt_client.get_metrics(job_id)
 
     if exposures_only:
         datasets = [
             dataset
@@ -355,12 +374,13 @@
         datasets = sync_datasets(
             superset_client,
             models,
             metrics,
             database,
             disallow_edits,
             external_url_prefix,
+            reload_columns=reload_columns,
         )
 
     if exposures:
         exposures = os.path.expanduser(exposures)
         sync_exposures(superset_client, Path(exposures), datasets, model_map)
```

### Comparing `preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/databases.py` & `preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/databases.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/datasets.py` & `preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/datasets.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from preset_cli.api.clients.superset import SupersetClient
 from preset_cli.api.operators import OneToMany
 from preset_cli.cli.superset.sync.dbt.metrics import (
     get_metric_expression,
     get_metrics_for_model,
 )
 
+DEFAULT_CERTIFICATION = {"details": "This table is produced by dbt"}
+
 _logger = logging.getLogger(__name__)
 
 
 def model_in_database(model: ModelSchema, url: SQLAlchemyURL) -> bool:
     """
     Return if a model is in the same database as a SQLAlchemy URI.
     """
@@ -62,31 +64,43 @@
             "table_name": model.get("alias") or model["name"],
             "sql": f"SELECT * FROM {source}",
         }
 
     return client.create_dataset(**kwargs)
 
 
-def sync_datasets(  # pylint: disable=too-many-locals, too-many-branches, too-many-arguments
+def sync_datasets(  # pylint: disable=too-many-locals, too-many-branches, too-many-arguments, too-many-statements
     client: SupersetClient,
     models: List[ModelSchema],
     metrics: List[MetricSchema],
     database: Any,
     disallow_edits: bool,
     external_url_prefix: str,
     certification: Optional[Dict[str, Any]] = None,
+    reload_columns: bool = True,
 ) -> List[Any]:
     """
     Read the dbt manifest and import models as datasets with metrics.
     """
     base_url = URL(external_url_prefix) if external_url_prefix else None
 
     # add datasets
     datasets = []
     for model in models:
+
+        # load additional metadata from dbt model definition
+        model_kwargs = model.get("meta", {}).pop("superset", {})
+
+        try:
+            certification_details = model_kwargs["extra"].pop("certification")
+        except KeyError:
+            certification_details = certification or DEFAULT_CERTIFICATION
+
+        certification_info = {"certification": certification_details}
+
         filters = {
             "database": OneToMany(database["id"]),
             "schema": model["schema"],
             "table_name": model.get("alias") or model["name"],
         }
         existing = client.get_datasets(**filters)
         if len(existing) > 1:
@@ -102,16 +116,23 @@
             except Exception:  # pylint: disable=broad-except
                 _logger.exception("Unable to create dataset")
                 continue
 
         extra = {
             "unique_id": model["unique_id"],
             "depends_on": "ref('{name}')".format(**model),
-            "certification": certification
-            or {"details": "This table is produced by dbt"},
+            **(
+                certification_info
+                if certification_info["certification"] is not None
+                else {}
+            ),
+            **model_kwargs.pop(
+                "extra",
+                {},
+            ),  # include any additional or custom field specified in model.meta.superset.extra
         }
 
         dataset_metrics = []
         model_metrics = {
             metric["name"]: metric for metric in get_metrics_for_model(model, metrics)
         }
         for name, metric in model_metrics.items():
@@ -124,30 +145,30 @@
                     "metric_type": (
                         metric.get("type")  # dbt < 1.3
                         or metric.get("calculation_method")  # dbt >= 1.3
                     ),
                     "verbose_name": metric.get("label", name),
                     "description": metric.get("description", ""),
                     "extra": json.dumps(meta),
-                    **kwargs,
+                    **kwargs,  # include additional metric metadata defined in metric.meta.superset
                 },
             )
 
-        # update dataset clearing metrics...
+        # update dataset metadata from dbt and clearing metrics
         update = {
             "description": model.get("description", ""),
             "extra": json.dumps(extra),
             "is_managed_externally": disallow_edits,
             "metrics": [],
+            **model_kwargs,  # include additional model metadata defined in model.meta.superset
         }
-        update.update(model.get("meta", {}).get("superset", {}))
         if base_url:
             fragment = "!/model/{unique_id}".format(**model)
             update["external_url"] = str(base_url.with_fragment(fragment))
-        client.update_dataset(dataset["id"], override_columns=True, **update)
+        client.update_dataset(dataset["id"], override_columns=reload_columns, **update)
 
         # ...then update metrics
         if dataset_metrics:
             update = {
                 "metrics": dataset_metrics,
             }
             client.update_dataset(dataset["id"], override_columns=False, **update)
@@ -170,14 +191,14 @@
                 # for some reason this is being sent as null sometimes
                 # https://github.com/preset-io/backend-sdk/issues/163
                 if "is_active" in column and column["is_active"] is None:
                     del column["is_active"]
 
             client.update_dataset(
                 dataset["id"],
-                override_columns=True,
+                override_columns=reload_columns,
                 columns=current_columns,
             )
 
         datasets.append(dataset)
 
     return datasets
```

### Comparing `preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/exposures.py` & `preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/exposures.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Sync Superset dashboards as dbt exposures.
 """
 
 import json
+import re
 from pathlib import Path
 from typing import Any, Dict, List, NamedTuple, Optional
 
 import yaml
 
 from preset_cli.api.clients.superset import SupersetClient
 
@@ -27,16 +28,25 @@
     chart: Any,
     model_map: Dict[ModelKey, str],
 ) -> List[str]:
     """
     Get all the dbt dependencies for a given chart.
     """
 
-    query_context = json.loads(chart["query_context"])
-    dataset_id = query_context["datasource"]["id"]
+    # imported charts have a null query context until loaded in Explore for the first time.
+    # in that case, we can get the dataset id from the params
+    if chart["query_context"]:
+        dataset_id = json.loads(chart["query_context"])["datasource"]["id"]
+    elif chart["params"]:
+        dataset_id = json.loads(chart["params"])["datasource"].split("__")[0]
+    else:
+        raise Exception(
+            f'Unable to find dataset information for Chart {chart["slice_name"]}',
+        )
+
     dataset = client.get_dataset(dataset_id)
     extra = json.loads(dataset["extra"] or "{}")
     if "depends_on" in extra:
         return [extra["depends_on"]]
 
     key = ModelKey(dataset["schema"], dataset["table_name"])
     if dataset["datasource_type"] == "table" and key in model_map:
@@ -106,16 +116,22 @@
             charts_ids.add(chart["id"])
         for dashboard in payload["dashboards"]["result"]:
             dashboards_ids.add(dashboard["id"])
 
     for chart_id in charts_ids:
         chart = client.get_chart(chart_id)
         first_owner = chart["owners"][0]
+
+        # remove unsupported characters for dbt exposures name
+        asset_title = re.sub(" ", "_", chart["slice_name"])
+        asset_title = re.sub(r"\W", "", asset_title)
+
         exposure = {
-            "name": chart["slice_name"] + " [chart]",
+            "name": asset_title + "_chart_" + str(chart_id),
+            "label": chart["slice_name"] + " [chart]",
             "type": "analysis",
             "maturity": "high" if chart["certified_by"] else "low",
             "url": str(
                 client.baseurl
                 / "superset/explore/"
                 % {"form_data": json.dumps({"slice_id": chart_id})},
             ),
@@ -127,16 +143,21 @@
             },
         }
         exposures.append(exposure)
 
     for dashboard_id in dashboards_ids:
         dashboard = client.get_dashboard(dashboard_id)
         first_owner = dashboard["owners"][0]
+
+        asset_title = re.sub(" ", "_", dashboard["dashboard_title"])
+        asset_title = re.sub(r"\W", "", asset_title)
+
         exposure = {
-            "name": dashboard["dashboard_title"] + " [dashboard]",
+            "name": asset_title + "_dashboard_" + str(dashboard_id),
+            "label": dashboard["dashboard_title"] + " [dashboard]",
             "type": "dashboard",
             "maturity": "high"
             if dashboard["published"] or dashboard["certified_by"]
             else "low",
             "url": str(client.baseurl / dashboard["url"].lstrip("/")),
             "description": "",
             "depends_on": get_dashboard_depends_on(client, dashboard, model_map),
```

### Comparing `preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/lib.py` & `preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/cli/superset/sync/dbt/metrics.py` & `preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/metrics.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/cli/superset/sync/native/command.py` & `preset-cli-0.2.2/src/preset_cli/cli/superset/sync/native/command.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/exceptions.py` & `preset-cli-0.2.2/src/preset_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli/lib.py` & `preset-cli-0.2.2/src/preset_cli/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli.egg-info/PKG-INFO` & `preset-cli-0.2.2/src/preset_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preset-cli
-Version: 0.2.1
+Version: 0.2.2
 Summary: A CLI to interact with Preset (https://preset.io/) workspaces.
 Home-page: https://github.com/preset-io/backend-sdk
 Author: Beto Dealmeida
 Author-email: beto@preset.io
 License: Other/Proprietary License
 Project-URL: Documentation, https://github.com/preset-io/backend-sdk/blob/master/README.rst
 Platform: any
@@ -381,14 +381,39 @@
 
 1. Read the dbt profile and create the ``$target`` database for the specified project in the Preset workspace.
 2. Every source in the project will be created as a dataset in the Preset workspace.
 3. Every model in the project will be created as a dataset in the Preset workspace.
 4. Any `metrics <https://docs.getdbt.com/docs/building-a-dbt-project/metrics>`_ will be added to the corresponding datasets.
 5. Every dashboard built on top of the dbt sources and/or models will be synchronized back to dbt as an `exposure <https://docs.getdbt.com/docs/building-a-dbt-project/exposures>`_.
 
+Descriptions, labels and other metadata is also synced from dbt models to the corresponding fields in the dataset. It's also possible to specify values for Superset-only fields directly in the model definition, under ``model.meta.superset.{{field_name}}``. For example, to specify the cache timeout for a dataset:
+
+.. code-block:: yaml
+
+    models:
+      - name: my_dbt_model
+        meta:
+          superset:
+            cache_timeout: 250 # Setting the dataset cache timeout to 250. 
+
+The same is applied for metrics. For example, to specify the d3 format for a metric:
+
+.. code-block:: yaml
+
+    - name: avg_revenue
+      label: "AVG Revenue"
+      model: ref('my_dbt_model')
+      calculation_method: average
+      expression: price_each
+      timestamp: date
+      meta:
+        superset:
+          d3format: '%d'
+
+
 The ``--external-url-prefix`` should point to your dbt docs, so that the resources in the workspace can point to the source of truth where they are being managed. Similar to the native sync, the dbt sync also supports the ``--disallow-edits`` flag.
 
 By default, the CLI sync would create a new database on the destination workspace using below name structure:
 
 .. code-block:: python
 
     f"{project_name}_{target_name}"
```

### Comparing `preset-cli-0.2.1/src/preset_cli.egg-info/SOURCES.txt` & `preset-cli-0.2.2/src/preset_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/src/preset_cli.egg-info/requires.txt` & `preset-cli-0.2.2/src/preset_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/api/clients/dbt_test.py` & `preset-cli-0.2.2/tests/api/clients/dbt_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/api/clients/preset_test.py` & `preset-cli-0.2.2/tests/api/clients/preset_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/api/clients/superset_test.py` & `preset-cli-0.2.2/tests/api/clients/superset_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -2147,15 +2147,15 @@
         "(filters:!((col:schema,opr:eq,value:main),"
         "(col:table_name,opr:eq,value:test_table)),"
         "order_column:changed_on_delta_humanized,"
         "order_direction:desc,page:1,page_size:100)",
         json={"result": []},
     )
     requests_mock.get(
-        "https://superset.example.org/roles/list/?_flt_0_name=Gamma",
+        "https://superset.example.org/roles/list/?_flt_3_name=Gamma",
         text="""
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="utf-8">
   </head>
   <body>
@@ -2238,15 +2238,15 @@
         "(filters:!((col:schema,opr:eq,value:main),"
         "(col:table_name,opr:eq,value:test_table)),"
         "order_column:changed_on_delta_humanized,"
         "order_direction:desc,page:1,page_size:100)",
         json={"result": []},
     )
     requests_mock.get(
-        "https://superset.example.org/roles/list/?_flt_0_name=Gamma",
+        "https://superset.example.org/roles/list/?_flt_3_name=Gamma",
         text="""
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="utf-8">
   </head>
   <body>
@@ -2293,15 +2293,15 @@
         "(filters:!((col:schema,opr:eq,value:main),"
         "(col:table_name,opr:eq,value:test_table)),"
         "order_column:changed_on_delta_humanized,"
         "order_direction:desc,page:1,page_size:100)",
         json={"result": []},
     )
     requests_mock.get(
-        "https://superset.example.org/roles/list/?_flt_0_name=Gamma",
+        "https://superset.example.org/roles/list/?_flt_3_name=Gamma",
         text="""
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="utf-8">
   </head>
   <body>
@@ -2377,15 +2377,15 @@
         "https://superset.example.org/api/v1/dataset/?q="
         "(filters:!((col:table_name,opr:eq,value:test_table)),"
         "order_column:changed_on_delta_humanized,"
         "order_direction:desc,page:1,page_size:100)",
         json={"result": []},
     )
     requests_mock.get(
-        "https://superset.example.org/roles/list/?_flt_0_name=Gamma",
+        "https://superset.example.org/roles/list/?_flt_3_name=Gamma",
         text="""
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="utf-8">
   </head>
   <body>
@@ -2538,15 +2538,15 @@
         "(filters:!((col:schema,opr:eq,value:main),"
         "(col:table_name,opr:eq,value:test_table)),"
         "order_column:changed_on_delta_humanized,"
         "order_direction:desc,page:1,page_size:100)",
         json={"result": []},
     )
     requests_mock.get(
-        "https://superset.example.org/roles/list/?_flt_0_name=Gamma",
+        "https://superset.example.org/roles/list/?_flt_3_name=Gamma",
         text="""
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="utf-8">
   </head>
   <body>
@@ -2599,15 +2599,15 @@
         "(filters:!((col:schema,opr:eq,value:main),"
         "(col:table_name,opr:eq,value:test_table)),"
         "order_column:changed_on_delta_humanized,"
         "order_direction:desc,page:1,page_size:100)",
         json={"result": []},
     )
     requests_mock.get(
-        "https://superset.example.org/roles/list/?_flt_0_name=Gamma",
+        "https://superset.example.org/roles/list/?_flt_3_name=Gamma",
         text="""
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="utf-8">
   </head>
   <body>
@@ -2666,15 +2666,15 @@
         "(filters:!((col:schema,opr:eq,value:main),"
         "(col:table_name,opr:eq,value:test_table)),"
         "order_column:changed_on_delta_humanized,"
         "order_direction:desc,page:1,page_size:100)",
         json={"result": []},
     )
     requests_mock.get(
-        "https://superset.example.org/roles/list/?_flt_0_name=Gamma",
+        "https://superset.example.org/roles/list/?_flt_3_name=Gamma",
         text="""
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="utf-8">
   </head>
   <body>
```

### Comparing `preset-cli-0.2.1/tests/auth/jwt_test.py` & `preset-cli-0.2.2/tests/auth/jwt_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/auth/lib_test.py` & `preset-cli-0.2.2/tests/auth/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/auth/main_test.py` & `preset-cli-0.2.2/tests/auth/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/auth/password_test.py` & `preset-cli-0.2.2/tests/auth/password_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/auth/preset_test.py` & `preset-cli-0.2.2/tests/auth/preset_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/cli/main_test.py` & `preset-cli-0.2.2/tests/cli/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/cli/superset/export_test.py` & `preset-cli-0.2.2/tests/cli/superset/export_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/cli/superset/import_test.py` & `preset-cli-0.2.2/tests/cli/superset/import_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/cli/superset/main_test.py` & `preset-cli-0.2.2/tests/cli/superset/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/cli/superset/sql_test.py` & `preset-cli-0.2.2/tests/cli/superset/sql_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/cli/superset/sync/dbt/command_test.py` & `preset-cli-0.2.2/tests/cli/superset/sync/dbt/command_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,140 @@
 )
 from preset_cli.exceptions import DatabaseNotFoundError
 
 dirname, _ = os.path.split(os.path.abspath(__file__))
 with open(os.path.join(dirname, "manifest.json"), encoding="utf-8") as fp:
     manifest_contents = fp.read()
 
+dbt_core_models = [
+    {
+        "database": "examples_dev",
+        "columns": [],
+        "meta": {},
+        "description": "",
+        "name": "messages_channels",
+        "tags": [],
+        "schema": "public",
+        "unique_id": "model.superset_examples.messages_channels",
+        "created_at": 1642628933.004452,
+        "children": ["metric.superset_examples.cnt"],
+        "depends_on": {
+            "macros": [],
+            "nodes": [
+                "source.superset_examples.public.channels",
+                "source.superset_examples.public.messages",
+            ],
+        },
+        "unrendered_config": {"materialized": "view"},
+        "resource_type": "model",
+        "path": "slack/messages_channels.sql",
+        "extra_ctes": [],
+        "package_name": "superset_examples",
+        "alias": "messages_channels",
+        "relation_name": '"examples_dev"."public"."messages_channels"',
+        "config": {
+            "enabled": True,
+            "alias": None,
+            "schema": None,
+            "database": None,
+            "tags": [],
+            "meta": {},
+            "materialized": "view",
+            "persist_docs": {},
+            "quoting": {},
+            "column_types": {},
+            "full_refresh": None,
+            "on_schema_change": "ignore",
+            "post-hook": [],
+            "pre-hook": [],
+        },
+        "patch_path": None,
+        "compiled_sql": (
+            "SELECT messages.ts, channels.name, messages.text "
+            'FROM "examples_dev"."public"."messages" messages '
+            'JOIN "examples_dev"."public"."channels" channels '
+            "ON messages.channel_id = channels.id"
+        ),
+        "extra_ctes_injected": True,
+        "deferred": False,
+        "root_path": "/Users/beto/Projects/dbt-examples/superset_examples",
+        "original_file_path": "models/slack/messages_channels.sql",
+        "refs": [],
+        "fqn": ["superset_examples", "slack", "messages_channels"],
+        "raw_sql": (
+            "SELECT messages.ts, channels.name, messages.text "
+            "FROM {{ source ('public', 'messages') }} messages "
+            "JOIN {{ source ('public', 'channels') }} channels "
+            "ON messages.channel_id = channels.id"
+        ),
+        "build_path": None,
+        "sources": [["public", "channels"], ["public", "messages"]],
+        "checksum": {
+            "name": "sha256",
+            "checksum": "b4ce232b28280daa522b37e12c36b67911e2a98456b8a3b99440075ec5564609",
+        },
+        "docs": {"show": True},
+        "compiled_path": "target/compiled/superset_examples/models/slack/messages_channels.sql",
+        "compiled": True,
+    },
+]
+
+dbt_core_metrics = [
+    {
+        "label": "",
+        "sql": "*",
+        "depends_on": ["model.superset_examples.messages_channels"],
+        "meta": {},
+        "description": "",
+        "name": "cnt",
+        "type": "count",
+        "filters": [],
+        "unique_id": "metric.superset_examples.cnt",
+        "created_at": 1642630986.1942852,
+        "package_name": "superset_examples",
+        "sources": [],
+        "root_path": "/Users/beto/Projects/dbt-examples/superset_examples",
+        "path": "slack/schema.yml",
+        "resource_type": "metric",
+        "original_file_path": "models/slack/schema.yml",
+        "model": "ref('messages_channels')",
+        "timestamp": None,
+        "fqn": ["superset_examples", "slack", "cnt"],
+        "time_grains": [],
+        "tags": [],
+        "refs": [["messages_channels"]],
+        "dimensions": [],
+    },
+]
+
+dbt_cloud_models = [
+    {
+        "database": "examples_dev",
+        "description": "",
+        "meta": {},
+        "name": "messages_channels",
+        "schema": "public",
+        "unique_id": "model.superset_examples.messages_channels",
+    },
+]
+
+dbt_cloud_metrics = [
+    {
+        "depends_on": ["model.superset_examples.messages_channels"],
+        "description": "",
+        "filters": [],
+        "label": "",
+        "meta": {},
+        "name": "cnt",
+        "sql": "*",
+        "type": "count",
+        "unique_id": "metric.superset_examples.cnt",
+    },
+]
+
 
 def test_dbt_core(mocker: MockerFixture, fs: FakeFilesystem) -> None:
     """
     Test the ``dbt-core`` command.
     """
     root = Path("/path/to/root")
     fs.create_dir(root)
@@ -75,126 +201,105 @@
         "default",
         "default",
         None,
         False,
         False,
         "",
     )
-    models = [
-        {
-            "database": "examples_dev",
-            "columns": [],
-            "meta": {},
-            "description": "",
-            "name": "messages_channels",
-            "tags": [],
-            "schema": "public",
-            "unique_id": "model.superset_examples.messages_channels",
-            "created_at": 1642628933.004452,
-            "children": ["metric.superset_examples.cnt"],
-            "depends_on": {
-                "macros": [],
-                "nodes": [
-                    "source.superset_examples.public.channels",
-                    "source.superset_examples.public.messages",
-                ],
-            },
-            "unrendered_config": {"materialized": "view"},
-            "resource_type": "model",
-            "path": "slack/messages_channels.sql",
-            "extra_ctes": [],
-            "package_name": "superset_examples",
-            "alias": "messages_channels",
-            "relation_name": '"examples_dev"."public"."messages_channels"',
-            "config": {
-                "enabled": True,
-                "alias": None,
-                "schema": None,
-                "database": None,
-                "tags": [],
-                "meta": {},
-                "materialized": "view",
-                "persist_docs": {},
-                "quoting": {},
-                "column_types": {},
-                "full_refresh": None,
-                "on_schema_change": "ignore",
-                "post-hook": [],
-                "pre-hook": [],
-            },
-            "patch_path": None,
-            "compiled_sql": (
-                "SELECT messages.ts, channels.name, messages.text "
-                'FROM "examples_dev"."public"."messages" messages '
-                'JOIN "examples_dev"."public"."channels" channels '
-                "ON messages.channel_id = channels.id"
-            ),
-            "extra_ctes_injected": True,
-            "deferred": False,
-            "root_path": "/Users/beto/Projects/dbt-examples/superset_examples",
-            "original_file_path": "models/slack/messages_channels.sql",
-            "refs": [],
-            "fqn": ["superset_examples", "slack", "messages_channels"],
-            "raw_sql": (
-                "SELECT messages.ts, channels.name, messages.text "
-                "FROM {{ source ('public', 'messages') }} messages "
-                "JOIN {{ source ('public', 'channels') }} channels "
-                "ON messages.channel_id = channels.id"
-            ),
-            "build_path": None,
-            "sources": [["public", "channels"], ["public", "messages"]],
-            "checksum": {
-                "name": "sha256",
-                "checksum": "b4ce232b28280daa522b37e12c36b67911e2a98456b8a3b99440075ec5564609",
-            },
-            "docs": {"show": True},
-            "compiled_path": "target/compiled/superset_examples/models/slack/messages_channels.sql",
-            "compiled": True,
-        },
-    ]
-    metrics = [
-        {
-            "label": "",
-            "sql": "*",
-            "depends_on": ["model.superset_examples.messages_channels"],
-            "meta": {},
-            "description": "",
-            "name": "cnt",
-            "type": "count",
-            "filters": [],
-            "unique_id": "metric.superset_examples.cnt",
-            "created_at": 1642630986.1942852,
-            "package_name": "superset_examples",
-            "sources": [],
-            "root_path": "/Users/beto/Projects/dbt-examples/superset_examples",
-            "path": "slack/schema.yml",
-            "resource_type": "metric",
-            "original_file_path": "models/slack/schema.yml",
-            "model": "ref('messages_channels')",
-            "timestamp": None,
-            "fqn": ["superset_examples", "slack", "cnt"],
-            "time_grains": [],
-            "tags": [],
-            "refs": [["messages_channels"]],
-            "dimensions": [],
-        },
-    ]
+
     sync_datasets.assert_called_with(
         client,
-        models,
-        metrics,
+        dbt_core_models,
+        dbt_core_metrics,
         sync_database(),
         False,
         "",
+        reload_columns=True,
     )
     sync_exposures.assert_called_with(
         client,
         exposures,
         sync_datasets(),
-        {("public", "messages_channels"): "ref(messages_channels)"},
+        {("public", "messages_channels"): "ref('messages_channels')"},
+    )
+
+
+def test_dbt_core_reload_columns_false(
+    mocker: MockerFixture,
+    fs: FakeFilesystem,
+) -> None:
+    """
+    Test the ``dbt-core`` command with --preserve-columns flag
+    """
+    root = Path("/path/to/root")
+    fs.create_dir(root)
+    manifest = root / "default/target/manifest.json"
+    fs.create_file(manifest, contents=manifest_contents)
+    profiles = root / ".dbt/profiles.yml"
+    fs.create_file(profiles)
+    exposures = root / "models/exposures.yml"
+    fs.create_file(exposures)
+
+    SupersetClient = mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.SupersetClient",
+    )
+    client = SupersetClient()
+    mocker.patch("preset_cli.cli.superset.main.UsernamePasswordAuth")
+    sync_database = mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.sync_database",
+    )
+    sync_datasets = mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.sync_datasets",
+    )
+    sync_exposures = mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.sync_exposures",
+    )
+
+    runner = CliRunner()
+    result = runner.invoke(
+        superset_cli,
+        [
+            "https://superset.example.org/",
+            "sync",
+            "dbt-core",
+            str(manifest),
+            "--profiles",
+            str(profiles),
+            "--exposures",
+            str(exposures),
+            "--preserve-columns",
+        ],
+        catch_exceptions=False,
+    )
+    assert result.exit_code == 0
+    sync_database.assert_called_with(
+        client,
+        profiles,
+        "default",
+        "default",
+        None,
+        False,
+        False,
+        "",
+    )
+
+    sync_datasets.assert_called_with(
+        client,
+        dbt_core_models,
+        dbt_core_metrics,
+        sync_database(),
+        False,
+        "",
+        reload_columns=False,
+    )
+    sync_exposures.assert_called_with(
+        client,
+        exposures,
+        sync_datasets(),
+        {("public", "messages_channels"): "ref('messages_channels')"},
     )
 
 
 def test_dbt_core_dbt_project(mocker: MockerFixture, fs: FakeFilesystem) -> None:
     """
     Test the ``dbt-core`` command with a ``dbt_project.yml`` file.
     """
@@ -439,20 +544,21 @@
     sync_datasets.assert_called_with(
         client,
         models,
         metrics,
         sync_database(),
         False,
         "",
+        reload_columns=True,
     )
     sync_exposures.assert_called_with(
         client,
         exposures,
         sync_datasets(),
-        {("public", "messages_channels"): "ref(messages_channels)"},
+        {("public", "messages_channels"): "ref('messages_channels')"},
     )
 
 
 def test_dbt_core_no_exposures(mocker: MockerFixture, fs: FakeFilesystem) -> None:
     """
     Test the ``dbt-core`` command when no exposures file is passed.
     """
@@ -592,39 +698,17 @@
     DBTClient = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.DBTClient",
     )
     dbt_client = DBTClient()
     sync_datasets = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.sync_datasets",
     )
-    models = [
-        {
-            "database": "examples_dev",
-            "description": "",
-            "meta": {},
-            "name": "messages_channels",
-            "schema": "public",
-            "unique_id": "model.superset_examples.messages_channels",
-        },
-    ]
-    dbt_client.get_models.return_value = models
-    metrics = [
-        {
-            "depends_on": ["model.superset_examples.messages_channels"],
-            "description": "",
-            "filters": [],
-            "label": "",
-            "meta": {},
-            "name": "cnt",
-            "sql": "*",
-            "type": "count",
-            "unique_id": "metric.superset_examples.cnt",
-        },
-    ]
-    dbt_client.get_metrics.return_value = metrics
+
+    dbt_client.get_models.return_value = dbt_cloud_models
+    dbt_client.get_metrics.return_value = dbt_cloud_metrics
     database = mocker.MagicMock()
     superset_client.get_databases.return_value = [database]
     superset_client.get_database.return_value = database
 
     runner = CliRunner()
     result = runner.invoke(
         superset_cli,
@@ -636,19 +720,68 @@
             "123",
         ],
         catch_exceptions=False,
     )
     assert result.exit_code == 0
     sync_datasets.assert_called_with(
         superset_client,
-        models,
-        metrics,
+        dbt_cloud_models,
+        dbt_cloud_metrics,
+        database,
+        False,
+        "",
+        reload_columns=True,
+    )
+
+
+def test_dbt_cloud_reload_columns_false(mocker: MockerFixture) -> None:
+    """
+    Test the ``dbt-cloud`` command with the --preserve-columns flag.
+    """
+    SupersetClient = mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.SupersetClient",
+    )
+    superset_client = SupersetClient()
+    mocker.patch("preset_cli.cli.superset.main.UsernamePasswordAuth")
+    DBTClient = mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.DBTClient",
+    )
+    dbt_client = DBTClient()
+    sync_datasets = mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.sync_datasets",
+    )
+
+    dbt_client.get_models.return_value = dbt_cloud_models
+    dbt_client.get_metrics.return_value = dbt_cloud_metrics
+    database = mocker.MagicMock()
+    superset_client.get_databases.return_value = [database]
+    superset_client.get_database.return_value = database
+
+    runner = CliRunner()
+    result = runner.invoke(
+        superset_cli,
+        [
+            "https://superset.example.org/",
+            "sync",
+            "dbt-cloud",
+            "XXX",
+            "123",
+            "--preserve-columns",
+        ],
+        catch_exceptions=False,
+    )
+    assert result.exit_code == 0
+    sync_datasets.assert_called_with(
+        superset_client,
+        dbt_cloud_models,
+        dbt_cloud_metrics,
         database,
         False,
         "",
+        reload_columns=False,
     )
 
 
 def test_dbt_cloud_no_job_id(mocker: MockerFixture) -> None:
     """
     Test the ``dbt-cloud`` command when no job ID is specified.
     """
@@ -660,39 +793,17 @@
     DBTClient = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.DBTClient",
     )
     dbt_client = DBTClient()
     sync_datasets = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.sync_datasets",
     )
-    models = [
-        {
-            "database": "examples_dev",
-            "description": "",
-            "meta": {},
-            "name": "messages_channels",
-            "schema": "public",
-            "unique_id": "model.superset_examples.messages_channels",
-        },
-    ]
-    dbt_client.get_models.return_value = models
-    metrics = [
-        {
-            "depends_on": ["model.superset_examples.messages_channels"],
-            "description": "",
-            "filters": [],
-            "label": "",
-            "meta": {},
-            "name": "cnt",
-            "sql": "*",
-            "type": "count",
-            "unique_id": "metric.superset_examples.cnt",
-        },
-    ]
-    dbt_client.get_metrics.return_value = metrics
+
+    dbt_client.get_models.return_value = dbt_cloud_models
+    dbt_client.get_metrics.return_value = dbt_cloud_metrics
     dbt_client.get_accounts.return_value = [{"id": 1, "name": "My account"}]
     dbt_client.get_projects.return_value = [{"id": 1000, "name": "My project"}]
     dbt_client.get_jobs.return_value = [{"id": 123, "name": "My job"}]
     database = mocker.MagicMock()
     superset_client.get_databases.return_value = [database]
     superset_client.get_database.return_value = database
 
@@ -709,19 +820,20 @@
     )
     assert result.exit_code == 0
     dbt_client.get_database_name.assert_called_with(123)
     dbt_client.get_models.assert_called_with(123)
     dbt_client.get_metrics.assert_called_with(123)
     sync_datasets.assert_called_with(
         superset_client,
-        models,
-        metrics,
+        dbt_cloud_models,
+        dbt_cloud_metrics,
         database,
         False,
         "",
+        reload_columns=True,
     )
 
 
 def test_get_account_id(mocker: MockerFixture) -> None:
     """
     Test the ``get_account_id`` helper.
     """
@@ -948,15 +1060,15 @@
     sync_datasets.assert_not_called()
     sync_exposures.assert_called_with(
         client,
         exposures,
         [
             {"schema": "public", "table_name": "messages_channels"},
         ],
-        {("public", "messages_channels"): "ref(messages_channels)"},
+        {("public", "messages_channels"): "ref('messages_channels')"},
     )
 
 
 def test_dbt_cloud_exposures_only(mocker: MockerFixture, fs: FakeFilesystem) -> None:
     """
     Test the ``--exposures-only`` option with dbt cloud.
     """
@@ -980,39 +1092,17 @@
     dbt_client = DBTClient()
     sync_datasets = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.sync_datasets",
     )
     sync_exposures = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.sync_exposures",
     )
-    models = [
-        {
-            "database": "examples_dev",
-            "description": "",
-            "meta": {},
-            "name": "messages_channels",
-            "schema": "public",
-            "unique_id": "model.superset_examples.messages_channels",
-        },
-    ]
-    dbt_client.get_models.return_value = models
-    metrics = [
-        {
-            "depends_on": ["model.superset_examples.messages_channels"],
-            "description": "",
-            "filters": [],
-            "label": "",
-            "meta": {},
-            "name": "cnt",
-            "sql": "*",
-            "type": "count",
-            "unique_id": "metric.superset_examples.cnt",
-        },
-    ]
-    dbt_client.get_metrics.return_value = metrics
+
+    dbt_client.get_models.return_value = dbt_cloud_models
+    dbt_client.get_metrics.return_value = dbt_cloud_metrics
     database = mocker.MagicMock()
     superset_client.get_databases.return_value = [database]
     superset_client.get_database.return_value = database
 
     runner = CliRunner()
     result = runner.invoke(
         superset_cli,
@@ -1032,9 +1122,9 @@
     sync_datasets.assert_not_called()
     sync_exposures.assert_called_with(
         superset_client,
         exposures,
         [
             {"schema": "public", "table_name": "messages_channels"},
         ],
-        {("public", "messages_channels"): "ref(messages_channels)"},
+        {("public", "messages_channels"): "ref('messages_channels')"},
     )
```

### Comparing `preset-cli-0.2.1/tests/cli/superset/sync/dbt/databases_test.py` & `preset-cli-0.2.2/tests/cli/superset/sync/dbt/databases_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/cli/superset/sync/dbt/datasets_test.py` & `preset-cli-0.2.2/tests/cli/superset/sync/dbt/datasets_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Tests for ``preset_cli.cli.superset.sync.dbt.datasets``.
 """
-# pylint: disable=invalid-name
+# pylint: disable=invalid-name, too-many-lines
 
 import json
 from typing import List, cast
 from unittest import mock
 
 import pytest
 from pytest_mock import MockerFixture
@@ -511,14 +511,93 @@
                     },
                 ],
             ),
         ],
     )
 
 
+def test_sync_datasets_preserve_columns(mocker: MockerFixture) -> None:
+    """
+    Test ``sync_datasets`` when setting ovverride_columns to false.
+    """
+    client = mocker.MagicMock()
+    client.get_datasets.side_effect = [[{"id": 1}], [{"id": 2}], [{"id": 3}]]
+    client.get_dataset.return_value = {
+        "columns": [
+            {
+                "column_name": "id",
+                "is_dttm": False,
+                "filterable": False,
+                "groupby": False,
+            },
+        ],
+    }
+
+    sync_datasets(
+        client=client,
+        models=models,
+        metrics=metrics,
+        database={"id": 1},
+        disallow_edits=False,
+        external_url_prefix="https://dbt.example.org/",
+        reload_columns=False,
+    )
+    client.create_dataset.assert_not_called()
+    client.update_dataset.assert_has_calls(
+        [
+            mock.call(
+                1,
+                override_columns=False,
+                description="",
+                extra=json.dumps(
+                    {
+                        "unique_id": "model.superset_examples.messages_channels",
+                        "depends_on": "ref('messages_channels')",
+                        "certification": {"details": "This table is produced by dbt"},
+                    },
+                ),
+                is_managed_externally=False,
+                metrics=[],
+                external_url=(
+                    "https://dbt.example.org/"
+                    "#!/model/model.superset_examples.messages_channels"
+                ),
+            ),
+            mock.call(
+                1,
+                override_columns=False,
+                metrics=[
+                    {
+                        "expression": "COUNT(*)",
+                        "metric_name": "cnt",
+                        "metric_type": "count",
+                        "verbose_name": "",
+                        "description": "",
+                        "extra": "{}",
+                    },
+                ],
+            ),
+            mock.call(
+                1,
+                override_columns=False,
+                columns=[
+                    {
+                        "column_name": "id",
+                        "description": "Primary key",
+                        "is_dttm": False,
+                        "filterable": False,
+                        "groupby": False,
+                        "verbose_name": "id",
+                    },
+                ],
+            ),
+        ],
+    )
+
+
 def test_sync_datasets_no_columns(mocker: MockerFixture) -> None:
     """
     Test ``sync_datasets`` when passing external URL prefix.
     """
     client = mocker.MagicMock()
     client.get_datasets.side_effect = [[{"id": 1}], [{"id": 2}], [{"id": 3}]]
 
@@ -626,7 +705,382 @@
     url = make_url("bigquery://project-1")
     assert model_in_database(cast(ModelSchema, {"database": "project-1"}), url)
     assert not model_in_database(cast(ModelSchema, {"database": "project-2"}), url)
 
     url = make_url("snowflake://user:password@host/db1")
     assert model_in_database(cast(ModelSchema, {"database": "db1"}), url)
     assert not model_in_database(cast(ModelSchema, {"database": "db2"}), url)
+
+
+def test_sync_datasets_null_certification(mocker: MockerFixture) -> None:
+    """
+    Test ``sync_datasets`` with no certification info
+    """
+    client = mocker.MagicMock()
+    client.get_datasets.return_value = []
+    client.create_dataset.side_effect = [{"id": 1}, {"id": 2}, {"id": 3}]
+    client.get_dataset.return_value = {
+        "columns": [
+            {"column_name": "id", "is_dttm": False, "type_generic": "INTEGER"},
+            {"column_name": "ts", "is_dttm": True, "type_generic": "TIMESTAMP"},
+        ],
+    }
+
+    models_with_null_certification: List[ModelSchema] = [
+        model_schema.load(
+            {
+                "database": "examples_dev",
+                "schema": "public",
+                "description": "",
+                "meta": {"superset": {"extra": {"certification": None}}},
+                "name": "messages_channels",
+                "unique_id": "model.superset_examples.messages_channels",
+                "columns": [{"name": "id", "description": "Primary key"}],
+            },
+        ),
+    ]
+    sync_datasets(
+        client=client,
+        models=models_with_null_certification,
+        metrics=metrics,
+        database={"id": 1, "sqlalchemy_uri": "postgresql://user@host/examples_dev"},
+        disallow_edits=False,
+        external_url_prefix="",
+    )
+    client.create_dataset.assert_has_calls(
+        [
+            mock.call(database=1, schema="public", table_name="messages_channels"),
+        ],
+    )
+    client.update_dataset.assert_has_calls(
+        [
+            mock.call(
+                1,
+                override_columns=True,
+                description="",
+                extra=json.dumps(
+                    {
+                        "unique_id": "model.superset_examples.messages_channels",
+                        "depends_on": "ref('messages_channels')",
+                    },
+                ),
+                is_managed_externally=False,
+                metrics=[],
+            ),
+            mock.call(
+                1,
+                override_columns=False,
+                metrics=[
+                    {
+                        "expression": "COUNT(*)",
+                        "metric_name": "cnt",
+                        "metric_type": "count",
+                        "verbose_name": "",
+                        "description": "",
+                        "extra": "{}",
+                    },
+                ],
+            ),
+            mock.call(
+                1,
+                override_columns=True,
+                columns=[
+                    {
+                        "column_name": "id",
+                        "description": "Primary key",
+                        "is_dttm": False,
+                        "verbose_name": "id",
+                    },
+                    {
+                        "column_name": "ts",
+                        "is_dttm": True,
+                    },
+                ],
+            ),
+        ],
+    )
+
+
+def test_sync_datasets_model_certification(mocker: MockerFixture) -> None:
+    """
+    Test ``sync_datasets`` with certification from model definition
+    """
+    client = mocker.MagicMock()
+    client.get_datasets.return_value = []
+    client.create_dataset.side_effect = [{"id": 1}, {"id": 2}, {"id": 3}]
+    client.get_dataset.return_value = {
+        "columns": [
+            {"column_name": "id", "is_dttm": False, "type_generic": "INTEGER"},
+            {"column_name": "ts", "is_dttm": True, "type_generic": "TIMESTAMP"},
+        ],
+    }
+
+    models_with_model_certification: List[ModelSchema] = [
+        model_schema.load(
+            {
+                "database": "examples_dev",
+                "schema": "public",
+                "description": "",
+                "meta": {
+                    "superset": {
+                        "extra": {
+                            "certification": {
+                                "details": "I declare this dataset certified",
+                                "certified_by": "Myself",
+                            },
+                        },
+                    },
+                },
+                "name": "messages_channels",
+                "unique_id": "model.superset_examples.messages_channels",
+                "columns": [{"name": "id", "description": "Primary key"}],
+            },
+        ),
+    ]
+    sync_datasets(
+        client=client,
+        models=models_with_model_certification,
+        metrics=metrics,
+        database={"id": 1, "sqlalchemy_uri": "postgresql://user@host/examples_dev"},
+        disallow_edits=False,
+        external_url_prefix="",
+    )
+    client.create_dataset.assert_has_calls(
+        [
+            mock.call(database=1, schema="public", table_name="messages_channels"),
+        ],
+    )
+    client.update_dataset.assert_has_calls(
+        [
+            mock.call(
+                1,
+                override_columns=True,
+                description="",
+                extra=json.dumps(
+                    {
+                        "unique_id": "model.superset_examples.messages_channels",
+                        "depends_on": "ref('messages_channels')",
+                        "certification": {
+                            "details": "I declare this dataset certified",
+                            "certified_by": "Myself",
+                        },
+                    },
+                ),
+                is_managed_externally=False,
+                metrics=[],
+            ),
+            mock.call(
+                1,
+                override_columns=False,
+                metrics=[
+                    {
+                        "expression": "COUNT(*)",
+                        "metric_name": "cnt",
+                        "metric_type": "count",
+                        "verbose_name": "",
+                        "description": "",
+                        "extra": "{}",
+                    },
+                ],
+            ),
+            mock.call(
+                1,
+                override_columns=True,
+                columns=[
+                    {
+                        "column_name": "id",
+                        "description": "Primary key",
+                        "is_dttm": False,
+                        "verbose_name": "id",
+                    },
+                    {
+                        "column_name": "ts",
+                        "is_dttm": True,
+                    },
+                ],
+            ),
+        ],
+    )
+
+
+def test_sync_datasets_warning(mocker: MockerFixture) -> None:
+    """
+    Test ``sync_datasets`` with warning information
+    """
+    client = mocker.MagicMock()
+    client.get_datasets.return_value = []
+    client.create_dataset.side_effect = [{"id": 1}, {"id": 2}, {"id": 3}]
+    client.get_dataset.return_value = {
+        "columns": [
+            {"column_name": "id", "is_dttm": False, "type_generic": "INTEGER"},
+            {"column_name": "ts", "is_dttm": True, "type_generic": "TIMESTAMP"},
+        ],
+    }
+
+    models_with_warning: List[ModelSchema] = [
+        model_schema.load(
+            {
+                "database": "examples_dev",
+                "schema": "public",
+                "description": "",
+                "meta": {
+                    "superset": {"extra": {"warning_markdown": "Under Construction"}},
+                },
+                "name": "messages_channels",
+                "unique_id": "model.superset_examples.messages_channels",
+                "columns": [{"name": "id", "description": "Primary key"}],
+            },
+        ),
+    ]
+    sync_datasets(
+        client=client,
+        models=models_with_warning,
+        metrics=metrics,
+        database={"id": 1, "sqlalchemy_uri": "postgresql://user@host/examples_dev"},
+        disallow_edits=False,
+        external_url_prefix="",
+    )
+    client.create_dataset.assert_has_calls(
+        [
+            mock.call(database=1, schema="public", table_name="messages_channels"),
+        ],
+    )
+    client.update_dataset.assert_has_calls(
+        [
+            mock.call(
+                1,
+                override_columns=True,
+                description="",
+                extra=json.dumps(
+                    {
+                        "unique_id": "model.superset_examples.messages_channels",
+                        "depends_on": "ref('messages_channels')",
+                        "certification": {"details": "This table is produced by dbt"},
+                        "warning_markdown": "Under Construction",
+                    },
+                ),
+                is_managed_externally=False,
+                metrics=[],
+            ),
+            mock.call(
+                1,
+                override_columns=False,
+                metrics=[
+                    {
+                        "expression": "COUNT(*)",
+                        "metric_name": "cnt",
+                        "metric_type": "count",
+                        "verbose_name": "",
+                        "description": "",
+                        "extra": "{}",
+                    },
+                ],
+            ),
+            mock.call(
+                1,
+                override_columns=True,
+                columns=[
+                    {
+                        "column_name": "id",
+                        "description": "Primary key",
+                        "is_dttm": False,
+                        "verbose_name": "id",
+                    },
+                    {
+                        "column_name": "ts",
+                        "is_dttm": True,
+                    },
+                ],
+            ),
+        ],
+    )
+
+
+def test_sync_datasets_meta_test(mocker: MockerFixture) -> None:
+    """
+    Test ``sync_datasets`` with an additional field set through meta.superset
+    """
+    client = mocker.MagicMock()
+    client.get_datasets.return_value = []
+    client.create_dataset.side_effect = [{"id": 1}, {"id": 2}, {"id": 3}]
+    client.get_dataset.return_value = {
+        "columns": [
+            {"column_name": "id", "is_dttm": False, "type_generic": "INTEGER"},
+            {"column_name": "ts", "is_dttm": True, "type_generic": "TIMESTAMP"},
+        ],
+    }
+
+    models_with_meta_info: List[ModelSchema] = [
+        model_schema.load(
+            {
+                "database": "examples_dev",
+                "schema": "public",
+                "description": "",
+                "meta": {"superset": {"cache_timeout": 250}},
+                "name": "messages_channels",
+                "unique_id": "model.superset_examples.messages_channels",
+                "columns": [{"name": "id", "description": "Primary key"}],
+            },
+        ),
+    ]
+    sync_datasets(
+        client=client,
+        models=models_with_meta_info,
+        metrics=metrics,
+        database={"id": 1, "sqlalchemy_uri": "postgresql://user@host/examples_dev"},
+        disallow_edits=False,
+        external_url_prefix="",
+    )
+    client.create_dataset.assert_has_calls(
+        [
+            mock.call(database=1, schema="public", table_name="messages_channels"),
+        ],
+    )
+    client.update_dataset.assert_has_calls(
+        [
+            mock.call(
+                1,
+                override_columns=True,
+                description="",
+                extra=json.dumps(
+                    {
+                        "unique_id": "model.superset_examples.messages_channels",
+                        "depends_on": "ref('messages_channels')",
+                        "certification": {"details": "This table is produced by dbt"},
+                    },
+                ),
+                is_managed_externally=False,
+                metrics=[],
+                cache_timeout=250,
+            ),
+            mock.call(
+                1,
+                override_columns=False,
+                metrics=[
+                    {
+                        "expression": "COUNT(*)",
+                        "metric_name": "cnt",
+                        "metric_type": "count",
+                        "verbose_name": "",
+                        "description": "",
+                        "extra": "{}",
+                    },
+                ],
+            ),
+            mock.call(
+                1,
+                override_columns=True,
+                columns=[
+                    {
+                        "column_name": "id",
+                        "description": "Primary key",
+                        "is_dttm": False,
+                        "verbose_name": "id",
+                    },
+                    {
+                        "column_name": "ts",
+                        "is_dttm": True,
+                    },
+                ],
+            ),
+        ],
+    )
```

### Comparing `preset-cli-0.2.1/tests/cli/superset/sync/dbt/exposures_test.py` & `preset-cli-0.2.2/tests/cli/superset/sync/dbt/exposures_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # pylint: disable=invalid-name
 
 import copy
 import json
 from pathlib import Path
 from typing import Any, Dict
 
+import pytest
 import yaml
 from pyfakefs.fake_filesystem import FakeFilesystem
 from pytest_mock import MockerFixture
 from yarl import URL
 
 from preset_cli.cli.superset.sync.dbt.exposures import (
     ModelKey,
@@ -590,27 +591,101 @@
 
     with open(exposures, encoding="utf-8") as input_:
         contents = yaml.load(input_, Loader=yaml.SafeLoader)
     assert contents == {
         "version": 2,
         "exposures": [
             {
-                "name": "Example chart [chart]",
+                "name": "Example_chart_chart_1",
+                "label": "Example chart [chart]",
                 "type": "analysis",
                 "maturity": "low",
                 "url": (
                     "https://superset.example.org/superset/explore/"
                     "?form_data=%7B%22slice_id%22:+1%7D"
                 ),
                 "description": "",
                 "depends_on": ["ref('messages_channels')"],
                 "owner": {"name": "admin admin", "email": "unknown"},
             },
             {
-                "name": "Example dashboard [dashboard]",
+                "name": "Example_dashboard_dashboard_12",
+                "label": "Example dashboard [dashboard]",
+                "type": "dashboard",
+                "maturity": "low",
+                "url": "https://superset.example.org/superset/dashboard/12/",
+                "description": "",
+                "depends_on": ["ref('messages_channels')"],
+                "owner": {"name": "admin admin", "email": "unknown"},
+            },
+        ],
+    }
+
+
+def test_sync_exposures_special_characters(
+    mocker: MockerFixture,
+    fs: FakeFilesystem,
+) -> None:
+    """
+    Test ``sync_exposures`` is generating a dbt-compatible name for the exposures.
+    """
+    root = Path("/path/to/root")
+    fs.create_dir(root / "models")
+    exposures = root / "models/exposures.yml"
+
+    client = mocker.MagicMock()
+    client.baseurl = URL("https://superset.example.org/")
+
+    chart_with_special_characters = copy.deepcopy(chart_response)
+    chart_with_special_characters["result"][
+        "slice_name"
+    ] = "T!tl3_ w1th $pecial characters()*"  # type: ignore
+    client.get_chart.return_value = chart_with_special_characters["result"]
+
+    dashboard_with_special_characters = copy.deepcopy(dashboard_response)
+    dashboard_with_special_characters["result"][
+        "dashboard_title"
+    ] = "D4shboard %^#? `wi_th` $pecial characters()*"  # type: ignore
+    client.get_dashboard.return_value = dashboard_with_special_characters["result"]
+
+    session = client.auth.session
+    session.get().json.return_value = related_objects_response
+    mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.exposures.get_dashboard_depends_on",
+        return_value=["ref('messages_channels')"],
+    )
+    mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.exposures.get_chart_depends_on",
+        return_value=["ref('messages_channels')"],
+    )
+
+    datasets = [dataset_response["result"]]
+    sync_exposures(client, exposures, datasets, {})
+
+    with open(exposures, encoding="utf-8") as input_:
+        contents = yaml.load(input_, Loader=yaml.SafeLoader)
+    assert contents == {
+        "version": 2,
+        "exposures": [
+            {
+                "name": "Ttl3__w1th_pecial_characters_chart_1",
+                "label": "T!tl3_ w1th $pecial characters()* [chart]",
+                "type": "analysis",
+                "maturity": "low",
+                "url": (
+                    "https://superset.example.org/superset/explore/"
+                    "?form_data=%7B%22slice_id%22:+1%7D"
+                ),
+                "description": "",
+                "depends_on": ["ref('messages_channels')"],
+                "owner": {"name": "admin admin", "email": "unknown"},
+            },
+            {
+                "name": "D4shboard__wi_th_pecial_characters_dashboard_12",
+                "label": "D4shboard %^#? `wi_th` $pecial characters()* [dashboard]",
                 "type": "dashboard",
                 "maturity": "low",
                 "url": "https://superset.example.org/superset/dashboard/12/",
                 "description": "",
                 "depends_on": ["ref('messages_channels')"],
                 "owner": {"name": "admin admin", "email": "unknown"},
             },
@@ -644,14 +719,33 @@
         contents = yaml.load(input_, Loader=yaml.SafeLoader)
     assert contents == {
         "version": 2,
         "exposures": [],
     }
 
 
+def test_get_chart_depends_on_null_query_context(
+    mocker: MockerFixture,
+) -> None:
+    """
+    Test ``get_chart_depends_on`` containing a chart that has ``query_context: null`.
+    """
+    client = mocker.MagicMock()
+    client.get_dataset.return_value = dataset_response["result"]
+    chart_response_no_query_context = copy.deepcopy(chart_response)
+    chart_response_no_query_context["result"]["query_context"] = None  # type: ignore
+
+    depends_on = get_chart_depends_on(
+        client,
+        chart_response_no_query_context["result"],
+        {},
+    )
+    assert depends_on == ["ref('messages_channels')"]
+
+
 def test_get_chart_depends_on_from_dataset(mocker: MockerFixture) -> None:
     """
     Test ``sync_exposures`` when datasets don't have model metadata.
 
     This is the case when users created the datasets manually, pointing them to dbt
     models, but still want to sync exposures back to dbt.
     """
@@ -660,17 +754,37 @@
     modified_dataset_response["result"]["extra"] = None  # type: ignore
     client.get_dataset.return_value = modified_dataset_response["result"]
 
     key = ModelKey("public", "messages_channels")
     depends_on = get_chart_depends_on(
         client,
         chart_response["result"],
-        {key: "ref(messages_channels)"},
+        {key: "ref('messages_channels')"},
+    )
+    assert depends_on == ["ref('messages_channels')"]
+
+
+def test_get_chart_depends_on_exception(
+    mocker: MockerFixture,
+) -> None:
+    """
+    Test ``get_chart_depends_on`` exception.
+    """
+    client = mocker.MagicMock()
+    client.get_dataset.return_value = dataset_response["result"]
+    chart_response_no_dataset_info = copy.deepcopy(chart_response)
+    chart_response_no_dataset_info["result"]["query_context"] = None  # type: ignore
+    chart_response_no_dataset_info["result"]["params"] = None  # type: ignore
+
+    with pytest.raises(Exception) as excinfo:
+        get_chart_depends_on(client, chart_response_no_dataset_info["result"], {})
+    assert (
+        str(excinfo.value)
+        == "Unable to find dataset information for Chart Example chart"
     )
-    assert depends_on == ["ref(messages_channels)"]
 
 
 def test_get_dashboard_depends_on_from_dataset(mocker: MockerFixture) -> None:
     """
     Test ``get_dashboard_depends_on`` when dataset don't have model metadata.
     """
     client = mocker.MagicMock()
@@ -680,10 +794,10 @@
     session = client.auth.session
     session.get().json.return_value = datasets_response
 
     key = ModelKey("public", "messages_channels")
     depends_on = get_dashboard_depends_on(
         client,
         dashboard_response["result"],
-        {key: "ref(messages_channels)"},
+        {key: "ref('messages_channels')"},
     )
-    assert depends_on == ["ref(messages_channels)"]
+    assert depends_on == ["ref('messages_channels')"]
```

### Comparing `preset-cli-0.2.1/tests/cli/superset/sync/dbt/lib_test.py` & `preset-cli-0.2.2/tests/cli/superset/sync/dbt/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/cli/superset/sync/dbt/manifest.json` & `preset-cli-0.2.2/tests/cli/superset/sync/dbt/manifest.json`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/cli/superset/sync/dbt/metrics_test.py` & `preset-cli-0.2.2/tests/cli/superset/sync/dbt/metrics_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/cli/superset/sync/native/command_test.py` & `preset-cli-0.2.2/tests/cli/superset/sync/native/command_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tests/lib_test.py` & `preset-cli-0.2.2/tests/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.1/tox.ini` & `preset-cli-0.2.2/tox.ini`

 * *Files identical despite different names*

