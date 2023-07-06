# Comparing `tmp/finops-0.1.9.tar.gz` & `tmp/finops-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finops-0.1.9.tar", last modified: Mon Jul  3 20:01:45 2023, max compression
+gzip compressed data, was "finops-0.2.0.tar", last modified: Thu Jul  6 19:06:58 2023, max compression
```

## Comparing `finops-0.1.9.tar` & `finops-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:01:45.505518 finops-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-03 20:01:36.000000 finops-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-03 20:01:45.505518 finops-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-03 20:01:36.000000 finops-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:01:45.501518 finops-0.1.9/finops/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 20:01:36.000000 finops-0.1.9/finops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-07-03 20:01:36.000000 finops-0.1.9/finops/codal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-07-03 20:01:36.000000 finops-0.1.9/finops/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-03 20:01:36.000000 finops-0.1.9/finops/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-03 20:01:36.000000 finops-0.1.9/finops/tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-03 20:01:36.000000 finops-0.1.9/finops/ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:01:45.501518 finops-0.1.9/finops/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:01:36.000000 finops-0.1.9/finops/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-03 20:01:36.000000 finops-0.1.9/finops/utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-07-03 20:01:36.000000 finops-0.1.9/finops/utils/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-03 20:01:36.000000 finops-0.1.9/finops/utils/scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-03 20:01:36.000000 finops-0.1.9/finops/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:01:45.501518 finops-0.1.9/finops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-03 20:01:45.000000 finops-0.1.9/finops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-03 20:01:45.000000 finops-0.1.9/finops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:01:45.000000 finops-0.1.9/finops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-03 20:01:45.000000 finops-0.1.9/finops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 20:01:45.000000 finops-0.1.9/finops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 20:01:45.505518 finops-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 20:01:36.000000 finops-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:01:45.505518 finops-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:01:36.000000 finops-0.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-03 20:01:36.000000 finops-0.1.9/tests/test_tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-03 20:01:36.000000 finops-0.1.9/tests/test_ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:01:45.505518 finops-0.1.9/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:01:36.000000 finops-0.1.9/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-03 20:01:36.000000 finops-0.1.9/tests/test_utils/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-03 20:01:36.000000 finops-0.1.9/tests/test_utils/test_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:06:58.512935 finops-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-06 19:06:42.000000 finops-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-06 19:06:58.512935 finops-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-06 19:06:42.000000 finops-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:06:58.508935 finops-0.2.0/finops/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 19:06:42.000000 finops-0.2.0/finops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-07-06 19:06:42.000000 finops-0.2.0/finops/codal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-07-06 19:06:42.000000 finops-0.2.0/finops/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-06 19:06:42.000000 finops-0.2.0/finops/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-06 19:06:42.000000 finops-0.2.0/finops/tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-06 19:06:42.000000 finops-0.2.0/finops/ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:06:58.512935 finops-0.2.0/finops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:06:42.000000 finops-0.2.0/finops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-06 19:06:42.000000 finops-0.2.0/finops/utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-07-06 19:06:42.000000 finops-0.2.0/finops/utils/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-06 19:06:42.000000 finops-0.2.0/finops/utils/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-06 19:06:42.000000 finops-0.2.0/finops/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:06:58.512935 finops-0.2.0/finops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-06 19:06:58.000000 finops-0.2.0/finops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-06 19:06:58.000000 finops-0.2.0/finops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:06:58.000000 finops-0.2.0/finops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-06 19:06:58.000000 finops-0.2.0/finops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 19:06:58.000000 finops-0.2.0/finops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:06:58.512935 finops-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 19:06:42.000000 finops-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:06:58.512935 finops-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:06:42.000000 finops-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-06 19:06:42.000000 finops-0.2.0/tests/test_tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-06 19:06:42.000000 finops-0.2.0/tests/test_ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:06:58.512935 finops-0.2.0/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:06:42.000000 finops-0.2.0/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-06 19:06:42.000000 finops-0.2.0/tests/test_utils/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-06 19:06:42.000000 finops-0.2.0/tests/test_utils/test_scraper.py
```

### Comparing `finops-0.1.9/LICENSE` & `finops-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `finops-0.1.9/PKG-INFO` & `finops-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python package for financial operations.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `finops-0.1.9/README.md` & `finops-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `finops-0.1.9/finops/codal.py` & `finops-0.2.0/finops/codal.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.9/finops/tehran_stock_exchange.py` & `finops-0.2.0/finops/tehran_stock_exchange.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.9/finops/ticker.py` & `finops-0.2.0/finops/ticker.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.9/finops/utils/downloader.py` & `finops-0.2.0/finops/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.9/finops/utils/preprocessor.py` & `finops-0.2.0/finops/utils/preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,29 +219,30 @@
                     "letter_title": letter["Title"],
                     "url": "https://www.codal.ir" + letter["Url"],
                 }
             )
         letters_list_df = pd.DataFrame(letters_list)
         return letters_list_df
 
-    @staticmethod
-    def _add_basic_letter_info(letter_df, info):
+    def _add_basic_letter_info(self, letter_df, info):
         letter_df["tracing_id"] = info["tracing_id"]
         letter_df["symbol"] = info["symbol"]
         letter_df["is_audited"] = "حسابرسی شده" in info["letter_title"]
         letter_df["is_correction"] = "اصلاحیه" in info["letter_title"]
         letter_df["is_consolidated"] = "تلفیقی" in info["letter_title"]
-        letter_df["period_type"] = re.search(
-            r"(سال مالی|میاندوره‌ای)", info["letter_title"]
-        ).group()
-
+        period_type = re.search(r"(سال مالی|میاندوره‌ای)", info["letter_title"]).group()
+        letter_df["period_type"] = "annual" if period_type == "سال مالی" else "interim"
         letter_df["period_length"] = (
-            re.search(r"\d+(?= ماهه)", info["letter_title"]).group()
+            int(
+                self._preprocess_persian_text(
+                    re.search(r"\d+(?= ماهه)", info["letter_title"]).group()
+                )
+            )
             if re.search(r"\d+(?= ماهه)", info["letter_title"])
-            else None
+            else 12
         )
         letter_df["period_end_date"] = (
             jdatetime.datetime.strptime(
                 re.search(r"\d{4}/\d{2}/\d{2}", info["letter_title"]).group(),
                 "%Y/%m/%d",
             )
             .date()
```

### Comparing `finops-0.1.9/finops/utils/scraper.py` & `finops-0.2.0/finops/utils/scraper.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.9/finops/utils/wrappers.py` & `finops-0.2.0/finops/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.9/finops.egg-info/PKG-INFO` & `finops-0.2.0/finops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python package for financial operations.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `finops-0.1.9/finops.egg-info/SOURCES.txt` & `finops-0.2.0/finops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finops-0.1.9/setup.py` & `finops-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='finops',
-    version='0.1.9',
+    version='0.2.0',
     description='A Python package for financial operations.',
     author='Alireza Nilgaran',
     author_email='alireza.nilgaran@gmail.com',
     url='https://github.com/nixuri/FinOps',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `finops-0.1.9/tests/test_tehran_stock_exchange.py` & `finops-0.2.0/tests/test_tehran_stock_exchange.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.9/tests/test_ticker.py` & `finops-0.2.0/tests/test_ticker.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.9/tests/test_utils/test_downloader.py` & `finops-0.2.0/tests/test_utils/test_downloader.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.9/tests/test_utils/test_scraper.py` & `finops-0.2.0/tests/test_utils/test_scraper.py`

 * *Files identical despite different names*

