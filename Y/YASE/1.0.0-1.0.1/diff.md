# Comparing `tmp/YASE-1.0.0.tar.gz` & `tmp/YASE-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YASE-1.0.0.tar", last modified: Thu Jul  6 01:21:38 2023, max compression
+gzip compressed data, was "YASE-1.0.1.tar", last modified: Thu Jul  6 18:10:55 2023, max compression
```

## Comparing `YASE-1.0.0.tar` & `YASE-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:21:38.664355 YASE-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-06 01:21:38.664355 YASE-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-06 01:20:58.000000 YASE-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:21:38.664355 YASE-1.0.0/YASE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-06 01:21:38.000000 YASE-1.0.0/YASE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-06 01:21:38.000000 YASE-1.0.0/YASE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 01:21:38.000000 YASE-1.0.0/YASE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 01:21:38.000000 YASE-1.0.0/YASE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 01:21:38.000000 YASE-1.0.0/YASE.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 01:21:38.664355 YASE-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-06 01:20:58.000000 YASE-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:21:38.664355 YASE-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-06 01:20:58.000000 YASE-1.0.0/tests/test_arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-06 01:20:58.000000 YASE-1.0.0/tests/test_fse.py
--rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-07-06 01:20:58.000000 YASE-1.0.0/tests/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-06 01:20:58.000000 YASE-1.0.0/tests/test_sentence_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 01:20:58.000000 YASE-1.0.0/tests/test_vaex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:21:38.664355 YASE-1.0.0/yase/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-06 01:20:58.000000 YASE-1.0.0/yase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-06 01:20:58.000000 YASE-1.0.0/yase/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-06 01:20:58.000000 YASE-1.0.0/yase/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-06 01:20:58.000000 YASE-1.0.0/yase/mergingmethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-06 01:20:58.000000 YASE-1.0.0/yase/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:10:55.147664 YASE-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-06 18:10:55.147664 YASE-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-06 18:10:23.000000 YASE-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:10:55.143664 YASE-1.0.1/YASE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-06 18:10:55.000000 YASE-1.0.1/YASE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-06 18:10:55.000000 YASE-1.0.1/YASE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:10:55.000000 YASE-1.0.1/YASE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 18:10:55.000000 YASE-1.0.1/YASE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 18:10:55.000000 YASE-1.0.1/YASE.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:10:55.147664 YASE-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-06 18:10:23.000000 YASE-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:10:55.147664 YASE-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-06 18:10:23.000000 YASE-1.0.1/tests/test_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-06 18:10:23.000000 YASE-1.0.1/tests/test_fse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-07-06 18:10:23.000000 YASE-1.0.1/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-06 18:10:23.000000 YASE-1.0.1/tests/test_sentence_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 18:10:23.000000 YASE-1.0.1/tests/test_vaex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:10:55.147664 YASE-1.0.1/yase/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-06 18:10:23.000000 YASE-1.0.1/yase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:10:55.147664 YASE-1.0.1/yase/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:10:23.000000 YASE-1.0.1/yase/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-07-06 18:10:23.000000 YASE-1.0.1/yase/arrow/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-07-06 18:10:23.000000 YASE-1.0.1/yase/arrow/stringprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-07-06 18:10:23.000000 YASE-1.0.1/yase/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-06 18:10:23.000000 YASE-1.0.1/yase/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-06 18:10:23.000000 YASE-1.0.1/yase/mergingmethods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:10:55.147664 YASE-1.0.1/yase/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:10:23.000000 YASE-1.0.1/yase/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12792 2023-07-06 18:10:23.000000 YASE-1.0.1/yase/pandas/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-06 18:10:23.000000 YASE-1.0.1/yase/pandas/stringprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-06 18:10:23.000000 YASE-1.0.1/yase/utils.py
```

### Comparing `YASE-1.0.0/PKG-INFO` & `YASE-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YASE
-Version: 1.0.0
+Version: 1.0.1
 Home-page: https://github.com/VHRanger/YASE/
 Author: Matt Ranger
 License: MIT
 Description-Content-Type: text/markdown
 
 # Yet Another Sentence Embedding Library
```

### Comparing `YASE-1.0.0/README.md` & `YASE-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `YASE-1.0.0/YASE.egg-info/PKG-INFO` & `YASE-1.0.1/YASE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YASE
-Version: 1.0.0
+Version: 1.0.1
 Home-page: https://github.com/VHRanger/YASE/
 Author: Matt Ranger
 License: MIT
 Description-Content-Type: text/markdown
 
 # Yet Another Sentence Embedding Library
```

### Comparing `YASE-1.0.0/setup.py` & `YASE-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name="YASE",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(),
     license='MIT',
     author='Matt Ranger',
     url='https://github.com/VHRanger/YASE/',
     long_description=long_description,
     long_description_content_type='text/markdown',
     package_data={
```

### Comparing `YASE-1.0.0/tests/test_arrow.py` & `YASE-1.0.1/tests/test_arrow.py`

 * *Files identical despite different names*

### Comparing `YASE-1.0.0/tests/test_fse.py` & `YASE-1.0.1/tests/test_fse.py`

 * *Files identical despite different names*

### Comparing `YASE-1.0.0/tests/test_pandas.py` & `YASE-1.0.1/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `YASE-1.0.0/tests/test_sentence_transformers.py` & `YASE-1.0.1/tests/test_sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `YASE-1.0.0/yase/encoders.py` & `YASE-1.0.1/yase/encoders.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     #    (using pa.Table.from_arrays)
     my_embeddings = pd.DataFrame(
         res,
         columns=[col_name + "_" + str(i) 
                 for i in range(vector_size)]
     )
     if verbose:
-        print(f"{column.name} time: {time.time() - start_t :.2f}")
+        print(f"{col_name} time: {time.time() - start_t :.2f}")
     return my_embeddings
 
 
 class ColumnEmbedder(TransformerMixin, BaseEstimator):
     def __init__(
         self, embedding_model,
         model_router=None,
```

### Comparing `YASE-1.0.0/yase/evaluation.py` & `YASE-1.0.1/yase/evaluation.py`

 * *Files identical despite different names*

### Comparing `YASE-1.0.0/yase/mergingmethods.py` & `YASE-1.0.1/yase/mergingmethods.py`

 * *Files identical despite different names*

### Comparing `YASE-1.0.0/yase/utils.py` & `YASE-1.0.1/yase/utils.py`

 * *Files identical despite different names*

