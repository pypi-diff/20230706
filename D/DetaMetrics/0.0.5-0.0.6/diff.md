# Comparing `tmp/DetaMetrics-0.0.5.tar.gz` & `tmp/DetaMetrics-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DetaMetrics-0.0.5.tar", last modified: Sat Jul  1 10:12:52 2023, max compression
+gzip compressed data, was "DetaMetrics-0.0.6.tar", last modified: Thu Jul  6 12:58:43 2023, max compression
```

## Comparing `DetaMetrics-0.0.5.tar` & `DetaMetrics-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 10:12:52.219591 DetaMetrics-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-07-01 10:12:52.209479 DetaMetrics-0.0.5/DetaMetrics.egg-info/
--rw-rw-rw-   0        0        0     1301 2023-07-01 10:12:52.000000 DetaMetrics-0.0.5/DetaMetrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-01 10:12:52.000000 DetaMetrics-0.0.5/DetaMetrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 10:12:52.000000 DetaMetrics-0.0.5/DetaMetrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-01 10:12:52.000000 DetaMetrics-0.0.5/DetaMetrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-01 10:12:52.000000 DetaMetrics-0.0.5/DetaMetrics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1075 2023-06-30 12:12:35.000000 DetaMetrics-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1301 2023-07-01 10:12:52.218579 DetaMetrics-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      923 2023-06-30 14:06:48.000000 DetaMetrics-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 10:12:52.216478 DetaMetrics-0.0.5/detametrics/
--rw-rw-rw-   0        0        0       28 2023-06-30 12:00:58.000000 DetaMetrics-0.0.5/detametrics/__init__.py
--rw-rw-rw-   0        0        0      781 2023-07-01 09:58:35.000000 DetaMetrics-0.0.5/detametrics/sdk.py
--rw-rw-rw-   0        0        0      523 2023-07-01 10:12:27.000000 DetaMetrics-0.0.5/detametrics/tf.py
--rw-rw-rw-   0        0        0      497 2023-07-01 10:12:36.000000 DetaMetrics-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 10:12:52.219591 DetaMetrics-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 12:58:43.349221 DetaMetrics-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-07-06 12:58:43.317805 DetaMetrics-0.0.6/DetaMetrics.egg-info/
+-rw-rw-rw-   0        0        0     1801 2023-07-06 12:58:43.000000 DetaMetrics-0.0.6/DetaMetrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-06 12:58:43.000000 DetaMetrics-0.0.6/DetaMetrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 12:58:43.000000 DetaMetrics-0.0.6/DetaMetrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-06 12:58:43.000000 DetaMetrics-0.0.6/DetaMetrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-06 12:58:43.000000 DetaMetrics-0.0.6/DetaMetrics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1075 2023-06-30 12:12:35.000000 DetaMetrics-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1801 2023-07-06 12:58:43.345186 DetaMetrics-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1423 2023-07-06 12:57:05.000000 DetaMetrics-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 12:58:43.326337 DetaMetrics-0.0.6/detametrics/
+-rw-rw-rw-   0        0        0       28 2023-06-30 12:00:58.000000 DetaMetrics-0.0.6/detametrics/__init__.py
+-rw-rw-rw-   0        0        0      781 2023-07-01 09:58:35.000000 DetaMetrics-0.0.6/detametrics/sdk.py
+-rw-rw-rw-   0        0        0     1444 2023-07-06 12:56:52.000000 DetaMetrics-0.0.6/detametrics/tf.py
+-rw-rw-rw-   0        0        0      497 2023-07-06 12:58:23.000000 DetaMetrics-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 12:58:43.349221 DetaMetrics-0.0.6/setup.cfg
```

### Comparing `DetaMetrics-0.0.5/DetaMetrics.egg-info/PKG-INFO` & `DetaMetrics-0.0.6/DetaMetrics.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,66 @@
 Metadata-Version: 2.1
 Name: DetaMetrics
