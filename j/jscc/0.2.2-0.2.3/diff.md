# Comparing `tmp/jscc-0.2.2.tar.gz` & `tmp/jscc-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jscc-0.2.2.tar", last modified: Thu Jun 15 04:25:22 2023, max compression
+gzip compressed data, was "jscc-0.2.3.tar", last modified: Thu Jul  6 15:35:15 2023, max compression
```

## Comparing `jscc-0.2.2.tar` & `jscc-0.2.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.962456 jscc-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-15 04:25:12.000000 jscc-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 04:25:12.000000 jscc-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-15 04:25:22.962456 jscc-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-15 04:25:12.000000 jscc-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.942456 jscc-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-15 04:25:12.000000 jscc-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.942456 jscc-0.2.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 04:25:12.000000 jscc-0.2.2/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 04:25:12.000000 jscc-0.2.2/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 04:25:12.000000 jscc-0.2.2/docs/api/schema.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.942456 jscc-0.2.2/docs/api/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-15 04:25:12.000000 jscc-0.2.2/docs/api/testing/checks.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 04:25:12.000000 jscc-0.2.2/docs/api/testing/filesystem.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 04:25:12.000000 jscc-0.2.2/docs/api/testing/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 04:25:12.000000 jscc-0.2.2/docs/api/testing/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-15 04:25:12.000000 jscc-0.2.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-15 04:25:12.000000 jscc-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-15 04:25:12.000000 jscc-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 04:25:12.000000 jscc-0.2.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.942456 jscc-0.2.2/jscc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:12.000000 jscc-0.2.2/jscc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-15 04:25:12.000000 jscc-0.2.2/jscc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-15 04:25:12.000000 jscc-0.2.2/jscc/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.946456 jscc-0.2.2/jscc/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:12.000000 jscc-0.2.2/jscc/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30688 2023-06-15 04:25:12.000000 jscc-0.2.2/jscc/testing/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-15 04:25:12.000000 jscc-0.2.2/jscc/testing/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-15 04:25:12.000000 jscc-0.2.2/jscc/testing/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.946456 jscc-0.2.2/jscc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-15 04:25:22.000000 jscc-0.2.2/jscc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-15 04:25:22.000000 jscc-0.2.2/jscc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 04:25:22.000000 jscc-0.2.2/jscc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 04:25:22.000000 jscc-0.2.2/jscc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 04:25:22.000000 jscc-0.2.2/jscc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 04:25:12.000000 jscc-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-15 04:25:22.962456 jscc-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.946456 jscc-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.950456 jscc-0.2.2/tests/cassettes/
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/cassettes/test_http_get_error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/cassettes/test_http_head_error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.950456 jscc-0.2.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/codelist.csv
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.954456 jscc-0.2.2/tests/fixtures/empty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/empty/empty-array.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/empty/empty-object.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/empty/empty-string.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/empty/false.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.954456 jscc-0.2.2/tests/fixtures/empty/htmlcov/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/empty/htmlcov/empty.txt
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/empty/invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/empty/null.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/empty/whitespace-string.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/empty/whitespace.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/empty/whitespace.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/empty/zero-float.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/empty/zero-int.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.954456 jscc-0.2.2/tests/fixtures/indent/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/indent/ascii.json
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/indent/compact.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/indent/indented.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/indent/invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/indent/no-newline.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.954456 jscc-0.2.2/tests/fixtures/json/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/json/duplicate-key.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/json/invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/json/valid.json
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/meta-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/patch.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.958456 jscc-0.2.2/tests/fixtures/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/array_items.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.958456 jscc-0.2.2/tests/fixtures/schema/build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/build/ignore.json
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/codelist_enum.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:25:22.962456 jscc-0.2.2/tests/fixtures/schema/codelists/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/codelists/+nonexistent.csv
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/codelists/extra.csv
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/codelists/failClosedArray.csv
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/codelists/failClosedString.csv
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/codelists/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/deep_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/items_type.json
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/letter_case.json
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/merge_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/metadata_presence.json
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/null_type.json
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/object_id.json
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/ref.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/fixtures/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-15 04:25:12.000000 jscc-0.2.2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.574728 jscc-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-06 15:35:06.000000 jscc-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-06 15:35:06.000000 jscc-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-06 15:35:15.574728 jscc-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-06 15:35:06.000000 jscc-0.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.566728 jscc-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-06 15:35:06.000000 jscc-0.2.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.566728 jscc-0.2.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 15:35:06.000000 jscc-0.2.3/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-06 15:35:06.000000 jscc-0.2.3/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 15:35:06.000000 jscc-0.2.3/docs/api/schema.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.566728 jscc-0.2.3/docs/api/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-06 15:35:06.000000 jscc-0.2.3/docs/api/testing/checks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-06 15:35:06.000000 jscc-0.2.3/docs/api/testing/filesystem.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-06 15:35:06.000000 jscc-0.2.3/docs/api/testing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 15:35:06.000000 jscc-0.2.3/docs/api/testing/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-06 15:35:06.000000 jscc-0.2.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-06 15:35:06.000000 jscc-0.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-06 15:35:06.000000 jscc-0.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 15:35:06.000000 jscc-0.2.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.566728 jscc-0.2.3/jscc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:06.000000 jscc-0.2.3/jscc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-06 15:35:06.000000 jscc-0.2.3/jscc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-06 15:35:06.000000 jscc-0.2.3/jscc/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.566728 jscc-0.2.3/jscc/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:06.000000 jscc-0.2.3/jscc/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30803 2023-07-06 15:35:06.000000 jscc-0.2.3/jscc/testing/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-06 15:35:06.000000 jscc-0.2.3/jscc/testing/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-06 15:35:06.000000 jscc-0.2.3/jscc/testing/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.566728 jscc-0.2.3/jscc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-06 15:35:15.000000 jscc-0.2.3/jscc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-06 15:35:15.000000 jscc-0.2.3/jscc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 15:35:15.000000 jscc-0.2.3/jscc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-06 15:35:15.000000 jscc-0.2.3/jscc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 15:35:15.000000 jscc-0.2.3/jscc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-06 15:35:06.000000 jscc-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-06 15:35:15.574728 jscc-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.566728 jscc-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.570728 jscc-0.2.3/tests/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/cassettes/test_http_get_error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/cassettes/test_http_head_error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.570728 jscc-0.2.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/codelist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.570728 jscc-0.2.3/tests/fixtures/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/empty/empty-array.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/empty/empty-object.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/empty/empty-string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/empty/false.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.570728 jscc-0.2.3/tests/fixtures/empty/htmlcov/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/empty/htmlcov/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/empty/invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/empty/null.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/empty/whitespace-string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/empty/whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/empty/whitespace.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/empty/zero-float.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/empty/zero-int.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.570728 jscc-0.2.3/tests/fixtures/indent/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/indent/ascii.json
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/indent/compact.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/indent/indented.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/indent/invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/indent/no-newline.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.570728 jscc-0.2.3/tests/fixtures/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/json/duplicate-key.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/json/invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/json/valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/meta-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/patch.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.574728 jscc-0.2.3/tests/fixtures/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/array_items.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.574728 jscc-0.2.3/tests/fixtures/schema/build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/build/ignore.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/codelist_enum.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:35:15.574728 jscc-0.2.3/tests/fixtures/schema/codelists/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/codelists/+nonexistent.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/codelists/extra.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/codelists/failClosedArray.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/codelists/failClosedString.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/codelists/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/deep_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/items_type.json
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/letter_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/merge_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/metadata_presence.json
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/null_type.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/object_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/ref.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/fixtures/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-06 15:35:06.000000 jscc-0.2.3/tests/test_util.py
```

### Comparing `jscc-0.2.2/LICENSE` & `jscc-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jscc-0.2.2/PKG-INFO` & `jscc-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jscc
-Version: 0.2.2
+Version: 0.2.3
 Summary: Tools for data standards that use JSON Schema and CSV codelists
 Home-page: https://github.com/open-contracting/jscc
 Author: Open Contracting Partnership and Open Data Services Co-operative Limited
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `jscc-0.2.2/README.rst` & `jscc-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `jscc-0.2.2/docs/Makefile` & `jscc-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jscc-0.2.2/docs/changelog.rst` & `jscc-0.2.3/docs/changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 Changelog
 =========
 
