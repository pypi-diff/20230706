# Comparing `tmp/wizata-dsapi-0.2.1.tar.gz` & `tmp/wizata-dsapi-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.2.1.tar", last modified: Thu Jun 22 13:55:25 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.2.2.tar", last modified: Thu Jul  6 08:02:48 2023, max compression
```

## Comparing `wizata-dsapi-0.2.1.tar` & `wizata-dsapi-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 13:55:25.334487 wizata-dsapi-0.2.1/
--rw-rw-rw-   0        0        0    11556 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0      176 2023-06-22 13:55:25.333990 wizata-dsapi-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-05-24 07:05:28.000000 wizata-dsapi-0.2.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-22 13:55:25.334487 wizata-dsapi-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-06-22 13:55:20.000000 wizata-dsapi-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 13:55:25.305719 wizata-dsapi-0.2.1/wizata_dsapi/
--rw-rw-rw-   0        0        0      996 2023-06-21 08:28:14.000000 wizata-dsapi-0.2.1/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.1/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     5763 2023-06-19 13:45:53.000000 wizata-dsapi-0.2.1/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     5714 2023-06-08 15:23:14.000000 wizata-dsapi-0.2.1/wizata_dsapi/datapoint.py
--rw-rw-rw-   0        0        0     1877 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.1/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.1/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    14903 2023-06-21 08:28:14.000000 wizata-dsapi-0.2.1/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3810 2023-06-08 07:54:01.000000 wizata-dsapi-0.2.1/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     9999 2023-06-21 05:55:35.000000 wizata-dsapi-0.2.1/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.1/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0    17900 2023-06-21 08:28:14.000000 wizata-dsapi-0.2.1/wizata_dsapi/pipeline.py
--rw-rw-rw-   0        0        0     2136 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.1/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0    17633 2023-06-21 08:28:14.000000 wizata-dsapi-0.2.1/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     8716 2023-06-12 20:23:50.000000 wizata-dsapi-0.2.1/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0     4961 2023-06-15 06:14:36.000000 wizata-dsapi-0.2.1/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0     2599 2023-06-22 09:21:08.000000 wizata-dsapi-0.2.1/wizata_dsapi/twin.py
--rw-rw-rw-   0        0        0     2701 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.1/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.1/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    56198 2023-06-22 13:44:33.000000 wizata-dsapi-0.2.1/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-06-22 13:55:25.332007 wizata-dsapi-0.2.1/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      176 2023-06-22 13:55:25.000000 wizata-dsapi-0.2.1/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      730 2023-06-22 13:55:25.000000 wizata-dsapi-0.2.1/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 13:55:25.000000 wizata-dsapi-0.2.1/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-06-22 13:55:25.000000 wizata-dsapi-0.2.1/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-22 13:55:25.000000 wizata-dsapi-0.2.1/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 08:02:48.793025 wizata-dsapi-0.2.2/
+-rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      176 2023-07-06 08:02:48.791023 wizata-dsapi-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-05-23 08:41:25.000000 wizata-dsapi-0.2.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-06 08:02:48.793025 wizata-dsapi-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1241 2023-07-06 08:02:29.000000 wizata-dsapi-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:02:48.765787 wizata-dsapi-0.2.2/wizata_dsapi/
+-rw-rw-rw-   0        0        0      996 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.2/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-03-25 08:43:45.000000 wizata-dsapi-0.2.2/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     5763 2023-06-18 19:31:22.000000 wizata-dsapi-0.2.2/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     5714 2023-06-12 08:44:45.000000 wizata-dsapi-0.2.2/wizata_dsapi/datapoint.py
+-rw-rw-rw-   0        0        0     1877 2023-05-07 10:55:37.000000 wizata-dsapi-0.2.2/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-03-20 14:32:36.000000 wizata-dsapi-0.2.2/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    14903 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.2/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3810 2023-06-01 19:11:05.000000 wizata-dsapi-0.2.2/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     9999 2023-06-20 18:59:20.000000 wizata-dsapi-0.2.2/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-06-20 16:08:31.000000 wizata-dsapi-0.2.2/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0    17900 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.2/wizata_dsapi/pipeline.py
+-rw-rw-rw-   0        0        0     2136 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.2/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0    18221 2023-07-06 08:02:29.000000 wizata-dsapi-0.2.2/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     8716 2023-06-14 12:20:26.000000 wizata-dsapi-0.2.2/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0     4961 2023-06-14 14:10:02.000000 wizata-dsapi-0.2.2/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0     2599 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.2/wizata_dsapi/twin.py
+-rw-rw-rw-   0        0        0     2701 2023-04-27 15:26:26.000000 wizata-dsapi-0.2.2/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.2/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    56198 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.2/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:02:48.789026 wizata-dsapi-0.2.2/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      176 2023-07-06 08:02:48.000000 wizata-dsapi-0.2.2/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      730 2023-07-06 08:02:48.000000 wizata-dsapi-0.2.2/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 08:02:48.000000 wizata-dsapi-0.2.2/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-07-06 08:02:48.000000 wizata-dsapi-0.2.2/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-06 08:02:48.000000 wizata-dsapi-0.2.2/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.2.1/LICENSE.txt` & `wizata-dsapi-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/setup.py` & `wizata-dsapi-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.2.1',
+    version='0.2.2',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/__init__.py` & `wizata-dsapi-0.2.2/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.2.2/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.2.2/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.2.2/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.2.2/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.2.2/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/execution.py` & `wizata-dsapi-0.2.2/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/experiment.py` & `wizata-dsapi-0.2.2/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.2.2/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.2.2/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.2.2/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/plot.py` & `wizata-dsapi-0.2.2/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/request.py` & `wizata-dsapi-0.2.2/wizata_dsapi/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,18 +240,29 @@
 
     def set_aggregation(self, method, interval):
         """
         Specifies aggregation properties
         :param method: 'mean' or 'stddev'
         :param interval: interval in ms (will be stored in seconds)
         """
