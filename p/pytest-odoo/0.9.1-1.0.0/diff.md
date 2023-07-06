# Comparing `tmp/pytest-odoo-0.9.1.tar.gz` & `tmp/pytest-odoo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-odoo-0.9.1.tar", last modified: Thu Nov 17 07:45:18 2022, max compression
+gzip compressed data, was "pytest-odoo-1.0.0.tar", last modified: Thu Jul  6 16:42:10 2023, max compression
```

## Comparing `pytest-odoo-0.9.1.tar` & `pytest-odoo-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-17 07:45:18.713130 pytest-odoo-0.9.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-11-17 07:45:01.000000 pytest-odoo-0.9.1/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      268 2022-11-17 07:45:01.000000 pytest-odoo-0.9.1/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)    34520 2022-11-17 07:45:01.000000 pytest-odoo-0.9.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2802 2022-11-17 07:45:18.713130 pytest-odoo-0.9.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2078 2022-11-17 07:45:01.000000 pytest-odoo-0.9.1/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-17 07:45:18.713130 pytest-odoo-0.9.1/pytest_odoo.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2802 2022-11-17 07:45:18.000000 pytest-odoo-0.9.1/pytest_odoo.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      311 2022-11-17 07:45:18.000000 pytest-odoo-0.9.1/pytest_odoo.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-11-17 07:45:18.000000 pytest-odoo-0.9.1/pytest_odoo.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       30 2022-11-17 07:45:18.000000 pytest-odoo-0.9.1/pytest_odoo.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-11-17 07:45:18.000000 pytest-odoo-0.9.1/pytest_odoo.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2022-11-17 07:45:18.000000 pytest-odoo-0.9.1/pytest_odoo.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2022-11-17 07:45:18.000000 pytest-odoo-0.9.1/pytest_odoo.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     8390 2022-11-17 07:45:01.000000 pytest-odoo-0.9.1/pytest_odoo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-11-17 07:45:18.713130 pytest-odoo-0.9.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1098 2022-11-17 07:45:01.000000 pytest-odoo-0.9.1/setup.py
+drwxrwxr-x   0 sorsi     (1000) sorsi     (1000)        0 2023-07-06 16:42:10.153491 pytest-odoo-1.0.0/
+-rw-rw-r--   0 sorsi     (1000) sorsi     (1000)       38 2022-10-20 06:45:17.000000 pytest-odoo-1.0.0/.gitignore
+-rw-rw-r--   0 sorsi     (1000) sorsi     (1000)      268 2022-10-20 06:45:17.000000 pytest-odoo-1.0.0/.travis.yml
+-rw-rw-r--   0 sorsi     (1000) sorsi     (1000)    34520 2022-10-20 06:45:17.000000 pytest-odoo-1.0.0/LICENSE
+-rw-rw-r--   0 sorsi     (1000) sorsi     (1000)     2875 2023-07-06 16:42:10.153491 pytest-odoo-1.0.0/PKG-INFO
+-rw-rw-r--   0 sorsi     (1000) sorsi     (1000)     2151 2023-07-03 08:13:52.000000 pytest-odoo-1.0.0/README.rst
+drwxrwxr-x   0 sorsi     (1000) sorsi     (1000)        0 2023-07-06 16:42:10.153491 pytest-odoo-1.0.0/pytest_odoo.egg-info/
+-rw-rw-r--   0 sorsi     (1000) sorsi     (1000)     2875 2023-07-06 16:42:10.000000 pytest-odoo-1.0.0/pytest_odoo.egg-info/PKG-INFO
+-rw-rw-r--   0 sorsi     (1000) sorsi     (1000)      311 2023-07-06 16:42:10.000000 pytest-odoo-1.0.0/pytest_odoo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sorsi     (1000) sorsi     (1000)        1 2023-07-06 16:42:10.000000 pytest-odoo-1.0.0/pytest_odoo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sorsi     (1000) sorsi     (1000)       30 2023-07-06 16:42:10.000000 pytest-odoo-1.0.0/pytest_odoo.egg-info/entry_points.txt
+-rw-rw-r--   0 sorsi     (1000) sorsi     (1000)        1 2022-10-20 06:46:24.000000 pytest-odoo-1.0.0/pytest_odoo.egg-info/not-zip-safe
+-rw-rw-r--   0 sorsi     (1000) sorsi     (1000)       14 2023-07-06 16:42:10.000000 pytest-odoo-1.0.0/pytest_odoo.egg-info/requires.txt
+-rw-rw-r--   0 sorsi     (1000) sorsi     (1000)       12 2023-07-06 16:42:10.000000 pytest-odoo-1.0.0/pytest_odoo.egg-info/top_level.txt
+-rw-rw-r--   0 sorsi     (1000) sorsi     (1000)     8744 2023-07-03 08:13:52.000000 pytest-odoo-1.0.0/pytest_odoo.py
+-rw-rw-r--   0 sorsi     (1000) sorsi     (1000)       38 2023-07-06 16:42:10.153491 pytest-odoo-1.0.0/setup.cfg
+-rw-rw-r--   0 sorsi     (1000) sorsi     (1000)     1098 2022-11-17 07:42:13.000000 pytest-odoo-1.0.0/setup.py
```

### Comparing `pytest-odoo-0.9.1/LICENSE` & `pytest-odoo-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-odoo-0.9.1/PKG-INFO` & `pytest-odoo-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-odoo
-Version: 0.9.1
+Version: 1.0.0
 Summary: py.test plugin to run Odoo tests
 Home-page: https://github.com/camptocamp/pytest-odoo
 Author: Guewen Baconnier
 Author-email: guewen.baconnier@camptocamp.com
 License: AGPLv3
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -44,20 +44,22 @@
 
 install via::
 
     pip install pytest-odoo
 
 usage::
 
