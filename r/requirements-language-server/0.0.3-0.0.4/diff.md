# Comparing `tmp/requirements-language-server-0.0.3.tar.gz` & `tmp/requirements-language-server-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requirements-language-server-0.0.3.tar", last modified: Tue Jun 20 15:11:55 2023, max compression
+gzip compressed data, was "requirements-language-server-0.0.4.tar", last modified: Thu Jul  6 11:51:43 2023, max compression
```

## Comparing `requirements-language-server-0.0.3.tar` & `requirements-language-server-0.0.4.tar`

### file list

```diff
@@ -1,58 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.838108 requirements-language-server-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.834108 requirements-language-server-0.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.834108 requirements-language-server-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-06-20 15:11:55.838108 requirements-language-server-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.834108 requirements-language-server-0.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.834108 requirements-language-server-0.0.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/docs/api/requirements-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.834108 requirements-language-server-0.0.3/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/docs/resources/requirements.md
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.834108 requirements-language-server-0.0.3/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.834108 requirements-language-server-0.0.3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/scripts/generate-api.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      179 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/scripts/generate-requirements.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:11:55.838108 requirements-language-server-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.830108 requirements-language-server-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.834108 requirements-language-server-0.0.3/src/requirements_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/src/requirements_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/src/requirements_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 15:11:55.000000 requirements-language-server-0.0.3/src/requirements_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/src/requirements_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.830108 requirements-language-server-0.0.3/src/requirements_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.838108 requirements-language-server-0.0.3/src/requirements_language_server/assets/jinja2/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/src/requirements_language_server/assets/jinja2/template.md.j2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/src/requirements_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/src/requirements_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.838108 requirements-language-server-0.0.3/src/requirements_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-06-20 15:11:55.000000 requirements-language-server-0.0.3/src/requirements_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-20 15:11:55.000000 requirements-language-server-0.0.3/src/requirements_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:11:55.000000 requirements-language-server-0.0.3/src/requirements_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-20 15:11:55.000000 requirements-language-server-0.0.3/src/requirements_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-20 15:11:55.000000 requirements-language-server-0.0.3/src/requirements_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-20 15:11:55.000000 requirements-language-server-0.0.3/src/requirements_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.838108 requirements-language-server-0.0.3/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.838108 requirements-language-server-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/tests/api_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/tests/requirements.txt.in
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/tests/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:43.974264 requirements-language-server-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:43.966264 requirements-language-server-0.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:43.966264 requirements-language-server-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-07-06 11:51:43.974264 requirements-language-server-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:43.966264 requirements-language-server-0.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:43.970264 requirements-language-server-0.0.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/docs/api/requirements-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:43.970264 requirements-language-server-0.0.4/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:43.970264 requirements-language-server-0.0.4/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:43.970264 requirements-language-server-0.0.4/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/scripts/generate-api.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/scripts/generate-requirements.md.pl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:43.970264 requirements-language-server-0.0.4/sdist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-06 11:51:43.000000 requirements-language-server-0.0.4/sdist/_requirements-language-server
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-06 11:51:43.000000 requirements-language-server-0.0.4/sdist/requirements-language-server
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-06 11:51:43.000000 requirements-language-server-0.0.4/sdist/requirements-language-server.1
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:51:43.974264 requirements-language-server-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:43.966264 requirements-language-server-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:43.970264 requirements-language-server-0.0.4/src/requirements_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/src/requirements_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/src/requirements_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-06 11:51:43.000000 requirements-language-server-0.0.4/src/requirements_language_server/_metainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 11:51:43.000000 requirements-language-server-0.0.4/src/requirements_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/src/requirements_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:43.966264 requirements-language-server-0.0.4/src/requirements_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:43.974264 requirements-language-server-0.0.4/src/requirements_language_server/assets/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/src/requirements_language_server/assets/jinja2/template.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/src/requirements_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/src/requirements_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:43.974264 requirements-language-server-0.0.4/src/requirements_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-07-06 11:51:43.000000 requirements-language-server-0.0.4/src/requirements_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-06 11:51:43.000000 requirements-language-server-0.0.4/src/requirements_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:51:43.000000 requirements-language-server-0.0.4/src/requirements_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-06 11:51:43.000000 requirements-language-server-0.0.4/src/requirements_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 11:51:43.000000 requirements-language-server-0.0.4/src/requirements_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 11:51:43.000000 requirements-language-server-0.0.4/src/requirements_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:43.974264 requirements-language-server-0.0.4/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:51:43.974264 requirements-language-server-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/tests/api_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/tests/requirements.txt.in
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-06 11:51:25.000000 requirements-language-server-0.0.4/tests/server_test.py
```

### Comparing `requirements-language-server-0.0.3/.github/workflows/main.yml` & `requirements-language-server-0.0.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.3/.gitignore` & `requirements-language-server-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.3/.pre-commit-config.yaml` & `requirements-language-server-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.3/LICENSE` & `requirements-language-server-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.3/PKG-INFO` & `requirements-language-server-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirements-language-server
-Version: 0.0.3
+Version: 0.0.4
 Summary: requirements language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://requirements-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/requirements-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/requirements-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/requirements-language-server
