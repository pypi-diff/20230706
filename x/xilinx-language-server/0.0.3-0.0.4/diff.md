# Comparing `tmp/xilinx-language-server-0.0.3.tar.gz` & `tmp/xilinx-language-server-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xilinx-language-server-0.0.3.tar", last modified: Tue Jul  4 16:43:43 2023, max compression
+gzip compressed data, was "xilinx-language-server-0.0.4.tar", last modified: Thu Jul  6 11:55:34 2023, max compression
```

## Comparing `xilinx-language-server-0.0.3.tar` & `xilinx-language-server-0.0.4.tar`

### file list

```diff
@@ -1,59 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:43:43.430264 xilinx-language-server-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:43:43.422263 xilinx-language-server-0.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:43:43.422263 xilinx-language-server-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-04 16:43:43.430264 xilinx-language-server-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:43:43.422263 xilinx-language-server-0.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:43:43.422263 xilinx-language-server-0.0.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/docs/api/xilinx-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:43:43.422263 xilinx-language-server-0.0.3/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/docs/resources/requirements.md
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:43:43.422263 xilinx-language-server-0.0.3/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:43:43.422263 xilinx-language-server-0.0.3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/scripts/generate-api.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/scripts/generate-requirements.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/scripts/vivado.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/scripts/xilinx.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/scripts/xsct.tcl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 16:43:43.430264 xilinx-language-server-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:43:43.418264 xilinx-language-server-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:43:43.422263 xilinx-language-server-0.0.3/src/xilinx_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/src/xilinx_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/src/xilinx_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-04 16:43:43.000000 xilinx-language-server-0.0.3/src/xilinx_language_server/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:43:43.418264 xilinx-language-server-0.0.3/src/xilinx_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:43:43.426263 xilinx-language-server-0.0.3/src/xilinx_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)  4024542 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/src/xilinx_language_server/assets/json/vivado.json
--rw-r--r--   0 runner    (1001) docker     (123)   111383 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/src/xilinx_language_server/assets/json/xsct.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/src/xilinx_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/src/xilinx_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:43:43.422263 xilinx-language-server-0.0.3/src/xilinx_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-04 16:43:43.000000 xilinx-language-server-0.0.3/src/xilinx_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-04 16:43:43.000000 xilinx-language-server-0.0.3/src/xilinx_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 16:43:43.000000 xilinx-language-server-0.0.3/src/xilinx_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-04 16:43:43.000000 xilinx-language-server-0.0.3/src/xilinx_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-04 16:43:43.000000 xilinx-language-server-0.0.3/src/xilinx_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 16:43:43.000000 xilinx-language-server-0.0.3/src/xilinx_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:43:43.426263 xilinx-language-server-0.0.3/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:43:43.426263 xilinx-language-server-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-04 16:43:33.000000 xilinx-language-server-0.0.3/tests/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:34.836713 xilinx-language-server-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:34.824713 xilinx-language-server-0.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:34.828713 xilinx-language-server-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/.github/workflows/version.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-06 11:55:34.836713 xilinx-language-server-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:34.828713 xilinx-language-server-0.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:34.828713 xilinx-language-server-0.0.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/docs/api/xilinx-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:34.828713 xilinx-language-server-0.0.4/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:34.828713 xilinx-language-server-0.0.4/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       97 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:34.828713 xilinx-language-server-0.0.4/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/scripts/generate-api.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/scripts/generate-requirements.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      376 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/scripts/git-commit.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      108 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/scripts/update.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/scripts/vivado.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/scripts/xilinx.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/scripts/xsct.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:34.828713 xilinx-language-server-0.0.4/sdist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-06 11:55:34.000000 xilinx-language-server-0.0.4/sdist/_xilinx-language-server
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-06 11:55:34.000000 xilinx-language-server-0.0.4/sdist/xilinx-language-server
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-06 11:55:34.000000 xilinx-language-server-0.0.4/sdist/xilinx-language-server.1
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:55:34.836713 xilinx-language-server-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:34.824713 xilinx-language-server-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:34.828713 xilinx-language-server-0.0.4/src/xilinx_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/src/xilinx_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/src/xilinx_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-06 11:55:34.000000 xilinx-language-server-0.0.4/src/xilinx_language_server/_metainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 11:55:34.000000 xilinx-language-server-0.0.4/src/xilinx_language_server/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:34.824713 xilinx-language-server-0.0.4/src/xilinx_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:34.836713 xilinx-language-server-0.0.4/src/xilinx_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)  4024542 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/src/xilinx_language_server/assets/json/vivado.json
+-rw-r--r--   0 runner    (1001) docker     (123)   111383 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/src/xilinx_language_server/assets/json/xsct.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/src/xilinx_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/src/xilinx_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:34.832713 xilinx-language-server-0.0.4/src/xilinx_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-06 11:55:34.000000 xilinx-language-server-0.0.4/src/xilinx_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-06 11:55:34.000000 xilinx-language-server-0.0.4/src/xilinx_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:55:34.000000 xilinx-language-server-0.0.4/src/xilinx_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-06 11:55:34.000000 xilinx-language-server-0.0.4/src/xilinx_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 11:55:34.000000 xilinx-language-server-0.0.4/src/xilinx_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 11:55:34.000000 xilinx-language-server-0.0.4/src/xilinx_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:34.836713 xilinx-language-server-0.0.4/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:55:34.836713 xilinx-language-server-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-06 11:55:20.000000 xilinx-language-server-0.0.4/tests/server_test.py
```

### Comparing `xilinx-language-server-0.0.3/.github/workflows/main.yml` & `xilinx-language-server-0.0.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.3/.gitignore` & `xilinx-language-server-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.3/.pre-commit-config.yaml` & `xilinx-language-server-0.0.4/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,17 @@
     rev: 2.7.1
     hooks:
       - id: editorconfig-checker
   - repo: https://github.com/jumanjihouse/pre-commit-hooks
     rev: 3.0.0
     hooks:
       - id: check-mailmap
