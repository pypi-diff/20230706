# Comparing `tmp/alpyvantage-0.2.0.tar.gz` & `tmp/alpyvantage-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpyvantage-0.2.0.tar", last modified: Wed Jul  5 13:17:20 2023, max compression
+gzip compressed data, was "alpyvantage-0.2.1.tar", last modified: Thu Jul  6 08:05:19 2023, max compression
```

## Comparing `alpyvantage-0.2.0.tar` & `alpyvantage-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-05 13:17:20.399092 alpyvantage-0.2.0/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-05 13:17:20.395759 alpyvantage-0.2.0/.github/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-05 13:17:20.395759 alpyvantage-0.2.0/.github/workflows/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1039 2023-07-05 11:21:18.000000 alpyvantage-0.2.0/.github/workflows/continuous-integration.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      173 2023-07-05 06:07:44.000000 alpyvantage-0.2.0/.gitignore
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      287 2023-07-05 06:07:44.000000 alpyvantage-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2023-07-05 06:07:44.000000 alpyvantage-0.2.0/.readthedocs.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2617 2023-07-05 13:17:20.399092 alpyvantage-0.2.0/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2217 2023-07-05 13:12:48.000000 alpyvantage-0.2.0/README.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-05 13:17:20.395759 alpyvantage-0.2.0/alpyvantage/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8660 2023-07-05 13:16:57.000000 alpyvantage-0.2.0/alpyvantage/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2023-07-05 13:16:36.000000 alpyvantage-0.2.0/alpyvantage/__version__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2052 2023-07-05 13:16:51.000000 alpyvantage-0.2.0/alpyvantage/data_formating.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      712 2023-07-05 13:09:12.000000 alpyvantage-0.2.0/alpyvantage/test_all.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-05 13:17:20.399092 alpyvantage-0.2.0/alpyvantage.egg-info/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2617 2023-07-05 13:17:20.000000 alpyvantage-0.2.0/alpyvantage.egg-info/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      519 2023-07-05 13:17:20.000000 alpyvantage-0.2.0/alpyvantage.egg-info/SOURCES.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-07-05 13:17:20.000000 alpyvantage-0.2.0/alpyvantage.egg-info/dependency_links.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       16 2023-07-05 13:17:20.000000 alpyvantage-0.2.0/alpyvantage.egg-info/requires.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       12 2023-07-05 13:17:20.000000 alpyvantage-0.2.0/alpyvantage.egg-info/top_level.txt
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-05 13:17:20.399092 alpyvantage-0.2.0/docs/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-07-05 06:12:18.000000 alpyvantage-0.2.0/docs/Makefile
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-05 13:17:20.395759 alpyvantage-0.2.0/docs/_static/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-05 13:17:20.399092 alpyvantage-0.2.0/docs/_static/css/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-07-05 06:12:18.000000 alpyvantage-0.2.0/docs/_static/css/custom.css
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1630 2023-07-05 06:12:55.000000 alpyvantage-0.2.0/docs/conf.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      101 2023-07-05 06:13:19.000000 alpyvantage-0.2.0/docs/index.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      795 2023-07-05 06:12:18.000000 alpyvantage-0.2.0/docs/make.bat
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       61 2023-07-05 06:13:05.000000 alpyvantage-0.2.0/docs/requirements.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       16 2023-07-05 11:19:25.000000 alpyvantage-0.2.0/requirements.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-07-05 13:17:20.399092 alpyvantage-0.2.0/setup.cfg
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1039 2023-07-05 11:19:18.000000 alpyvantage-0.2.0/setup.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-06 08:05:19.986562 alpyvantage-0.2.1/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-06 08:05:19.963229 alpyvantage-0.2.1/.github/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-06 08:05:19.973229 alpyvantage-0.2.1/.github/workflows/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1039 2023-07-05 11:21:18.000000 alpyvantage-0.2.1/.github/workflows/continuous-integration.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      173 2023-07-05 06:07:44.000000 alpyvantage-0.2.1/.gitignore
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      287 2023-07-05 06:07:44.000000 alpyvantage-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2023-07-05 06:07:44.000000 alpyvantage-0.2.1/.readthedocs.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-07-05 13:40:58.000000 alpyvantage-0.2.1/LICENSE
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2639 2023-07-06 08:05:19.983228 alpyvantage-0.2.1/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2217 2023-07-05 13:12:48.000000 alpyvantage-0.2.1/README.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-06 08:05:19.976562 alpyvantage-0.2.1/alpyvantage/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8732 2023-07-06 07:22:34.000000 alpyvantage-0.2.1/alpyvantage/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2023-07-06 08:02:44.000000 alpyvantage-0.2.1/alpyvantage/__version__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2363 2023-07-06 07:28:42.000000 alpyvantage-0.2.1/alpyvantage/data_formating.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      930 2023-07-05 20:39:44.000000 alpyvantage-0.2.1/alpyvantage/test_all.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-06 08:05:19.976562 alpyvantage-0.2.1/alpyvantage.egg-info/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2639 2023-07-06 08:05:19.000000 alpyvantage-0.2.1/alpyvantage.egg-info/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      527 2023-07-06 08:05:19.000000 alpyvantage-0.2.1/alpyvantage.egg-info/SOURCES.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-07-06 08:05:19.000000 alpyvantage-0.2.1/alpyvantage.egg-info/dependency_links.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       16 2023-07-06 08:05:19.000000 alpyvantage-0.2.1/alpyvantage.egg-info/requires.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       12 2023-07-06 08:05:19.000000 alpyvantage-0.2.1/alpyvantage.egg-info/top_level.txt
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-06 08:05:19.983228 alpyvantage-0.2.1/docs/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-07-05 06:12:18.000000 alpyvantage-0.2.1/docs/Makefile
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-06 08:05:19.966562 alpyvantage-0.2.1/docs/_static/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-06 08:05:19.983228 alpyvantage-0.2.1/docs/_static/css/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-07-05 06:12:18.000000 alpyvantage-0.2.1/docs/_static/css/custom.css
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1630 2023-07-05 06:12:55.000000 alpyvantage-0.2.1/docs/conf.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      101 2023-07-05 06:13:19.000000 alpyvantage-0.2.1/docs/index.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      795 2023-07-05 06:12:18.000000 alpyvantage-0.2.1/docs/make.bat
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       61 2023-07-05 06:13:05.000000 alpyvantage-0.2.1/docs/requirements.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       16 2023-07-05 11:19:25.000000 alpyvantage-0.2.1/requirements.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-07-06 08:05:19.986562 alpyvantage-0.2.1/setup.cfg
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1039 2023-07-05 11:19:18.000000 alpyvantage-0.2.1/setup.py
```

### Comparing `alpyvantage-0.2.0/.github/workflows/continuous-integration.yml` & `alpyvantage-0.2.1/.github/workflows/continuous-integration.yml`

 * *Files identical despite different names*

### Comparing `alpyvantage-0.2.0/.readthedocs.yaml` & `alpyvantage-0.2.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `alpyvantage-0.2.0/PKG-INFO` & `alpyvantage-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: alpyvantage
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python API to Alpha Vantage
 Home-page: https://github.com/gboehl/alpyvantage
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 
 alpyvantage
 =============
 
 **An alternative python backend to the Alpha Vantage API**
 
 .. image:: https://img.shields.io/badge/GitHub-gboehl%2Falpyvantage-blue.svg?style=flat
```

