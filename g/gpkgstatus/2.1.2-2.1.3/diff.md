# Comparing `tmp/gpkgstatus-2.1.2.tar.gz` & `tmp/gpkgstatus-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpkgstatus-2.1.2.tar", last modified: Fri Mar 31 17:56:42 2023, max compression
+gzip compressed data, was "gpkgstatus-2.1.3.tar", last modified: Thu Jul  6 18:41:33 2023, max compression
```

## Comparing `gpkgstatus-2.1.2.tar` & `gpkgstatus-2.1.3.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:56:42.717278 gpkgstatus-2.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:56:42.713278 gpkgstatus-2.1.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/.devcontainer/dev-reqs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:56:42.709278 gpkgstatus-2.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:56:42.713278 gpkgstatus-2.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/.github/workflows/python-publish-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-03-31 17:56:42.717278 gpkgstatus-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/dev-reqs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:56:42.713278 gpkgstatus-2.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    54772 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/docs/code_of_conduct.html
--rw-r--r--   0 runner    (1001) docker     (123)    63615 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/docs/contributing.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:56:42.713278 gpkgstatus-2.1.2/docs/gpkgstatus/
--rw-r--r--   0 runner    (1001) docker     (123)   154832 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/docs/gpkgstatus/gpkgstatus.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:56:42.713278 gpkgstatus-2.1.2/docs/gpkgstatus/utils/
--rw-r--r--   0 runner    (1001) docker     (123)   118802 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/docs/gpkgstatus/utils/config.html
--rw-r--r--   0 runner    (1001) docker     (123)   117835 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/docs/gpkgstatus/utils/json_file_reader.html
--rw-r--r--   0 runner    (1001) docker     (123)   103999 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/docs/gpkgstatus/utils/url_reader.html
--rw-r--r--   0 runner    (1001) docker     (123)    49824 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/docs/gpkgstatus/utils.html
--rw-r--r--   0 runner    (1001) docker     (123)    48551 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/docs/gpkgstatus.html
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    30728 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/docs/search.js
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 17:56:42.717278 gpkgstatus-2.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:56:42.709278 gpkgstatus-2.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:56:42.717278 gpkgstatus-2.1.2/src/gpkgstatus/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/src/gpkgstatus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/src/gpkgstatus/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/src/gpkgstatus/gpkgstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:56:42.717278 gpkgstatus-2.1.2/src/gpkgstatus/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/src/gpkgstatus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/src/gpkgstatus/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/src/gpkgstatus/utils/json_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/src/gpkgstatus/utils/url_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:56:42.717278 gpkgstatus-2.1.2/src/gpkgstatus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-03-31 17:56:42.000000 gpkgstatus-2.1.2/src/gpkgstatus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-31 17:56:42.000000 gpkgstatus-2.1.2/src/gpkgstatus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 17:56:42.000000 gpkgstatus-2.1.2/src/gpkgstatus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-31 17:56:42.000000 gpkgstatus-2.1.2/src/gpkgstatus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-31 17:56:42.000000 gpkgstatus-2.1.2/src/gpkgstatus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-31 17:56:42.000000 gpkgstatus-2.1.2/src/gpkgstatus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:56:42.717278 gpkgstatus-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/tests/test_fedora_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/tests/test_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-31 17:56:32.000000 gpkgstatus-2.1.2/tests/test_url_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:41:33.824115 gpkgstatus-2.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:41:33.820115 gpkgstatus-2.1.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/.devcontainer/dev-reqs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:41:33.820115 gpkgstatus-2.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:41:33.820115 gpkgstatus-2.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/.github/workflows/python-publish-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-07-06 18:41:33.824115 gpkgstatus-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/dev-reqs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:41:33.824115 gpkgstatus-2.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    54772 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/docs/code_of_conduct.html
+-rw-r--r--   0 runner    (1001) docker     (123)    63615 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/docs/contributing.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:41:33.824115 gpkgstatus-2.1.3/docs/gpkgstatus/
+-rw-r--r--   0 runner    (1001) docker     (123)   154832 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/docs/gpkgstatus/gpkgstatus.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:41:33.824115 gpkgstatus-2.1.3/docs/gpkgstatus/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)   118802 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/docs/gpkgstatus/utils/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)   117835 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/docs/gpkgstatus/utils/json_file_reader.html
+-rw-r--r--   0 runner    (1001) docker     (123)   103999 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/docs/gpkgstatus/utils/url_reader.html
+-rw-r--r--   0 runner    (1001) docker     (123)    49824 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/docs/gpkgstatus/utils.html
+-rw-r--r--   0 runner    (1001) docker     (123)    48551 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/docs/gpkgstatus.html
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    30728 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/docs/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/faqs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:41:33.824115 gpkgstatus-2.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:41:33.820115 gpkgstatus-2.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:41:33.824115 gpkgstatus-2.1.3/src/gpkgstatus/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/src/gpkgstatus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/src/gpkgstatus/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/src/gpkgstatus/gpkgstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:41:33.824115 gpkgstatus-2.1.3/src/gpkgstatus/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/src/gpkgstatus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/src/gpkgstatus/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/src/gpkgstatus/utils/json_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/src/gpkgstatus/utils/url_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:41:33.824115 gpkgstatus-2.1.3/src/gpkgstatus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-07-06 18:41:33.000000 gpkgstatus-2.1.3/src/gpkgstatus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-06 18:41:33.000000 gpkgstatus-2.1.3/src/gpkgstatus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:41:33.000000 gpkgstatus-2.1.3/src/gpkgstatus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 18:41:33.000000 gpkgstatus-2.1.3/src/gpkgstatus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-06 18:41:33.000000 gpkgstatus-2.1.3/src/gpkgstatus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 18:41:33.000000 gpkgstatus-2.1.3/src/gpkgstatus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:41:33.824115 gpkgstatus-2.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/tests/test_fedora_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/tests/test_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-06 18:41:24.000000 gpkgstatus-2.1.3/tests/test_url_reader.py
```

### Comparing `gpkgstatus-2.1.2/.devcontainer/dev-reqs.txt` & `gpkgstatus-2.1.3/.devcontainer/dev-reqs.txt`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/.github/workflows/codeql.yml` & `gpkgstatus-2.1.3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/.github/workflows/python-publish-test.yml` & `gpkgstatus-2.1.3/.github/workflows/python-publish-test.yml`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/.github/workflows/python-publish.yml` & `gpkgstatus-2.1.3/.github/workflows/python-publish.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # This workflow will:
 # - black-formatting: Analyze code with black.
 
 # - test: (on supported python versions)
 #   Analyze code with Pylint 
 #   Validate pyproject.toml for errors
