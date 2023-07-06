# Comparing `tmp/jaraco.packaging-9.2.0.tar.gz` & `tmp/jaraco.packaging-9.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.packaging-9.2.0.tar", last modified: Fri May 12 19:21:01 2023, max compression
+gzip compressed data, was "jaraco.packaging-9.3.0.tar", last modified: Thu Jul  6 02:21:55 2023, max compression
```

## Comparing `jaraco.packaging-9.2.0.tar` & `jaraco.packaging-9.3.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:21:01.214823 jaraco.packaging-9.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:21:01.206822 jaraco.packaging-9.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:21:01.206822 jaraco.packaging-9.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-12 19:21:01.214823 jaraco.packaging-9.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:21:01.210823 jaraco.packaging-9.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:21:01.198822 jaraco.packaging-9.2.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:21:01.214823 jaraco.packaging-9.2.0/jaraco/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/jaraco/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/jaraco/packaging/make-tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/jaraco/packaging/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:21:01.210823 jaraco.packaging-9.2.0/jaraco.packaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-12 19:21:01.000000 jaraco.packaging-9.2.0/jaraco.packaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-12 19:21:01.000000 jaraco.packaging-9.2.0/jaraco.packaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:21:01.000000 jaraco.packaging-9.2.0/jaraco.packaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-12 19:21:01.000000 jaraco.packaging-9.2.0/jaraco.packaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 19:21:01.000000 jaraco.packaging-9.2.0/jaraco.packaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-12 19:21:01.214823 jaraco.packaging-9.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:55.443220 jaraco.packaging-9.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:55.439220 jaraco.packaging-9.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:55.439220 jaraco.packaging-9.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-06 02:21:55.443220 jaraco.packaging-9.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:55.439220 jaraco.packaging-9.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:55.439220 jaraco.packaging-9.3.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:55.439220 jaraco.packaging-9.3.0/jaraco/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/jaraco/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/jaraco/packaging/make-tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/jaraco/packaging/sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:55.439220 jaraco.packaging-9.3.0/jaraco.packaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-06 02:21:55.000000 jaraco.packaging-9.3.0/jaraco.packaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-06 02:21:55.000000 jaraco.packaging-9.3.0/jaraco.packaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 02:21:55.000000 jaraco.packaging-9.3.0/jaraco.packaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-06 02:21:55.000000 jaraco.packaging-9.3.0/jaraco.packaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 02:21:55.000000 jaraco.packaging-9.3.0/jaraco.packaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-06 02:21:55.443220 jaraco.packaging-9.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/tox.ini
```

### Comparing `jaraco.packaging-9.2.0/.github/workflows/main.yml` & `jaraco.packaging-9.3.0/.github/workflows/main.yml`

 * *Files 5% similar despite different names*

```diff
@@ -38,57 +38,51 @@
 
 
 jobs:
   test:
     strategy:
       matrix:
         python:
-        - "3.7"
+        - "3.8"
         - "3.11"
         - "3.12"
-        # Workaround for actions/setup-python#508
-        dev:
-        - -dev
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
-        - python: "3.8"
-          platform: ubuntu-latest
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
         - python: pypy3.9
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
     continue-on-error: ${{ matrix.python == '3.12' }}
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
+          python-version: ${{ matrix.python }}
+          allow-prereleases: true
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
 
   docs:
     runs-on: ubuntu-latest
     env:
       TOXENV: docs
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
@@ -115,15 +109,15 @@
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: 3.11-dev
+          python-version: 3.x
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Release
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `jaraco.packaging-9.2.0/CHANGES.rst` & `jaraco.packaging-9.3.0/NEWS.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+v9.3.0
+======
+
+Features
+--------
+
+- Add sidebar-links directive.
+- Require Python 3.8 or later.
+
+
 v9.2.0
 ======
 
 #7, #10, #11: Added environment variable to bypass
 building metadata for offline builds.
 
 v9.1.2
```

### Comparing `jaraco.packaging-9.2.0/LICENSE` & `jaraco.packaging-9.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.2.0/PKG-INFO` & `jaraco.packaging-9.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: jaraco.packaging
-Version: 9.2.0
+Version: 9.3.0
 Summary: tools to supplement packaging Python releases
 Home-page: https://github.com/jaraco/jaraco.packaging
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Sphinx :: Extension
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.packaging.svg
    :target: https://pypi.org/project/jaraco.packaging
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.packaging.svg
 
 .. image:: https://github.com/jaraco/jaraco.packaging/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.packaging/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracopackaging/badge/?version=latest
    :target: https://jaracopackaging.readthedocs.io/en/latest/?badge=latest
