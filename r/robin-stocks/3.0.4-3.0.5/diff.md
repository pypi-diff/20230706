# Comparing `tmp/robin_stocks-3.0.4.tar.gz` & `tmp/robin_stocks-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robin_stocks-3.0.4.tar", last modified: Sat Jun 17 05:01:07 2023, max compression
+gzip compressed data, was "robin_stocks-3.0.5.tar", last modified: Thu Jul  6 03:30:33 2023, max compression
```

## Comparing `robin_stocks-3.0.4.tar` & `robin_stocks-3.0.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 05:01:07.416613 robin_stocks-3.0.4/
--rw-r--r--   0 josh       (501) staff       (20)     1062 2018-10-17 16:32:18.000000 robin_stocks-3.0.4/LICENSE.txt
--rw-r--r--   0 josh       (501) staff       (20)       88 2018-09-27 04:22:53.000000 robin_stocks-3.0.4/MANIFEST.in
--rw-r--r--   0 josh       (501) staff       (20)     5087 2023-06-17 05:01:07.416217 robin_stocks-3.0.4/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     4629 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/README.rst
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 05:01:07.398390 robin_stocks-3.0.4/robin_stocks/
--rw-r--r--   0 josh       (501) staff       (20)       47 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/__init__.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 05:01:07.403811 robin_stocks-3.0.4/robin_stocks/gemini/
--rw-r--r--   0 josh       (501) staff       (20)      789 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/gemini/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    12995 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/gemini/account.py
--rw-r--r--   0 josh       (501) staff       (20)     2499 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/gemini/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)    10801 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/gemini/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)      585 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/gemini/globals.py
--rw-r--r--   0 josh       (501) staff       (20)     6140 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/gemini/helper.py
--rw-r--r--   0 josh       (501) staff       (20)    18993 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/gemini/orders.py
--rw-r--r--   0 josh       (501) staff       (20)     3859 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/gemini/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 05:01:07.409840 robin_stocks-3.0.4/robin_stocks/robinhood/
--rw-r--r--   0 josh       (501) staff       (20)     5064 2023-06-17 04:58:36.000000 robin_stocks-3.0.4/robin_stocks/robinhood/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    30654 2023-05-22 00:46:39.000000 robin_stocks-3.0.4/robin_stocks/robinhood/account.py
--rw-r--r--   0 josh       (501) staff       (20)     8596 2021-10-20 03:38:49.000000 robin_stocks-3.0.4/robin_stocks/robinhood/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)     9715 2021-05-12 02:09:12.000000 robin_stocks-3.0.4/robin_stocks/robinhood/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)     6602 2023-05-22 00:46:39.000000 robin_stocks-3.0.4/robin_stocks/robinhood/export.py
--rw-r--r--   0 josh       (501) staff       (20)      902 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/robinhood/globals.py
--rw-r--r--   0 josh       (501) staff       (20)    13217 2021-02-23 04:29:35.000000 robin_stocks-3.0.4/robin_stocks/robinhood/helper.py
--rw-r--r--   0 josh       (501) staff       (20)    11649 2021-02-27 17:30:21.000000 robin_stocks-3.0.4/robin_stocks/robinhood/markets.py
--rw-r--r--   0 josh       (501) staff       (20)    20412 2023-06-17 04:58:36.000000 robin_stocks-3.0.4/robin_stocks/robinhood/options.py
--rw-r--r--   0 josh       (501) staff       (20)    65100 2023-06-17 04:52:06.000000 robin_stocks-3.0.4/robin_stocks/robinhood/orders.py
--rw-r--r--   0 josh       (501) staff       (20)     9622 2023-05-22 00:46:39.000000 robin_stocks-3.0.4/robin_stocks/robinhood/profiles.py
--rw-r--r--   0 josh       (501) staff       (20)    25261 2023-05-22 01:12:04.000000 robin_stocks-3.0.4/robin_stocks/robinhood/stocks.py
--rw-r--r--   0 josh       (501) staff       (20)     7621 2023-06-17 02:17:53.000000 robin_stocks-3.0.4/robin_stocks/robinhood/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 05:01:07.413592 robin_stocks-3.0.4/robin_stocks/tda/
--rw-r--r--   0 josh       (501) staff       (20)      713 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/tda/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     4761 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/tda/accounts.py
--rw-r--r--   0 josh       (501) staff       (20)     6608 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/tda/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)      753 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/tda/globals.py
--rw-r--r--   0 josh       (501) staff       (20)     9765 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/tda/helper.py
--rw-r--r--   0 josh       (501) staff       (20)     3433 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/tda/markets.py
--rw-r--r--   0 josh       (501) staff       (20)     4714 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/tda/orders.py
--rw-r--r--   0 josh       (501) staff       (20)    12030 2021-02-20 06:33:23.000000 robin_stocks-3.0.4/robin_stocks/tda/stocks.py
--rw-r--r--   0 josh       (501) staff       (20)     3161 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/tda/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 05:01:07.400360 robin_stocks-3.0.4/robin_stocks.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)     5087 2023-06-17 05:01:07.000000 robin_stocks-3.0.4/robin_stocks.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     1330 2023-06-17 05:01:07.000000 robin_stocks-3.0.4/robin_stocks.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2023-06-17 05:01:07.000000 robin_stocks-3.0.4/robin_stocks.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2018-02-23 03:52:33.000000 robin_stocks-3.0.4/robin_stocks.egg-info/not-zip-safe
--rw-r--r--   0 josh       (501) staff       (20)       42 2023-06-17 05:01:07.000000 robin_stocks-3.0.4/robin_stocks.egg-info/requires.txt
--rw-r--r--   0 josh       (501) staff       (20)       19 2023-06-17 05:01:07.000000 robin_stocks-3.0.4/robin_stocks.egg-info/top_level.txt
--rw-r--r--   0 josh       (501) staff       (20)       38 2023-06-17 05:01:07.416724 robin_stocks-3.0.4/setup.cfg
--rw-r--r--   0 josh       (501) staff       (20)      931 2023-06-17 05:00:40.000000 robin_stocks-3.0.4/setup.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 05:01:07.415647 robin_stocks-3.0.4/tests/
--rw-r--r--   0 josh       (501) staff       (20)        0 2020-06-15 04:00:04.000000 robin_stocks-3.0.4/tests/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     9843 2023-05-22 02:31:15.000000 robin_stocks-3.0.4/tests/app_tests.py
--rw-r--r--   0 josh       (501) staff       (20)     2157 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/tests/test_gemini.py
--rw-r--r--   0 josh       (501) staff       (20)    32945 2023-05-22 02:32:23.000000 robin_stocks-3.0.4/tests/test_robinhood.py
--rw-r--r--   0 josh       (501) staff       (20)      571 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/tests/test_tda.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-06 03:30:33.808555 robin_stocks-3.0.5/
+-rw-r--r--   0 josh       (501) staff       (20)     1062 2018-10-17 16:32:18.000000 robin_stocks-3.0.5/LICENSE.txt
+-rw-r--r--   0 josh       (501) staff       (20)       88 2018-09-27 04:22:53.000000 robin_stocks-3.0.5/MANIFEST.in
+-rw-r--r--   0 josh       (501) staff       (20)     5087 2023-07-06 03:30:33.808074 robin_stocks-3.0.5/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     4629 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/README.rst
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-06 03:30:33.787011 robin_stocks-3.0.5/robin_stocks/
+-rw-r--r--   0 josh       (501) staff       (20)       47 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/__init__.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-06 03:30:33.793959 robin_stocks-3.0.5/robin_stocks/gemini/
+-rw-r--r--   0 josh       (501) staff       (20)      789 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/gemini/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    12995 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/gemini/account.py
+-rw-r--r--   0 josh       (501) staff       (20)     2499 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/gemini/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)    10801 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/gemini/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)      585 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/gemini/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)     6140 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/gemini/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)    18993 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/gemini/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)     3859 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/gemini/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-06 03:30:33.800479 robin_stocks-3.0.5/robin_stocks/robinhood/
+-rw-r--r--   0 josh       (501) staff       (20)     5064 2023-06-17 04:58:36.000000 robin_stocks-3.0.5/robin_stocks/robinhood/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    30664 2023-06-17 05:10:20.000000 robin_stocks-3.0.5/robin_stocks/robinhood/account.py
+-rw-r--r--   0 josh       (501) staff       (20)     8596 2021-10-20 03:38:49.000000 robin_stocks-3.0.5/robin_stocks/robinhood/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)     9715 2021-05-12 02:09:12.000000 robin_stocks-3.0.5/robin_stocks/robinhood/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)     6602 2023-05-22 00:46:39.000000 robin_stocks-3.0.5/robin_stocks/robinhood/export.py
+-rw-r--r--   0 josh       (501) staff       (20)      902 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/robinhood/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)    13321 2023-07-06 02:38:32.000000 robin_stocks-3.0.5/robin_stocks/robinhood/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)    11649 2021-02-27 17:30:21.000000 robin_stocks-3.0.5/robin_stocks/robinhood/markets.py
+-rw-r--r--   0 josh       (501) staff       (20)    20412 2023-06-17 04:58:36.000000 robin_stocks-3.0.5/robin_stocks/robinhood/options.py
+-rw-r--r--   0 josh       (501) staff       (20)    65728 2023-07-06 02:38:32.000000 robin_stocks-3.0.5/robin_stocks/robinhood/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)     9622 2023-05-22 00:46:39.000000 robin_stocks-3.0.5/robin_stocks/robinhood/profiles.py
+-rw-r--r--   0 josh       (501) staff       (20)    25274 2023-07-06 02:38:32.000000 robin_stocks-3.0.5/robin_stocks/robinhood/stocks.py
+-rw-r--r--   0 josh       (501) staff       (20)     7682 2023-07-06 02:38:32.000000 robin_stocks-3.0.5/robin_stocks/robinhood/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-06 03:30:33.804880 robin_stocks-3.0.5/robin_stocks/tda/
+-rw-r--r--   0 josh       (501) staff       (20)      713 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/tda/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     4761 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/tda/accounts.py
+-rw-r--r--   0 josh       (501) staff       (20)     6608 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/tda/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)      753 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/tda/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)     9765 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/tda/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)     3433 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/tda/markets.py
+-rw-r--r--   0 josh       (501) staff       (20)     4714 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/tda/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)    12030 2021-02-20 06:33:23.000000 robin_stocks-3.0.5/robin_stocks/tda/stocks.py
+-rw-r--r--   0 josh       (501) staff       (20)     3161 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/tda/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-06 03:30:33.789833 robin_stocks-3.0.5/robin_stocks.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)     5087 2023-07-06 03:30:33.000000 robin_stocks-3.0.5/robin_stocks.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     1330 2023-07-06 03:30:33.000000 robin_stocks-3.0.5/robin_stocks.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2023-07-06 03:30:33.000000 robin_stocks-3.0.5/robin_stocks.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2018-02-23 03:52:33.000000 robin_stocks-3.0.5/robin_stocks.egg-info/not-zip-safe
+-rw-r--r--   0 josh       (501) staff       (20)       42 2023-07-06 03:30:33.000000 robin_stocks-3.0.5/robin_stocks.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)       19 2023-07-06 03:30:33.000000 robin_stocks-3.0.5/robin_stocks.egg-info/top_level.txt
+-rw-r--r--   0 josh       (501) staff       (20)       38 2023-07-06 03:30:33.808706 robin_stocks-3.0.5/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)      931 2023-07-06 02:38:52.000000 robin_stocks-3.0.5/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-06 03:30:33.807455 robin_stocks-3.0.5/tests/
+-rw-r--r--   0 josh       (501) staff       (20)        0 2020-06-15 04:00:04.000000 robin_stocks-3.0.5/tests/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     9843 2023-05-22 02:31:15.000000 robin_stocks-3.0.5/tests/app_tests.py
+-rw-r--r--   0 josh       (501) staff       (20)     2157 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/tests/test_gemini.py
+-rw-r--r--   0 josh       (501) staff       (20)    32945 2023-07-06 02:51:59.000000 robin_stocks-3.0.5/tests/test_robinhood.py
+-rw-r--r--   0 josh       (501) staff       (20)      571 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/tests/test_tda.py
```

### Comparing `robin_stocks-3.0.4/LICENSE.txt` & `robin_stocks-3.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/PKG-INFO` & `robin_stocks-3.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin_stocks
-Version: 3.0.4
+Version: 3.0.5
 Summary: A Python wrapper around the Robinhood API
 Home-page: https://github.com/jmfernandes/robin_stocks
 Author: Josh Fernandes
 Author-email: joshfernandes@mac.com
 License: MIT
 Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
 Requires: requests