-#   Test with pytest 
 
 # - build-n-publish: Build and Publish Python package
 # to PyPI.
 
 name: Publish Package on PyPI
 
 on:
@@ -79,18 +78,14 @@
       
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
           pip install pytest
 
-      - name: Test with pytest
-        run: |
-          pytest -v .
-
   
   build-n-publish:
     needs: test
     name: Build and publish Python 🐍 distributions 📦 to PyPI and TestPyPI
     runs-on: ubuntu-latest
 
     steps:
```

### Comparing `gpkgstatus-2.1.2/.github/workflows/python-test.yml` & `gpkgstatus-2.1.3/.github/workflows/python-test.yml`

 * *Files 6% similar despite different names*

```diff
@@ -56,11 +56,7 @@
         run: >-
           pylint 
           src/
       
       - name: Validate pyproject.toml
         run: |
           validate-pyproject pyproject.toml
-
-      - name: Test with pytest
-        run: |
-          pytest -v .
```

### Comparing `gpkgstatus-2.1.2/.github/workflows/release.yml` & `gpkgstatus-2.1.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/.gitignore` & `gpkgstatus-2.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/CODE_OF_CONDUCT.md` & `gpkgstatus-2.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/CONTRIBUTING.md` & `gpkgstatus-2.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/LICENSE` & `gpkgstatus-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/PKG-INFO` & `gpkgstatus-2.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpkgstatus
-Version: 2.1.2
+Version: 2.1.3
 Summary: Get Current Package Status from Fedora Updates System
 Author: Dhanush Kovi
 License: GPL-2.0-or-later
 Project-URL: Homepage, https://dkvc.github.io/gpkgstatus/
 Project-URL: Documentation, https://dkvc.github.io/gpkgstatus/
 Project-URL: Repository, https://github.com/dkvc/gpkgstatus
 Keywords: fedora,updates,package,status,fedora-updates,gpkgstatus,bodhi