+0.2.3 (2023-07-06)
+------------------
+
+Changed
+~~~~~~~
+
+- Add support for `$defs` keyword in:
+
+  -  :meth:`jscc.testing.checks.validate_letter_case`
+  -  :meth:`jscc.testing.checks.validate_metadata_presence`
+  -  :meth:`jscc.testing.checks.validate_null_types`
+  -  :meth:`jscc.testing.checks.validate_deep_properties`
+  -  :meth:`jscc.schema.is_json_schema`
+  -  :meth:`jscc.schema.is_json_merge_patch`
+
 0.2.2 (2023-06-14)
 ------------------
 
 Removed
 ~~~~~~~
 
 -  :meth:`~jscc.testing.checks.get_invalid_csv_files`, as Python's CSV parser errors only if the CSV dialect is configured.
```

### Comparing `jscc-0.2.2/docs/conf.py` & `jscc-0.2.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "JSON Schema and CSV Codelists"
 copyright = "2020, Open Contracting Partnership and Open Data Services Co-operative Limited"
 author = "Open Contracting Partnership and Open Data Services Co-operative Limited"
 
 # The short X.Y version
-version = "0.2.2"
+version = "0.2.3"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `jscc-0.2.2/jscc/exceptions.py` & `jscc-0.2.3/jscc/exceptions.py`

 * *Files identical despite different names*

