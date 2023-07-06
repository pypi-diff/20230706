# Comparing `tmp/finops-0.2.1.tar.gz` & `tmp/finops-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finops-0.2.1.tar", last modified: Thu Jul  6 20:42:57 2023, max compression
+gzip compressed data, was "finops-0.2.2.tar", last modified: Thu Jul  6 21:44:01 2023, max compression
```

## Comparing `finops-0.2.1.tar` & `finops-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:57.197455 finops-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-06 20:42:47.000000 finops-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-06 20:42:57.197455 finops-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-06 20:42:47.000000 finops-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:57.197455 finops-0.2.1/finops/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 20:42:47.000000 finops-0.2.1/finops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-07-06 20:42:47.000000 finops-0.2.1/finops/codal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-07-06 20:42:47.000000 finops-0.2.1/finops/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-06 20:42:47.000000 finops-0.2.1/finops/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-06 20:42:47.000000 finops-0.2.1/finops/tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-06 20:42:47.000000 finops-0.2.1/finops/ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:57.197455 finops-0.2.1/finops/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:47.000000 finops-0.2.1/finops/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-06 20:42:47.000000 finops-0.2.1/finops/utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-06 20:42:47.000000 finops-0.2.1/finops/utils/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-06 20:42:47.000000 finops-0.2.1/finops/utils/scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-06 20:42:47.000000 finops-0.2.1/finops/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:57.197455 finops-0.2.1/finops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-06 20:42:57.000000 finops-0.2.1/finops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-06 20:42:57.000000 finops-0.2.1/finops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:42:57.000000 finops-0.2.1/finops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-06 20:42:57.000000 finops-0.2.1/finops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 20:42:57.000000 finops-0.2.1/finops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:42:57.197455 finops-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 20:42:47.000000 finops-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:57.197455 finops-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:47.000000 finops-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-06 20:42:47.000000 finops-0.2.1/tests/test_tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-06 20:42:47.000000 finops-0.2.1/tests/test_ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:57.197455 finops-0.2.1/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:47.000000 finops-0.2.1/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-06 20:42:47.000000 finops-0.2.1/tests/test_utils/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-06 20:42:47.000000 finops-0.2.1/tests/test_utils/test_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:44:01.854472 finops-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-06 21:43:50.000000 finops-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-06 21:44:01.854472 finops-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-06 21:43:50.000000 finops-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:44:01.850472 finops-0.2.2/finops/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 21:43:50.000000 finops-0.2.2/finops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-07-06 21:43:50.000000 finops-0.2.2/finops/codal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-07-06 21:43:50.000000 finops-0.2.2/finops/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-06 21:43:50.000000 finops-0.2.2/finops/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-06 21:43:50.000000 finops-0.2.2/finops/tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-06 21:43:50.000000 finops-0.2.2/finops/ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:44:01.854472 finops-0.2.2/finops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:43:50.000000 finops-0.2.2/finops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-06 21:43:50.000000 finops-0.2.2/finops/utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-07-06 21:43:50.000000 finops-0.2.2/finops/utils/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-06 21:43:50.000000 finops-0.2.2/finops/utils/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-06 21:43:50.000000 finops-0.2.2/finops/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:44:01.854472 finops-0.2.2/finops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-06 21:44:01.000000 finops-0.2.2/finops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-06 21:44:01.000000 finops-0.2.2/finops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:44:01.000000 finops-0.2.2/finops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-06 21:44:01.000000 finops-0.2.2/finops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 21:44:01.000000 finops-0.2.2/finops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:44:01.854472 finops-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 21:43:50.000000 finops-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:44:01.854472 finops-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:43:50.000000 finops-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-06 21:43:50.000000 finops-0.2.2/tests/test_tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-06 21:43:50.000000 finops-0.2.2/tests/test_ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:44:01.854472 finops-0.2.2/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:43:50.000000 finops-0.2.2/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-06 21:43:50.000000 finops-0.2.2/tests/test_utils/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-06 21:43:50.000000 finops-0.2.2/tests/test_utils/test_scraper.py
```

### Comparing `finops-0.2.1/LICENSE` & `finops-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `finops-0.2.1/PKG-INFO` & `finops-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package for financial operations.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `finops-0.2.1/README.md` & `finops-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `finops-0.2.1/finops/codal.py` & `finops-0.2.2/finops/codal.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.1/finops/config.py` & `finops-0.2.2/finops/config.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.1/finops/tehran_stock_exchange.py` & `finops-0.2.2/finops/tehran_stock_exchange.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.1/finops/ticker.py` & `finops-0.2.2/finops/ticker.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.1/finops/utils/downloader.py` & `finops-0.2.2/finops/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.1/finops/utils/preprocessor.py` & `finops-0.2.2/finops/utils/preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,16 @@
                 selected_columns.append(df.loc[:, column])
             except KeyError:
                 selected_columns.append(pd.Series(dtype="object", name=column))
         return pd.concat(selected_columns, axis=1)
 
     def _preprocess_balance_sheet_df(self, df):
         df = df.applymap(self._preprocess_codal_text)
+        if len(df.columns) == 56:
+            df = df.iloc[:, 6:8]
         if len(df.columns) == 24:
             df = df.iloc[:, 3:5]
         if len(df.columns) == 18:
             df = df.iloc[:, 2:4]
         if len(df.columns) == 12:
             df = df.iloc[:, 1:3]
         if len(df.columns) == 10:
@@ -230,16 +232,17 @@
 
     def _add_basic_letter_info(self, letter_df, info):
         letter_df["tracing_id"] = info["tracing_id"]
         letter_df["symbol"] = info["symbol"]
         letter_df["is_audited"] = "حسابرسی شده" in info["letter_title"]
         letter_df["is_correction"] = "اصلاحیه" in info["letter_title"]
         letter_df["is_consolidated"] = "تلفیقی" in info["letter_title"]
-        period_type = re.search(r"(سال مالی|میاندوره‌ای)", info["letter_title"]).group()
-        letter_df["period_type"] = "annual" if period_type == "سال مالی" else "interim"
+        period_type = re.search(r"(سال مالی|میاندوره‌ای)", info["letter_title"])
+        if period_type is not None:
+            letter_df["period_type"] = "annual" if period_type.group() == "سال مالی" else "interim"
         letter_df["period_length"] = (
             int(
                 self._preprocess_persian_text(
                     re.search(r"\d+(?= ماهه)", info["letter_title"]).group()
                 )
             )
             if re.search(r"\d+(?= ماهه)", info["letter_title"])
```

