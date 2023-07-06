# Comparing `tmp/oenv2config-1.1.0.tar.gz` & `tmp/oenv2config-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oenv2config-1.1.0.tar", last modified: Fri Jun 16 14:20:12 2023, max compression
+gzip compressed data, was "oenv2config-1.2.0.tar", last modified: Thu Jul  6 13:27:30 2023, max compression
```

## Comparing `oenv2config-1.1.0.tar` & `oenv2config-1.2.0.tar`

### file list

```diff
@@ -1,121 +1,122 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.556730 oenv2config-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1885 2023-05-05 10:29:38.000000 oenv2config-1.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-06-14 10:38:37.000000 oenv2config-1.1.0/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.456730 oenv2config-1.1.0/.idea/
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-05-02 08:56:52.000000 oenv2config-1.1.0/.idea/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-05-02 08:56:52.000000 oenv2config-1.1.0/.idea/misc.xml
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-06-14 09:09:25.000000 oenv2config-1.1.0/.idea/modules.xml
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-02 08:56:52.000000 oenv2config-1.1.0/.idea/oenv2config.iml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.460730 oenv2config-1.1.0/.idea/runConfigurations/
--rw-rw-rw-   0 root         (0) root         (0)     1712 2023-06-14 09:09:25.000000 oenv2config-1.1.0/.idea/runConfigurations/Python_tests__no_Odoo_.xml
--rw-rw-rw-   0 root         (0) root         (0)     1565 2023-05-05 10:29:38.000000 oenv2config-1.1.0/.idea/runConfigurations/Python_tests_in_tests_odoo.xml
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-05-02 08:56:52.000000 oenv2config-1.1.0/.idea/vcs.xml
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-05-02 08:56:52.000000 oenv2config-1.1.0/.local-antora-playbook.yml
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-05 10:29:38.000000 oenv2config-1.1.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 10:31:13.000000 oenv2config-1.1.0/.ruff
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-16 14:20:12.556730 oenv2config-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      857 2023-05-02 08:56:52.000000 oenv2config-1.1.0/README.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.460730 oenv2config-1.1.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/antora.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.464730 oenv2config-1.1.0/docs/mkdocs/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/cli.md
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/db_options.md
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/entry.md
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/index.md
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/mappers.md
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/options.md
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/reference.md
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/mkdocs/utils.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.448730 oenv2config-1.1.0/docs/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.464730 oenv2config-1.1.0/docs/modules/ROOT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.500730 oenv2config-1.1.0/docs/modules/ROOT/images/
--rw-rw-rw-   0 root         (0) root         (0)    44111 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/modules/ROOT/images/run_odoo_test.png
--rw-rw-rw-   0 root         (0) root         (0)    35877 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/modules/ROOT/images/run_test.png
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/modules/ROOT/nav.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.504730 oenv2config-1.1.0/docs/modules/ROOT/pages/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/modules/ROOT/pages/antora.adoc
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/modules/ROOT/pages/contribute.adoc
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/modules/ROOT/pages/index.adoc
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.1.0/docs/modules/ROOT/pages/mkdocs.adoc
--rw-rw-rw-   0 root         (0) root         (0)      769 2023-06-09 15:06:52.000000 oenv2config-1.1.0/docs/modules/ROOT/pages/tests.adoc
--rw-rw-rw-   0 root         (0) root         (0)     1878 2023-06-09 15:06:52.000000 oenv2config-1.1.0/docs/modules/ROOT/pages/tests_odoo.adoc
--rwxrwxrwx   0 root         (0) root         (0)      320 2023-05-05 10:29:38.000000 oenv2config-1.1.0/in_docker_test.sh
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-02 08:56:52.000000 oenv2config-1.1.0/mkdocs-plugins.txt
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-05-02 08:56:52.000000 oenv2config-1.1.0/mkdocs.yml
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-05-05 10:29:38.000000 oenv2config-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 14:20:12.556730 oenv2config-1.1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      399 2023-05-02 08:56:52.000000 oenv2config-1.1.0/setup.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.448730 oenv2config-1.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.508730 oenv2config-1.1.0/src/odoo_env_config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.1.0/src/odoo_env_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-16 14:20:12.000000 oenv2config-1.1.0/src/odoo_env_config/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4656 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/api.py
--rw-rw-rw-   0 root         (0) root         (0)     4121 2023-06-14 09:03:06.000000 oenv2config-1.1.0/src/odoo_env_config/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3782 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/entry.py
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-02 08:56:52.000000 oenv2config-1.1.0/src/odoo_env_config/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4853 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/mappers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.448730 oenv2config-1.1.0/src/odoo_env_config/odoo_modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.512730 oenv2config-1.1.0/src/odoo_env_config/odoo_modules/env2config/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-05 10:31:13.000000 oenv2config-1.1.0/src/odoo_env_config/odoo_modules/env2config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-02 08:56:52.000000 oenv2config-1.1.0/src/odoo_env_config/odoo_modules/env2config/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.512730 oenv2config-1.1.0/src/odoo_env_config/odoo_modules/env2config/cli/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-02 08:56:52.000000 oenv2config-1.1.0/src/odoo_env_config/odoo_modules/env2config/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.516730 oenv2config-1.1.0/src/odoo_env_config/section/
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/addons_path_section.py
--rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/db_section.py
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/http_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2155 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/limit_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/log_section.py
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/misc_section.py
--rw-rw-rw-   0 root         (0) root         (0)      830 2023-06-16 12:49:50.000000 oenv2config-1.1.0/src/odoo_env_config/section/s3_section.py
--rw-rw-rw-   0 root         (0) root         (0)      865 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/test_section.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/update_init_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/widemodule_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2326 2023-06-09 15:06:52.000000 oenv2config-1.1.0/src/odoo_env_config/section/worker_section.py
--rw-rw-rw-   0 root         (0) root         (0)    10125 2023-05-02 08:56:52.000000 oenv2config-1.1.0/src/odoo_env_config/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.516730 oenv2config-1.1.0/src/oenv2config.egg-info/
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-16 14:20:12.000000 oenv2config-1.1.0/src/oenv2config.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3285 2023-06-16 14:20:12.000000 oenv2config-1.1.0/src/oenv2config.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 14:20:12.000000 oenv2config-1.1.0/src/oenv2config.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-16 14:20:12.000000 oenv2config-1.1.0/src/oenv2config.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-06-16 14:20:12.000000 oenv2config-1.1.0/src/oenv2config.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-16 14:20:12.000000 oenv2config-1.1.0/src/oenv2config.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.520730 oenv2config-1.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2148 2023-05-05 10:29:38.000000 oenv2config-1.1.0/tests/_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     3154 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_doctests.py
--rw-rw-rw-   0 root         (0) root         (0)     4551 2023-06-09 15:06:52.000000 oenv2config-1.1.0/tests/test_entry.py
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-09 15:06:52.000000 oenv2config-1.1.0/tests/test_libs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.520730 oenv2config-1.1.0/tests/test_mapper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_mapper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9833 2023-06-14 09:03:06.000000 oenv2config-1.1.0/tests/test_mapper/test_mapper_clever_cloud_cellar.py
--rw-rw-rw-   0 root         (0) root         (0)    10835 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_mapper/test_mapper_clever_cloud_postgres.py
--rw-rw-rw-   0 root         (0) root         (0)     6535 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_mapper/test_mapper_odoo_compatibility.py
--rw-rw-rw-   0 root         (0) root         (0)     5002 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_mapper/test_mapper_queue_job.py
--rw-rw-rw-   0 root         (0) root         (0)     3921 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_mapper/test_mapper_redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.524730 oenv2config-1.1.0/tests/test_section/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_section/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-05-05 10:29:38.000000 oenv2config-1.1.0/tests/test_section/test_addons_path_section.py
--rw-rw-rw-   0 root         (0) root         (0)     7581 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_section/test_db_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_section/test_http_section.py
--rw-rw-rw-   0 root         (0) root         (0)     5567 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_section/test_limit_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2489 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_section/test_log_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1389 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_section/test_misc_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2040 2023-06-16 13:07:56.000000 oenv2config-1.1.0/tests/test_section/test_s3_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1989 2023-05-05 10:29:38.000000 oenv2config-1.1.0/tests/test_section/test_test_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1259 2023-05-05 10:29:38.000000 oenv2config-1.1.0/tests/test_section/test_update_init_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_section/test_widemodule_section.py
--rw-rw-rw-   0 root         (0) root         (0)     6727 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/test_section/test_worker_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2436 2023-06-09 15:06:52.000000 oenv2config-1.1.0/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.528730 oenv2config-1.1.0/tests/tests_odoo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/tests_odoo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4906 2023-05-05 10:29:38.000000 oenv2config-1.1.0/tests/tests_odoo/_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:20:12.556730 oenv2config-1.1.0/tests/tests_odoo/profiles/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/tests_odoo/profiles/filestore_s3.env
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/tests_odoo/profiles/filestore_s3_cellar.env
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/tests_odoo/profiles/test_db_clever.env
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-05-02 08:56:52.000000 oenv2config-1.1.0/tests/tests_odoo/profiles/test_db_clever_direct.env
--rw-rw-rw-   0 root         (0) root         (0)     4115 2023-05-05 10:29:38.000000 oenv2config-1.1.0/tests/tests_odoo/test_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.265119 oenv2config-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2023-06-26 12:10:44.000000 oenv2config-1.2.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-06-26 12:10:44.000000 oenv2config-1.2.0/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.257120 oenv2config-1.2.0/.idea/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-06-26 12:10:44.000000 oenv2config-1.2.0/.idea/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-06-26 12:10:44.000000 oenv2config-1.2.0/.idea/misc.xml
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-06-26 12:10:44.000000 oenv2config-1.2.0/.idea/modules.xml
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-06-26 12:10:44.000000 oenv2config-1.2.0/.idea/oenv2config.iml
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-06 13:22:33.000000 oenv2config-1.2.0/.idea/ruff.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.257120 oenv2config-1.2.0/.idea/runConfigurations/
+-rw-rw-rw-   0 root         (0) root         (0)     1712 2023-06-26 12:10:44.000000 oenv2config-1.2.0/.idea/runConfigurations/Python_tests__no_Odoo_.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2023-06-26 12:10:44.000000 oenv2config-1.2.0/.idea/runConfigurations/Python_tests_in_tests_odoo.xml
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-26 12:10:44.000000 oenv2config-1.2.0/.idea/vcs.xml
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-06-26 12:10:44.000000 oenv2config-1.2.0/.local-antora-playbook.yml
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-07-06 13:22:33.000000 oenv2config-1.2.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.0/.ruff
+-rw-r--r--   0 root         (0) root         (0)      182 2023-07-06 13:27:30.265119 oenv2config-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2023-06-26 12:10:44.000000 oenv2config-1.2.0/README.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.257120 oenv2config-1.2.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/antora.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.257120 oenv2config-1.2.0/docs/mkdocs/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/mkdocs/cli.md
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/mkdocs/db_options.md
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/mkdocs/entry.md
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/mkdocs/index.md
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/mkdocs/mappers.md
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/mkdocs/options.md
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/mkdocs/reference.md
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/mkdocs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/mkdocs/utils.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.253119 oenv2config-1.2.0/docs/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.257120 oenv2config-1.2.0/docs/modules/ROOT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.257120 oenv2config-1.2.0/docs/modules/ROOT/images/
+-rw-rw-rw-   0 root         (0) root         (0)    44111 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/modules/ROOT/images/run_odoo_test.png
+-rw-rw-rw-   0 root         (0) root         (0)    35877 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/modules/ROOT/images/run_test.png
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/modules/ROOT/nav.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.261119 oenv2config-1.2.0/docs/modules/ROOT/pages/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/modules/ROOT/pages/antora.adoc
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/modules/ROOT/pages/contribute.adoc
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/modules/ROOT/pages/index.adoc
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/modules/ROOT/pages/mkdocs.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      769 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/modules/ROOT/pages/tests.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     1878 2023-06-26 12:10:44.000000 oenv2config-1.2.0/docs/modules/ROOT/pages/tests_odoo.adoc
+-rwxrwxrwx   0 root         (0) root         (0)      320 2023-06-26 12:10:44.000000 oenv2config-1.2.0/in_docker_test.sh
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-06-26 12:10:44.000000 oenv2config-1.2.0/mkdocs-plugins.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-06-26 12:10:44.000000 oenv2config-1.2.0/mkdocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-07-06 13:22:33.000000 oenv2config-1.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 13:27:30.265119 oenv2config-1.2.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      399 2023-06-26 12:10:44.000000 oenv2config-1.2.0/setup.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.253119 oenv2config-1.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.261119 oenv2config-1.2.0/src/odoo_env_config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-06 13:27:30.000000 oenv2config-1.2.0/src/odoo_env_config/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4656 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4546 2023-06-26 13:17:37.000000 oenv2config-1.2.0/src/odoo_env_config/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3782 2023-07-06 13:22:33.000000 oenv2config-1.2.0/src/odoo_env_config/entry.py
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4853 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/mappers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.253119 oenv2config-1.2.0/src/odoo_env_config/odoo_modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.261119 oenv2config-1.2.0/src/odoo_env_config/odoo_modules/env2config/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/odoo_modules/env2config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/odoo_modules/env2config/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.261119 oenv2config-1.2.0/src/odoo_env_config/odoo_modules/env2config/cli/
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-06 13:22:33.000000 oenv2config-1.2.0/src/odoo_env_config/odoo_modules/env2config/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.261119 oenv2config-1.2.0/src/odoo_env_config/section/
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-07-06 13:22:33.000000 oenv2config-1.2.0/src/odoo_env_config/section/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/section/addons_path_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/section/db_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/section/http_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2155 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/section/limit_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/section/log_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/section/misc_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/section/s3_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/section/test_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/section/update_init_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/section/widemodule_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/section/worker_section.py
+-rw-rw-rw-   0 root         (0) root         (0)    10125 2023-06-26 12:10:44.000000 oenv2config-1.2.0/src/odoo_env_config/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.261119 oenv2config-1.2.0/src/oenv2config.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      182 2023-07-06 13:27:30.000000 oenv2config-1.2.0/src/oenv2config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3300 2023-07-06 13:27:30.000000 oenv2config-1.2.0/src/oenv2config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 13:27:30.000000 oenv2config-1.2.0/src/oenv2config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-06 13:27:30.000000 oenv2config-1.2.0/src/oenv2config.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-07-06 13:27:30.000000 oenv2config-1.2.0/src/oenv2config.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-06 13:27:30.000000 oenv2config-1.2.0/src/oenv2config.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.261119 oenv2config-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2023-07-06 13:22:33.000000 oenv2config-1.2.0/tests/_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5458 2023-07-06 13:22:33.000000 oenv2config-1.2.0/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_doctests.py
+-rw-rw-rw-   0 root         (0) root         (0)     4524 2023-07-06 13:22:33.000000 oenv2config-1.2.0/tests/test_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_libs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.265119 oenv2config-1.2.0/tests/test_mapper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_mapper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9833 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_mapper/test_mapper_clever_cloud_cellar.py
+-rw-rw-rw-   0 root         (0) root         (0)    10835 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_mapper/test_mapper_clever_cloud_postgres.py
+-rw-rw-rw-   0 root         (0) root         (0)     6535 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_mapper/test_mapper_odoo_compatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)     5002 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_mapper/test_mapper_queue_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_mapper/test_mapper_redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.265119 oenv2config-1.2.0/tests/test_section/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_section/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_section/test_addons_path_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     7581 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_section/test_db_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_section/test_http_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     5567 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_section/test_limit_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2489 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_section/test_log_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_section/test_misc_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2040 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_section/test_s3_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1989 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_section/test_test_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_section/test_update_init_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_section/test_widemodule_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     6727 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_section/test_worker_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2436 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.265119 oenv2config-1.2.0/tests/tests_odoo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/tests_odoo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4907 2023-07-06 13:22:33.000000 oenv2config-1.2.0/tests/tests_odoo/_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 13:27:30.265119 oenv2config-1.2.0/tests/tests_odoo/profiles/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/tests_odoo/profiles/filestore_s3.env
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/tests_odoo/profiles/filestore_s3_cellar.env
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/tests_odoo/profiles/test_db_clever.env
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-06-26 12:10:44.000000 oenv2config-1.2.0/tests/tests_odoo/profiles/test_db_clever_direct.env
+-rw-rw-rw-   0 root         (0) root         (0)     4117 2023-07-06 13:22:33.000000 oenv2config-1.2.0/tests/tests_odoo/test_base.py
```

### Comparing `oenv2config-1.1.0/.gitignore` & `oenv2config-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/.gitlab-ci.yml` & `oenv2config-1.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/.idea/oenv2config.iml` & `oenv2config-1.2.0/.idea/oenv2config.iml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/.idea/runConfigurations/Python_tests__no_Odoo_.xml` & `oenv2config-1.2.0/.idea/runConfigurations/Python_tests__no_Odoo_.xml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/.idea/runConfigurations/Python_tests_in_tests_odoo.xml` & `oenv2config-1.2.0/.idea/runConfigurations/Python_tests_in_tests_odoo.xml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/.pre-commit-config.yaml` & `oenv2config-1.2.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,18 @@
         exclude: .gitlab-ci.yml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