```

### Comparing `robin_stocks-3.0.4/README.rst` & `robin_stocks-3.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/gemini/__init__.py` & `robin_stocks-3.0.5/robin_stocks/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/gemini/account.py` & `robin_stocks-3.0.5/robin_stocks/gemini/account.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/gemini/authentication.py` & `robin_stocks-3.0.5/robin_stocks/gemini/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/gemini/crypto.py` & `robin_stocks-3.0.5/robin_stocks/gemini/crypto.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/gemini/globals.py` & `robin_stocks-3.0.5/robin_stocks/gemini/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/gemini/helper.py` & `robin_stocks-3.0.5/robin_stocks/gemini/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/gemini/orders.py` & `robin_stocks-3.0.5/robin_stocks/gemini/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/gemini/urls.py` & `robin_stocks-3.0.5/robin_stocks/gemini/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/robinhood/__init__.py` & `robin_stocks-3.0.5/robin_stocks/robinhood/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/robinhood/account.py` & `robin_stocks-3.0.5/robin_stocks/robinhood/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     if bounds not in bounds_check:
         print('ERROR: Bounds must be "extended","regular",or "trading"')
         return([None])
     if (bounds == 'extended' or bounds == 'trading') and span != 'day':
         print('ERROR: extended and trading bounds can only be used with a span of "day"', file=get_output())
         return([None])
 
