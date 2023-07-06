# Comparing `tmp/brainchain-0.1.2.tar.gz` & `tmp/brainchain-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.1.2.tar", max compression
+gzip compressed data, was "brainchain-0.1.3.tar", max compression
```

## Comparing `brainchain-0.1.2.tar` & `brainchain-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6082 2023-07-06 19:49:19.686228 brainchain-0.1.2/brainchain/.aider.chat.history.md
--rw-r--r--   0        0        0     1874 2023-07-06 19:48:47.151645 brainchain-0.1.2/brainchain/.aider.input.history
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.1.2/brainchain/README.md
--rw-r--r--   0        0        0      104 2023-07-06 19:41:43.280891 brainchain-0.1.2/brainchain/__init__.py
--rw-r--r--   0        0        0     4906 2023-07-06 20:01:02.512674 brainchain-0.1.2/brainchain/brainchain.py
--rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.1.2/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.1.2/brainchain/coredata.py
--rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.1.2/brainchain/factcheck.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.1.2/brainchain/requirements.txt
--rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.1.2/brainchain/sales_intel.py
--rw-r--r--   0        0        0      531 2023-07-06 20:01:10.356538 brainchain-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 brainchain-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6082 2023-07-06 19:49:19.686228 brainchain-0.1.3/brainchain/.aider.chat.history.md
+-rw-r--r--   0        0        0     1874 2023-07-06 19:48:47.151645 brainchain-0.1.3/brainchain/.aider.input.history
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.1.3/brainchain/README.md
+-rw-r--r--   0        0        0      104 2023-07-06 20:07:36.323879 brainchain-0.1.3/brainchain/__init__.py
+-rw-r--r--   0        0        0     4887 2023-07-06 20:09:08.132511 brainchain-0.1.3/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.1.3/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.1.3/brainchain/coredata.py
+-rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.1.3/brainchain/factcheck.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.1.3/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.1.3/brainchain/sales_intel.py
+-rw-r--r--   0        0        0      531 2023-07-06 20:06:17.638584 brainchain-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 brainchain-0.1.3/PKG-INFO
```

### Comparing `brainchain-0.1.2/brainchain/.aider.chat.history.md` & `brainchain-0.1.3/brainchain/.aider.chat.history.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.1.2/brainchain/.aider.input.history` & `brainchain-0.1.3/brainchain/.aider.input.history`

 * *Files identical despite different names*

### Comparing `brainchain-0.1.2/brainchain/README.md` & `brainchain-0.1.3/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.1.2/brainchain/brainchain.py` & `brainchain-0.1.3/brainchain/brainchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import sys
 import json
 import requests
 from urllib.parse import quote
-from brainchain import SalesIntel
-from brainchain import FactCheck
-
+from . import SalesIntel
+from . import FactCheck
 
 class Brainchain:
     def __init__(self, env: str = "prod", api_key: str = os.environ["BRAINCHAIN_API_KEY"], service_url="https://brainchain--agent.modal.run/", salesintel_api_key=os.environ["SALESINTEL_API_KEY"]):
         self.api_key = api_key
         self.env = env
         self.fact_check_instance = FactCheck(environment=env)
         self.sales_intel_client = SalesIntel(salesintel_api_key)
```

### Comparing `brainchain-0.1.2/brainchain/carnivore.py` & `brainchain-0.1.3/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.1.2/brainchain/coredata.py` & `brainchain-0.1.3/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.1.2/brainchain/factcheck.py` & `brainchain-0.1.3/brainchain/factcheck.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.1.2/brainchain/requirements.txt` & `brainchain-0.1.3/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.1.2/brainchain/sales_intel.py` & `brainchain-0.1.3/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.1.2/pyproject.toml` & `brainchain-0.1.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.1.2"
+version = "0.1.3"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = "2.31.0"
 promptlayer = "0.1.90"
```

### Comparing `brainchain-0.1.2/PKG-INFO` & `brainchain-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.1.2
+Version: 0.1.3
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

