# Comparing `tmp/dbt-teradata-1.3.3.1.tar.gz` & `tmp/dbt-teradata-1.4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-teradata-1.3.3.1.tar", last modified: Thu Jun  8 09:09:24 2023, max compression
+gzip compressed data, was "dbt-teradata-1.4.0.0.tar", last modified: Thu Jul  6 07:17:36 2023, max compression
```

## Comparing `dbt-teradata-1.3.3.1.tar` & `dbt-teradata-1.4.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20980 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.792976 dbt-teradata-1.3.3.1/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.792976 dbt-teradata-1.3.3.1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/dbt/adapters/teradata/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/adapters/teradata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 09:09:21.000000 dbt-teradata-1.3.3.1/dbt/adapters/teradata/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/adapters/teradata/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/adapters/teradata/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/adapters/teradata/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/adapters/teradata/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.792976 dbt-teradata-1.3.3.1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/dbt/include/teradata/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/columns.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.792976 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/incremental/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/seed/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/seed/seed.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/snapshot/
--rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/test/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/test/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/dbt_teradata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-06-08 09:09:24.000000 dbt-teradata-1.3.3.1/dbt_teradata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-08 09:09:24.000000 dbt-teradata-1.3.3.1/dbt_teradata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:09:24.000000 dbt-teradata-1.3.3.1/dbt_teradata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 09:09:24.000000 dbt-teradata-1.3.3.1/dbt_teradata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 09:09:24.000000 dbt-teradata-1.3.3.1/dbt_teradata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-08 09:09:21.000000 dbt-teradata-1.3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.450156 dbt-teradata-1.4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21751 2023-07-06 07:17:36.450156 dbt-teradata-1.4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21442 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.442156 dbt-teradata-1.4.0.0/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.442156 dbt-teradata-1.4.0.0/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.446156 dbt-teradata-1.4.0.0/dbt/adapters/teradata/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/adapters/teradata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 07:17:33.000000 dbt-teradata-1.4.0.0/dbt/adapters/teradata/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/adapters/teradata/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/adapters/teradata/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/adapters/teradata/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/adapters/teradata/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.442156 dbt-teradata-1.4.0.0/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.446156 dbt-teradata-1.4.0.0/dbt/include/teradata/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.446156 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/columns.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.442156 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.446156 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/incremental/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.450156 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/seed/
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/seed/seed.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.450156 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.450156 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/test/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.450156 dbt-teradata-1.4.0.0/dbt_teradata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21751 2023-07-06 07:17:36.000000 dbt-teradata-1.4.0.0/dbt_teradata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-06 07:17:36.000000 dbt-teradata-1.4.0.0/dbt_teradata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:17:36.000000 dbt-teradata-1.4.0.0/dbt_teradata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 07:17:36.000000 dbt-teradata-1.4.0.0/dbt_teradata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 07:17:36.000000 dbt-teradata-1.4.0.0/dbt_teradata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 07:17:36.450156 dbt-teradata-1.4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-06 07:17:33.000000 dbt-teradata-1.4.0.0/setup.py
```

### Comparing `dbt-teradata-1.3.3.1/LICENSE` & `dbt-teradata-1.4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.1/PKG-INFO` & `dbt-teradata-1.4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-teradata
-Version: 1.3.3.1
+Version: 1.4.0.0
 Summary: The Teradata adapter plugin for dbt (data build tool)
 Home-page: https://github.com/Teradata/dbt-teradata
 Author: Teradata Corporation
 Author-email: developers@teradata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,15 +12,16 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dbt-teradata
 
 This plugin ports [dbt](https://getdbt.com) functionality to Teradata Vantage.
 
@@ -28,14 +29,20 @@
 
 ```
 pip install dbt-teradata
 ```
 
 If you are new to dbt on Teradata see [dbt with Teradata Vantage tutorial](https://quickstarts.teradata.com/dbt.html).
 
+**_NOTE:_** If the virtual environment in Python is not activating properly on Windows, you can try running the below command in the command-line interface (CLI) before attempting to activate the virtual environment.
+
+```
+Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUse
+```
+
 ## Sample profile
 
 Here is a working example of a `dbt-teradata` profile:
 
 ```yaml
 my-teradata-db-profile:
   target: dev
@@ -49,23 +56,24 @@
       tmode: ANSI
 ```
 
 At a minimum, you need to specify `host`, `user`, `password`, `schema` (database), `tmode`.
 
 ## Python compatibility
 
-| Plugin version | Python 3.6  | Python 3.7  | Python 3.8  | Python 3.9  | Python 3.10 |
-| -------------- | ----------- | ----------- | ----------- | ----------- | ----------- |
-| 0.19.0.x           | ✅          | ✅          | ✅          | ❌          | ❌          |
-| 0.20.0.x           | ✅          | ✅          | ✅          | ✅          | ❌          |
-| 0.21.1.x           | ✅          | ✅          | ✅          | ✅          | ❌          |
-| 1.0.0.x           | ❌           | ✅          | ✅          | ✅          | ❌          |
-|1.1.0.x            | ❌           | ✅          | ✅          | ✅          | ✅          |
-|1.2.0.x            | ❌           | ✅          | ✅          | ✅          | ✅          |
-|1.3.0.x            | ❌           | ✅          | ✅          | ✅          | ✅          |
+| Plugin version | Python 3.6  | Python 3.7  | Python 3.8  | Python 3.9  | Python 3.10 | Python 3.11  |
+| -------------- | ----------- | ----------- | ----------- | ----------- | ----------- | ------------ |
+| 0.19.0.x           | ✅          | ✅          | ✅          | ❌          | ❌          | ❌
+| 0.20.0.x           | ✅          | ✅          | ✅          | ✅          | ❌          | ❌
+| 0.21.1.x           | ✅          | ✅          | ✅          | ✅          | ❌          | ❌
+| 1.0.0.x           | ❌           | ✅          | ✅          | ✅          | ❌          | ❌
+|1.1.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
+|1.2.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
+|1.3.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
+|1.4.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ✅
 
 
 ##  dbt dependent packages version compatibility
 | dbt-teradta |  dbt-core  | dbt-teradata-util |  dbt-util      |
 |-------------|------------|-------------------|----------------|
 | 1.2.x       | 1.2.x      | 0.1.0             | 0.9.x or below |
```

### Comparing `dbt-teradata-1.3.3.1/README.md` & `dbt-teradata-1.4.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 ```
 pip install dbt-teradata
 ```
 
 If you are new to dbt on Teradata see [dbt with Teradata Vantage tutorial](https://quickstarts.teradata.com/dbt.html).
 
+**_NOTE:_** If the virtual environment in Python is not activating properly on Windows, you can try running the below command in the command-line interface (CLI) before attempting to activate the virtual environment.
+
+```
+Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUse
+```
+
 ## Sample profile
 
 Here is a working example of a `dbt-teradata` profile:
 
 ```yaml
 my-teradata-db-profile:
   target: dev
@@ -27,23 +33,24 @@
       tmode: ANSI
 ```
 
 At a minimum, you need to specify `host`, `user`, `password`, `schema` (database), `tmode`.
 
 ## Python compatibility
 
-| Plugin version | Python 3.6  | Python 3.7  | Python 3.8  | Python 3.9  | Python 3.10 |
-| -------------- | ----------- | ----------- | ----------- | ----------- | ----------- |
-| 0.19.0.x           | ✅          | ✅          | ✅          | ❌          | ❌          |
-| 0.20.0.x           | ✅          | ✅          | ✅          | ✅          | ❌          |
-| 0.21.1.x           | ✅          | ✅          | ✅          | ✅          | ❌          |
-| 1.0.0.x           | ❌           | ✅          | ✅          | ✅          | ❌          |
-|1.1.0.x            | ❌           | ✅          | ✅          | ✅          | ✅          |
-|1.2.0.x            | ❌           | ✅          | ✅          | ✅          | ✅          |
-|1.3.0.x            | ❌           | ✅          | ✅          | ✅          | ✅          |
+| Plugin version | Python 3.6  | Python 3.7  | Python 3.8  | Python 3.9  | Python 3.10 | Python 3.11  |
+| -------------- | ----------- | ----------- | ----------- | ----------- | ----------- | ------------ |
+| 0.19.0.x           | ✅          | ✅          | ✅          | ❌          | ❌          | ❌
+| 0.20.0.x           | ✅          | ✅          | ✅          | ✅          | ❌          | ❌
+| 0.21.1.x           | ✅          | ✅          | ✅          | ✅          | ❌          | ❌
+| 1.0.0.x           | ❌           | ✅          | ✅          | ✅          | ❌          | ❌
+|1.1.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
+|1.2.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
+|1.3.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
+|1.4.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ✅
 
 
 ##  dbt dependent packages version compatibility
 | dbt-teradta |  dbt-core  | dbt-teradata-util |  dbt-util      |
 |-------------|------------|-------------------|----------------|
 | 1.2.x       | 1.2.x      | 0.1.0             | 0.9.x or below |
```

### Comparing `dbt-teradata-1.3.3.1/dbt/adapters/teradata/__init__.py` & `dbt-teradata-1.4.0.0/dbt/adapters/teradata/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.1/dbt/adapters/teradata/column.py` & `dbt-teradata-1.4.0.0/dbt/adapters/teradata/column.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.1/dbt/adapters/teradata/connections.py` & `dbt-teradata-1.4.0.0/dbt/adapters/teradata/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,24 +55,24 @@
 
     def __post_init__(self):
         # teradata classifies database and schema as the same thing
         if (
             self.database is not None and
             self.database != self.schema
         ):
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 f"    schema: {self.schema} \n"
                 f"    database: {self.database} \n"
                 f"On Teradata, database must be omitted or have the same value as"
                 f" schema."
             )
 
         # Only allow the ANSI transaction mode
         if self.tmode != "ANSI":
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 f"This version only allows a tmode of ANSI."
             )
 
     @property
     def type(self):
         return "teradata"
 
@@ -204,15 +204,15 @@
             logger.debug("Got an error when attempting to open a teradata "
                          "connection: '{}'"
                          .format(e))
 
             connection.handle = None
             connection.state = 'fail'
 
-            raise dbt.exceptions.FailedToConnectException(str(e))
+            raise dbt.exceptions.FailedToConnectError(str(e))
 
         return connection
 
     @classmethod
     def get_credentials(cls, credentials):
         return credentials
 
@@ -229,27 +229,27 @@
 
             try:
                 self.rollback_if_open()
             except teradatasql.Error:
                 logger.debug("Failed to release connection!")
                 pass
 
-            raise dbt.exceptions.DatabaseException(str(e).strip()) from e
+            raise dbt.exceptions.DbtDatabaseError(str(e).strip()) from e
 
         except Exception as e:
             logger.debug("Error running SQL: {}", sql)
             logger.debug("Rolling back transaction.")
             self.rollback_if_open()
-            if isinstance(e, dbt.exceptions.RuntimeException):
+            if isinstance(e, dbt.exceptions.DbtRuntimeError):
                 # during a sql query, an internal to dbt exception was raised.
                 # this sounds a lot like a signal handler and probably has
                 # useful information, so raise it without modification.
                 raise
 
-            raise dbt.exceptions.RuntimeException(e) from e
+            raise dbt.exceptions.DbtRuntimeError(e) from e
 
     @classmethod
     def get_response(cls, cursor):
         # There's no real way to get this from teradatasql, so just return "OK"
         num_rows = 0
         if cursor is not None and cursor.rowcount is not None:
           num_rows = cursor.rowcount
```

### Comparing `dbt-teradata-1.3.3.1/dbt/adapters/teradata/impl.py` & `dbt-teradata-1.4.0.0/dbt/adapters/teradata/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,44 +102,44 @@
     ) -> List[TeradataRelation]:
         kwargs = {'schema_relation': schema_relation}
         try:
             results = self.execute_macro(
                 LIST_RELATIONS_MACRO_NAME,
                 kwargs=kwargs
             )
