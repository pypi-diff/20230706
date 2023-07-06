# Comparing `tmp/termux-language-server-0.0.1.tar.gz` & `tmp/termux-language-server-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termux-language-server-0.0.1.tar", last modified: Tue Jun 20 13:51:27 2023, max compression
+gzip compressed data, was "termux-language-server-0.0.2.tar", last modified: Thu Jul  6 11:53:32 2023, max compression
```

## Comparing `termux-language-server-0.0.1.tar` & `termux-language-server-0.0.2.tar`

### file list

```diff
@@ -1,57 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:51:27.369076 termux-language-server-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:51:27.361076 termux-language-server-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:51:27.361076 termux-language-server-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-20 13:51:27.365076 termux-language-server-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:51:27.361076 termux-language-server-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:51:27.361076 termux-language-server-0.0.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/docs/api/termux-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:51:27.361076 termux-language-server-0.0.1/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/docs/resources/requirements.md
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:51:27.361076 termux-language-server-0.0.1/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/requirements/web.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:51:27.365076 termux-language-server-0.0.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/scripts/generate-api.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      179 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/scripts/generate-requirements.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:51:27.369076 termux-language-server-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:51:27.357076 termux-language-server-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:51:27.365076 termux-language-server-0.0.1/src/termux_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/src/termux_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/src/termux_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 13:51:27.000000 termux-language-server-0.0.1/src/termux_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/src/termux_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:51:27.357076 termux-language-server-0.0.1/src/termux_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:51:27.365076 termux-language-server-0.0.1/src/termux_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/src/termux_language_server/assets/json/termux.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/src/termux_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/src/termux_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:51:27.365076 termux-language-server-0.0.1/src/termux_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-20 13:51:27.000000 termux-language-server-0.0.1/src/termux_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-20 13:51:27.000000 termux-language-server-0.0.1/src/termux_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:51:27.000000 termux-language-server-0.0.1/src/termux_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-20 13:51:27.000000 termux-language-server-0.0.1/src/termux_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 13:51:27.000000 termux-language-server-0.0.1/src/termux_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 13:51:27.000000 termux-language-server-0.0.1/src/termux_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:51:27.365076 termux-language-server-0.0.1/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:51:27.365076 termux-language-server-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-20 13:51:10.000000 termux-language-server-0.0.1/tests/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:32.358362 termux-language-server-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:32.350362 termux-language-server-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:32.350362 termux-language-server-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-06 11:53:32.358362 termux-language-server-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:32.350362 termux-language-server-0.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:32.350362 termux-language-server-0.0.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/docs/api/termux-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:32.350362 termux-language-server-0.0.2/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:32.350362 termux-language-server-0.0.2/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/requirements/web.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:32.354362 termux-language-server-0.0.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/scripts/generate-api.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/scripts/generate-requirements.md.pl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:32.354362 termux-language-server-0.0.2/sdist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-06 11:53:32.000000 termux-language-server-0.0.2/sdist/_termux-language-server
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-06 11:53:32.000000 termux-language-server-0.0.2/sdist/termux-language-server
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-06 11:53:32.000000 termux-language-server-0.0.2/sdist/termux-language-server.1
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:53:32.358362 termux-language-server-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:32.346362 termux-language-server-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:32.354362 termux-language-server-0.0.2/src/termux_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/src/termux_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/src/termux_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-06 11:53:32.000000 termux-language-server-0.0.2/src/termux_language_server/_metainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 11:53:32.000000 termux-language-server-0.0.2/src/termux_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/src/termux_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:32.346362 termux-language-server-0.0.2/src/termux_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:32.354362 termux-language-server-0.0.2/src/termux_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/src/termux_language_server/assets/json/termux.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/src/termux_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/src/termux_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:32.354362 termux-language-server-0.0.2/src/termux_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-06 11:53:32.000000 termux-language-server-0.0.2/src/termux_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-06 11:53:32.000000 termux-language-server-0.0.2/src/termux_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:53:32.000000 termux-language-server-0.0.2/src/termux_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-06 11:53:32.000000 termux-language-server-0.0.2/src/termux_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 11:53:32.000000 termux-language-server-0.0.2/src/termux_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 11:53:32.000000 termux-language-server-0.0.2/src/termux_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:32.358362 termux-language-server-0.0.2/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:53:32.358362 termux-language-server-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-06 11:53:19.000000 termux-language-server-0.0.2/tests/server_test.py
```

### Comparing `termux-language-server-0.0.1/.github/workflows/main.yml` & `termux-language-server-0.0.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.1/.gitignore` & `termux-language-server-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.1/.pre-commit-config.yaml` & `termux-language-server-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.1/LICENSE` & `termux-language-server-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.1/PKG-INFO` & `termux-language-server-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termux-language-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: termux language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://termux-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/termux-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/termux-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/termux-language-server
```

### Comparing `termux-language-server-0.0.1/README.md` & `termux-language-server-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.1/docs/conf.py` & `termux-language-server-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.1/docs/resources/configure.md` & `termux-language-server-0.0.2/docs/resources/configure.md`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.1/docs/resources/install.md` & `termux-language-server-0.0.2/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.1/flake.nix` & `termux-language-server-0.0.2/flake.nix`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.1/pyproject.toml` & `termux-language-server-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 [build-system]
-# FIXME: setuptools-generate stop setuptools_scm working
-requires = [
-  "setuptools_scm[toml] >= 6.2",
-  # "setuptools-generate >= 0.0.6"
-]
+requires = ["setuptools_scm[toml] >= 6.2", "setuptools-generate >= 0.0.6"]
 build-backend = "setuptools.build_meta"
 
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [project]
 name = "termux-language-server"
 description = "termux language server"
 readme = "README.md"