```

### Comparing `requirements-language-server-0.0.3/README.md` & `requirements-language-server-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.3/docs/conf.py` & `requirements-language-server-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.3/docs/resources/configure.md` & `requirements-language-server-0.0.4/docs/resources/configure.md`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.3/docs/resources/install.md` & `requirements-language-server-0.0.4/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.3/flake.nix` & `requirements-language-server-0.0.4/flake.nix`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.3/pyproject.toml` & `requirements-language-server-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [build-system]
-# FIXME: setuptools-generate stop setuptools_scm working
 requires = [
   "setuptools_scm[toml] >= 6.2",
-  # "setuptools-generate >= 0.0.6",
-  # "platformdirs",
+  "setuptools-generate >= 0.0.6",
+  "platformdirs",
 ]
 build-backend = "setuptools.build_meta"
 
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [project]
 name = "requirements-language-server"
 description = "requirements language server"
@@ -50,18 +49,18 @@
 
 [project.scripts]
 requirements-language-server = "requirements_language_server.__main__:main"
 
 [tool.setuptools.package-data]
 requirements_language_server = ["py.typed", "assets/**"]
 
-# [tool.setuptools.data-files]
-# "share/man/man1" = ["sdist/requirements-language-server.1"]
-# "share/bash-completion/completions" = ["sdist/requirements-language-server"]
-# "share/zsh/site-functions" = ["sdist/_requirements-language-server"]
+[tool.setuptools.data-files]
+"share/man/man1" = ["sdist/requirements-language-server.1"]
+"share/bash-completion/completions" = ["sdist/requirements-language-server"]
+"share/zsh/site-functions" = ["sdist/_requirements-language-server"]
 
 [tool.setuptools.dynamic.dependencies]
 file = "requirements.txt"
 
 # begin: scripts/update-pyproject.toml.pl
 [tool.setuptools.dynamic.optional-dependencies.dev]
 file = "requirements/dev.txt"
```

### Comparing `requirements-language-server-0.0.3/src/requirements_language_server/__init__.py` & `requirements-language-server-0.0.4/src/requirements_language_server/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 r"""Provide ``__version__`` for
 `importlib.metadata.version() <https://docs.python.org/3/library/importlib.metadata.html#distribution-versions>`_.
 """
 import os
 
 from platformdirs import user_cache_dir, user_config_dir
 
-from ._version import __version__, __version_tuple__  # type: ignore
+try:
+    from ._version import __version__, __version_tuple__  # type: ignore
+except ImportError:  # for setuptools-generate
+    __version__ = "rolling"
+    __version_tuple__ = (0, 0, 0, __version__, "")
 
 __all__ = ["__version__", "__version_tuple__"]
 
 NOT_FOUND = "Not found installed package!"
 # https://pip.pypa.io/en/stable/reference/requirements-file-format/#supported-options
 WHITELIST = [
     "-i",
```

### Comparing `requirements-language-server-0.0.3/src/requirements_language_server/__main__.py` & `requirements-language-server-0.0.4/src/requirements_language_server/__main__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 
 def get_parser() -> ArgumentParser:
     r"""Get a parser for unit test."""
     parser = ArgumentParser(
         epilog=EPILOG,
         formatter_class=RawDescriptionHelpFormatter,
     )
+    with suppress(ImportError):
+        import shtab
+
+        shtab.add_argument_to(parser)
     parser.add_argument("--version", version=VERSION, action="version")
     parser.add_argument(
         "--print-config",
         choices=["template", "cache", "all"],
         help="print config value",
     )
     parser.add_argument(
         "--generate-cache",
         action="store_true",
         help="generate cache",
     )
-    with suppress(ImportError):
-        import shtab
-
-        shtab.add_argument_to(parser)
     return parser
 
 
 def main() -> None:
     r"""Parse arguments and provide shell completions."""
     parser = get_parser()
     args = parser.parse_args()
```

### Comparing `requirements-language-server-0.0.3/src/requirements_language_server/api.py` & `requirements-language-server-0.0.4/src/requirements_language_server/api.py`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.3/src/requirements_language_server/server.py` & `requirements-language-server-0.0.4/src/requirements_language_server/server.py`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.3/src/requirements_language_server.egg-info/PKG-INFO` & `requirements-language-server-0.0.4/src/requirements_language_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirements-language-server
-Version: 0.0.3
+Version: 0.0.4
 Summary: requirements language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://requirements-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/requirements-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/requirements-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/requirements-language-server
```

### Comparing `requirements-language-server-0.0.3/src/requirements_language_server.egg-info/SOURCES.txt` & `requirements-language-server-0.0.4/src/requirements_language_server.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,16 +16,20 @@
 docs/api/requirements-language-server.md
 docs/resources/configure.md
 docs/resources/install.md
 docs/resources/requirements.md
 requirements/dev.txt
 scripts/generate-api.md.pl
 scripts/generate-requirements.md.pl
+sdist/_requirements-language-server
+sdist/requirements-language-server
+sdist/requirements-language-server.1
 src/requirements_language_server/__init__.py
 src/requirements_language_server/__main__.py
+src/requirements_language_server/_metainfo.py
 src/requirements_language_server/_version.py
 src/requirements_language_server/api.py
 src/requirements_language_server/py.typed
 src/requirements_language_server/server.py
 src/requirements_language_server.egg-info/PKG-INFO
 src/requirements_language_server.egg-info/SOURCES.txt
 src/requirements_language_server.egg-info/dependency_links.txt
```

