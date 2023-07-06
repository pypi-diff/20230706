# Comparing `tmp/pyreindexer-0.2.8.tar.gz` & `tmp/pyreindexer-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreindexer-0.2.8.tar", last modified: Mon Nov 29 16:17:22 2021, max compression
+gzip compressed data, was "pyreindexer-0.2.9.tar", last modified: Mon Nov 29 17:18:24 2021, max compression
```

## Comparing `pyreindexer-0.2.8.tar` & `pyreindexer-0.2.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 16:17:22.790054 pyreindexer-0.2.8/
--rw-r--r--   0 runner     (501) staff       (20)    11342 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      366 2021-11-29 16:17:22.789612 pyreindexer-0.2.8/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    12027 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 16:17:22.776476 pyreindexer-0.2.8/pyreindexer/
--rw-r--r--   0 runner     (501) staff       (20)     1683 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      217 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 16:17:22.778720 pyreindexer-0.2.8/pyreindexer/example/
--rw-r--r--   0 runner     (501) staff       (20)     2170 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/example/main.py
--rw-r--r--   0 runner     (501) staff       (20)     2620 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/index_definition.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 16:17:22.772184 pyreindexer-0.2.8/pyreindexer/lib/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 16:17:22.779871 pyreindexer-0.2.8/pyreindexer/lib/include/
--rw-r--r--   0 runner     (501) staff       (20)     4093 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/lib/include/pyobjtools.cc
--rw-r--r--   0 runner     (501) staff       (20)      658 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/lib/include/pyobjtools.h
--rw-r--r--   0 runner     (501) staff       (20)      984 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/lib/include/queryresults_wrapper.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 16:17:22.781867 pyreindexer-0.2.8/pyreindexer/lib/src/
--rw-r--r--   0 runner     (501) staff       (20)     9237 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/lib/src/rawpyreindexer.cc
--rw-r--r--   0 runner     (501) staff       (20)     4442 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/lib/src/rawpyreindexer.h
--rw-r--r--   0 runner     (501) staff       (20)     2899 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/lib/src/reindexerinterface.cc
--rw-r--r--   0 runner     (501) staff       (20)     5879 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/lib/src/reindexerinterface.h
--rw-r--r--   0 runner     (501) staff       (20)     2286 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/query_results.py
--rw-r--r--   0 runner     (501) staff       (20)      792 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/raiser_mixin.py
--rw-r--r--   0 runner     (501) staff       (20)    14178 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/rx_connector.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 16:17:22.782633 pyreindexer-0.2.8/pyreindexer/tests/
--rw-r--r--   0 runner     (501) staff       (20)        0 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2957 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/conftest.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 16:17:22.785491 pyreindexer-0.2.8/pyreindexer/tests/helpers/
--rw-r--r--   0 runner     (501) staff       (20)        0 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/helpers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      829 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/helpers/index.py
--rw-r--r--   0 runner     (501) staff       (20)     1049 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/helpers/items.py
--rw-r--r--   0 runner     (501) staff       (20)     1494 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/helpers/log_helper.py
--rw-r--r--   0 runner     (501) staff       (20)      684 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/helpers/metadata.py
--rw-r--r--   0 runner     (501) staff       (20)     1268 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/helpers/namespace.py
--rw-r--r--   0 runner     (501) staff       (20)      260 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/helpers/sql.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 16:17:22.786251 pyreindexer-0.2.8/pyreindexer/tests/test_data/
--rw-r--r--   0 runner     (501) staff       (20)        0 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/test_data/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1230 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/test_data/constants.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 16:17:22.789093 pyreindexer-0.2.8/pyreindexer/tests/tests/
--rw-r--r--   0 runner     (501) staff       (20)        0 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1028 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/tests/test_database.py
--rw-r--r--   0 runner     (501) staff       (20)     3553 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/tests/test_index.py
--rw-r--r--   0 runner     (501) staff       (20)     4486 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/tests/test_items.py
--rw-r--r--   0 runner     (501) staff       (20)     2152 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/tests/test_metadata.py
--rw-r--r--   0 runner     (501) staff       (20)     1533 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/tests/test_namespace.py
--rw-r--r--   0 runner     (501) staff       (20)     3322 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/pyreindexer/tests/tests/test_sql.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 16:17:22.778355 pyreindexer-0.2.8/pyreindexer.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      366 2021-11-29 16:17:22.000000 pyreindexer-0.2.8/pyreindexer.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1347 2021-11-29 16:17:22.000000 pyreindexer-0.2.8/pyreindexer.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2021-11-29 16:17:22.000000 pyreindexer-0.2.8/pyreindexer.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       62 2021-11-29 16:17:22.000000 pyreindexer-0.2.8/pyreindexer.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       27 2021-11-29 16:17:22.000000 pyreindexer-0.2.8/pyreindexer.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2021-11-29 16:17:22.790168 pyreindexer-0.2.8/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     3018 2021-11-29 16:07:57.000000 pyreindexer-0.2.8/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 17:18:24.225950 pyreindexer-0.2.9/
+-rw-r--r--   0 runner     (501) staff       (20)    11342 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      366 2021-11-29 17:18:24.225565 pyreindexer-0.2.9/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    12027 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 17:18:24.208727 pyreindexer-0.2.9/pyreindexer/
+-rw-r--r--   0 runner     (501) staff       (20)     1683 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)      217 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 17:18:24.214105 pyreindexer-0.2.9/pyreindexer/example/
+-rw-r--r--   0 runner     (501) staff       (20)     2170 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/example/main.py
+-rw-r--r--   0 runner     (501) staff       (20)     2620 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/index_definition.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 17:18:24.203834 pyreindexer-0.2.9/pyreindexer/lib/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 17:18:24.215329 pyreindexer-0.2.9/pyreindexer/lib/include/
+-rw-r--r--   0 runner     (501) staff       (20)     4093 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/lib/include/pyobjtools.cc
+-rw-r--r--   0 runner     (501) staff       (20)      658 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/lib/include/pyobjtools.h
+-rw-r--r--   0 runner     (501) staff       (20)      984 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/lib/include/queryresults_wrapper.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 17:18:24.217236 pyreindexer-0.2.9/pyreindexer/lib/src/
+-rw-r--r--   0 runner     (501) staff       (20)     9237 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/lib/src/rawpyreindexer.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4442 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/lib/src/rawpyreindexer.h
+-rw-r--r--   0 runner     (501) staff       (20)     2899 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/lib/src/reindexerinterface.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5879 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/lib/src/reindexerinterface.h
+-rw-r--r--   0 runner     (501) staff       (20)     2286 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/query_results.py
+-rw-r--r--   0 runner     (501) staff       (20)      792 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/raiser_mixin.py
+-rw-r--r--   0 runner     (501) staff       (20)    14178 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/rx_connector.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 17:18:24.218053 pyreindexer-0.2.9/pyreindexer/tests/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2957 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/conftest.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 17:18:24.221050 pyreindexer-0.2.9/pyreindexer/tests/helpers/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/helpers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      829 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/helpers/index.py
+-rw-r--r--   0 runner     (501) staff       (20)     1049 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/helpers/items.py
+-rw-r--r--   0 runner     (501) staff       (20)     1494 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/helpers/log_helper.py
+-rw-r--r--   0 runner     (501) staff       (20)      684 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/helpers/metadata.py
+-rw-r--r--   0 runner     (501) staff       (20)     1268 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/helpers/namespace.py
+-rw-r--r--   0 runner     (501) staff       (20)      260 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/helpers/sql.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 17:18:24.221959 pyreindexer-0.2.9/pyreindexer/tests/test_data/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/test_data/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1230 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/test_data/constants.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 17:18:24.224949 pyreindexer-0.2.9/pyreindexer/tests/tests/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1028 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/tests/test_database.py
+-rw-r--r--   0 runner     (501) staff       (20)     3553 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/tests/test_index.py
+-rw-r--r--   0 runner     (501) staff       (20)     4486 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/tests/test_items.py
+-rw-r--r--   0 runner     (501) staff       (20)     2152 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/tests/test_metadata.py
+-rw-r--r--   0 runner     (501) staff       (20)     1533 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/tests/test_namespace.py
+-rw-r--r--   0 runner     (501) staff       (20)     3324 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/pyreindexer/tests/tests/test_sql.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-11-29 17:18:24.213606 pyreindexer-0.2.9/pyreindexer.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)      366 2021-11-29 17:18:24.000000 pyreindexer-0.2.9/pyreindexer.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1347 2021-11-29 17:18:24.000000 pyreindexer-0.2.9/pyreindexer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2021-11-29 17:18:24.000000 pyreindexer-0.2.9/pyreindexer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       62 2021-11-29 17:18:24.000000 pyreindexer-0.2.9/pyreindexer.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       27 2021-11-29 17:18:24.000000 pyreindexer-0.2.9/pyreindexer.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)       38 2021-11-29 17:18:24.226058 pyreindexer-0.2.9/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     3018 2021-11-29 17:09:06.000000 pyreindexer-0.2.9/setup.py
```

### Comparing `pyreindexer-0.2.8/LICENSE` & `pyreindexer-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/README.md` & `pyreindexer-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/CMakeLists.txt` & `pyreindexer-0.2.9/pyreindexer/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/example/main.py` & `pyreindexer-0.2.9/pyreindexer/example/main.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/index_definition.py` & `pyreindexer-0.2.9/pyreindexer/index_definition.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/lib/include/pyobjtools.cc` & `pyreindexer-0.2.9/pyreindexer/lib/include/pyobjtools.cc`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/lib/include/pyobjtools.h` & `pyreindexer-0.2.9/pyreindexer/lib/include/pyobjtools.h`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/lib/include/queryresults_wrapper.h` & `pyreindexer-0.2.9/pyreindexer/lib/include/queryresults_wrapper.h`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/lib/src/rawpyreindexer.cc` & `pyreindexer-0.2.9/pyreindexer/lib/src/rawpyreindexer.cc`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/lib/src/rawpyreindexer.h` & `pyreindexer-0.2.9/pyreindexer/lib/src/rawpyreindexer.h`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/lib/src/reindexerinterface.cc` & `pyreindexer-0.2.9/pyreindexer/lib/src/reindexerinterface.cc`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/lib/src/reindexerinterface.h` & `pyreindexer-0.2.9/pyreindexer/lib/src/reindexerinterface.h`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/query_results.py` & `pyreindexer-0.2.9/pyreindexer/query_results.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/raiser_mixin.py` & `pyreindexer-0.2.9/pyreindexer/raiser_mixin.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/rx_connector.py` & `pyreindexer-0.2.9/pyreindexer/rx_connector.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/tests/conftest.py` & `pyreindexer-0.2.9/pyreindexer/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/tests/helpers/index.py` & `pyreindexer-0.2.9/pyreindexer/tests/helpers/index.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/tests/helpers/items.py` & `pyreindexer-0.2.9/pyreindexer/tests/helpers/items.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/tests/helpers/log_helper.py` & `pyreindexer-0.2.9/pyreindexer/tests/helpers/log_helper.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/tests/helpers/metadata.py` & `pyreindexer-0.2.9/pyreindexer/tests/helpers/metadata.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/tests/helpers/namespace.py` & `pyreindexer-0.2.9/pyreindexer/tests/helpers/namespace.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/tests/test_data/constants.py` & `pyreindexer-0.2.9/pyreindexer/tests/test_data/constants.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/tests/tests/test_database.py` & `pyreindexer-0.2.9/pyreindexer/tests/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/tests/tests/test_index.py` & `pyreindexer-0.2.9/pyreindexer/tests/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/tests/tests/test_items.py` & `pyreindexer-0.2.9/pyreindexer/tests/tests/test_items.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/tests/tests/test_metadata.py` & `pyreindexer-0.2.9/pyreindexer/tests/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/tests/tests/test_namespace.py` & `pyreindexer-0.2.9/pyreindexer/tests/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/pyreindexer/tests/tests/test_sql.py` & `pyreindexer-0.2.9/pyreindexer/tests/tests/test_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         # Then ("Check that selected item is in result")
         assert_that(item_list, has_item(equal_to({'id': 3, 'val': 'testval3'})), "Can't SQL select data with condition")
 
     def test_sql_update(self, namespace, index, item):
         # Given("Create namespace with item")
         db, namespace_name = namespace
         # When ("Execute SQL query UPDATE")
-        query = f"UPDATE {namespace_name} SET 'val' = 'new_val' WHERE id = 100"
+        query = f"UPDATE {namespace_name} SET \"val\" = 'new_val' WHERE id = 100"
         item_list = sql_query(namespace, query)
         # Then ("Check that item is updated")
         assert_that(item_list, has_item(equal_to({'id': 100, 'val': 'new_val'})), "Can't SQL update data")
 
     def test_sql_delete(self, namespace, index, item):
         # Given("Create namespace with item")
         db, namespace_name = namespace
```

### Comparing `pyreindexer-0.2.8/pyreindexer.egg-info/SOURCES.txt` & `pyreindexer-0.2.9/pyreindexer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreindexer-0.2.8/setup.py` & `pyreindexer-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         if not self.dry_run:
             self.spawn(['cmake', '--build', '.'])
 
         os.chdir(cwd)
 
 
 setup(name=PACKAGE_NAME,
-      version='0.2.8',
+      version='0.2.9',
       description='A connector that allows to interact with Reindexer',
       url='https://github.com/Restream/reindexer-py',
       author='Igor Tulmentyev',
       author_email='igtulm@gmail.com',
       maintainer='Oleg Gerasimov',
       maintainer_email='ogerasimov@gmail.com',
       license='Apache License 2.0',
```