+      - id: shellcheck
+        exclude_types:
+          - zsh
   - repo: https://github.com/rhysd/actionlint
     rev: v1.6.25
     hooks:
       - id: actionlint
   - repo: https://github.com/adrienverge/yamllint
     rev: v1.32.0
     hooks:
@@ -73,14 +76,18 @@
       - id: markdownlint-cli2
         additional_dependencies:
           - markdown-it-texmath@0.9.1
   - repo: https://github.com/perltidy/perltidy
     rev: "20230309.03"
     hooks:
       - id: perltidy
+  - repo: https://github.com/scop/pre-commit-shfmt
+    rev: v3.6.0-2
+    hooks:
+      - id: shfmt
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
```

### Comparing `xilinx-language-server-0.0.3/LICENSE` & `xilinx-language-server-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.3/PKG-INFO` & `xilinx-language-server-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xilinx-language-server
-Version: 0.0.3
+Version: 0.0.4
 Summary: xilinx language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://xilinx-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/xilinx-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/xilinx-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/xilinx-language-server
```

### Comparing `xilinx-language-server-0.0.3/README.md` & `xilinx-language-server-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.3/docs/conf.py` & `xilinx-language-server-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.3/docs/resources/configure.md` & `xilinx-language-server-0.0.4/docs/resources/configure.md`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.3/docs/resources/install.md` & `xilinx-language-server-0.0.4/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.3/flake.nix` & `xilinx-language-server-0.0.4/flake.nix`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.3/pyproject.toml` & `xilinx-language-server-0.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

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
 name = "xilinx-language-server"
 description = "xilinx language server"
 readme = "README.md"
@@ -49,18 +45,18 @@
 
 [project.scripts]
 xilinx-language-server = "xilinx_language_server.__main__:main"
 
 [tool.setuptools.package-data]
 xilinx_language_server = ["py.typed", "assets/**"]
 
-# [tool.setuptools.data-files]
-# "share/man/man1" = ["sdist/xilinx-language-server.1"]
-# "share/bash-completion/completions" = ["sdist/xilinx-language-server"]
-# "share/zsh/site-functions" = ["sdist/_xilinx-language-server"]
+[tool.setuptools.data-files]
+"share/man/man1" = ["sdist/xilinx-language-server.1"]
+"share/bash-completion/completions" = ["sdist/xilinx-language-server"]
+"share/zsh/site-functions" = ["sdist/_xilinx-language-server"]
 
 [tool.setuptools.dynamic.dependencies]
 file = "requirements.txt"
 
 # begin: scripts/update-pyproject.toml.pl
 [tool.setuptools.dynamic.optional-dependencies.dev]
 file = "requirements/dev.txt"
```

### Comparing `xilinx-language-server-0.0.3/scripts/xilinx.tcl` & `xilinx-language-server-0.0.4/scripts/xilinx.tcl`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.3/src/xilinx_language_server/__main__.py` & `xilinx-language-server-0.0.4/src/xilinx_language_server/__main__.py`

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

### Comparing `xilinx-language-server-0.0.3/src/xilinx_language_server/assets/json/vivado.json` & `xilinx-language-server-0.0.4/src/xilinx_language_server/assets/json/vivado.json`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.3/src/xilinx_language_server/assets/json/xsct.json` & `xilinx-language-server-0.0.4/src/xilinx_language_server/assets/json/xsct.json`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.3/src/xilinx_language_server/server.py` & `xilinx-language-server-0.0.4/src/xilinx_language_server/server.py`

 * *Files identical despite different names*

### Comparing `xilinx-language-server-0.0.3/src/xilinx_language_server.egg-info/PKG-INFO` & `xilinx-language-server-0.0.4/src/xilinx_language_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xilinx-language-server
-Version: 0.0.3
+Version: 0.0.4
 Summary: xilinx language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://xilinx-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/xilinx-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/xilinx-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/xilinx-language-server
```

### Comparing `xilinx-language-server-0.0.3/src/xilinx_language_server.egg-info/SOURCES.txt` & `xilinx-language-server-0.0.4/src/xilinx_language_server.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,36 @@
 LICENSE
 README.md
 flake.nix
 pyproject.toml
 requirements.txt
 .github/FUNDING.yml
 .github/workflows/main.yml
+.github/workflows/version.yml
 docs/conf.py
 docs/index.md
 docs/requirements.txt
 docs/api/xilinx-language-server.md
 docs/resources/configure.md
 docs/resources/install.md
 docs/resources/requirements.md
 requirements/dev.txt
 scripts/generate-api.md.pl
 scripts/generate-requirements.md.pl
+scripts/git-commit.sh
+scripts/update.sh
 scripts/vivado.tcl
 scripts/xilinx.tcl
 scripts/xsct.tcl
+sdist/_xilinx-language-server
+sdist/xilinx-language-server
+sdist/xilinx-language-server.1
 src/xilinx_language_server/__init__.py
 src/xilinx_language_server/__main__.py
+src/xilinx_language_server/_metainfo.py
 src/xilinx_language_server/_version.py
 src/xilinx_language_server/py.typed
 src/xilinx_language_server/server.py
 src/xilinx_language_server.egg-info/PKG-INFO
 src/xilinx_language_server.egg-info/SOURCES.txt
 src/xilinx_language_server.egg-info/dependency_links.txt
 src/xilinx_language_server.egg-info/entry_points.txt
```