+  - repo: https://github.com/pycqa/isort
+    rev: 5.12.0
+    hooks:
+      - id: isort
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: 'v0.0.263'
     hooks:
       - id: ruff
   - repo: https://gitlab.com/devopshq/gitlab-ci-linter
     rev: v1.0.3
     hooks:
```

### Comparing `oenv2config-1.1.0/README.adoc` & `oenv2config-1.2.0/README.adoc`

 * *Files 12% similar despite different names*

```diff
@@ -24,16 +24,20 @@
 - [ ] Add documentation How to test
 - [ ] Add documentation How to build `mkdocs`
 - [ ] Add documentation How to test the `cli`
 
 == Contributing
 
 == Launch Test
+`python -m unittest discover`
 
 === Launch test with Odoo
 
 == Documentation
 === mkdocs
 Installation de mkdocs. Voir https://gitlab.ndp-systemes.fr/documentation/docs[la documentation] de ndp sur mkdocs.
 
 === Antora
 Installation d'antora. Voir https://gitlab.ndp-systemes.fr/documentation/docs-antora[la documentation] de ndp.
+
+=== Developper
+To test the CLI locally, ` pip install -e .` et `odoo-env2config --odoo-bin /toto --dest /caraibe`
```

### Comparing `oenv2config-1.1.0/docs/modules/ROOT/images/run_odoo_test.png` & `oenv2config-1.2.0/docs/modules/ROOT/images/run_odoo_test.png`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/docs/modules/ROOT/images/run_test.png` & `oenv2config-1.2.0/docs/modules/ROOT/images/run_test.png`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/docs/modules/ROOT/pages/tests.adoc` & `oenv2config-1.2.0/docs/modules/ROOT/pages/tests.adoc`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/docs/modules/ROOT/pages/tests_odoo.adoc` & `oenv2config-1.2.0/docs/modules/ROOT/pages/tests_odoo.adoc`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/mkdocs.yml` & `oenv2config-1.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/pyproject.toml` & `oenv2config-1.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -32,7 +32,10 @@
 
 
 [tool.black]
 line-length = 120
 
 [tool.ruff]
 line-length = 120
