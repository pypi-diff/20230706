# Comparing `tmp/pytest_netdut-0.7.0.tar.gz` & `tmp/pytest_netdut-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_netdut-0.7.0.tar", last modified: Mon Jun 19 04:56:09 2023, max compression
+gzip compressed data, was "pytest_netdut-0.8.0.tar", last modified: Thu Jul  6 02:55:31 2023, max compression
```

## Comparing `pytest_netdut-0.7.0.tar` & `pytest_netdut-0.8.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.320307 pytest_netdut-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.316307 pytest_netdut-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.316307 pytest_netdut-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-19 04:56:09.320307 pytest_netdut-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.316307 pytest_netdut-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.316307 pytest_netdut-0.7.0/docs/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.316307 pytest_netdut-0.7.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   114704 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/docs/images/failed_assertion.png
--rw-r--r--   0 runner    (1001) docker     (123)    90069 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/docs/images/test_showver_results.png
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.320307 pytest_netdut-0.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/examples/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/examples/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/examples/test_eapi_ssh_x.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/examples/test_showver.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/examples/test_skip_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/examples/test_using_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-19 04:56:09.320307 pytest_netdut-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.316307 pytest_netdut-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.320307 pytest_netdut-0.7.0/src/pytest_netdut/
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/src/pytest_netdut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/src/pytest_netdut/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    18406 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/src/pytest_netdut/px.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/src/pytest_netdut/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/src/pytest_netdut/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.320307 pytest_netdut-0.7.0/src/pytest_netdut.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-19 04:56:09.000000 pytest_netdut-0.7.0/src/pytest_netdut.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-19 04:56:09.000000 pytest_netdut-0.7.0/src/pytest_netdut.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 04:56:09.000000 pytest_netdut-0.7.0/src/pytest_netdut.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-19 04:56:09.000000 pytest_netdut-0.7.0/src/pytest_netdut.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 04:56:09.000000 pytest_netdut-0.7.0/src/pytest_netdut.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:56:09.320307 pytest_netdut-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/tests/test_netdut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/tests/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/tests/test_wait_for.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/tests/test_xapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-19 04:55:54.000000 pytest_netdut-0.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:55:31.446746 pytest_netdut-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:55:31.442746 pytest_netdut-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:55:31.442746 pytest_netdut-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-07-06 02:55:31.446746 pytest_netdut-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:55:31.442746 pytest_netdut-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:55:31.442746 pytest_netdut-0.8.0/docs/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:55:31.442746 pytest_netdut-0.8.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   114704 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/docs/images/failed_assertion.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90069 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/docs/images/test_showver_results.png
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:55:31.446746 pytest_netdut-0.8.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/examples/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/examples/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/examples/test_eapi_ssh_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/examples/test_showver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/examples/test_skip_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/examples/test_using_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-06 02:55:31.446746 pytest_netdut-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:55:31.442746 pytest_netdut-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:55:31.446746 pytest_netdut-0.8.0/src/pytest_netdut/
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/src/pytest_netdut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/src/pytest_netdut/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18406 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/src/pytest_netdut/px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/src/pytest_netdut/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/src/pytest_netdut/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:55:31.446746 pytest_netdut-0.8.0/src/pytest_netdut.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-07-06 02:55:31.000000 pytest_netdut-0.8.0/src/pytest_netdut.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 02:55:31.000000 pytest_netdut-0.8.0/src/pytest_netdut.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 02:55:31.000000 pytest_netdut-0.8.0/src/pytest_netdut.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-06 02:55:31.000000 pytest_netdut-0.8.0/src/pytest_netdut.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 02:55:31.000000 pytest_netdut-0.8.0/src/pytest_netdut.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:55:31.446746 pytest_netdut-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/tests/test_netdut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/tests/test_wait_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/tests/test_xapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-06 02:55:09.000000 pytest_netdut-0.8.0/tox.ini
```

### Comparing `pytest_netdut-0.7.0/.github/workflows/build.yaml` & `pytest_netdut-0.8.0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/.github/workflows/release.yaml` & `pytest_netdut-0.8.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/.gitignore` & `pytest_netdut-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/Dockerfile` & `pytest_netdut-0.8.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/LICENSE` & `pytest_netdut-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/Makefile` & `pytest_netdut-0.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/PKG-INFO` & `pytest_netdut-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_netdut
-Version: 0.7.0
+Version: 0.8.0
 Summary: "Automated software testing for switches using pytest"
 Home-page: https://github.com/aristanetworks/pytest-netdut
 Author: "David Snowdon"
 Author-email: "daves@arista.com"
 Maintainer: "Alex Webster"
 Maintainer-email: "alexw@arista.com"
 License: "BSD 3-Clause License"