### Comparing `jscc-0.2.2/jscc/schema.py` & `jscc-0.2.3/jscc/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,24 @@
 
 def is_json_schema(data):
     """
     :param dict data: JSON data
     :returns: whether the JSON data is a JSON Schema
     :rtype: bool
     """
-    return '$schema' in data or 'definitions' in data or 'properties' in data
+    return '$schema' in data or 'definitions' in data or '$defs' in data or 'properties' in data
 
 
 def is_json_merge_patch(data):
     """
     :param dict data: JSON data
     :returns: whether the JSON data is a JSON Merge Patch
     :rtype: bool
     """
-    return '$schema' not in data and ('definitions' in data or 'properties' in data)
+    return '$schema' not in data and ('definitions' in data or '$defs' in data or 'properties' in data)
 
 
 def is_array_of_objects(field):
     """
     :param dict field: the field
     :returns: whether a field is an array of objects
     :rtype: bool
```

### Comparing `jscc-0.2.2/jscc/testing/checks.py` & `jscc-0.2.3/jscc/testing/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
         parent = pointer.rsplit('/', 1)[-1]
 
         if parent == 'properties':
             for key in data.keys():
                 if not re.search(r'^[a-z][A-Za-z]+$', key) and key not in property_exceptions:
                     errors += 1
                     warn(f"{path}: {pointer}/{key} field isn't lowerCamelCase ASCII letters", LetterCaseWarning)
-        elif parent == 'definitions':
+        elif parent in ('definitions', '$defs'):
             for key in data.keys():
                 if not re.search(r'^[A-Z][A-Za-z]+$', key) and key not in definition_exceptions:
                     errors += 1
                     warn(f"{path}: {pointer}/{key} block isn't UpperCamelCase ASCII letters", LetterCaseWarning)
 
         return errors
 
@@ -272,15 +272,15 @@
     properties, unless it has a `"$ref" <https://tools.ietf.org/html/draft-pbryan-zyp-json-ref-03>`__ property.
 
     :param function allow_missing: a method that accepts a JSON Pointer, and returns whether the field is allowed to
                                    not have a "title" or "description" property
     :returns: the number of errors
     :rtype: int
     """  # noqa: E501
-    schema_fields = {'definitions', 'deprecated', 'items', 'patternProperties', 'properties'}
+    schema_fields = {'definitions', '$defs', 'deprecated', 'items', 'patternProperties', 'properties'}
     schema_sections = {'patternProperties'}
     required_properties = {'title', 'description'}
 
     def block(path, data, pointer):
         errors = 0
 
         parts = pointer.rsplit('/')
@@ -359,15 +359,15 @@
             elif null_in_type and pointer not in allow_null:
                 errors += 1
                 warn(f'{path} includes "null" in "type" at {pointer}', NullTypeWarning)
 
         required = data.get('required', [])
 
         for key, value in data.items():