@@ -99,7 +99,15 @@
   -v, --verbose         Enable verbose output
   --version             gpkgstatus version
 ```
 
 ## Contributing
 
 You are welcome to contribute to this project. Make sure to read [Contributing Guidelines](https://github.com/dkvc/gpkgstatus/blob/main/CONTRIBUTING.md). If you have any questions regarding contributing to this project, you can open an issue about it.
+
+## Credits
+The development of this project would not have been possible without [Bodhi](https://bodhi.fedoraproject.org) developed by the [Fedora Project](https://fedoraproject.org). Although this project is unofficial and not affiliated with Bodhi or Fedora, we appreciate the valuable contributions made by the Bodhi and its developers.
+
+For more information about the Bodhi Project, please visit their [official repository](https://github.com/fedora-infra/bodhi) on GitHub.
+
+## FAQs
+You can find FAQs (Frequently Asked Questions) in [faqs.md](./faqs.md)
```

### Comparing `gpkgstatus-2.1.2/README.md` & `gpkgstatus-2.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -74,7 +74,15 @@
   -v, --verbose         Enable verbose output
   --version             gpkgstatus version
 ```
 
 ## Contributing
 
 You are welcome to contribute to this project. Make sure to read [Contributing Guidelines](https://github.com/dkvc/gpkgstatus/blob/main/CONTRIBUTING.md). If you have any questions regarding contributing to this project, you can open an issue about it.
+
+## Credits
+The development of this project would not have been possible without [Bodhi](https://bodhi.fedoraproject.org) developed by the [Fedora Project](https://fedoraproject.org). Although this project is unofficial and not affiliated with Bodhi or Fedora, we appreciate the valuable contributions made by the Bodhi and its developers.
+
+For more information about the Bodhi Project, please visit their [official repository](https://github.com/fedora-infra/bodhi) on GitHub.
+
+## FAQs
+You can find FAQs (Frequently Asked Questions) in [faqs.md](./faqs.md)
```

### Comparing `gpkgstatus-2.1.2/dev-reqs.txt` & `gpkgstatus-2.1.3/dev-reqs.txt`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/docs/code_of_conduct.html` & `gpkgstatus-2.1.3/docs/code_of_conduct.html`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/docs/contributing.html` & `gpkgstatus-2.1.3/docs/contributing.html`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/docs/gpkgstatus/gpkgstatus.html` & `gpkgstatus-2.1.3/docs/gpkgstatus/gpkgstatus.html`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/docs/gpkgstatus/utils/config.html` & `gpkgstatus-2.1.3/docs/gpkgstatus/utils/config.html`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/docs/gpkgstatus/utils/json_file_reader.html` & `gpkgstatus-2.1.3/docs/gpkgstatus/utils/json_file_reader.html`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/docs/gpkgstatus/utils/url_reader.html` & `gpkgstatus-2.1.3/docs/gpkgstatus/utils/url_reader.html`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/docs/gpkgstatus/utils.html` & `gpkgstatus-2.1.3/docs/gpkgstatus/utils.html`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/docs/gpkgstatus.html` & `gpkgstatus-2.1.3/docs/gpkgstatus.html`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/docs/search.js` & `gpkgstatus-2.1.3/docs/search.js`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/pyproject.toml` & `gpkgstatus-2.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/src/gpkgstatus/gpkgstatus.py` & `gpkgstatus-2.1.3/src/gpkgstatus/gpkgstatus.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,21 @@
     If terminal does not support ASCII colors, then normal text
     is printed.
 
     Args:
         update (dict): Dictionary of Updates containing metadata.
         status_color (str): ASCII Color if explicitly given.
     """
-    colors = {"stable": "green", "testing": "yellow", "pending": "red"}
+    colors = {
+        "stable": "green",
+        "testing": "yellow",
+        "pending": "red",
+        "unpushed": "cyan",
+        "obselete": "magneta",
+    }
 
     if update["status"].lower() in colors:
         status_color = colors[update["status"]]
     else:
         status_color = "blue"
 
     print(colored(f"Update ID: {update['updateid']}", status_color))
```

### Comparing `gpkgstatus-2.1.2/src/gpkgstatus/utils/config.py` & `gpkgstatus-2.1.3/src/gpkgstatus/utils/config.py`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/src/gpkgstatus/utils/json_file_reader.py` & `gpkgstatus-2.1.3/src/gpkgstatus/utils/json_file_reader.py`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/src/gpkgstatus/utils/url_reader.py` & `gpkgstatus-2.1.3/src/gpkgstatus/utils/url_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,16 @@
         there is an issue parsing JSON from corresponding url and might
         not be a valid JSON url.
 
         Returns:
             Any: Returns JSON response of corresponding JSON url.
         """
         try:
