# Comparing `tmp/pkgbuild-language-server-0.0.5.tar.gz` & `tmp/pkgbuild-language-server-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgbuild-language-server-0.0.5.tar", last modified: Tue Jun 20 15:26:03 2023, max compression
+gzip compressed data, was "pkgbuild-language-server-0.0.6.tar", last modified: Thu Jul  6 12:01:05 2023, max compression
```

## Comparing `pkgbuild-language-server-0.0.5.tar` & `pkgbuild-language-server-0.0.6.tar`

### file list

```diff
@@ -1,62 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:03.164041 pkgbuild-language-server-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:03.156041 pkgbuild-language-server-0.0.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:03.156041 pkgbuild-language-server-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-06-20 15:26:03.164041 pkgbuild-language-server-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:03.156041 pkgbuild-language-server-0.0.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:03.156041 pkgbuild-language-server-0.0.5/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/docs/api/pkgbuild-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:03.156041 pkgbuild-language-server-0.0.5/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/docs/resources/requirements.md
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:03.160041 pkgbuild-language-server-0.0.5/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/requirements/cache.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      128 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/requirements/diagnostic.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/requirements/package.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:03.160041 pkgbuild-language-server-0.0.5/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/scripts/generate-api.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/scripts/generate-requirements.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:26:03.164041 pkgbuild-language-server-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:03.148041 pkgbuild-language-server-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:03.160041 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 15:26:03.000000 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:03.148041 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:03.160041 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/assets/jinja2/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/assets/jinja2/template.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:03.164041 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/assets/json/pkgbuild.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/package.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:03.160041 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-06-20 15:26:03.000000 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-20 15:26:03.000000 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:26:03.000000 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 15:26:03.000000 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 15:26:03.000000 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 15:26:03.000000 pkgbuild-language-server-0.0.5/src/pkgbuild_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:03.164041 pkgbuild-language-server-0.0.5/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:26:03.164041 pkgbuild-language-server-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 15:25:49.000000 pkgbuild-language-server-0.0.5/tests/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.898765 pkgbuild-language-server-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.894765 pkgbuild-language-server-0.0.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.894765 pkgbuild-language-server-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-07-06 12:01:05.898765 pkgbuild-language-server-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.894765 pkgbuild-language-server-0.0.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.894765 pkgbuild-language-server-0.0.6/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/docs/api/pkgbuild-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.894765 pkgbuild-language-server-0.0.6/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.894765 pkgbuild-language-server-0.0.6/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/requirements/cache.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      128 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/requirements/diagnostic.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/requirements/package.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.894765 pkgbuild-language-server-0.0.6/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/scripts/generate-api.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/scripts/generate-requirements.md.pl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.894765 pkgbuild-language-server-0.0.6/sdist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-06 12:01:05.000000 pkgbuild-language-server-0.0.6/sdist/_pkgbuild-language-server
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-06 12:01:05.000000 pkgbuild-language-server-0.0.6/sdist/pkgbuild-language-server
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-06 12:01:05.000000 pkgbuild-language-server-0.0.6/sdist/pkgbuild-language-server.1
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 12:01:05.898765 pkgbuild-language-server-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.894765 pkgbuild-language-server-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.898765 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 12:01:05.000000 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/_metainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 12:01:05.000000 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.894765 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.898765 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/assets/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/assets/jinja2/template.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.898765 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/assets/json/pkgbuild.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.898765 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-07-06 12:01:05.000000 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-06 12:01:05.000000 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:01:05.000000 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-06 12:01:05.000000 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 12:01:05.000000 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 12:01:05.000000 pkgbuild-language-server-0.0.6/src/pkgbuild_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.898765 pkgbuild-language-server-0.0.6/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:05.898765 pkgbuild-language-server-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-06 12:00:49.000000 pkgbuild-language-server-0.0.6/tests/server_test.py
```

### Comparing `pkgbuild-language-server-0.0.5/.github/workflows/main.yml` & `pkgbuild-language-server-0.0.6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.5/.gitignore` & `pkgbuild-language-server-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.5/.pre-commit-config.yaml` & `pkgbuild-language-server-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.5/LICENSE` & `pkgbuild-language-server-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.5/PKG-INFO` & `pkgbuild-language-server-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkgbuild-language-server
-Version: 0.0.5
+Version: 0.0.6
 Summary: pkgbuild language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://pkgbuild-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/pkgbuild-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/pkgbuild-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/pkgbuild-language-server