```

### Comparing `jaraco.packaging-9.2.0/README.rst` & `jaraco.packaging-9.3.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.packaging.svg
 
 .. image:: https://github.com/jaraco/jaraco.packaging/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.packaging/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracopackaging/badge/?version=latest
    :target: https://jaracopackaging.readthedocs.io/en/latest/?badge=latest
```

### Comparing `jaraco.packaging-9.2.0/docs/conf.py` & `jaraco.packaging-9.3.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 master_doc = "index"
 html_theme = "furo"
 
 # Link dates and other references in the changelog
 extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
@@ -32,11 +32,12 @@
 nitpicky = True
 
 # Include Python intersphinx mapping to prevent failures
 # jaraco/skeleton#51
 extensions += ['sphinx.ext.intersphinx']
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
+    'sphinx': ('https://www.sphinx-doc.org/en/stable/', None),
 }
 
 # Preserve authored syntax for defaults
 autodoc_preserve_defaults = True
```

### Comparing `jaraco.packaging-9.2.0/jaraco/packaging/make-tree.py` & `jaraco.packaging-9.3.0/jaraco/packaging/make-tree.py`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.2.0/jaraco.packaging.egg-info/PKG-INFO` & `jaraco.packaging-9.3.0/jaraco.packaging.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: jaraco.packaging
-Version: 9.2.0
+Version: 9.3.0
 Summary: tools to supplement packaging Python releases
 Home-page: https://github.com/jaraco/jaraco.packaging
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Sphinx :: Extension
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.packaging.svg
    :target: https://pypi.org/project/jaraco.packaging
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.packaging.svg
 
 .. image:: https://github.com/jaraco/jaraco.packaging/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.packaging/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracopackaging/badge/?version=latest
    :target: https://jaracopackaging.readthedocs.io/en/latest/?badge=latest
```

### Comparing `jaraco.packaging-9.2.0/jaraco.packaging.egg-info/SOURCES.txt` & `jaraco.packaging-9.3.0/jaraco.packaging.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 .coveragerc
 .editorconfig
 .pre-commit-config.yaml
 .readthedocs.yaml
-CHANGES.rst
 LICENSE
+NEWS.rst
 README.rst
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
+towncrier.toml
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
 jaraco.packaging.egg-info/PKG-INFO
```

### Comparing `jaraco.packaging-9.2.0/pytest.ini` & `jaraco.packaging-9.3.0/pytest.ini`

 * *Files 8% similar despite different names*

```diff
@@ -17,8 +17,11 @@
 
 	# realpython/pytest-mypy#152
 	ignore:'encoding' argument not specified::pytest_mypy
 
 	# python/cpython#100750
 	ignore:'encoding' argument not specified::platform
 
+	# pypa/build#615
+	ignore:'encoding' argument not specified::build.env
+
 	## end upstream
```

### Comparing `jaraco.packaging-9.2.0/setup.cfg` & `jaraco.packaging-9.3.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Framework :: Sphinx :: Extension
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
-	importlib_metadata; python_version < "3.8"
 	build[virtualenv]
 	jaraco.context
+	sphinx
+	domdf-python-tools
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
 	docs*
 	tests*
@@ -34,16 +35,18 @@
 	pytest >= 6
 	pytest-checkdocs >= 2.4
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.3
+	pytest-enabler >= 2.2
 	pytest-ruff
+	
+	types-docutils
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
```

### Comparing `jaraco.packaging-9.2.0/tox.ini` & `jaraco.packaging-9.3.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 [tox]
-envlist = python
-minversion = 3.2
-# https://github.com/jaraco/skeleton/issues/6
-tox_pip_extensions_ext_venv_update = true
 toxworkdir={env:TOX_WORK_DIR:.tox}
 
 
 [testenv]
 deps =
 setenv =
 	PYTHONWARNDEFAULTENCODING = 1
@@ -21,14 +17,24 @@
 	docs
 	testing
 changedir = docs
 commands =
 	python -m sphinx -W --keep-going . {toxinidir}/build/html
 	python -m sphinxlint
 
+[testenv:finalize]
+skip_install = True
+deps =
+	towncrier
+	jaraco.develop >= 7.23
+passenv = *
+commands =
+	python -m jaraco.develop.finalize
+
+
 [testenv:release]
 skip_install = True
 deps =
 	build
 	twine>=3
 	jaraco.develop>=7.1
 passenv =
```