+        if method not in self.list_agg_methods():
+            raise KeyError(f'unsupported agg_method {method}.')
         self.aggregation = method
         if interval is not None:
             self.interval = int(interval) / 1000
 
+    def list_agg_methods(self) -> list:
+        """
+        get a list of all authorized methods.
+        :return: list of all authorized methods.
+        """
+        return [
+            "mean", "stddev", "mode", "median", "count", "sum", "first", "last", "max", "min"
+        ]
+
     def select_template(self,
                         template_id=None,
                         template_key=None,
                         twin_id=None,
                         twin_hardware_id=None):
         """
         Select a template and its registration.
@@ -401,14 +412,16 @@
             self.end = datetime.fromtimestamp(json_data["timeframe"]["end"] / 1000, timezone.utc)
 
         if "aggregations" not in json_data.keys():
             raise KeyError("No 'aggregations' have been selected, please set it up and re-try.")
 
         if "agg_method" not in json_data["aggregations"].keys():
             raise KeyError("No 'Aggregation Method' have been selected, please set it up and re-try.")
+        if json_data["aggregations"]["agg_method"] not in self.list_agg_methods():
+            raise KeyError(f'unsupported agg_method {json_data["aggregations"]["agg_method"]}.')
         self.aggregation = json_data["aggregations"]["agg_method"]
 
         if "interval" not in json_data["aggregations"].keys():
             raise KeyError("No 'Aggregation Interval' have been selected, please set it up and re-try.")
         self.interval = int(json_data["aggregations"]["interval"] / 1000)
 
         if "filters" in json_data.keys():
```

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/script.py` & `wizata-dsapi-0.2.2/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/template.py` & `wizata-dsapi-0.2.2/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/twin.py` & `wizata-dsapi-0.2.2/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.2.2/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.2.2/wizata_dsapi/wizata_dsapi_client.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.2.2/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.1/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.2.2/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