-   pytest -s --odoo-database=test --odoo-log-level=debug_sql
+   pytest -s --odoo-database=test --odoo-log-level=debug_sql [--odoo-http]
 
 The custom options are:
 
 * ``--odoo-database``: name of the database to test.
 * ``--odoo-log-level``: log level as expected by odoo. As time of writing: info, debug_rpc, warn, test, critical, debug_sql, error, debug, debug_rpc_answer. The default is critical to have a clean output.
 * ``--odoo-config``: path of the odoo.cfg file to use.
+* ``--odoo-http``: Allow to launch the Odoo http instance
+
 
 Alternatively, you can use the ``OPENERP_SERVER`` environment variable using an odoo configuration file, containing at least the ``database`` option with the name of the database to test::
 
    export OPENERP_SERVER=/path/to/odoo/config.cfg
    pytest ...
```

### Comparing `pytest-odoo-0.9.1/README.rst` & `pytest-odoo-1.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -23,20 +23,22 @@
 
 install via::
 
     pip install pytest-odoo
 
 usage::
 
-   pytest -s --odoo-database=test --odoo-log-level=debug_sql
+   pytest -s --odoo-database=test --odoo-log-level=debug_sql [--odoo-http]
 
 The custom options are:
 
 * ``--odoo-database``: name of the database to test.
 * ``--odoo-log-level``: log level as expected by odoo. As time of writing: info, debug_rpc, warn, test, critical, debug_sql, error, debug, debug_rpc_answer. The default is critical to have a clean output.
 * ``--odoo-config``: path of the odoo.cfg file to use.
+* ``--odoo-http``: Allow to launch the Odoo http instance
+
 
 Alternatively, you can use the ``OPENERP_SERVER`` environment variable using an odoo configuration file, containing at least the ``database`` option with the name of the database to test::
 
    export OPENERP_SERVER=/path/to/odoo/config.cfg
    pytest ...
```

### Comparing `pytest-odoo-0.9.1/pytest_odoo.egg-info/PKG-INFO` & `pytest-odoo-1.0.0/pytest_odoo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-odoo
-Version: 0.9.1
+Version: 1.0.0
 Summary: py.test plugin to run Odoo tests
 Home-page: https://github.com/camptocamp/pytest-odoo
 Author: Guewen Baconnier
 Author-email: guewen.baconnier@camptocamp.com
 License: AGPLv3
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -44,20 +44,22 @@
 
 install via::
 
     pip install pytest-odoo
 
 usage::
 
-   pytest -s --odoo-database=test --odoo-log-level=debug_sql
+   pytest -s --odoo-database=test --odoo-log-level=debug_sql [--odoo-http]
 
 The custom options are:
 
 * ``--odoo-database``: name of the database to test.
 * ``--odoo-log-level``: log level as expected by odoo. As time of writing: info, debug_rpc, warn, test, critical, debug_sql, error, debug, debug_rpc_answer. The default is critical to have a clean output.
 * ``--odoo-config``: path of the odoo.cfg file to use.
+* ``--odoo-http``: Allow to launch the Odoo http instance
+
 
 Alternatively, you can use the ``OPENERP_SERVER`` environment variable using an odoo configuration file, containing at least the ``database`` option with the name of the database to test::
 
    export OPENERP_SERVER=/path/to/odoo/config.cfg
    pytest ...
```

### Comparing `pytest-odoo-0.9.1/pytest_odoo.py` & `pytest-odoo-1.0.0/pytest_odoo.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,37 +9,36 @@
 import signal
 import sys
 import threading
 from pathlib import Path
 from typing import Optional
 
 import _pytest
-import _pytest.python
-import pytest
-
-from _pytest._code.code import ExceptionInfo
 import _pytest._py.error as error
-
-from pathlib import Path
-
+import _pytest.python
 import odoo
 import odoo.tests
+import pytest
+from _pytest._code.code import ExceptionInfo
 
 
 def pytest_addoption(parser):
     parser.addoption("--odoo-database",
                      action="store",
                      help="Name of the Odoo database to test")
     parser.addoption("--odoo-config",
                      action="store",
                      help="Path of the Odoo configuration file")
     parser.addoption("--odoo-log-level",
                      action="store",
                      default='critical',
                      help="Log-level used by the Odoo process during tests")
+    parser.addoption("--odoo-http",
+                     action="store_true",
+                     help="If pytest should launch an Odoo http server.")
 
 
 @pytest.hookimpl(hookwrapper=True)
 def pytest_cmdline_main(config):
 
     if (config.getoption('--odoo-database')
             or config.getoption('--odoo-config')
@@ -75,14 +74,21 @@
                 yield
         else:
             yield
     else:
         yield
 
 
+@pytest.fixture(scope="module", autouse=True)
+def load_http(request):
+    if request.config.getoption("--odoo-http"):
+        odoo.service.server.start(stop=True)
+        signal.signal(signal.SIGINT, signal.default_int_handler)
+
+
 @pytest.fixture(scope='session', autouse=True)
 def load_registry():
     # Initialize the registry before running tests.
     # If we don't do that, the modules will be loaded *inside* of the first
     # test we run, which would trigger the launch of the postinstall tests
     # (because we force 'test_enable' to True and the at end of the loading of
     # the registry, the postinstall tests are run when test_enable is enabled).
```

### Comparing `pytest-odoo-0.9.1/setup.py` & `pytest-odoo-1.0.0/setup.py`

 * *Files identical despite different names*

