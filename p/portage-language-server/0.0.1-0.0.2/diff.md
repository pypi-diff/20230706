# Comparing `tmp/portage-language-server-0.0.1.tar.gz` & `tmp/portage-language-server-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portage-language-server-0.0.1.tar", last modified: Wed Jun 21 12:33:47 2023, max compression
+gzip compressed data, was "portage-language-server-0.0.2.tar", last modified: Thu Jul  6 11:58:37 2023, max compression
```

## Comparing `portage-language-server-0.0.1.tar` & `portage-language-server-0.0.2.tar`

### file list

```diff
@@ -1,57 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:47.685635 portage-language-server-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:47.681635 portage-language-server-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:47.681635 portage-language-server-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-06-21 12:33:47.685635 portage-language-server-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:47.681635 portage-language-server-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:47.681635 portage-language-server-0.0.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/docs/api/portage-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:47.681635 portage-language-server-0.0.1/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/docs/resources/requirements.md
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:47.681635 portage-language-server-0.0.1/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/requirements/cache.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:47.681635 portage-language-server-0.0.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/scripts/generate-api.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/scripts/generate-requirements.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 12:33:47.685635 portage-language-server-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:47.681635 portage-language-server-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:47.681635 portage-language-server-0.0.1/src/portage_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/src/portage_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/src/portage_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 12:33:47.000000 portage-language-server-0.0.1/src/portage_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/src/portage_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:47.681635 portage-language-server-0.0.1/src/portage_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:47.685635 portage-language-server-0.0.1/src/portage_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)   110635 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/src/portage_language_server/assets/json/portage.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/src/portage_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/src/portage_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:47.685635 portage-language-server-0.0.1/src/portage_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-06-21 12:33:47.000000 portage-language-server-0.0.1/src/portage_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-21 12:33:47.000000 portage-language-server-0.0.1/src/portage_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:33:47.000000 portage-language-server-0.0.1/src/portage_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-21 12:33:47.000000 portage-language-server-0.0.1/src/portage_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 12:33:47.000000 portage-language-server-0.0.1/src/portage_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-21 12:33:47.000000 portage-language-server-0.0.1/src/portage_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:47.685635 portage-language-server-0.0.1/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:47.685635 portage-language-server-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-21 12:33:37.000000 portage-language-server-0.0.1/tests/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:37.353920 portage-language-server-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:37.349920 portage-language-server-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:37.349920 portage-language-server-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-07-06 11:58:37.353920 portage-language-server-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:37.349920 portage-language-server-0.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:37.353920 portage-language-server-0.0.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/docs/api/portage-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:37.353920 portage-language-server-0.0.2/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:37.353920 portage-language-server-0.0.2/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/requirements/cache.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:37.353920 portage-language-server-0.0.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/scripts/generate-api.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/scripts/generate-requirements.md.pl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:37.353920 portage-language-server-0.0.2/sdist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-06 11:58:37.000000 portage-language-server-0.0.2/sdist/_portage-language-server
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-06 11:58:37.000000 portage-language-server-0.0.2/sdist/portage-language-server
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-06 11:58:37.000000 portage-language-server-0.0.2/sdist/portage-language-server.1
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:58:37.353920 portage-language-server-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:37.349920 portage-language-server-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:37.353920 portage-language-server-0.0.2/src/portage_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/src/portage_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/src/portage_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-06 11:58:37.000000 portage-language-server-0.0.2/src/portage_language_server/_metainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 11:58:37.000000 portage-language-server-0.0.2/src/portage_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/src/portage_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:37.349920 portage-language-server-0.0.2/src/portage_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:37.353920 portage-language-server-0.0.2/src/portage_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)   110635 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/src/portage_language_server/assets/json/portage.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/src/portage_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/src/portage_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:37.353920 portage-language-server-0.0.2/src/portage_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-07-06 11:58:37.000000 portage-language-server-0.0.2/src/portage_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-06 11:58:37.000000 portage-language-server-0.0.2/src/portage_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:58:37.000000 portage-language-server-0.0.2/src/portage_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-06 11:58:37.000000 portage-language-server-0.0.2/src/portage_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 11:58:37.000000 portage-language-server-0.0.2/src/portage_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 11:58:37.000000 portage-language-server-0.0.2/src/portage_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:37.353920 portage-language-server-0.0.2/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:58:37.353920 portage-language-server-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-06 11:58:24.000000 portage-language-server-0.0.2/tests/server_test.py
```

### Comparing `portage-language-server-0.0.1/.github/workflows/main.yml` & `portage-language-server-0.0.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `portage-language-server-0.0.1/.gitignore` & `portage-language-server-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `portage-language-server-0.0.1/.pre-commit-config.yaml` & `portage-language-server-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `portage-language-server-0.0.1/LICENSE` & `portage-language-server-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `portage-language-server-0.0.1/PKG-INFO` & `portage-language-server-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portage-language-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: portage language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://portage-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/portage-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/portage-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/portage-language-server
```

### Comparing `portage-language-server-0.0.1/README.md` & `portage-language-server-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `portage-language-server-0.0.1/docs/conf.py` & `portage-language-server-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `portage-language-server-0.0.1/docs/resources/configure.md` & `portage-language-server-0.0.2/docs/resources/configure.md`

 * *Files identical despite different names*

### Comparing `portage-language-server-0.0.1/docs/resources/install.md` & `portage-language-server-0.0.2/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `portage-language-server-0.0.1/flake.nix` & `portage-language-server-0.0.2/flake.nix`

 * *Files identical despite different names*