-    account = load_account_profile('account_number')
+    account = load_account_profile(info='account_number')
     url = portfolis_historicals_url(account)
     payload = {
         'interval': interval,
         'span': span,
         'bounds': bounds
     }
     data = request_get(url, 'regular', payload)
@@ -492,15 +492,15 @@
 
     :param info: Will filter the results to get a specific value.
     :type info: Optional[str]
     :returns: Returns a list of dictionaries of key/value pairs for each day trade. If info parameter is provided, \
     a list of strings is returned where the strings are the value of the key that matches info.
 
     """
-    account = load_account_profile('account_number')
+    account = load_account_profile(info='account_number')
     url = daytrades_url(account)
     data = request_get(url, 'regular')
     return(filter_data(data, info))
 
 
 @login_required
 def get_documents(info=None):
```

### Comparing `robin_stocks-3.0.4/robin_stocks/robinhood/authentication.py` & `robin_stocks-3.0.5/robin_stocks/robinhood/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/robinhood/crypto.py` & `robin_stocks-3.0.5/robin_stocks/robinhood/crypto.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/robinhood/export.py` & `robin_stocks-3.0.5/robin_stocks/robinhood/export.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/robinhood/globals.py` & `robin_stocks-3.0.5/robin_stocks/robinhood/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/robinhood/helper.py` & `robin_stocks-3.0.5/robin_stocks/robinhood/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,14 +345,16 @@
         if json:
             update_session('Content-Type', 'application/json')
             res = SESSION.post(url, json=payload, timeout=timeout)
             update_session(
                 'Content-Type', 'application/x-www-form-urlencoded; charset=utf-8')
         else:
             res = SESSION.post(url, data=payload, timeout=timeout)
+        if res.status_code in [500,400]:
+            raise Exception("Received "+ str(res.status_code))
         data = res.json()
     except Exception as message:
         print("Error in request_post: {0}".format(message), file=get_output())
     # Either return response <200,401,etc.> or the data that is returned from requests.
     if jsonify_data:
         return(data)
     else:
```

### Comparing `robin_stocks-3.0.4/robin_stocks/robinhood/markets.py` & `robin_stocks-3.0.5/robin_stocks/robinhood/markets.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/robinhood/options.py` & `robin_stocks-3.0.5/robin_stocks/robinhood/options.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/robinhood/orders.py` & `robin_stocks-3.0.5/robin_stocks/robinhood/orders.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,24 +49,24 @@
     """
     url = crypto_orders_url()
     data = request_get(url, 'pagination')
     return(filter_data(data, info))
 
 
 @login_required