-            if key in ('properties', 'definitions'):
+            if key in ('properties', 'definitions', '$defs'):
                 for k, v in data[key].items():
                     expect_null = key == 'properties' and k not in required
                     errors += validate_null_type(path, v, pointer=f'{pointer}/{key}/{k}', **kwargs, no_null=no_null,
                                                  expect_null=expect_null)
             else:
                 v = data['items'] if key == 'items' else value
                 errors += validate_null_type(path, v, pointer=f'{pointer}/{key}', **kwargs, no_null=no_null,
@@ -524,15 +524,15 @@
     return _traverse(block)(*args)
 
 
 def validate_deep_properties(*args, allow_deep=()):
     """
     Warns and returns the number of errors relating to deep objects.
 
-    The schema must use "definitions" instead of nesting "properties".
+    The schema must use "definitions" or "$defs" instead of nesting "properties".
 
     :param allow_deep: JSON Pointers of fields to ignore
     :type allow_deep: list, tuple or set
     :returns: the number of errors
     :rtype: int
     """
     def block(path, data, pointer):
@@ -540,15 +540,20 @@
 
         parts = pointer.rsplit('/', 2)
         if len(parts) == 3:
             grandparent = parts[-2]
         else:
             grandparent = None
 
-        if pointer and grandparent != 'definitions' and 'properties' in data and pointer not in allow_deep:
+        if (
+            pointer
+            and grandparent not in ('definitions', '$defs')
+            and 'properties' in data
+            and pointer not in allow_deep
+        ):
             errors += 1
             warn(f'{path} has "properties" within "properties" at {pointer}', DeepPropertiesWarning)
 
         return errors
 
     return _traverse(block)(*args)
```

### Comparing `jscc-0.2.2/jscc/testing/filesystem.py` & `jscc-0.2.3/jscc/testing/filesystem.py`

 * *Files identical despite different names*

### Comparing `jscc-0.2.2/jscc/testing/util.py` & `jscc-0.2.3/jscc/testing/util.py`

 * *Files identical despite different names*

### Comparing `jscc-0.2.2/jscc.egg-info/PKG-INFO` & `jscc-0.2.3/jscc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jscc
-Version: 0.2.2
+Version: 0.2.3
 Summary: Tools for data standards that use JSON Schema and CSV codelists
 Home-page: https://github.com/open-contracting/jscc
 Author: Open Contracting Partnership and Open Data Services Co-operative Limited
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `jscc-0.2.2/jscc.egg-info/SOURCES.txt` & `jscc-0.2.3/jscc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jscc-0.2.2/setup.cfg` & `jscc-0.2.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jscc
-version = 0.2.2
+version = 0.2.3
 author = Open Contracting Partnership and Open Data Services Co-operative Limited
 author_email = data@open-contracting.org
 license = BSD
 description = Tools for data standards that use JSON Schema and CSV codelists
 url = https://github.com/open-contracting/jscc
 long_description = file: README.rst
 long_description_content_type = text/x-rst
```

### Comparing `jscc-0.2.2/tests/cassettes/test_http_get_error.yaml` & `jscc-0.2.3/tests/cassettes/test_http_get_error.yaml`

 * *Files identical despite different names*

### Comparing `jscc-0.2.2/tests/cassettes/test_http_head_error.yaml` & `jscc-0.2.3/tests/cassettes/test_http_head_error.yaml`

 * *Files identical despite different names*

### Comparing `jscc-0.2.2/tests/fixtures/meta-schema.json` & `jscc-0.2.3/tests/fixtures/meta-schema.json`

 * *Files identical despite different names*

### Comparing `jscc-0.2.2/tests/fixtures/schema/codelist_enum.json` & `jscc-0.2.3/tests/fixtures/schema/codelist_enum.json`

 * *Files identical despite different names*

### Comparing `jscc-0.2.2/tests/fixtures/schema/null_type.json` & `jscc-0.2.3/tests/fixtures/schema/null_type.json`

 * *Files identical despite different names*

### Comparing `jscc-0.2.2/tests/fixtures/schema/object_id.json` & `jscc-0.2.3/tests/fixtures/schema/object_id.json`

 * *Files identical despite different names*

### Comparing `jscc-0.2.2/tests/fixtures/schema.json` & `jscc-0.2.3/tests/fixtures/schema.json`

 * *Files identical despite different names*

### Comparing `jscc-0.2.2/tests/test_checks.py` & `jscc-0.2.3/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `jscc-0.2.2/tests/test_schema.py` & `jscc-0.2.3/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `jscc-0.2.2/tests/test_util.py` & `jscc-0.2.3/tests/test_util.py`

 * *Files identical despite different names*

