# Comparing `tmp/sublime-syntax-language-server-0.0.2.tar.gz` & `tmp/sublime-syntax-language-server-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sublime-syntax-language-server-0.0.2.tar", last modified: Tue Jun 20 15:11:35 2023, max compression
+gzip compressed data, was "sublime-syntax-language-server-0.0.3.tar", last modified: Thu Jul  6 12:03:23 2023, max compression
```

## Comparing `sublime-syntax-language-server-0.0.2.tar` & `sublime-syntax-language-server-0.0.3.tar`

### file list

```diff
@@ -1,59 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.732149 sublime-syntax-language-server-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-06-20 15:11:35.732149 sublime-syntax-language-server-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/docs/api/sublime-syntax-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/docs/resources/requirements.md
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/requirements/web.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/scripts/generate-api.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      179 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/scripts/generate-requirements.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:11:35.732149 sublime-syntax-language-server-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.732149 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 15:11:35.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.732149 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)    28115 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/assets/json/sublime-syntax.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.732149 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-06-20 15:11:35.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-20 15:11:35.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:11:35.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-20 15:11:35.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 15:11:35.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 15:11:35.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.732149 sublime-syntax-language-server-0.0.2/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.732149 sublime-syntax-language-server-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/tests/Requirementstxt.sublime-syntax
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/tests/server_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/tests/syntax_test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:23.323661 sublime-syntax-language-server-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:23.315661 sublime-syntax-language-server-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:23.315661 sublime-syntax-language-server-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-06 12:03:23.323661 sublime-syntax-language-server-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:23.315661 sublime-syntax-language-server-0.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:23.315661 sublime-syntax-language-server-0.0.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/docs/api/sublime-syntax-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:23.315661 sublime-syntax-language-server-0.0.3/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:23.319661 sublime-syntax-language-server-0.0.3/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/requirements/web.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:23.319661 sublime-syntax-language-server-0.0.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/scripts/generate-api.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/scripts/generate-requirements.md.pl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:23.319661 sublime-syntax-language-server-0.0.3/sdist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-06 12:03:23.000000 sublime-syntax-language-server-0.0.3/sdist/_sublime-syntax-language-server
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-06 12:03:23.000000 sublime-syntax-language-server-0.0.3/sdist/sublime-syntax-language-server
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-06 12:03:23.000000 sublime-syntax-language-server-0.0.3/sdist/sublime-syntax-language-server.1
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 12:03:23.323661 sublime-syntax-language-server-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:23.311661 sublime-syntax-language-server-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:23.319661 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-06 12:03:23.000000 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server/_metainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 12:03:23.000000 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:23.311661 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:23.323661 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)    28115 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server/assets/json/sublime-syntax.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:23.323661 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-06 12:03:23.000000 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-06 12:03:23.000000 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:03:23.000000 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-06 12:03:23.000000 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 12:03:23.000000 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 12:03:23.000000 sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:23.323661 sublime-syntax-language-server-0.0.3/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:03:23.323661 sublime-syntax-language-server-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/tests/Requirementstxt.sublime-syntax
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/tests/server_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-06 12:03:09.000000 sublime-syntax-language-server-0.0.3/tests/syntax_test_requirements.txt
```

### Comparing `sublime-syntax-language-server-0.0.2/.github/workflows/main.yml` & `sublime-syntax-language-server-0.0.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.2/.gitignore` & `sublime-syntax-language-server-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.2/.pre-commit-config.yaml` & `sublime-syntax-language-server-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.2/LICENSE` & `sublime-syntax-language-server-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.2/PKG-INFO` & `sublime-syntax-language-server-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sublime-syntax-language-server
-Version: 0.0.2
+Version: 0.0.3
 Summary: sublime-syntax language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://sublime-syntax-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/sublime-syntax-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/sublime-syntax-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/sublime-syntax-language-server