-def get_all_open_stock_orders(info=None):
+def get_all_open_stock_orders(info=None, account_number=None):
     """Returns a list of all the orders that are currently open.
 
     :param info: Will filter the results to get a specific value.
     :type info: Optional[str]
     :returns: Returns a list of dictionaries of key/value pairs for each order. If info parameter is provided, \
     a list of strings is returned where the strings are the value of the key that matches info.
 
     """
-    url = orders_url()
+    url = orders_url(account_number=account_number)
     data = request_get(url, 'pagination')
 
     data = [item for item in data if item['cancel'] is not None]
 
     return(filter_data(data, info))
 
 
@@ -346,15 +346,15 @@
     the price, and the quantity.
 
     """ 
     return order(symbol, quantity, "buy", account_number, None, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
-def order_buy_fractional_by_price(symbol, amountInDollars, account_number=None, timeInForce='gfd', extendedHours=False, jsonify=True):
+def order_buy_fractional_by_price(symbol, amountInDollars, account_number=None, timeInForce='gfd', extendedHours=False, jsonify=True, market_hours='regular_hours'):
     """Submits a market order to be executed immediately for fractional shares by specifying the amount in dollars that you want to trade.
     Good for share fractions up to 6 decimal places. Robinhood does not currently support placing limit, stop, or stop loss orders
     for fractional trades.
 
     :param symbol: The stock ticker of the stock to purchase.
     :type symbol: str
     :param amountInDollars: The amount in dollars of the fractional shares you want to buy.