@@ -19,28 +19,28 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/markdown
 
 Netdut: automated software testing for switches using pytest
 ============================================================
 
-![PyPi](https://img.shields.io/pypi/v/pytest-netdut.svg) 
+![PyPi](https://img.shields.io/pypi/v/pytest-netdut.svg)
 ![Python Versions](https://img.shields.io/pypi/pyversions/pytest-netdut.svg)
-![collection version](https://img.shields.io/github/v/release/aristanetworks/pytest-netdut) 
+![collection version](https://img.shields.io/github/v/release/aristanetworks/pytest-netdut)
 ![License](https://img.shields.io/github/license/aristanetworks/pytest-netdut)
 
 Netdut is a [pytest](https://docs.pytest.org/) plugin which provides infrastructure (e.g. pytest fixtures) which make it easy to write automated tests for network switches.
 
 
 Features
 --------
 
 * Brings the power, maturity and ecosystem of pytest to testing on network switches.
-* The `dut` fixture (Device Under Test) providing serial, ssh or [EAPI](https://github.com/arista-eosplus/pyeapi) connectivity for running CLI commands on a network switch. 
-* Command-line configuration of a hostname and console name. 
+* The `dut` fixture (Device Under Test) providing serial, ssh or [EAPI](https://github.com/arista-eosplus/pyeapi) connectivity for running CLI commands on a network switch.
+* Command-line configuration of a hostname and console name.
 * Markers for skipping tests based on the device's type or software configuration.
 * Compatibility with both Arista's EOS operating system, and the Metamako MOS operating system.
 * A pythonic interfaces for writing EOS CLI commands.
 
 
 Requirements
 ------------
@@ -174,14 +174,26 @@
 ```python
 @pytest.mark.eos
 @pytest.mark.skip_device_type("DCS-7130.*")
 def test_that_only_runs_on_eos_on_7130(dut):
     logging.info("Must be EOS on 7130!")
 ```
 
+OS decorators accept the following keywords:
+ - min_version (string)
+ - min_change_number (int)
+
+If both kwargs are specified, min_change_number takes precedence.
+```python
+@pytest.mark.eos(min_version="4.30.0", min_change_number=3452345)
+@pytest.mark.skip_device_type("DCS-7130.*")
+def test_that_only_runs_on_eos_on_7130(dut):
+    logging.info("Must be EOS on 7130!")
+```
+
 ### Building test harnesses
 
 Pytest's fixture mechanism is very powerful in this scenario, allowing us to set up and tear
 down test configurations with low overhead.
 
 ```python
 @pytest.fixture
@@ -234,15 +246,15 @@
 
 The translator will also process return values; MOS EAPI result keys are camelCased and the translator will convert all keys
 to snake_case.
 
 The translator has a predefined set of translations which can be extended by subclassing the Translator class and overriding `config_patterns`.
 Return values are processed by the `translate_key` function which must be defined in the subclass.
 
-Set the new translator class via `eapi.set_translator(<class instance>)`. 
+Set the new translator class via `eapi.set_translator(<class instance>)`.
 
 Contributing
 ------------
 This project is under active use and development. We would appreciate help to improve it,
 via pull request. Tests can be run with `make ci` or `tox`.
 
 Docstrings are according to [Google's docstring conventions](https://google.github.io/styleguide/pyguide.html) ([examples](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html)).
```

### Comparing `pytest_netdut-0.7.0/README.md` & `pytest_netdut-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Netdut: automated software testing for switches using pytest
 ============================================================
 
-![PyPi](https://img.shields.io/pypi/v/pytest-netdut.svg) 
+![PyPi](https://img.shields.io/pypi/v/pytest-netdut.svg)
 ![Python Versions](https://img.shields.io/pypi/pyversions/pytest-netdut.svg)
-![collection version](https://img.shields.io/github/v/release/aristanetworks/pytest-netdut) 
+![collection version](https://img.shields.io/github/v/release/aristanetworks/pytest-netdut)
 ![License](https://img.shields.io/github/license/aristanetworks/pytest-netdut)
 
 Netdut is a [pytest](https://docs.pytest.org/) plugin which provides infrastructure (e.g. pytest fixtures) which make it easy to write automated tests for network switches.
 
 
 Features
 --------
 
 * Brings the power, maturity and ecosystem of pytest to testing on network switches.
-* The `dut` fixture (Device Under Test) providing serial, ssh or [EAPI](https://github.com/arista-eosplus/pyeapi) connectivity for running CLI commands on a network switch. 
-* Command-line configuration of a hostname and console name. 
+* The `dut` fixture (Device Under Test) providing serial, ssh or [EAPI](https://github.com/arista-eosplus/pyeapi) connectivity for running CLI commands on a network switch.
+* Command-line configuration of a hostname and console name.
 * Markers for skipping tests based on the device's type or software configuration.
 * Compatibility with both Arista's EOS operating system, and the Metamako MOS operating system.
 * A pythonic interfaces for writing EOS CLI commands.
 
 
 Requirements
 ------------
@@ -152,14 +152,26 @@
 ```python
 @pytest.mark.eos
 @pytest.mark.skip_device_type("DCS-7130.*")
 def test_that_only_runs_on_eos_on_7130(dut):
     logging.info("Must be EOS on 7130!")
 ```
 
+OS decorators accept the following keywords:
+ - min_version (string)
+ - min_change_number (int)
+
+If both kwargs are specified, min_change_number takes precedence.
+```python
+@pytest.mark.eos(min_version="4.30.0", min_change_number=3452345)
+@pytest.mark.skip_device_type("DCS-7130.*")
+def test_that_only_runs_on_eos_on_7130(dut):
+    logging.info("Must be EOS on 7130!")
+```
+
 ### Building test harnesses
 
 Pytest's fixture mechanism is very powerful in this scenario, allowing us to set up and tear
 down test configurations with low overhead.
 
 ```python
 @pytest.fixture
@@ -212,15 +224,15 @@
 
 The translator will also process return values; MOS EAPI result keys are camelCased and the translator will convert all keys
 to snake_case.
 
 The translator has a predefined set of translations which can be extended by subclassing the Translator class and overriding `config_patterns`.
 Return values are processed by the `translate_key` function which must be defined in the subclass.
 
-Set the new translator class via `eapi.set_translator(<class instance>)`. 
+Set the new translator class via `eapi.set_translator(<class instance>)`.
 
 Contributing
 ------------
 This project is under active use and development. We would appreciate help to improve it,
 via pull request. Tests can be run with `make ci` or `tox`.
 
 Docstrings are according to [Google's docstring conventions](https://google.github.io/styleguide/pyguide.html) ([examples](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html)).
```

### Comparing `pytest_netdut-0.7.0/docs/images/failed_assertion.png` & `pytest_netdut-0.8.0/docs/images/failed_assertion.png`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/docs/images/test_showver_results.png` & `pytest_netdut-0.8.0/docs/images/test_showver_results.png`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/examples/test_daemon.py` & `pytest_netdut-0.8.0/examples/test_daemon.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/examples/test_eapi_ssh_x.py` & `pytest_netdut-0.8.0/examples/test_eapi_ssh_x.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/examples/test_skip_demo.py` & `pytest_netdut-0.8.0/examples/test_skip_demo.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/mkdocs.yml` & `pytest_netdut-0.8.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/setup.cfg` & `pytest_netdut-0.8.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 package_dir = 
 	=src
 install_requires = 
 	pexpect >= 4.8.0
 	pyeapi>=0.8.4
 	pytest>=3.5.0
 	six>=1.15
+	packaging>=22.0
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = README.md
```

### Comparing `pytest_netdut-0.7.0/src/pytest_netdut/__init__.py` & `pytest_netdut-0.8.0/src/pytest_netdut/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,14 +140,15 @@
     fixtures = [
         factories.create_dut_fixture(name),
         factories.create_eapi_fixture(name),
         factories.create_hostname_fixture(name),
         factories.create_console_url_fixture(name),
         factories.create_skipper_fixture(name),
         factories.create_sku_fixture(name),
+        factories.create_os_version_fixture(name),
         factories.create_softened_fixture(name),
         factories.create_ssh_fixture(name),
         factories.create_xapi_fixture(name),
         factories.create_console_fixture(name),
     ]
 
     for fixture in fixtures:
```

### Comparing `pytest_netdut-0.7.0/src/pytest_netdut/factories.py` & `pytest_netdut-0.8.0/src/pytest_netdut/factories.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # - Tags:
 # -   license-bsd-3-clause
 # -
 # -------------------------------------------------------------------------------
 import logging
 import re
 import pytest
+from packaging import version
 from .wrappers import CLI, xapi
 
 logger = logging.getLogger(__name__)
 
 
 def create_dut_fixture(name):
     @pytest.fixture(name=f"{name}")
@@ -68,24 +69,54 @@
     @pytest.fixture(scope="session", name=f"{name}_console_url")
     def _console_url(request):
         yield request.getfixturevalue(f"{name}_info")["console_url"]
 
     return _console_url
 
 
+def parse_version(v):
+    """Return series of dot separated digits from beginning of string
+    as release and the last group delimited by - as change number."""
+    _regex = r"""
+        (?P<release>[0-9]+(?:\.[0-9]+)*)
+        (?:
+            [-]?
+            (?P<change_number>[\w]+)
+        )*
+    """
+    _regex = re.compile(_regex, re.VERBOSE)
+    # _regex = r"(?P<release>[\d\.]*)"
+    parsed = re.match(_regex, v)
+    return (parsed.group("release"), parsed.group("change_number"))
+
+
+def version_skipper(found, expected):
+    try:
+        found = version.Version(str(found))
+        expected = version.Version(str(expected))
+        if found < expected:
+            pytest.skip(f"min_version {expected} not satisfied: {found}")
+    except version.InvalidVersion:
+        logging.error("Could not parse versions: %s < %s", found, expected)
+
+
 def create_skipper_fixture(name):
     @pytest.fixture(scope="session", name=f"{name}_skipper")
     def _skipper(request):
         def skipper(node):
             allowed_os = set()
+            min_version = None
+            min_chg_num = None
 
             # Restrict SKUs
             for marker in node.iter_markers():
                 if marker.name in {"mos", "eos"}:
                     allowed_os.add(marker.name)
+                    min_chg_num = marker.kwargs.get("min_change_number", None)
+                    min_version = marker.kwargs.get("min_version", None)
 
                 elif marker.name == "only_device_type":
                     pattern = marker.args[0]
                     sku = request.getfixturevalue(f"{name}_sku")
                     if not re.search(pattern, sku):
                         pytest.skip(f"Skipped on this SKU: {sku} (only runs on {pattern})")
 
@@ -93,16 +124,24 @@
                     pattern = marker.args[0]
                     sku = request.getfixturevalue(f"{name}_sku")
                     if re.search(pattern, sku):
                         pytest.skip(f"Skipped on this SKU: {sku}")
 
             if allowed_os:
                 dut_ssh = request.getfixturevalue(f"{name}_ssh")
+                dut_os_version = request.getfixturevalue(f"{name}_os_version")
                 if dut_ssh.cli_flavor not in allowed_os:
-                    pytest.skip(f"cannot run on platform {dut_ssh.cli_flavor}")
+                    pytest.skip(f"Cannot run on platform {dut_ssh.cli_flavor}")
+                if min_version or min_chg_num:
+                    # matches the pattern X.XX.X.XX with digits only
+                    release, change_number = parse_version(dut_os_version)
+                    if min_chg_num:
+                        version_skipper(change_number, min_chg_num)
+                    else:
+                        version_skipper(release, min_version)
 
         return skipper
 
     return _skipper
 
 
 def create_sku_fixture(name):
@@ -114,14 +153,27 @@
         matcher = re.search(r"(DCS-7.*)", output)
         logging.info("Got SKU: %s", matcher.group(1))
         yield matcher.group(1)
 
     return _sku
 
 
+def create_os_version_fixture(name):
+    @pytest.fixture(scope="session", name=f"{name}_os_version")
+    def _os_version(request):
+        ssh = request.getfixturevalue(f"{name}_ssh")
+        assert ssh.cli_flavor in {"eos", "mos"}
+        output = ssh.sendcmd("show version", timeout=300)
+        matcher = re.search(r"Software image version: (\S*)", output)
+        logging.info("Got OS version: %s", matcher.group(1))
+        yield matcher.group(1)
+
+    return _os_version
+
+
 def create_softened_fixture(name):
     @pytest.fixture(scope="session", name=f"{name}_softened")
     def _softened(dut_ssh):
         # Set up a standard operating environment.
         dut_ssh.sendcmds(
             """
             enable
```

### Comparing `pytest_netdut-0.7.0/src/pytest_netdut/px.py` & `pytest_netdut-0.8.0/src/pytest_netdut/px.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/src/pytest_netdut/utils.py` & `pytest_netdut-0.8.0/src/pytest_netdut/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/src/pytest_netdut/wrappers.py` & `pytest_netdut-0.8.0/src/pytest_netdut/wrappers.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/src/pytest_netdut.egg-info/PKG-INFO` & `pytest_netdut-0.8.0/src/pytest_netdut.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-netdut
-Version: 0.7.0
+Version: 0.8.0
 Summary: "Automated software testing for switches using pytest"
 Home-page: https://github.com/aristanetworks/pytest-netdut
 Author: "David Snowdon"
 Author-email: "daves@arista.com"
 Maintainer: "Alex Webster"
 Maintainer-email: "alexw@arista.com"
 License: "BSD 3-Clause License"
@@ -19,28 +19,28 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/markdown
 
 Netdut: automated software testing for switches using pytest
 ============================================================
 
-![PyPi](https://img.shields.io/pypi/v/pytest-netdut.svg) 
+![PyPi](https://img.shields.io/pypi/v/pytest-netdut.svg)
 ![Python Versions](https://img.shields.io/pypi/pyversions/pytest-netdut.svg)
-![collection version](https://img.shields.io/github/v/release/aristanetworks/pytest-netdut) 
+![collection version](https://img.shields.io/github/v/release/aristanetworks/pytest-netdut)
 ![License](https://img.shields.io/github/license/aristanetworks/pytest-netdut)
 
 Netdut is a [pytest](https://docs.pytest.org/) plugin which provides infrastructure (e.g. pytest fixtures) which make it easy to write automated tests for network switches.
 
 
 Features
 --------
 
 * Brings the power, maturity and ecosystem of pytest to testing on network switches.
-* The `dut` fixture (Device Under Test) providing serial, ssh or [EAPI](https://github.com/arista-eosplus/pyeapi) connectivity for running CLI commands on a network switch. 
-* Command-line configuration of a hostname and console name. 
+* The `dut` fixture (Device Under Test) providing serial, ssh or [EAPI](https://github.com/arista-eosplus/pyeapi) connectivity for running CLI commands on a network switch.
+* Command-line configuration of a hostname and console name.
 * Markers for skipping tests based on the device's type or software configuration.
 * Compatibility with both Arista's EOS operating system, and the Metamako MOS operating system.
 * A pythonic interfaces for writing EOS CLI commands.
 
 
 Requirements
 ------------
@@ -174,14 +174,26 @@
 ```python
 @pytest.mark.eos
 @pytest.mark.skip_device_type("DCS-7130.*")
 def test_that_only_runs_on_eos_on_7130(dut):
     logging.info("Must be EOS on 7130!")
 ```
 
+OS decorators accept the following keywords:
+ - min_version (string)
+ - min_change_number (int)
+
+If both kwargs are specified, min_change_number takes precedence.
+```python
+@pytest.mark.eos(min_version="4.30.0", min_change_number=3452345)
+@pytest.mark.skip_device_type("DCS-7130.*")
+def test_that_only_runs_on_eos_on_7130(dut):
+    logging.info("Must be EOS on 7130!")
+```
+
 ### Building test harnesses
 
 Pytest's fixture mechanism is very powerful in this scenario, allowing us to set up and tear
 down test configurations with low overhead.
 
 ```python
 @pytest.fixture
@@ -234,15 +246,15 @@
 
 The translator will also process return values; MOS EAPI result keys are camelCased and the translator will convert all keys
 to snake_case.
 
 The translator has a predefined set of translations which can be extended by subclassing the Translator class and overriding `config_patterns`.
 Return values are processed by the `translate_key` function which must be defined in the subclass.
 
-Set the new translator class via `eapi.set_translator(<class instance>)`. 
+Set the new translator class via `eapi.set_translator(<class instance>)`.
 
 Contributing
 ------------
 This project is under active use and development. We would appreciate help to improve it,
 via pull request. Tests can be run with `make ci` or `tox`.
 
 Docstrings are according to [Google's docstring conventions](https://google.github.io/styleguide/pyguide.html) ([examples](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html)).
```

### Comparing `pytest_netdut-0.7.0/src/pytest_netdut.egg-info/SOURCES.txt` & `pytest_netdut-0.8.0/src/pytest_netdut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/tests/conftest.py` & `pytest_netdut-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/tests/test_netdut.py` & `pytest_netdut-0.8.0/tests/test_netdut.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/tests/test_translator.py` & `pytest_netdut-0.8.0/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/tests/test_wait_for.py` & `pytest_netdut-0.8.0/tests/test_wait_for.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/tests/test_xapi.py` & `pytest_netdut-0.8.0/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.7.0/tox.ini` & `pytest_netdut-0.8.0/tox.ini`

 * *Files identical despite different names*