-Version: 0.0.5
+Version: 0.0.6
 Summary: SDK for DetaMetrics TensorBoard alternative.
 Author: SamTheProgrammer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DetaMetricsSDK
 
 A Python SDK for interacting with my TensorBoard alternative that runs on [Deta Space](https://deta.space).
 
+- [DetaMetricsSDK](#detametricssdk)
+  - [Installation](#installation)
+  - [Usage](#usage)
+    - [TensorFlow Callback](#tensorflow-callback)
+    - [Base API](#base-api)
+
+---
+
 ## Installation
 
 ```powershell
 pip install detametrics
 ```
 
 ## Usage
 
+> All API classes need an URL ID, which can be gotten from the app UI.
+
+> They also need a Deta Space App API key, which can be gotten from...
+> - Click the 3 dots on the app on your Deta Space Canvas
+> - Click **"Keys"**
+> - Add an API Key, and input it in the box on the App UI and in your Python code as seen below
+
 ### TensorFlow Callback
 Requires Tensorflow to be installed.
 
 ```python
 from detametrics.tf import DetaMetricsTFCallback
 
 # use in your keras model
 model = ...
 model.fit(
   ..., # other params here
-  callbacks=[DetaMetricsTFCallback("MY_URL_ID")]
+  callbacks=[DetaMetricsTFCallback("MY_URL_ID", "MY_API_KEY")]
 )
 ```
 
 ### Base API
 Get your URL id from the UI on the [Deta Space app](https://deta.space/discovery/@sam-the-programmer/detametrics).
 
 ```python
 from detametrics import DetaMetrics
 
-metrics = DetaMetrics("MY_URL_ID") # get it from the Deta Space App UI
+metrics = DetaMetrics("MY_URL_ID", "MY_API_KEY")
 metrics.clear() # WARNING: clears all past metrics
 
 metrics.set("GraphName", "LineName", 0.1)
 metrics.set("GraphName", "LineName", 123.45)
 metrics.set("GraphName", "LineName", 78.9)
 ```
```

### Comparing `DetaMetrics-0.0.5/LICENSE` & `DetaMetrics-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `DetaMetrics-0.0.5/PKG-INFO` & `DetaMetrics-0.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,66 @@
 Metadata-Version: 2.1
 Name: DetaMetrics
-Version: 0.0.5
+Version: 0.0.6
 Summary: SDK for DetaMetrics TensorBoard alternative.
 Author: SamTheProgrammer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DetaMetricsSDK
 
 A Python SDK for interacting with my TensorBoard alternative that runs on [Deta Space](https://deta.space).
 
+- [DetaMetricsSDK](#detametricssdk)
+  - [Installation](#installation)
+  - [Usage](#usage)
+    - [TensorFlow Callback](#tensorflow-callback)
+    - [Base API](#base-api)
+
+---
+
 ## Installation
 
 ```powershell
 pip install detametrics
 ```
 
 ## Usage
 
+> All API classes need an URL ID, which can be gotten from the app UI.
+
+> They also need a Deta Space App API key, which can be gotten from...
+> - Click the 3 dots on the app on your Deta Space Canvas
+> - Click **"Keys"**
+> - Add an API Key, and input it in the box on the App UI and in your Python code as seen below
+
 ### TensorFlow Callback
 Requires Tensorflow to be installed.
 
 ```python
 from detametrics.tf import DetaMetricsTFCallback
 
 # use in your keras model
 model = ...
 model.fit(
   ..., # other params here
-  callbacks=[DetaMetricsTFCallback("MY_URL_ID")]
+  callbacks=[DetaMetricsTFCallback("MY_URL_ID", "MY_API_KEY")]
 )
 ```
 
 ### Base API
 Get your URL id from the UI on the [Deta Space app](https://deta.space/discovery/@sam-the-programmer/detametrics).
 
 ```python
 from detametrics import DetaMetrics
 
-metrics = DetaMetrics("MY_URL_ID") # get it from the Deta Space App UI
+metrics = DetaMetrics("MY_URL_ID", "MY_API_KEY")
 metrics.clear() # WARNING: clears all past metrics
 
 metrics.set("GraphName", "LineName", 0.1)
 metrics.set("GraphName", "LineName", 123.45)
 metrics.set("GraphName", "LineName", 78.9)
 ```
```

### Comparing `DetaMetrics-0.0.5/README.md` & `DetaMetrics-0.0.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,54 @@
 # DetaMetricsSDK
 
 A Python SDK for interacting with my TensorBoard alternative that runs on [Deta Space](https://deta.space).
 
+- [DetaMetricsSDK](#detametricssdk)
+  - [Installation](#installation)
+  - [Usage](#usage)
+    - [TensorFlow Callback](#tensorflow-callback)
+    - [Base API](#base-api)
+
+---
+
 ## Installation
 
 ```powershell
 pip install detametrics
 ```
 
 ## Usage
 
+> All API classes need an URL ID, which can be gotten from the app UI.
+
+> They also need a Deta Space App API key, which can be gotten from...
+> - Click the 3 dots on the app on your Deta Space Canvas
+> - Click **"Keys"**
+> - Add an API Key, and input it in the box on the App UI and in your Python code as seen below
+
 ### TensorFlow Callback
 Requires Tensorflow to be installed.
 
 ```python
 from detametrics.tf import DetaMetricsTFCallback
 
 # use in your keras model
 model = ...
 model.fit(
   ..., # other params here
-  callbacks=[DetaMetricsTFCallback("MY_URL_ID")]
+  callbacks=[DetaMetricsTFCallback("MY_URL_ID", "MY_API_KEY")]
 )
 ```
 
 ### Base API
 Get your URL id from the UI on the [Deta Space app](https://deta.space/discovery/@sam-the-programmer/detametrics).
 
 ```python
 from detametrics import DetaMetrics
 
-metrics = DetaMetrics("MY_URL_ID") # get it from the Deta Space App UI
+metrics = DetaMetrics("MY_URL_ID", "MY_API_KEY")
 metrics.clear() # WARNING: clears all past metrics
 
 metrics.set("GraphName", "LineName", 0.1)
 metrics.set("GraphName", "LineName", 123.45)
 metrics.set("GraphName", "LineName", 78.9)
 ```
```

### Comparing `DetaMetrics-0.0.5/detametrics/sdk.py` & `DetaMetrics-0.0.6/detametrics/sdk.py`

 * *Files identical despite different names*