-        except dbt.exceptions.RuntimeException as e:
+        except dbt.exceptions.DbtRuntimeError as e:
             errmsg = getattr(e, 'msg', '')
             if f"Teradata database '{schema_relation}' not found" in errmsg:
                 return []
             else:
                 description = "Error while retrieving information about"
                 logger.debug(f"{description} {schema_relation}: {e.msg}")
                 return []
 
         relations = []
         for row in results:
             if len(row) != 4:
-                raise dbt.exceptions.RuntimeException(
+                raise dbt.exceptions.DbtRuntimeError(
                     f'Invalid value from "teradata__list_relations_without_caching({kwargs})", '
                     f'got {len(row)} values, expected 4'
                 )
             _, name, _schema, relation_type = row
-            relation = self.Relation.create(
+            relation: BaseRelation = self.Relation.create(
                 schema=_schema,
                 identifier=name,
                 type=relation_type
             )
             relations.append(relation)
 
         return relations
 
     def get_relation(
         self, database: str, schema: str, identifier: str
     ) -> Optional[BaseRelation]:
-        if not self.Relation.include_policy.database:
+        if not self.Relation.get_default_include_policy().database:
             database = None
 
         return super().get_relation(database, schema, identifier)
 
     def get_catalog(self, manifest):
         schema_map = self._get_catalog_schemas(manifest)
         with executor(self.config) as tpe:
@@ -156,15 +156,15 @@
     def _get_one_catalog(
         self,
         information_schema: InformationSchema,
         schemas: Set[str],
         manifest: Manifest,
     ) -> agate.Table:
         if len(schemas) != 1:
-            dbt.exceptions.raise_compiler_error(
+            dbt.exceptions.CompilationError(
                 f'Expected only one schema in _get_one_catalog() for Teradata adapter, found '
                 f'{schemas}'
             )
 
         return super()._get_one_catalog(information_schema, schemas, manifest)
 
     @classmethod
@@ -211,15 +211,15 @@
         self, add_to: str, value: str, location='append',
     ) -> str:
         if location == 'append':
             return f"concat(cast(trim({add_to}) as varchar(63800)), '{value}')"
         elif location == 'prepend':
             return f"concat('{value}', cast(trim({add_to}) as varchar(63800))"
         else:
-            raise RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 f'Got an unexpected location value of "{location}"'
             )
 
     def get_rows_different_sql(
         self,
         relation_a: TeradataRelation,
         relation_b: TeradataRelation,
```

### Comparing `dbt-teradata-1.3.3.1/dbt/adapters/teradata/relation.py` & `dbt-teradata-1.4.0.0/dbt/adapters/teradata/relation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 from dbt.adapters.base.relation import BaseRelation, Policy
-from dbt.exceptions import RuntimeException
+from dbt.exceptions import DbtRuntimeError
 
 @dataclass
 class TeradataQuotePolicy(Policy):
     database: bool = False
     schema: bool = True
     identifier: bool = True
 
@@ -15,18 +15,18 @@
     database: bool = False
     schema: bool = True
     identifier: bool = True
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class TeradataRelation(BaseRelation):
-    quote_policy: TeradataQuotePolicy = TeradataQuotePolicy()
-    include_policy: TeradataIncludePolicy = TeradataIncludePolicy()
+    quote_policy: Policy = field(default_factory=lambda: TeradataQuotePolicy())
+    include_policy: Policy = field(default_factory=lambda: TeradataIncludePolicy())
     quote_character: str = '"'
 
     def render(self):
         if self.include_policy.database and self.include_policy.schema:
-            raise RuntimeException(
+            raise DbtRuntimeError(
                 f"Got a teradata relation with schema and database set to "
                 "include, but only one can be set"
             )
         return super().render()
```

### Comparing `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/adapters.sql` & `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/adapters.sql`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,14 @@
 
   {{ sql_header if sql_header is not none }}
   REPLACE VIEW {{ relation.include(database=False) }} AS
     {{ sql }}
 
 {% endmacro %}
 
-{% macro teradata__current_timestamp() -%}
-CURRENT_TIMESTAMP(6)
-{%- endmacro %}
 
 {% macro teradata__rename_relation(from_relation, to_relation) -%}
   {#
     Teradata rename fails when the relation already exists, so a 2-step process is needed:
     1. Drop the existing relation
     2. Rename the new relation to the existing relation
   #}
```

### Comparing `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/apply_grants.sql` & `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/catalog.sql` & `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/columns.sql` & `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/incremental/helpers.sql` & `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/incremental/helpers.sql`

 * *Files 18% similar despite different names*

```diff
@@ -6,25 +6,25 @@
   {% endif %}
 
   {% set invalid_strategy_msg -%}
     Invalid incremental strategy provided: {{ strategy }}
     Expected one of:  'append','delete+insert','merge'
   {%- endset %}
   {%- if strategy not in ['append','delete+insert','merge'] %}
-    {% do exceptions.raise_compiler_error(invalid_strategy_msg) %}
+    {% do exceptions.CompilationError(invalid_strategy_msg) %}
   {%- endif %}
 
   {% do return(strategy) %}
 {%- endmacro %}
 
 
 {% macro teradata__get_incremental_sql(strategy, target_relation, tmp_relation, unique_key, dest_columns,incremental_predicates) %}
   {% if strategy == 'delete+insert' %}
-    {% do return(teradata__get_delete_insert_merge_sql(target_relation, tmp_relation, unique_key, dest_columns)) %}
+    {% do return(teradata__get_delete_insert_merge_sql(target_relation, tmp_relation, unique_key, dest_columns, incremental_predicates)) %}
   {% elif strategy == 'append' %}
     {% do return(teradata__get_incremental_append_sql(target_relation, tmp_relation,  dest_columns)) %}
   {% elif strategy == 'merge' %}
     {% do return(teradata__get_merge_sql(target_relation, tmp_relation, unique_key, dest_columns,incremental_predicates)) %}
   {% else %}
-    {% do exceptions.raise_compiler_error("Invalid Strategy") %}
+    {% do exceptions.CompilationError("Invalid Strategy") %}
   {% endif %}
 {% endmacro %}
```

### Comparing `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/incremental/incremental.sql` & `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/incremental/incremental.sql`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 {% set target_relation = this.incorporate(type='table') %}
 {% set existing_relation = load_relation(this) %}
 {% set tmp_relation = make_temp_relation(this) %}
 
 -- {#-- Validate early so we don't run SQL if the strategy is invalid --#}
 {% set strategy = teradata__validate_get_incremental_strategy(config) %}
 
-{% set incremental_predicates = config.get('incremental_predicates', none) %}
+{% set incremental_predicates = config.get('predicates', none) or config.get('incremental_predicates', none) %}
 
 {% set on_schema_change = incremental_validate_on_schema_change(config.get('on_schema_change'), default='ignore') %}
 
 {%- set preexisting_tmp_relation = load_cached_relation(tmp_relation) -%}
 {{ drop_relation_if_exists(preexisting_tmp_relation) }}
 
 {{ run_hooks(pre_hooks, inside_transaction=False) }}
```

### Comparing `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/incremental/strategies.sql` & `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/incremental/strategies.sql`

 * *Files 14% similar despite different names*

```diff
@@ -20,24 +20,46 @@
     insert into {{ target_relation }} ({{ dest_cols_csv }})
         select {{ dest_cols_csv }}
         from {{ tmp_relation }}
     
 {% endmacro %}
 
 
-{% macro teradata__get_delete_insert_merge_sql(target_relation, tmp_relation, unique_key, dest_columns) %}
+{% macro teradata__get_delete_insert_merge_sql(target_relation, tmp_relation, unique_key, dest_columns, incremental_predicates) %}
     {%- set dest_cols_csv = dest_columns | map(attribute='quoted') | join(', ') -%}
 
-    {%- if unique_key is not none -%}
-    DELETE
-    FROM {{ target_relation }}
-    WHERE ({{ unique_key }}) IN (
-        SELECT ({{ unique_key }})
-        FROM {{ tmp_relation }}
-    );
+    {%- if unique_key -%}
+        {% if unique_key is sequence and unique_key is not string %}
+            delete from {{target_relation }}
+            where (
+                {% for key in unique_key %}
+                    {{ tmp_relation }}.{{ key }} = {{ target_relation }}.{{ key }}
+                    {{ "and " if not loop.last}}
+                {% endfor %}
+                {% if incremental_predicates %}
+                    {% for predicate in incremental_predicates %}
+                        and {{ predicate }}
+                    {% endfor %}
+                {% endif %}
+            );
+        {% else %}    
+            DELETE
+            FROM {{ target_relation }}
+            WHERE ({{ unique_key }}) IN (
+                SELECT ({{ unique_key }})
+                FROM {{ tmp_relation }}
+            )
+            {%- if incremental_predicates %}
+                {% for predicate in incremental_predicates %}
+                    and {{ predicate }}
+                {% endfor %}
+            {%- endif -%};
+
+        {% endif %}
+        
     {%- endif %}
 
     INSERT INTO {{ target_relation }} ({{ dest_cols_csv }})
        SELECT {{ dest_cols_csv }}
        FROM {{ tmp_relation }}
     ;
 {%- endmacro %}
@@ -64,15 +86,15 @@
                 DBT_INTERNAL_SOURCE.{{ unique_key }} = DBT_INTERNAL_DEST.{{ unique_key }}
             {% endset %}
             {% do predicates.append(unique_key_match) %}
         {% endif %}
     {% else %}
         {% set error_msg= "Unique key is required for merge incremental strategy, please provide unique key in configuration and try again
         or consider using Append strategy" %}
-        {% do exceptions.raise_compiler_error(error_msg) %}
+        {% do exceptions.CompilationError(error_msg) %}
     {% endif %}
 
     {{ sql_header if sql_header is not none }}
 
     merge into {{ target }} as DBT_INTERNAL_DEST
         using {{ source }} as DBT_INTERNAL_SOURCE
         on {{ predicates | join(' and ') }}
```

### Comparing `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/seed/seed.sql` & `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/seed/seed.sql`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
   -- `BEGIN TRANSACTION` happens here (for tmode=TERA):
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
   -- build model
   {% set create_table_sql = "" %}
   {% if exists_as_view %}
-    {{ exceptions.raise_compiler_error("Cannot seed to '{}', it is a view".format(old_relation)) }}
+    {{ exceptions.CompilationError("Cannot seed to '{}', it is a view".format(old_relation)) }}
   {% elif exists_as_table %}
     {% set create_table_sql = reset_csv_table(model, full_refresh_mode, old_relation, agate_table) %}
   {% else %}
     {% set create_table_sql = create_csv_table(model, agate_table) %}
   {% endif %}
 
   {% set code = 'CREATE' if full_refresh_mode else 'INSERT' %}
```

### Comparing `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql` & `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-
-{% macro teradata__snapshot_string_as_time(timestamp) -%}
-    {%- set timestamp_string = timestamp.strftime('%Y-%m-%d %H:%M:%S.%f%z') -%}
-    {%- set result = "TO_TIMESTAMP_TZ('" ~ "{0}:{1}".format(timestamp_string[:-2], timestamp_string[-2:]) ~ "')" -%}
-    {{ return(result) }}
-{%- endmacro %}
-
 {% macro snapshot_staging_table(strategy, source_sql, target_relation) -%}
 
     WITH snapshot_query AS (
 
         {{ source_sql }}
 
     ),
@@ -251,26 +244,26 @@
     {% set select_current_time -%}
         SELECT {{ snapshot_get_time() }} AS snapshot_start
     {%- endset %}
 
     {#-- don't access the column by name, to avoid dealing with casing issues on snowflake #}
     {%- set now = run_query(select_current_time)[0][0] -%}
     {% if now is none or now is undefined -%}
-        {%- do exceptions.raise_compiler_error('Could not get a snapshot start time from the database') -%}
+        {%- do exceptions.CompilationError('Could not get a snapshot start time from the database') -%}
     {%- endif %}
     {% set updated_at = snapshot_string_as_time(now) %}
 
     {% set column_added = false %}
 
     {% if check_cols_config == 'all' %}
         {% set column_added, check_cols = snapshot_check_all_get_existing_columns(node, target_exists) %}
     {% elif check_cols_config is iterable and (check_cols_config | length) > 0 %}
         {% set check_cols = check_cols_config %}
     {% else %}
-        {% do exceptions.raise_compiler_error("Invalid value for 'check_cols': " ~ check_cols_config) %}
+        {% do exceptions.CompilationError("Invalid value for 'check_cols': " ~ check_cols_config) %}
     {% endif %}
 
     {%- set row_changed_expr -%}
     (
     {%- if column_added -%}
         TRUE
     {%- else -%}
```

### Comparing `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/test/test.sql` & `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/test/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.1/dbt_teradata.egg-info/PKG-INFO` & `dbt-teradata-1.4.0.0/dbt_teradata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-teradata
-Version: 1.3.3.1
+Version: 1.4.0.0
 Summary: The Teradata adapter plugin for dbt (data build tool)
 Home-page: https://github.com/Teradata/dbt-teradata
 Author: Teradata Corporation
 Author-email: developers@teradata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,15 +12,16 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dbt-teradata
 
 This plugin ports [dbt](https://getdbt.com) functionality to Teradata Vantage.
 
@@ -28,14 +29,20 @@
 
 ```
 pip install dbt-teradata
 ```
 
 If you are new to dbt on Teradata see [dbt with Teradata Vantage tutorial](https://quickstarts.teradata.com/dbt.html).
 
+**_NOTE:_** If the virtual environment in Python is not activating properly on Windows, you can try running the below command in the command-line interface (CLI) before attempting to activate the virtual environment.
+
+```
+Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUse
+```
+
 ## Sample profile
 
 Here is a working example of a `dbt-teradata` profile:
 
 ```yaml
 my-teradata-db-profile:
   target: dev
@@ -49,23 +56,24 @@
       tmode: ANSI
 ```
 
 At a minimum, you need to specify `host`, `user`, `password`, `schema` (database), `tmode`.
 
 ## Python compatibility
 
-| Plugin version | Python 3.6  | Python 3.7  | Python 3.8  | Python 3.9  | Python 3.10 |
-| -------------- | ----------- | ----------- | ----------- | ----------- | ----------- |
-| 0.19.0.x           | ✅          | ✅          | ✅          | ❌          | ❌          |
-| 0.20.0.x           | ✅          | ✅          | ✅          | ✅          | ❌          |
-| 0.21.1.x           | ✅          | ✅          | ✅          | ✅          | ❌          |
-| 1.0.0.x           | ❌           | ✅          | ✅          | ✅          | ❌          |
-|1.1.0.x            | ❌           | ✅          | ✅          | ✅          | ✅          |
-|1.2.0.x            | ❌           | ✅          | ✅          | ✅          | ✅          |
-|1.3.0.x            | ❌           | ✅          | ✅          | ✅          | ✅          |
+| Plugin version | Python 3.6  | Python 3.7  | Python 3.8  | Python 3.9  | Python 3.10 | Python 3.11  |
+| -------------- | ----------- | ----------- | ----------- | ----------- | ----------- | ------------ |
+| 0.19.0.x           | ✅          | ✅          | ✅          | ❌          | ❌          | ❌
+| 0.20.0.x           | ✅          | ✅          | ✅          | ✅          | ❌          | ❌
+| 0.21.1.x           | ✅          | ✅          | ✅          | ✅          | ❌          | ❌
+| 1.0.0.x           | ❌           | ✅          | ✅          | ✅          | ❌          | ❌
+|1.1.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
+|1.2.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
+|1.3.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
+|1.4.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ✅
 
 
 ##  dbt dependent packages version compatibility
 | dbt-teradta |  dbt-core  | dbt-teradata-util |  dbt-util      |
 |-------------|------------|-------------------|----------------|
 | 1.2.x       | 1.2.x      | 0.1.0             | 0.9.x or below |
```

### Comparing `dbt-teradata-1.3.3.1/dbt_teradata.egg-info/SOURCES.txt` & `dbt-teradata-1.4.0.0/dbt_teradata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.1/setup.py` & `dbt-teradata-1.4.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
 import os
 import sys
 
 from setuptools import setup
 
 
-if sys.version_info < (3, 7) or sys.version_info >= (3, 11):
+if sys.version_info < (3, 7) or sys.version_info >= (3, 12):
     print('Error: dbt-teradata does not support this version of Python.')
-    print('Please install Python 3.7 or higher but less than 3.11.')
+    print('Please install Python 3.7 or higher but less than 3.12.')
     sys.exit(1)
 
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 package_name = "dbt-teradata"
-package_version = "1.3.3.1"
+package_version = "1.4.0.0"
 description = """The Teradata adapter plugin for dbt (data build tool)"""
 
 
 setup(
     name=package_name,
     version=package_version,
 
@@ -41,15 +41,15 @@
             'macros/*.sql',
             'macros/materializations/**/*.sql',
             'dbt_project.yml',
             'sample_profiles.yml',
         ],
     },
     install_requires=[
-        "dbt-core==1.3.3",
+        "dbt-core==1.4.6",
         "teradatasql>=16.20.0.0",
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
 
         'License :: OSI Approved :: Apache Software License',
 
@@ -57,10 +57,11 @@
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: POSIX :: Linux',
 
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
-    python_requires=">=3.7,<3.11",
+    python_requires=">=3.7,<3.12",
 )
```