### Comparing `portage-language-server-0.0.1/pyproject.toml` & `portage-language-server-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 [build-system]
-# FIXME: setuptools-generate stop setuptools_scm working
-requires = [
-  "setuptools_scm[toml] >= 6.2",
-  # "setuptools-generate >= 0.0.6",
-]
+requires = ["setuptools_scm[toml] >= 6.2", "setuptools-generate >= 0.0.6"]
 build-backend = "setuptools.build_meta"
 
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [project]
 name = "portage-language-server"
 description = "portage language server"
 readme = "README.md"
@@ -49,18 +45,18 @@
 
 [project.scripts]
 portage-language-server = "portage_language_server.__main__:main"
 
 [tool.setuptools.package-data]
 portage_language_server = ["py.typed", "assets/**"]
 
-# [tool.setuptools.data-files]
-# "share/man/man1" = ["sdist/portage-language-server.1"]
-# "share/bash-completion/completions" = ["sdist/portage-language-server"]
-# "share/zsh/site-functions" = ["sdist/_portage-language-server"]
+[tool.setuptools.data-files]
+"share/man/man1" = ["sdist/portage-language-server.1"]
+"share/bash-completion/completions" = ["sdist/portage-language-server"]
+"share/zsh/site-functions" = ["sdist/_portage-language-server"]
 
 [tool.setuptools.dynamic.dependencies]
 file = "requirements.txt"
 
 # begin: scripts/update-pyproject.toml.pl
 [tool.setuptools.dynamic.optional-dependencies.dev]
 file = "requirements/dev.txt"
```

### Comparing `portage-language-server-0.0.1/src/portage_language_server/__main__.py` & `portage-language-server-0.0.2/src/portage_language_server/__main__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
 def get_parser():
     r"""Get a parser for unit test."""
     parser = ArgumentParser(
         epilog=EPILOG,
         formatter_class=RawDescriptionHelpFormatter,
     )
-    parser.add_argument("--version", version=VERSION, action="version")
     with suppress(ImportError):
         import shtab
 
         shtab.add_argument_to(parser)
+    parser.add_argument("--version", version=VERSION, action="version")
     return parser
 
 
 def main():
     r"""Parse arguments and provide shell completions."""
     parser = get_parser()
     parser.parse_args()
```

### Comparing `portage-language-server-0.0.1/src/portage_language_server/api.py` & `portage-language-server-0.0.2/src/portage_language_server/api.py`

 * *Files identical despite different names*

### Comparing `portage-language-server-0.0.1/src/portage_language_server/assets/json/portage.json` & `portage-language-server-0.0.2/src/portage_language_server/assets/json/portage.json`

 * *Files identical despite different names*

### Comparing `portage-language-server-0.0.1/src/portage_language_server/server.py` & `portage-language-server-0.0.2/src/portage_language_server/server.py`

 * *Files identical despite different names*

### Comparing `portage-language-server-0.0.1/src/portage_language_server.egg-info/PKG-INFO` & `portage-language-server-0.0.2/src/portage_language_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portage-language-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: portage language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://portage-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/portage-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/portage-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/portage-language-server
```

### Comparing `portage-language-server-0.0.1/src/portage_language_server.egg-info/SOURCES.txt` & `portage-language-server-0.0.2/src/portage_language_server.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -17,16 +17,20 @@
 docs/resources/configure.md
 docs/resources/install.md
 docs/resources/requirements.md
 requirements/cache.txt
 requirements/dev.txt
 scripts/generate-api.md.pl
 scripts/generate-requirements.md.pl
+sdist/_portage-language-server
+sdist/portage-language-server
+sdist/portage-language-server.1
 src/portage_language_server/__init__.py
 src/portage_language_server/__main__.py
+src/portage_language_server/_metainfo.py
 src/portage_language_server/_version.py
 src/portage_language_server/api.py
 src/portage_language_server/py.typed
 src/portage_language_server/server.py
 src/portage_language_server.egg-info/PKG-INFO
 src/portage_language_server.egg-info/SOURCES.txt
 src/portage_language_server.egg-info/dependency_links.txt
```