@@ -376,15 +376,15 @@
         print("ERROR: Fractional share price should meet minimum 1.00.", file=get_output())
         return None
 
     # turn the money amount into decimal number of shares
     price = next(iter(get_latest_price(symbol, 'ask_price', extendedHours)), 0.00)
     fractional_shares = 0 if (price == 0.00) else round_price(amountInDollars/float(price))
     
-    return order(symbol, fractional_shares, "buy", account_number, None, None, timeInForce, extendedHours, jsonify)
+    return order(symbol, fractional_shares, "buy", None, None, account_number,  timeInForce, extendedHours, jsonify, market_hours)
 
 
 @login_required
 def order_buy_limit(symbol, quantity, limitPrice, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a limit order to be executed once a certain price is reached.
 
     :param symbol: The stock ticker of the stock to purchase.
@@ -518,15 +518,15 @@
     the price, and the quantity.
 
     """ 
     return order(symbol, quantity, "sell", account_number, None, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
-def order_sell_fractional_by_quantity(symbol, quantity, account_number=None, timeInForce='gfd', priceType='bid_price', extendedHours=False, jsonify=True):
+def order_sell_fractional_by_quantity(symbol, quantity, account_number=None, timeInForce='gfd', priceType='bid_price', extendedHours=False, jsonify=True, market_hours='regular_hours'):
     """Submits a market order to be executed immediately for fractional shares by specifying the amount that you want to trade.
     Good for share fractions up to 6 decimal places. Robinhood does not currently support placing limit, stop, or stop loss orders
     for fractional trades.
 
     :param symbol: The stock ticker of the stock to purchase.
     :type symbol: str
     :param quantity: The amount of the fractional shares you want to buy.
@@ -540,15 +540,15 @@
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "sell", account_number, None, None, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "sell", None, None, account_number,  timeInForce, extendedHours, jsonify, market_hours)
 
 
 @login_required
 def order_sell_fractional_by_price(symbol, amountInDollars, account_number=None, timeInForce='gfd', extendedHours=False, jsonify=True):
     """Submits a market order to be executed immediately for fractional shares by specifying the amount in dollars that you want to trade.
     Good for share fractions up to 6 decimal places. Robinhood does not currently support placing limit, stop, or stop loss orders
     for fractional trades.
@@ -771,15 +771,15 @@
     url = orders_url()
     data = request_post(url, payload, json=True, jsonify_data=jsonify)
 
     return (data)
 
 
 @login_required
-def order(symbol, quantity, side, limitPrice=None, stopPrice=None, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
+def order(symbol, quantity, side, limitPrice=None, stopPrice=None, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True, market_hours='regular_hours'):
     """A generic order function.
 
     :param symbol: The stock ticker of the stock to sell.
     :type symbol: str
     :param quantity: The number of stocks to sell.
     :type quantity: int
     :param side: Either 'buy' or 'sell'
@@ -841,25 +841,36 @@
         'quantity': quantity,
         'ref_id': str(uuid4()),
         'type': orderType,
         'stop_price': stopPrice,
         'time_in_force': timeInForce,
         'trigger': trigger,
         'side': side,
-        'extended_hours': extendedHours
+        'market_hours': market_hours, # choices are ['regular_hours', 'all_day_hours']
+        'extended_hours': extendedHours,
+        'order_form_version': 4
     }
-    # BEGIN PATCH FOR NEW ROBINHOOD BUY FORM (GuitarGuyChrisB 5/26/2023)
-    if side == "buy":
-        payload['order_form_version'] = "2"
-        payload['preset_percent_limit'] = "0.05"
-    # END PATCH FOR NEW ROBINHOOD BUY FORM (GuitarGuyChrisB 5/26/2023)
-
+    # adjust market orders
+    if orderType == 'market':
+        del payload['stop_price']
+        del payload['extended_hours'] 
+        
+    if market_hours == 'regular_hours':
+        if side == "buy":
+            payload['preset_percent_limit'] = "0.05"
+            payload['type'] = 'limit' 
+        # regular market sell
+        elif orderType == 'market' and side == 'sell':
+            del payload['price']   
+    elif market_hours == 'all_day_hours': 
+        payload['type'] = 'limit' 
+        payload['quantity']=int(payload['quantity']) # round to integer instead of fractional
+        
     url = orders_url()
 