@@ -49,18 +45,18 @@
 
 [project.scripts]
 termux-language-server = "termux_language_server.__main__:main"
 
 [tool.setuptools.package-data]
 termux_language_server = ["py.typed", "assets/**"]
 
-# [tool.setuptools.data-files]
-# "share/man/man1" = ["sdist/termux-language-server.1"]
-# "share/bash-completion/completions" = ["sdist/termux-language-server"]
-# "share/zsh/site-functions" = ["sdist/_termux-language-server"]
+[tool.setuptools.data-files]
+"share/man/man1" = ["sdist/termux-language-server.1"]
+"share/bash-completion/completions" = ["sdist/termux-language-server"]
+"share/zsh/site-functions" = ["sdist/_termux-language-server"]
 
 [tool.setuptools.dynamic.dependencies]
 file = "requirements.txt"
 
 # begin: scripts/update-pyproject.toml.pl
 [tool.setuptools.dynamic.optional-dependencies.dev]
 file = "requirements/dev.txt"
```

### Comparing `termux-language-server-0.0.1/src/termux_language_server/__main__.py` & `termux-language-server-0.0.2/src/termux_language_server/__main__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 
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

### Comparing `termux-language-server-0.0.1/src/termux_language_server/api.py` & `termux-language-server-0.0.2/src/termux_language_server/api.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.1/src/termux_language_server/assets/json/termux.json` & `termux-language-server-0.0.2/src/termux_language_server/assets/json/termux.json`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.1/src/termux_language_server/server.py` & `termux-language-server-0.0.2/src/termux_language_server/server.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.1/src/termux_language_server.egg-info/PKG-INFO` & `termux-language-server-0.0.2/src/termux_language_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termux-language-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: termux language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://termux-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/termux-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/termux-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/termux-language-server
```

### Comparing `termux-language-server-0.0.1/src/termux_language_server.egg-info/SOURCES.txt` & `termux-language-server-0.0.2/src/termux_language_server.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,20 @@
 docs/resources/configure.md
 docs/resources/install.md
 docs/resources/requirements.md
 requirements/dev.txt
 requirements/web.txt
 scripts/generate-api.md.pl
 scripts/generate-requirements.md.pl
+sdist/_termux-language-server
+sdist/termux-language-server
+sdist/termux-language-server.1
 src/termux_language_server/__init__.py
 src/termux_language_server/__main__.py
+src/termux_language_server/_metainfo.py
 src/termux_language_server/_version.py
 src/termux_language_server/api.py
 src/termux_language_server/py.typed
 src/termux_language_server/server.py
 src/termux_language_server.egg-info/PKG-INFO
 src/termux_language_server.egg-info/SOURCES.txt
 src/termux_language_server.egg-info/dependency_links.txt
```