### Comparing `finops-0.2.1/finops/utils/scraper.py` & `finops-0.2.2/finops/utils/scraper.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.1/finops/utils/wrappers.py` & `finops-0.2.2/finops/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.1/finops.egg-info/PKG-INFO` & `finops-0.2.2/finops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package for financial operations.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `finops-0.2.1/finops.egg-info/SOURCES.txt` & `finops-0.2.2/finops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finops-0.2.1/setup.py` & `finops-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='finops',
-    version='0.2.1',
+    version='0.2.2',
     description='A Python package for financial operations.',
     author='Alireza Nilgaran',
     author_email='alireza.nilgaran@gmail.com',
     url='https://github.com/nixuri/FinOps',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `finops-0.2.1/tests/test_tehran_stock_exchange.py` & `finops-0.2.2/tests/test_tehran_stock_exchange.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.1/tests/test_ticker.py` & `finops-0.2.2/tests/test_ticker.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.1/tests/test_utils/test_downloader.py` & `finops-0.2.2/tests/test_utils/test_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import requests
 import unittest
 from unittest.mock import patch, Mock
 from io import StringIO
 from finops.utils.downloader import Downloader
 
 
-class TestBaseDownloader(unittest.TestCase):
+class TestDownloader(unittest.TestCase):
     def setUp(self):
         self.columns = ["col1", "col2", "col3"]
         self.path = "test.csv"
         self.url = "http://cdn.tsetmc.com/api/Shareholder/65883838195688438/20230522"
         self.user_agent = "Mozilla/5.0"
         self.timeout = (1, 1)
```

### Comparing `finops-0.2.1/tests/test_utils/test_scraper.py` & `finops-0.2.2/tests/test_utils/test_scraper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 import pandas as pd
 from datetime import date
 from finops.utils.scraper import Scraper
 
 
-class TestBaseScraper(unittest.TestCase):
+class TestScraper(unittest.TestCase):
     def setUp(self):
         self.traded_dates = [
             date(2022, 1, 1),
             date(2022, 1, 2),
             date(2022, 1, 3),
             date(2022, 1, 4),
             date(2022, 1, 5),
```