-
     data = request_post(url, payload, jsonify_data=jsonify)
 
     return(data)
 
 
 @login_required
 def order_option_credit_spread(price, symbol, quantity, spread, timeInForce='gtc', account_number=None, jsonify=True):
```

### Comparing `robin_stocks-3.0.4/robin_stocks/robinhood/profiles.py` & `robin_stocks-3.0.5/robin_stocks/robinhood/profiles.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/robinhood/stocks.py` & `robin_stocks-3.0.5/robin_stocks/robinhood/stocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Contains information in regards to stocks."""
-from functools import cache
+from functools import lru_cache as cache
 
 from robin_stocks.robinhood.helper import *
 from robin_stocks.robinhood.urls import *
 
 def get_quotes(inputSymbols, info=None):
     """Takes any number of stock tickers and returns information pertaining to its price.
```

### Comparing `robin_stocks-3.0.4/robin_stocks/robinhood/urls.py` & `robin_stocks-3.0.5/robin_stocks/robinhood/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -285,12 +285,15 @@
     return('https://api.robinhood.com/orders/{0}/cancel/'.format(url))
 
 
 def option_cancel_url(id):
     return('https://api.robinhood.com/options/orders/{0}/cancel/'.format(id))
 
 
-def orders_url(orderID=None):
+def orders_url(orderID=None, account_number=None):
+    url = 'https://api.robinhood.com/orders/'
     if orderID:
-        return('https://api.robinhood.com/orders/{0}/'.format(orderID))
-    else:
-        return('https://api.robinhood.com/orders/')
+        url += '{0}/'.format(orderID)
+    if account_number:
+        url += ('?account_numbers='+account_number)
+
+    return url
```

### Comparing `robin_stocks-3.0.4/robin_stocks/tda/__init__.py` & `robin_stocks-3.0.5/robin_stocks/tda/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/tda/accounts.py` & `robin_stocks-3.0.5/robin_stocks/tda/accounts.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/tda/authentication.py` & `robin_stocks-3.0.5/robin_stocks/tda/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/tda/globals.py` & `robin_stocks-3.0.5/robin_stocks/tda/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/tda/helper.py` & `robin_stocks-3.0.5/robin_stocks/tda/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/tda/markets.py` & `robin_stocks-3.0.5/robin_stocks/tda/markets.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/tda/orders.py` & `robin_stocks-3.0.5/robin_stocks/tda/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/tda/stocks.py` & `robin_stocks-3.0.5/robin_stocks/tda/stocks.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks/tda/urls.py` & `robin_stocks-3.0.5/robin_stocks/tda/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/robin_stocks.egg-info/PKG-INFO` & `robin_stocks-3.0.5/robin_stocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin-stocks
-Version: 3.0.4
+Version: 3.0.5
 Summary: A Python wrapper around the Robinhood API
 Home-page: https://github.com/jmfernandes/robin_stocks
 Author: Josh Fernandes
 Author-email: joshfernandes@mac.com
 License: MIT
 Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
 Requires: requests
```

### Comparing `robin_stocks-3.0.4/robin_stocks.egg-info/SOURCES.txt` & `robin_stocks-3.0.5/robin_stocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/setup.py` & `robin_stocks-3.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='robin_stocks',
-      version='3.0.4',
+      version='3.0.5',
       description='A Python wrapper around the Robinhood API',
       long_description=long_description,
       long_description_content_type='text/x-rst',
       url='https://github.com/jmfernandes/robin_stocks',
       author='Josh Fernandes',
       author_email='joshfernandes@mac.com',
       keywords=['robinhood','robin stocks','finance app','stocks','options','trading','investing'],
```

### Comparing `robin_stocks-3.0.4/tests/app_tests.py` & `robin_stocks-3.0.5/tests/app_tests.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/tests/test_gemini.py` & `robin_stocks-3.0.5/tests/test_gemini.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/tests/test_robinhood.py` & `robin_stocks-3.0.5/tests/test_robinhood.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.4/tests/test_tda.py` & `robin_stocks-3.0.5/tests/test_tda.py`

 * *Files identical despite different names*