+
+[tool.isort]
+profile = "black"
```

### Comparing `oenv2config-1.1.0/src/odoo_env_config/api.py` & `oenv2config-1.2.0/src/odoo_env_config/api.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/src/odoo_env_config/cli.py` & `oenv2config-1.2.0/src/odoo_env_config/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,26 @@
 from typing import List
 
 from dotenv import dotenv_values
 
 from . import api, entry
 
 
+class SplitArgs(argparse.Action):
+    def __call__(self, parser, namespace, values, option_string=None):
+        # start or ending comma removed to avoid empty value in list
+        setattr(namespace, self.dest, getattr(namespace, self.dest, []) + list(filter(None, values.split(","))))
+
+
 def get_odoo_cmd_parser() -> argparse.ArgumentParser:
     p = argparse.ArgumentParser()
     p.add_argument("--profile", action="append", dest="profiles", default=[], help="profile to use")
+    p.add_argument(
+        "--profiles", action=SplitArgs, dest="profiles", default=[], help="profiles to use (comma separated)"
+    )
     p.add_argument("--dest", dest="config_dest", help="Path to odoo configuration file")
     return p
 
 
 class OdooCommand:
     """
     This contains a new OdooCommand named `env2config`
```

### Comparing `oenv2config-1.1.0/src/odoo_env_config/entry.py` & `oenv2config-1.2.0/src/odoo_env_config/entry.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from .section import (
     AddonsPathConfigSection,
     DatabaseOdooConfigSection,
     HttpOdooConfigSection,
     LimitOdooConfigSection,
     LoggerSection,
     MiscSection,
+    S3Section,
     ServerWideModuleConfigSection,
     TestOdooConfigSection,
     UpdateInstallSection,
     WorkersOdooConfigSection,
-    S3Section,
 )
 
 Section = TypeVar("Section", bound=api.EnvConfigSection)
 
 CONVERTER: Set[Type[Section]] = {
     AddonsPathConfigSection,
     DatabaseOdooConfigSection,
```

### Comparing `oenv2config-1.1.0/src/odoo_env_config/mappers.py` & `oenv2config-1.2.0/src/odoo_env_config/mappers.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/src/odoo_env_config/odoo_modules/env2config/__manifest__.py` & `oenv2config-1.2.0/src/odoo_env_config/odoo_modules/env2config/__manifest__.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/src/odoo_env_config/section/__init__.py` & `oenv2config-1.2.0/src/odoo_env_config/section/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 ]
 from .addons_path_section import AddonsPathConfigSection
 from .db_section import DatabaseOdooConfigSection
 from .http_section import HttpOdooConfigSection
 from .limit_section import LimitOdooConfigSection
 from .log_section import LoggerSection
 from .misc_section import MiscSection
+from .s3_section import S3Section
 from .test_section import TestOdooConfigSection
 from .update_init_section import UpdateInstallSection
 from .widemodule_section import ServerWideModuleConfigSection
 from .worker_section import WorkersOdooConfigSection
-from .s3_section import S3Section
```

### Comparing `oenv2config-1.1.0/src/odoo_env_config/section/addons_path_section.py` & `oenv2config-1.2.0/src/odoo_env_config/section/addons_path_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/src/odoo_env_config/section/db_section.py` & `oenv2config-1.2.0/src/odoo_env_config/section/db_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/src/odoo_env_config/section/http_section.py` & `oenv2config-1.2.0/src/odoo_env_config/section/http_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/src/odoo_env_config/section/limit_section.py` & `oenv2config-1.2.0/src/odoo_env_config/section/limit_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/src/odoo_env_config/section/log_section.py` & `oenv2config-1.2.0/src/odoo_env_config/section/log_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/src/odoo_env_config/section/misc_section.py` & `oenv2config-1.2.0/src/odoo_env_config/section/misc_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/src/odoo_env_config/section/s3_section.py` & `oenv2config-1.2.0/src/odoo_env_config/section/s3_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/src/odoo_env_config/section/test_section.py` & `oenv2config-1.2.0/src/odoo_env_config/section/test_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/src/odoo_env_config/section/update_init_section.py` & `oenv2config-1.2.0/src/odoo_env_config/section/update_init_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/src/odoo_env_config/section/widemodule_section.py` & `oenv2config-1.2.0/src/odoo_env_config/section/widemodule_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/src/odoo_env_config/section/worker_section.py` & `oenv2config-1.2.0/src/odoo_env_config/section/worker_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/src/odoo_env_config/utils.py` & `oenv2config-1.2.0/src/odoo_env_config/utils.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/src/oenv2config.egg-info/SOURCES.txt` & `oenv2config-1.2.0/src/oenv2config.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 mkdocs.yml
 pyproject.toml
 setup.sh
 .idea/.gitignore
 .idea/misc.xml
 .idea/modules.xml
 .idea/oenv2config.iml
+.idea/ruff.xml
 .idea/vcs.xml
 .idea/runConfigurations/Python_tests__no_Odoo_.xml
 .idea/runConfigurations/Python_tests_in_tests_odoo.xml
 docs/antora.yml
 docs/mkdocs/cli.md
 docs/mkdocs/db_options.md
 docs/mkdocs/entry.md
```

### Comparing `oenv2config-1.1.0/tests/_decorators.py` & `oenv2config-1.2.0/tests/_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import unittest
+
 from odoo_env_config.api import Env
 
 try:
     ODOO_VERSION = int(float(os.getenv("ODOO_VERSION", "0")))
 except ValueError:
     ODOO_VERSION = None
```

### Comparing `oenv2config-1.1.0/tests/test_entry.py` & `oenv2config-1.2.0/tests/test_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf8 -*-
 import unittest
 
-from odoo_env_config import entry
-from odoo_env_config import api
+from odoo_env_config import api, entry
 from odoo_env_config.section.db_section import DatabaseOdooConfigSection
 
 
 class TestOdooConfig(unittest.TestCase):
     def test_no_config(self):
         config = entry.env_to_odoo_args()
         self.assertFalse(config)
```

### Comparing `oenv2config-1.1.0/tests/test_libs.py` & `oenv2config-1.2.0/tests/test_libs.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_mapper/test_mapper_clever_cloud_cellar.py` & `oenv2config-1.2.0/tests/test_mapper/test_mapper_clever_cloud_cellar.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_mapper/test_mapper_clever_cloud_postgres.py` & `oenv2config-1.2.0/tests/test_mapper/test_mapper_clever_cloud_postgres.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_mapper/test_mapper_odoo_compatibility.py` & `oenv2config-1.2.0/tests/test_mapper/test_mapper_odoo_compatibility.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_mapper/test_mapper_queue_job.py` & `oenv2config-1.2.0/tests/test_mapper/test_mapper_queue_job.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_mapper/test_mapper_redis.py` & `oenv2config-1.2.0/tests/test_mapper/test_mapper_redis.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_section/test_addons_path_section.py` & `oenv2config-1.2.0/tests/test_section/test_addons_path_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_section/test_db_section.py` & `oenv2config-1.2.0/tests/test_section/test_db_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_section/test_http_section.py` & `oenv2config-1.2.0/tests/test_section/test_http_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_section/test_limit_section.py` & `oenv2config-1.2.0/tests/test_section/test_limit_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_section/test_log_section.py` & `oenv2config-1.2.0/tests/test_section/test_log_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_section/test_misc_section.py` & `oenv2config-1.2.0/tests/test_section/test_misc_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_section/test_s3_section.py` & `oenv2config-1.2.0/tests/test_section/test_s3_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_section/test_test_section.py` & `oenv2config-1.2.0/tests/test_section/test_test_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_section/test_update_init_section.py` & `oenv2config-1.2.0/tests/test_section/test_update_init_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_section/test_widemodule_section.py` & `oenv2config-1.2.0/tests/test_section/test_widemodule_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_section/test_worker_section.py` & `oenv2config-1.2.0/tests/test_section/test_worker_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/test_utils.py` & `oenv2config-1.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.1.0/tests/tests_odoo/_helpers.py` & `oenv2config-1.2.0/tests/tests_odoo/_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import configparser
 import os
 import unittest
 import uuid
 from os.path import join as pjoin
 from typing import Any, Dict, List, Tuple
+
 from odoo_env_config import api, cli
 
 
 def _try_find_addons_info() -> Tuple[str, int]:
     """
     Try to find the odoo path to be able to run the test inside Odoo on local host or inside a odoo docker image
```

### Comparing `oenv2config-1.1.0/tests/tests_odoo/test_base.py` & `oenv2config-1.2.0/tests/tests_odoo/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import unittest
+
 from tests import _decorators
-from ._helpers import create_config, assertParser
+
+from ._helpers import assertParser, create_config
 
 
 @_decorators.SkipUnless.env_odoo
 class AllOdooVersionTest(unittest.TestCase):
     def test_db(self):
         parser = create_config()
         self.assertFalse(parser.getboolean("options", "db_host"))
```