-            response = requests.get(self._url, timeout=15)
+            headers = {"accept": "application/json"}
+            response = requests.get(self._url, timeout=15, headers=headers)
             sleep(1)
             logging.info("GET Request from %s succeeded", self._url)
 
             return response.json()
         except requests.exceptions.JSONDecodeError:
             print(
                 colored(
```

### Comparing `gpkgstatus-2.1.2/src/gpkgstatus.egg-info/PKG-INFO` & `gpkgstatus-2.1.3/src/gpkgstatus.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpkgstatus
-Version: 2.1.2
+Version: 2.1.3
 Summary: Get Current Package Status from Fedora Updates System
 Author: Dhanush Kovi
 License: GPL-2.0-or-later
 Project-URL: Homepage, https://dkvc.github.io/gpkgstatus/
 Project-URL: Documentation, https://dkvc.github.io/gpkgstatus/
 Project-URL: Repository, https://github.com/dkvc/gpkgstatus
 Keywords: fedora,updates,package,status,fedora-updates,gpkgstatus,bodhi
@@ -99,7 +99,15 @@
   -v, --verbose         Enable verbose output
   --version             gpkgstatus version
 ```
 
 ## Contributing
 
 You are welcome to contribute to this project. Make sure to read [Contributing Guidelines](https://github.com/dkvc/gpkgstatus/blob/main/CONTRIBUTING.md). If you have any questions regarding contributing to this project, you can open an issue about it.
+
+## Credits
+The development of this project would not have been possible without [Bodhi](https://bodhi.fedoraproject.org) developed by the [Fedora Project](https://fedoraproject.org). Although this project is unofficial and not affiliated with Bodhi or Fedora, we appreciate the valuable contributions made by the Bodhi and its developers.
+
+For more information about the Bodhi Project, please visit their [official repository](https://github.com/fedora-infra/bodhi) on GitHub.
+
+## FAQs
+You can find FAQs (Frequently Asked Questions) in [faqs.md](./faqs.md)
```

### Comparing `gpkgstatus-2.1.2/src/gpkgstatus.egg-info/SOURCES.txt` & `gpkgstatus-2.1.3/src/gpkgstatus.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitignore
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 dev-reqs.txt
+faqs.md
 pyproject.toml
 requirements.txt
 .devcontainer/Dockerfile
 .devcontainer/dev-reqs.txt
 .devcontainer/devcontainer.json
 .github/workflows/codeql.yml
 .github/workflows/python-publish-test.yml
```

### Comparing `gpkgstatus-2.1.2/src/gpkgstatus.egg-info/requires.txt` & `gpkgstatus-2.1.3/src/gpkgstatus.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-requests==2.28.2
+requests==2.31.0
 termcolor==2.2.0
 
 [dev]
 altgraph>=0.17.3
 astroid>=2.14.2
 attrs>=22.2.0
 black>=23.1.0
```

### Comparing `gpkgstatus-2.1.2/tests/test_fedora_updates.py` & `gpkgstatus-2.1.3/tests/test_fedora_updates.py`

 * *Files identical despite different names*

### Comparing `gpkgstatus-2.1.2/tests/test_url_reader.py` & `gpkgstatus-2.1.3/tests/test_url_reader.py`

 * *Files identical despite different names*

