# Comparing `tmp/brainchain-0.0.9.tar.gz` & `tmp/brainchain-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.0.9.tar", max compression
+gzip compressed data, was "brainchain-0.1.0.tar", max compression
```

## Comparing `brainchain-0.0.9.tar` & `brainchain-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.0.9/brainchain/README.md
--rw-r--r--   0        0        0      135 2023-07-06 18:44:17.612198 brainchain-0.0.9/brainchain/__init__.py
--rw-r--r--   0        0        0     4973 2023-07-06 18:49:50.794690 brainchain-0.0.9/brainchain/brainchain.py
--rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.0.9/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.0.9/brainchain/coredata.py
--rw-r--r--   0        0        0     1548 2023-07-06 16:58:13.696070 brainchain-0.0.9/brainchain/example.py
--rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.0.9/brainchain/factcheck.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.0.9/brainchain/requirements.txt
--rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.0.9/brainchain/sales_intel.py
--rw-r--r--   0        0        0      531 2023-07-06 18:51:03.565362 brainchain-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 brainchain-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.1.0/brainchain/README.md
+-rw-r--r--   0        0        0      104 2023-07-06 19:35:52.689406 brainchain-0.1.0/brainchain/__init__.py
+-rw-r--r--   0        0        0     4973 2023-07-06 18:49:50.794690 brainchain-0.1.0/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.1.0/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.1.0/brainchain/coredata.py
+-rw-r--r--   0        0        0     1548 2023-07-06 16:58:13.696070 brainchain-0.1.0/brainchain/example.py
+-rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.1.0/brainchain/factcheck.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.1.0/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.1.0/brainchain/sales_intel.py
+-rw-r--r--   0        0        0      531 2023-07-06 19:36:00.918108 brainchain-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 brainchain-0.1.0/PKG-INFO
```

### Comparing `brainchain-0.0.9/brainchain/README.md` & `brainchain-0.1.0/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.0.9/brainchain/brainchain.py` & `brainchain-0.1.0/brainchain/brainchain.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.0.9/brainchain/carnivore.py` & `brainchain-0.1.0/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.0.9/brainchain/coredata.py` & `brainchain-0.1.0/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.0.9/brainchain/example.py` & `brainchain-0.1.0/brainchain/example.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.0.9/brainchain/factcheck.py` & `brainchain-0.1.0/brainchain/factcheck.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.0.9/brainchain/requirements.txt` & `brainchain-0.1.0/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.0.9/brainchain/sales_intel.py` & `brainchain-0.1.0/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.0.9/pyproject.toml` & `brainchain-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.0.9"
+version = "0.1.0"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = "2.31.0"
 promptlayer = "0.1.90"
```

### Comparing `brainchain-0.0.9/PKG-INFO` & `brainchain-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.0.9
+Version: 0.1.0
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

