# Comparing `tmp/shipyard_snowflake-0.1.1a0.tar.gz` & `tmp/shipyard_snowflake-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_snowflake-0.1.1a0.tar", max compression
+gzip compressed data, was "shipyard_snowflake-0.1.1a1.tar", max compression
```

## Comparing `shipyard_snowflake-0.1.1a0.tar` & `shipyard_snowflake-0.1.1a1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-03 22:01:51.349436 shipyard_snowflake-0.1.1a0/README.md
--rw-r--r--   0        0        0      728 2023-07-05 20:56:55.150272 shipyard_snowflake-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0      172 2023-07-01 18:13:28.547777 shipyard_snowflake-0.1.1a0/shipyard_snowflake/__init__.py
--rw-r--r--   0        0        0      606 2023-05-10 22:55:38.756415 shipyard_snowflake-0.1.1a0/shipyard_snowflake/cli/authtest.py
--rw-r--r--   0        0        0     1653 2023-07-05 18:58:44.925942 shipyard_snowflake-0.1.1a0/shipyard_snowflake/cli/execute_sql.py
--rw-r--r--   0        0        0     3159 2023-07-05 19:07:53.618101 shipyard_snowflake-0.1.1a0/shipyard_snowflake/cli/fetch.py
--rw-r--r--   0        0        0     4914 2023-07-05 14:55:01.424292 shipyard_snowflake-0.1.1a0/shipyard_snowflake/cli/upload.py
--rw-r--r--   0        0        0     5662 2023-07-01 18:14:30.347997 shipyard_snowflake-0.1.1a0/shipyard_snowflake/snowflake.py
--rw-r--r--   0        0        0     1828 2023-07-05 19:30:16.442690 shipyard_snowflake-0.1.1a0/shipyard_snowflake/test/tests.py
--rw-r--r--   0        0        0     5570 2023-07-01 21:20:29.827868 shipyard_snowflake-0.1.1a0/shipyard_snowflake/utils.py
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 shipyard_snowflake-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-03 22:01:51.349436 shipyard_snowflake-0.1.1a1/README.md
+-rw-r--r--   0        0        0      757 2023-07-05 21:41:10.314727 shipyard_snowflake-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-07-01 18:13:28.547777 shipyard_snowflake-0.1.1a1/shipyard_snowflake/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-10 22:55:38.756415 shipyard_snowflake-0.1.1a1/shipyard_snowflake/cli/authtest.py
+-rw-r--r--   0        0        0     1653 2023-07-05 18:58:44.925942 shipyard_snowflake-0.1.1a1/shipyard_snowflake/cli/execute_sql.py
+-rw-r--r--   0        0        0     3159 2023-07-05 19:07:53.618101 shipyard_snowflake-0.1.1a1/shipyard_snowflake/cli/fetch.py
+-rw-r--r--   0        0        0     4914 2023-07-05 14:55:01.424292 shipyard_snowflake-0.1.1a1/shipyard_snowflake/cli/upload.py
+-rw-r--r--   0        0        0     5662 2023-07-01 18:14:30.347997 shipyard_snowflake-0.1.1a1/shipyard_snowflake/snowflake.py
+-rw-r--r--   0        0        0     1828 2023-07-05 19:30:16.442690 shipyard_snowflake-0.1.1a1/shipyard_snowflake/test/tests.py
+-rw-r--r--   0        0        0     5570 2023-07-01 21:20:29.827868 shipyard_snowflake-0.1.1a1/shipyard_snowflake/utils.py
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 shipyard_snowflake-0.1.1a1/PKG-INFO
```

### Comparing `shipyard_snowflake-0.1.1a0/pyproject.toml` & `shipyard_snowflake-0.1.1a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "shipyard-snowflake"
-version = "0.1.1a0"
+version = "0.1.1a1"
 description = "A local client for conecting and working with Snowflake"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_snowflake"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "1.5.3"
 dask = "2022.2.0"
 psutil = "^5.9.5"
 snowflake-connector-python = {version = "^3.0.4", extras = ["pandas"]}
 shipyard-bp-utils = "^0.1.0"
+shipyard-templates = "0.1.6"
 [tool.poetry.group.dev.dependencies]
 shipyard-bp-utils = {path = "../shipyard-bp-utils", develop = true}
 shipyard-templates = {path = "../../shipyard-templates", develop = true}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shipyard_snowflake-0.1.1a0/shipyard_snowflake/cli/authtest.py` & `shipyard_snowflake-0.1.1a1/shipyard_snowflake/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.1.1a0/shipyard_snowflake/cli/execute_sql.py` & `shipyard_snowflake-0.1.1a1/shipyard_snowflake/cli/execute_sql.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.1.1a0/shipyard_snowflake/cli/fetch.py` & `shipyard_snowflake-0.1.1a1/shipyard_snowflake/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.1.1a0/shipyard_snowflake/cli/upload.py` & `shipyard_snowflake-0.1.1a1/shipyard_snowflake/cli/upload.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.1.1a0/shipyard_snowflake/snowflake.py` & `shipyard_snowflake-0.1.1a1/shipyard_snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.1.1a0/shipyard_snowflake/test/tests.py` & `shipyard_snowflake-0.1.1a1/shipyard_snowflake/test/tests.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.1.1a0/shipyard_snowflake/utils.py` & `shipyard_snowflake-0.1.1a1/shipyard_snowflake/utils.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.1.1a0/PKG-INFO` & `shipyard_snowflake-0.1.1a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: shipyard-snowflake
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: A local client for conecting and working with Snowflake
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dask (==2022.2.0)
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: shipyard-bp-utils (>=0.1.0,<0.2.0)
+Requires-Dist: shipyard-templates (==0.1.6)
 Requires-Dist: snowflake-connector-python[pandas] (>=3.0.4,<4.0.0)
 Description-Content-Type: text/markdown
```