```

### Comparing `sublime-syntax-language-server-0.0.2/README.md` & `sublime-syntax-language-server-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.2/docs/conf.py` & `sublime-syntax-language-server-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.2/docs/resources/configure.md` & `sublime-syntax-language-server-0.0.3/docs/resources/configure.md`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.2/docs/resources/install.md` & `sublime-syntax-language-server-0.0.3/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.2/flake.nix` & `sublime-syntax-language-server-0.0.3/flake.nix`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.2/pyproject.toml` & `sublime-syntax-language-server-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

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
 name = "sublime-syntax-language-server"
 description = "sublime-syntax language server"
 readme = "README.md"
@@ -49,18 +45,18 @@
 
 [project.scripts]
 sublime-syntax-language-server = "sublime_syntax_language_server.__main__:main"
 
 [tool.setuptools.package-data]
 sublime_syntax_language_server = ["py.typed", "assets/**"]
 
-# [tool.setuptools.data-files]
-# "share/man/man1" = ["sdist/sublime-syntax-language-server.1"]
-# "share/bash-completion/completions" = ["sdist/sublime-syntax-language-server"]
-# "share/zsh/site-functions" = ["sdist/_sublime-syntax-language-server"]
+[tool.setuptools.data-files]
+"share/man/man1" = ["sdist/sublime-syntax-language-server.1"]
+"share/bash-completion/completions" = ["sdist/sublime-syntax-language-server"]
+"share/zsh/site-functions" = ["sdist/_sublime-syntax-language-server"]
 
 [tool.setuptools.dynamic.dependencies]
 file = "requirements.txt"
 
 # begin: scripts/update-pyproject.toml.pl
 [tool.setuptools.dynamic.optional-dependencies.dev]
 file = "requirements/dev.txt"
```

### Comparing `sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/__main__.py` & `sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server/__main__.py`

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

### Comparing `sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/api.py` & `sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server/api.py`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/assets/json/sublime-syntax.json` & `sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server/assets/json/sublime-syntax.json`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/server.py` & `sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server/server.py`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/PKG-INFO` & `sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sublime-syntax-language-server
-Version: 0.0.2
+Version: 0.0.3
 Summary: sublime-syntax language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://sublime-syntax-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/sublime-syntax-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/sublime-syntax-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/sublime-syntax-language-server
```

### Comparing `sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/SOURCES.txt` & `sublime-syntax-language-server-0.0.3/src/sublime_syntax_language_server.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -17,16 +17,20 @@
 docs/resources/configure.md
 docs/resources/install.md
 docs/resources/requirements.md
 requirements/dev.txt
 requirements/web.txt
 scripts/generate-api.md.pl
 scripts/generate-requirements.md.pl
+sdist/_sublime-syntax-language-server
+sdist/sublime-syntax-language-server
+sdist/sublime-syntax-language-server.1
 src/sublime_syntax_language_server/__init__.py
 src/sublime_syntax_language_server/__main__.py
+src/sublime_syntax_language_server/_metainfo.py
 src/sublime_syntax_language_server/_version.py
 src/sublime_syntax_language_server/api.py
 src/sublime_syntax_language_server/py.typed
 src/sublime_syntax_language_server/server.py
 src/sublime_syntax_language_server.egg-info/PKG-INFO
 src/sublime_syntax_language_server.egg-info/SOURCES.txt
 src/sublime_syntax_language_server.egg-info/dependency_links.txt
```

### Comparing `sublime-syntax-language-server-0.0.2/tests/Requirementstxt.sublime-syntax` & `sublime-syntax-language-server-0.0.3/tests/Requirementstxt.sublime-syntax`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.2/tests/server_test.py` & `sublime-syntax-language-server-0.0.3/tests/server_test.py`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.2/tests/syntax_test_requirements.txt` & `sublime-syntax-language-server-0.0.3/tests/syntax_test_requirements.txt`

 * *Files identical despite different names*

