# Comparing `tmp/maccarone-0.1.5.tar.gz` & `tmp/maccarone-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maccarone-0.1.5.tar", last modified: Wed Jul  5 23:55:01 2023, max compression
+gzip compressed data, was "maccarone-0.1.6.tar", last modified: Thu Jul  6 17:00:38 2023, max compression
```

## Comparing `maccarone-0.1.5.tar` & `maccarone-0.1.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:55:01.390445 maccarone-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:55:01.386445 maccarone-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:55:01.390445 maccarone-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-05 23:54:49.000000 maccarone-0.1.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-05 23:54:49.000000 maccarone-0.1.5/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-05 23:54:49.000000 maccarone-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-05 23:54:49.000000 maccarone-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-05 23:55:01.390445 maccarone-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-05 23:54:49.000000 maccarone-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-05 23:54:49.000000 maccarone-0.1.5/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:55:01.390445 maccarone-0.1.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 23:54:49.000000 maccarone-0.1.5/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-05 23:54:49.000000 maccarone-0.1.5/examples/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-05 23:54:49.000000 maccarone-0.1.5/examples/file_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-05 23:54:49.000000 maccarone-0.1.5/examples/file_sizes_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-05 23:54:49.000000 maccarone-0.1.5/examples/fizzbuzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-05 23:54:49.000000 maccarone-0.1.5/examples/todo.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-05 23:54:49.000000 maccarone-0.1.5/local-dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-05 23:54:49.000000 maccarone-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 23:55:01.390445 maccarone-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:55:01.390445 maccarone-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:55:01.390445 maccarone-0.1.5/src/maccarone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 23:54:49.000000 maccarone-0.1.5/src/maccarone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-05 23:54:49.000000 maccarone-0.1.5/src/maccarone/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-07-05 23:54:49.000000 maccarone-0.1.5/src/maccarone/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:55:01.390445 maccarone-0.1.5/src/maccarone/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-05 23:54:49.000000 maccarone-0.1.5/src/maccarone/scripts/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:55:01.390445 maccarone-0.1.5/src/maccarone/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-05 23:54:49.000000 maccarone-0.1.5/src/maccarone/test/test_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:55:01.390445 maccarone-0.1.5/src/maccarone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-05 23:55:01.000000 maccarone-0.1.5/src/maccarone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-05 23:55:01.000000 maccarone-0.1.5/src/maccarone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 23:55:01.000000 maccarone-0.1.5/src/maccarone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-05 23:55:01.000000 maccarone-0.1.5/src/maccarone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 23:55:01.000000 maccarone-0.1.5/src/maccarone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 23:55:01.000000 maccarone-0.1.5/src/maccarone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:38.794605 maccarone-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:38.790605 maccarone-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:38.790605 maccarone-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-06 17:00:27.000000 maccarone-0.1.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-06 17:00:27.000000 maccarone-0.1.6/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-06 17:00:27.000000 maccarone-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 17:00:27.000000 maccarone-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-06 17:00:38.794605 maccarone-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-06 17:00:27.000000 maccarone-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-06 17:00:27.000000 maccarone-0.1.6/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:38.790605 maccarone-0.1.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 17:00:27.000000 maccarone-0.1.6/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-06 17:00:27.000000 maccarone-0.1.6/examples/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-06 17:00:27.000000 maccarone-0.1.6/examples/file_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-06 17:00:27.000000 maccarone-0.1.6/examples/file_sizes_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-06 17:00:27.000000 maccarone-0.1.6/examples/fizzbuzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-06 17:00:27.000000 maccarone-0.1.6/examples/todo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-06 17:00:27.000000 maccarone-0.1.6/local-dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-06 17:00:27.000000 maccarone-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 17:00:38.794605 maccarone-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:38.790605 maccarone-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:38.790605 maccarone-0.1.6/src/maccarone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:27.000000 maccarone-0.1.6/src/maccarone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-06 17:00:27.000000 maccarone-0.1.6/src/maccarone/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-07-06 17:00:27.000000 maccarone-0.1.6/src/maccarone/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:38.794605 maccarone-0.1.6/src/maccarone/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-06 17:00:27.000000 maccarone-0.1.6/src/maccarone/scripts/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:38.794605 maccarone-0.1.6/src/maccarone/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-06 17:00:27.000000 maccarone-0.1.6/src/maccarone/test/test_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:38.794605 maccarone-0.1.6/src/maccarone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-06 17:00:38.000000 maccarone-0.1.6/src/maccarone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-06 17:00:38.000000 maccarone-0.1.6/src/maccarone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 17:00:38.000000 maccarone-0.1.6/src/maccarone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 17:00:38.000000 maccarone-0.1.6/src/maccarone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-06 17:00:38.000000 maccarone-0.1.6/src/maccarone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 17:00:38.000000 maccarone-0.1.6/src/maccarone.egg-info/top_level.txt
```

### Comparing `maccarone-0.1.5/.github/workflows/publish-to-pypi.yml` & `maccarone-0.1.6/.github/workflows/publish-to-pypi.yml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   release:
     types: [published]
 jobs:
   publish-to-pypi:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.10"]
+        python-version: ["3.8"]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - run: python -m pip install --upgrade pip
       - name: Build package
```

### Comparing `maccarone-0.1.5/.gitignore` & `maccarone-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.5/LICENSE` & `maccarone-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.5/PKG-INFO` & `maccarone-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maccarone
-Version: 0.1.5
+Version: 0.1.6
 Summary: Mix natural language into your Python code
 Project-URL: Homepage, https://github.com/bsilverthorn/maccarone
 Project-URL: Repository, https://github.com/bsilverthorn/maccarone
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `maccarone-0.1.5/README.md` & `maccarone-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.5/dev-requirements.txt` & `maccarone-0.1.6/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.5/examples/file_sizes_ext.py` & `maccarone-0.1.6/examples/file_sizes_ext.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.5/examples/todo.py` & `maccarone-0.1.6/examples/todo.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.5/pyproject.toml` & `maccarone-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.5/src/maccarone/openai.py` & `maccarone-0.1.6/src/maccarone/openai.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.5/src/maccarone/preprocessor.py` & `maccarone-0.1.6/src/maccarone/preprocessor.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.5/src/maccarone/scripts/preprocess.py` & `maccarone-0.1.6/src/maccarone/scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.5/src/maccarone/test/test_preprocessor.py` & `maccarone-0.1.6/src/maccarone/test/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.5/src/maccarone.egg-info/PKG-INFO` & `maccarone-0.1.6/src/maccarone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maccarone
-Version: 0.1.5
+Version: 0.1.6
 Summary: Mix natural language into your Python code
 Project-URL: Homepage, https://github.com/bsilverthorn/maccarone
 Project-URL: Repository, https://github.com/bsilverthorn/maccarone
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `maccarone-0.1.5/src/maccarone.egg-info/SOURCES.txt` & `maccarone-0.1.6/src/maccarone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

