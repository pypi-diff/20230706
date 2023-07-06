# Comparing `tmp/lacuscore-1.6.0.tar.gz` & `tmp/lacuscore-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.6.0.tar", max compression
+gzip compressed data, was "lacuscore-1.6.1.tar", max compression
```

## Comparing `lacuscore-1.6.0.tar` & `lacuscore-1.6.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.6.0/LICENSE
--rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.6.0/README.md
--rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.6.0/lacuscore/__init__.py
--rw-r--r--   0        0        0     2138 2023-06-27 10:03:30.510884 lacuscore-1.6.0/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    33491 2023-06-27 10:02:06.046544 lacuscore-1.6.0/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.6.0/lacuscore/py.typed
--rw-r--r--   0        0        0     1596 2023-06-30 14:22:29.631600 lacuscore-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.6.1/LICENSE
+-rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.6.1/README.md
+-rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.6.1/lacuscore/__init__.py
+-rw-r--r--   0        0        0     2138 2023-06-27 10:03:30.510884 lacuscore-1.6.1/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    33491 2023-06-27 10:02:06.046544 lacuscore-1.6.1/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.6.1/lacuscore/py.typed
+-rw-r--r--   0        0        0     1596 2023-07-06 13:24:21.207741 lacuscore-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.6.1/PKG-INFO
```

### Comparing `lacuscore-1.6.0/LICENSE` & `lacuscore-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.6.0/README.md` & `lacuscore-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.6.0/lacuscore/lacus_monitoring.py` & `lacuscore-1.6.1/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.6.0/lacuscore/lacuscore.py` & `lacuscore-1.6.1/lacuscore/lacuscore.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.6.0/pyproject.toml` & `lacuscore-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.6.0"
+version = "1.6.1"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -28,24 +28,24 @@
 
 include = ['README.md']
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
 Sphinx = { version = "^7.0.1", optional = true }
-playwrightcapture = {extras = ["recaptcha"], version = "^1.21.0"}
+playwrightcapture = {extras = ["recaptcha"], version = "^1.21.1"}
 defang = "^0.5.3"
 ua-parser = "^0.16.1"
 redis = {version = "^4.6.0", extras = ["hiredis"]}
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [tool.poetry.group.dev.dependencies]
-types-redis = {version = "^4.6.0.0"}
+types-redis = {version = "^4.6.0.2"}
 mypy = "^1.4.1"
 types-requests = "^2.31.0.1"
 ipython = [
     {version = "<8.13.0", python = "<3.9"},
     {version = "^8.13.0", python = ">=3.9"}
 ]
 pytest = "^7.4.0"
```

### Comparing `lacuscore-1.6.0/PKG-INFO` & `lacuscore-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.6.0
+Version: 1.6.1
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=7.0.1,<8.0.0) ; extra == "docs"
 Requires-Dist: defang (>=0.5.3,<0.6.0)
-Requires-Dist: playwrightcapture[recaptcha] (>=1.21.0,<2.0.0)
+Requires-Dist: playwrightcapture[recaptcha] (>=1.21.1,<2.0.0)
 Requires-Dist: redis[hiredis] (>=4.6.0,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ua-parser (>=0.16.1,<0.17.0)
 Project-URL: Documentation, https://lacuscore.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/ail-project/LacusCore
 Description-Content-Type: text/markdown
```

