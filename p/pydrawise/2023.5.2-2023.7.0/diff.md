# Comparing `tmp/pydrawise-2023.5.2.tar.gz` & `tmp/pydrawise-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydrawise-2023.5.2.tar", last modified: Sun May 21 01:37:02 2023, max compression
+gzip compressed data, was "pydrawise-2023.7.0.tar", last modified: Thu Jul  6 20:18:43 2023, max compression
```

## Comparing `pydrawise-2023.5.2.tar` & `pydrawise-2023.7.0.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.324782 pydrawise-2023.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.320783 pydrawise-2023.5.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.320783 pydrawise-2023.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.github/workflows/publish-python.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.320783 pydrawise-2023.5.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-21 01:37:02.324782 pydrawise-2023.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.320783 pydrawise-2023.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.324782 pydrawise-2023.5.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/docs/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/docs/reference/schema.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/hydrawise.graphql
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.324782 pydrawise-2023.5.2/pydrawise/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/pydrawise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-21 01:37:02.000000 pydrawise-2023.5.2/pydrawise/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/pydrawise/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/pydrawise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/pydrawise/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/pydrawise/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/pydrawise/schema_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.324782 pydrawise-2023.5.2/pydrawise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-21 01:37:02.000000 pydrawise-2023.5.2/pydrawise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-21 01:37:02.000000 pydrawise-2023.5.2/pydrawise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 01:37:02.000000 pydrawise-2023.5.2/pydrawise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-21 01:37:02.000000 pydrawise-2023.5.2/pydrawise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 01:37:02.000000 pydrawise-2023.5.2/pydrawise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 01:37:02.000000 pydrawise-2023.5.2/pydrawise.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 01:37:02.324782 pydrawise-2023.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.324782 pydrawise-2023.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.527273 pydrawise-2023.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.523273 pydrawise-2023.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.523273 pydrawise-2023.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.github/workflows/publish-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.523273 pydrawise-2023.7.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-06 20:18:43.527273 pydrawise-2023.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.523273 pydrawise-2023.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.527273 pydrawise-2023.7.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/docs/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/docs/reference/schema.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/hydrawise.graphql
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.527273 pydrawise-2023.7.0/pydrawise/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pydrawise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-06 20:18:43.000000 pydrawise-2023.7.0/pydrawise/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pydrawise/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pydrawise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pydrawise/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.527273 pydrawise-2023.7.0/pydrawise/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pydrawise/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pydrawise/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pydrawise/schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.527273 pydrawise-2023.7.0/pydrawise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-06 20:18:43.000000 pydrawise-2023.7.0/pydrawise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-06 20:18:43.000000 pydrawise-2023.7.0/pydrawise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:18:43.000000 pydrawise-2023.7.0/pydrawise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-06 20:18:43.000000 pydrawise-2023.7.0/pydrawise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 20:18:43.000000 pydrawise-2023.7.0/pydrawise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:18:43.000000 pydrawise-2023.7.0/pydrawise.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:18:43.527273 pydrawise-2023.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.527273 pydrawise-2023.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18279 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/tests/test_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/tests/test_schema.py
```

### Comparing `pydrawise-2023.5.2/.devcontainer.json` & `pydrawise-2023.7.0/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.2/.github/workflows/build-and-test.yml` & `pydrawise-2023.7.0/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.2/.github/workflows/publish-python.yml` & `pydrawise-2023.7.0/.github/workflows/publish-python.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.2/.gitignore` & `pydrawise-2023.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.2/.pre-commit-config.yaml` & `pydrawise-2023.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.2/LICENSE` & `pydrawise-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.2/PKG-INFO` & `pydrawise-2023.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydrawise
-Version: 2023.5.2
+Version: 2023.7.0
 Summary: Python API for interacting with Hydrawise sprinkler controllers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pydrawise
 Project-URL: Source Code, https://github.com/dknowles2/pydrawise
 Project-URL: Bug Reports, https://github.com/dknowles2/pydrawise/issues
 Keywords: hydrawise,api,iot
```

### Comparing `pydrawise-2023.5.2/README.md` & `pydrawise-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.2/docs/index.md` & `pydrawise-2023.7.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.2/hydrawise.graphql` & `pydrawise-2023.7.0/hydrawise.graphql`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.2/mkdocs.yml` & `pydrawise-2023.7.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.2/pydrawise/auth.py` & `pydrawise-2023.7.0/pydrawise/auth.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.2/pydrawise/client.py` & `pydrawise-2023.7.0/pydrawise/client.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.2/pydrawise/schema.py` & `pydrawise-2023.7.0/pydrawise/schema.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.2/pydrawise/schema_utils.py` & `pydrawise-2023.7.0/pydrawise/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.2/pydrawise.egg-info/PKG-INFO` & `pydrawise-2023.7.0/pydrawise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydrawise
-Version: 2023.5.2
+Version: 2023.7.0
 Summary: Python API for interacting with Hydrawise sprinkler controllers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pydrawise
 Project-URL: Source Code, https://github.com/dknowles2/pydrawise
 Project-URL: Bug Reports, https://github.com/dknowles2/pydrawise/issues
 Keywords: hydrawise,api,iot
```

### Comparing `pydrawise-2023.5.2/pydrawise.egg-info/SOURCES.txt` & `pydrawise-2023.7.0/pydrawise.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -30,11 +30,13 @@
 pydrawise/schema_utils.py
 pydrawise.egg-info/PKG-INFO
 pydrawise.egg-info/SOURCES.txt
 pydrawise.egg-info/dependency_links.txt
 pydrawise.egg-info/requires.txt
 pydrawise.egg-info/top_level.txt
 pydrawise.egg-info/zip-safe
+pydrawise/legacy/__init__.py
 tests/__init__.py
 tests/test_auth.py
 tests/test_client.py
+tests/test_legacy.py
 tests/test_schema.py
```

### Comparing `pydrawise-2023.5.2/pyproject.toml` & `pydrawise-2023.7.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name            = "pydrawise"
 description     = "Python API for interacting with Hydrawise sprinkler controllers."
 authors         = [
     {name = "David Knowles", email = "dknowles2@gmail.com"},
 ]
-dependencies    = ["aiohttp ", "apischema", "gql[aiohttp]", "graphql-core"]
+dependencies    = ["aiohttp ", "apischema", "gql[aiohttp]", "graphql-core", "requests"]
 requires-python = ">=3.10"
 dynamic         = ["readme", "version"]
 license         = {text = "Apache License 2.0"}
 keywords        = ["hydrawise", "api", "iot"]
 classifiers     = [
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
```

### Comparing `pydrawise-2023.5.2/tests/test_auth.py` & `pydrawise-2023.7.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.2/tests/test_client.py` & `pydrawise-2023.7.0/tests/test_client.py`

 * *Files identical despite different names*