```

### Comparing `pkgbuild-language-server-0.0.5/README.md` & `pkgbuild-language-server-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.5/docs/conf.py` & `pkgbuild-language-server-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.5/docs/resources/configure.md` & `pkgbuild-language-server-0.0.6/docs/resources/configure.md`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.5/docs/resources/install.md` & `pkgbuild-language-server-0.0.6/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.5/flake.nix` & `pkgbuild-language-server-0.0.6/flake.nix`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.5/pyproject.toml` & `pkgbuild-language-server-0.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

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
 name = "pkgbuild-language-server"
 description = "pkgbuild language server"
@@ -50,18 +49,18 @@
 
 [project.scripts]
 pkgbuild-language-server = "pkgbuild_language_server.__main__:main"
 
 [tool.setuptools.package-data]
 pkgbuild_language_server = ["py.typed", "assets/**"]
 
-# [tool.setuptools.data-files]
-# "share/man/man1" = ["sdist/pkgbuild-language-server.1"]
-# "share/bash-completion/completions" = ["sdist/pkgbuild-language-server"]
-# "share/zsh/site-functions" = ["sdist/_pkgbuild-language-server"]
+[tool.setuptools.data-files]
+"share/man/man1" = ["sdist/pkgbuild-language-server.1"]
+"share/bash-completion/completions" = ["sdist/pkgbuild-language-server"]
+"share/zsh/site-functions" = ["sdist/_pkgbuild-language-server"]
 
 [tool.setuptools.dynamic.dependencies]
 file = "requirements.txt"
 
 # begin: scripts/update-pyproject.toml.pl
 [tool.setuptools.dynamic.optional-dependencies.dev]
 file = "requirements/dev.txt"
```

### Comparing `pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/__main__.py` & `pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/__main__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,29 +23,29 @@
 
 def get_parser():
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
         help="generate cache for archlinux packages",
     )
-    with suppress(ImportError):
-        import shtab
-
-        shtab.add_argument_to(parser)
     return parser
 
 
 def main():
     r"""Parse arguments and provide shell completions."""
     parser = get_parser()
     args = parser.parse_args()
```

### Comparing `pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/api.py` & `pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/api.py`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/assets/jinja2/template.md.j2` & `pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/assets/jinja2/template.md.j2`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/assets/json/pkgbuild.json` & `pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/assets/json/pkgbuild.json`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/package.py` & `pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/package.py`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.5/src/pkgbuild_language_server/server.py` & `pkgbuild-language-server-0.0.6/src/pkgbuild_language_server/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,17 +76,16 @@
 
 
 def get_document(
     method: Literal["builtin", "cache", "system"] = "builtin"
 ) -> dict[str, tuple[str, str, str]]:
     r"""Get document. ``builtin`` will use builtin pkgbuild.json. ``cache``
     will generate a cache from ``${XDG_CACHE_DIRS:-/usr/share}
-    /info/pkgbuild.info.gz``. ``system`` is same as ``cache`` except it doesn't
-    generate cache. Some distribution's pkgbuild doesn't contain textinfo. So
-    we use ``builtin`` as default.
+    /man/man5/PKGBUILD.5.gz``. ``system`` is same as ``cache`` except it
+    doesn't generate cache. We use ``builtin`` as default.
 
     :param method:
     :type method: Literal["builtin", "cache", "system"]
     :rtype: dict[str, tuple[str, str, str]]
     """
     if method == "builtin":
         file = os.path.join(
```

### Comparing `pkgbuild-language-server-0.0.5/src/pkgbuild_language_server.egg-info/PKG-INFO` & `pkgbuild-language-server-0.0.6/src/pkgbuild_language_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkgbuild-language-server
-Version: 0.0.5
+Version: 0.0.6
 Summary: pkgbuild language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://pkgbuild-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/pkgbuild-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/pkgbuild-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/pkgbuild-language-server
```

### Comparing `pkgbuild-language-server-0.0.5/src/pkgbuild_language_server.egg-info/SOURCES.txt` & `pkgbuild-language-server-0.0.6/src/pkgbuild_language_server.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,20 @@
 docs/resources/requirements.md
 requirements/cache.txt
 requirements/dev.txt
 requirements/diagnostic.txt
 requirements/package.txt
 scripts/generate-api.md.pl
 scripts/generate-requirements.md.pl
+sdist/_pkgbuild-language-server
+sdist/pkgbuild-language-server
+sdist/pkgbuild-language-server.1
 src/pkgbuild_language_server/__init__.py
 src/pkgbuild_language_server/__main__.py
+src/pkgbuild_language_server/_metainfo.py
 src/pkgbuild_language_server/_version.py
 src/pkgbuild_language_server/api.py
 src/pkgbuild_language_server/package.py
 src/pkgbuild_language_server/py.typed
 src/pkgbuild_language_server/server.py
 src/pkgbuild_language_server.egg-info/PKG-INFO
 src/pkgbuild_language_server.egg-info/SOURCES.txt
```

