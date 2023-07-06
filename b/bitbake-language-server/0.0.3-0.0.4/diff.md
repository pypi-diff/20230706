# Comparing `tmp/bitbake-language-server-0.0.3.tar.gz` & `tmp/bitbake-language-server-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitbake-language-server-0.0.3.tar", last modified: Fri Jun 23 09:07:51 2023, max compression
+gzip compressed data, was "bitbake-language-server-0.0.4.tar", last modified: Thu Jul  6 11:47:31 2023, max compression
```

## Comparing `bitbake-language-server-0.0.3.tar` & `bitbake-language-server-0.0.4.tar`

### file list

```diff
@@ -1,57 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.675937 bitbake-language-server-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.667937 bitbake-language-server-0.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.667937 bitbake-language-server-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-23 09:07:51.675937 bitbake-language-server-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.671937 bitbake-language-server-0.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.671937 bitbake-language-server-0.0.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/docs/api/bitbake-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.671937 bitbake-language-server-0.0.3/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/docs/resources/requirements.md
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.671937 bitbake-language-server-0.0.3/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/requirements/web.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.671937 bitbake-language-server-0.0.3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/scripts/generate-api.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/scripts/generate-requirements.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:07:51.675937 bitbake-language-server-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.667937 bitbake-language-server-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.671937 bitbake-language-server-0.0.3/src/bitbake_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/src/bitbake_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/src/bitbake_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 09:07:51.000000 bitbake-language-server-0.0.3/src/bitbake_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/src/bitbake_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.667937 bitbake-language-server-0.0.3/src/bitbake_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.671937 bitbake-language-server-0.0.3/src/bitbake_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)    51606 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/src/bitbake_language_server/assets/json/bitbake.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/src/bitbake_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/src/bitbake_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.671937 bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-23 09:07:51.000000 bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-23 09:07:51.000000 bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:07:51.000000 bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 09:07:51.000000 bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 09:07:51.000000 bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 09:07:51.000000 bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.675937 bitbake-language-server-0.0.3/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:07:51.675937 bitbake-language-server-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-23 09:07:39.000000 bitbake-language-server-0.0.3/tests/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:31.325238 bitbake-language-server-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:31.321238 bitbake-language-server-0.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:31.321238 bitbake-language-server-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-06 11:47:31.325238 bitbake-language-server-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:31.321238 bitbake-language-server-0.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:31.321238 bitbake-language-server-0.0.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/docs/api/bitbake-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:31.321238 bitbake-language-server-0.0.4/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:31.321238 bitbake-language-server-0.0.4/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/requirements/web.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:31.321238 bitbake-language-server-0.0.4/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/scripts/generate-api.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/scripts/generate-requirements.md.pl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:31.321238 bitbake-language-server-0.0.4/sdist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-06 11:47:31.000000 bitbake-language-server-0.0.4/sdist/_bitbake-language-server
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-06 11:47:31.000000 bitbake-language-server-0.0.4/sdist/bitbake-language-server
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-06 11:47:31.000000 bitbake-language-server-0.0.4/sdist/bitbake-language-server.1
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:47:31.325238 bitbake-language-server-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:31.321238 bitbake-language-server-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:31.321238 bitbake-language-server-0.0.4/src/bitbake_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/src/bitbake_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/src/bitbake_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-06 11:47:31.000000 bitbake-language-server-0.0.4/src/bitbake_language_server/_metainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 11:47:31.000000 bitbake-language-server-0.0.4/src/bitbake_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/src/bitbake_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:31.321238 bitbake-language-server-0.0.4/src/bitbake_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:31.325238 bitbake-language-server-0.0.4/src/bitbake_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)    51606 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/src/bitbake_language_server/assets/json/bitbake.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/src/bitbake_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/src/bitbake_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:31.325238 bitbake-language-server-0.0.4/src/bitbake_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-06 11:47:31.000000 bitbake-language-server-0.0.4/src/bitbake_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-06 11:47:31.000000 bitbake-language-server-0.0.4/src/bitbake_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:47:31.000000 bitbake-language-server-0.0.4/src/bitbake_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-06 11:47:31.000000 bitbake-language-server-0.0.4/src/bitbake_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 11:47:31.000000 bitbake-language-server-0.0.4/src/bitbake_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 11:47:31.000000 bitbake-language-server-0.0.4/src/bitbake_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:31.325238 bitbake-language-server-0.0.4/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:47:31.325238 bitbake-language-server-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-06 11:47:17.000000 bitbake-language-server-0.0.4/tests/server_test.py
```

### Comparing `bitbake-language-server-0.0.3/.github/workflows/main.yml` & `bitbake-language-server-0.0.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.3/.gitignore` & `bitbake-language-server-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.3/.pre-commit-config.yaml` & `bitbake-language-server-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.3/LICENSE` & `bitbake-language-server-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.3/PKG-INFO` & `bitbake-language-server-0.0.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitbake-language-server
-Version: 0.0.3
+Version: 0.0.4
 Summary: bitbake language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://bitbake-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/bitbake-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/bitbake-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/bitbake-language-server
```

### Comparing `bitbake-language-server-0.0.3/README.md` & `bitbake-language-server-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.3/docs/conf.py` & `bitbake-language-server-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.3/docs/resources/configure.md` & `bitbake-language-server-0.0.4/docs/resources/configure.md`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.3/docs/resources/install.md` & `bitbake-language-server-0.0.4/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.3/flake.nix` & `bitbake-language-server-0.0.4/flake.nix`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.3/pyproject.toml` & `bitbake-language-server-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

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
 name = "bitbake-language-server"
 description = "bitbake language server"
 readme = "README.md"
@@ -49,18 +45,18 @@
 
 [project.scripts]
 bitbake-language-server = "bitbake_language_server.__main__:main"
 
 [tool.setuptools.package-data]
 bitbake_language_server = ["py.typed", "assets/**"]
 
-# [tool.setuptools.data-files]
-# "share/man/man1" = ["sdist/bitbake-language-server.1"]
-# "share/bash-completion/completions" = ["sdist/bitbake-language-server"]
-# "share/zsh/site-functions" = ["sdist/_bitbake-language-server"]
+[tool.setuptools.data-files]
+"share/man/man1" = ["sdist/bitbake-language-server.1"]
+"share/bash-completion/completions" = ["sdist/bitbake-language-server"]
+"share/zsh/site-functions" = ["sdist/_bitbake-language-server"]
 
 [tool.setuptools.dynamic.dependencies]
 file = "requirements.txt"
 
 # begin: scripts/update-pyproject.toml.pl
 [tool.setuptools.dynamic.optional-dependencies.dev]
 file = "requirements/dev.txt"
```

### Comparing `bitbake-language-server-0.0.3/src/bitbake_language_server/__main__.py` & `bitbake-language-server-0.0.4/src/bitbake_language_server/__main__.py`

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

### Comparing `bitbake-language-server-0.0.3/src/bitbake_language_server/api.py` & `bitbake-language-server-0.0.4/src/bitbake_language_server/api.py`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.3/src/bitbake_language_server/assets/json/bitbake.json` & `bitbake-language-server-0.0.4/src/bitbake_language_server/assets/json/bitbake.json`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.3/src/bitbake_language_server/server.py` & `bitbake-language-server-0.0.4/src/bitbake_language_server/server.py`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.3/src/bitbake_language_server.egg-info/PKG-INFO` & `bitbake-language-server-0.0.4/src/bitbake_language_server.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitbake-language-server
-Version: 0.0.3
+Version: 0.0.4
 Summary: bitbake language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://bitbake-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/bitbake-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/bitbake-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/bitbake-language-server
```