### Comparing `alpyvantage-0.2.0/README.rst` & `alpyvantage-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `alpyvantage-0.2.0/alpyvantage/__init__.py` & `alpyvantage-0.2.1/alpyvantage/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,14 @@
         return full output by default for any call
     """
 
     raw_url = 'https://www.alphavantage.co/query?'
     ordering = ['function', 'symbol', 'interval', 'month', 'outputsize']
 
     def __init__(self, api_key, to_pandas=True, outputsize='full'):
-        """Initialize the API
-        """
         self.key = api_key
         self.use_pandas = to_pandas
         self.outputsize = outputsize
 
     def __call__(self, function, data_key=None, **kwargs):
         """API call. Requires the function as in the original Alpha Vantage documentation (https://www.alphavantage.co/documentation/) and takes the API key as given
 
@@ -61,26 +59,27 @@
             '&'.join([k + '=' + str(kwargs[k]) for k in ordered_keys])
         r = requests.get(url)
         # catch server errors
         if r.status_code != 200:
             raise ConnectionError(
                 f"Server request status code is {r.status_code}.")
 
-        data_raw = r.json()
+        call_response = r.json()
         # API error handling
-        if 'Note' in data_raw:
-            raise AlphaVantageError(data_raw['Note'])
-        if 'Information' in data_raw:
-            raise AlphaVantageError(data_raw['Information'])
+        for message in ('Note', 'Information', 'Error Message'):
+            if message in call_response:
+                raise AlphaVantageError(call_response[message])
+        if not bool(call_response):
+            raise KeyError("API call returned an empty response.")
 
         # return as pandas dataframe if desired
         if self.use_pandas and data_key is not None:
-            return _format_to_pandas(data_raw, data_key)
+            return _format_to_pandas(call_response, data_key, **kwargs)
         else:
-            return data_raw, None
+            return call_response, None
 
     def time_series_intraday(self, symbol, interval='1min', **kwargs):
         """API call to TIME_SERIES_INTRADAY
 
         Parameters
         ----------
         symbol : string
```

### Comparing `alpyvantage-0.2.0/alpyvantage/data_formating.py` & `alpyvantage-0.2.1/alpyvantage/data_formating.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # -*- coding: utf-8 -*-
 import pandas as pd
 
 
-def _format_to_pandas(call_response, data_key):
+def _format_to_pandas(call_response, data_key, meta_data_key=None, **kwargs):
     # mainly taken from alpha_vantage package: https://github.com/RomelTorres/alpha_vantage
-    meta_data_key = 'Meta Data'
 
     if data_key is not None:
         data = call_response[data_key]
     else:
         data = call_response
     if meta_data_key is not None:
         meta_data = call_response[meta_data_key]
     else:
-        meta_data = None
+        meta_data = call_response.get('Meta Data')
     # Allow to override the output parameter in the call
     if isinstance(data, list):
         # If the call returns a list, then we will append them
         # in the resulting data frame. If in the future
         # alphavantage decides to do more with returning arrays
         # this might become buggy. For now will do the trick.
         if not data:
             data_pandas = pd.DataFrame()
         else:
             data_array = []
             for val in data:
                 data_array.append([v for _, v in val.items()])
             data_pandas = pd.DataFrame(data_array, columns=[
                 k for k, _ in data[0].items()])
+            data_pandas.set_index('date', inplace=True)
     else:
         try:
             data_pandas = pd.DataFrame.from_dict(data,
                                                  orient='index',
                                                  dtype='float')
         # This is for Global quotes or any other new Alpha Vantage
         # data that is added.
@@ -42,9 +42,16 @@
             data_pandas = pd.DataFrame.from_dict(data,
                                                  orient='index',
                                                  dtype='object')
             return data_pandas, meta_data
     data_pandas.index.name = 'date'
     # convert to pandas._libs.tslibs.timestamps.Timestamp
     data_pandas.index = pd.to_datetime(data_pandas.index)
-    data_pandas.columns = [col.split('. ')[1] for col in data_pandas.columns]
+    data_pandas.sort_index(inplace=True)
+    data_pandas = data_pandas.astype(float, errors='ignore')
+    try:
+        data_pandas.columns = [col.split('. ')[1]
+                               for col in data_pandas.columns]
+    except IndexError:
+        # columns names don't have a dot in them
+        pass
     return data_pandas, meta_data
```

### Comparing `alpyvantage-0.2.0/alpyvantage/test_all.py` & `alpyvantage-0.2.1/alpyvantage/test_all.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # -*- coding: utf-8 -*-
 
 from . import API
+from . import _format_to_pandas
 
 api = API('demo')
 
 
 def test_call():
     data, _ = api("TIME_SERIES_INTRADAY", symbol="IBM",
                   interval='5min', month='2009-01', outputsize="full")
     assert data['Time Series (5min)']['2009-01-20 08:05:00']['5. volume'] == '993'
 
 
 def test_intraday():
     data, _ = api.time_series_intraday("IBM", interval='5min', month='2009-01')
-    assert data.iloc[-1]['open'] == 49.575
+    assert data.iloc[0]['open'] == 49.575
 
 
 def test_weekly():
     data, _ = api.time_series_weekly("TSCO.LON")
-    assert data.iloc[-1]['open'] == 319.7501
+    assert data.iloc[0]['open'] == 319.7501
 
 
 def test_other():
     # pure testing, no comparison
     _ = api.quote_endpoint('IBM')
     _ = api.ticker_search('tencent')
     _ = api.global_market_status()
+
+def test_custom():
+    data, _ = api("WTI", interval="monthly")
+    data, _ = _format_to_pandas(data, data_key="data", meta_data_key=None)
+    assert data["value"]["1986-01-01"] == 22.93
```

### Comparing `alpyvantage-0.2.0/alpyvantage.egg-info/PKG-INFO` & `alpyvantage-0.2.1/alpyvantage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: alpyvantage
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python API to Alpha Vantage
 Home-page: https://github.com/gboehl/alpyvantage
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 
 alpyvantage
 =============
 
 **An alternative python backend to the Alpha Vantage API**
 
 .. image:: https://img.shields.io/badge/GitHub-gboehl%2Falpyvantage-blue.svg?style=flat
```

### Comparing `alpyvantage-0.2.0/alpyvantage.egg-info/SOURCES.txt` & `alpyvantage-0.2.1/alpyvantage.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
+LICENSE
 README.rst
 requirements.txt
 setup.py
 .github/workflows/continuous-integration.yml
 alpyvantage/__init__.py
 alpyvantage/__version__.py
 alpyvantage/data_formating.py
```

### Comparing `alpyvantage-0.2.0/docs/Makefile` & `alpyvantage-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `alpyvantage-0.2.0/docs/conf.py` & `alpyvantage-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `alpyvantage-0.2.0/docs/make.bat` & `alpyvantage-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `alpyvantage-0.2.0/setup.py` & `alpyvantage-0.2.1/setup.py`

 * *Files identical despite different names*

