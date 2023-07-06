# Comparing `tmp/DetaMetrics-0.0.6.tar.gz` & `tmp/DetaMetrics-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DetaMetrics-0.0.6.tar", last modified: Thu Jul  6 12:58:43 2023, max compression
+gzip compressed data, was "DetaMetrics-0.0.7.tar", last modified: Thu Jul  6 13:15:29 2023, max compression
```

## Comparing `DetaMetrics-0.0.6.tar` & `DetaMetrics-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 12:58:43.349221 DetaMetrics-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-07-06 12:58:43.317805 DetaMetrics-0.0.6/DetaMetrics.egg-info/
--rw-rw-rw-   0        0        0     1801 2023-07-06 12:58:43.000000 DetaMetrics-0.0.6/DetaMetrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-06 12:58:43.000000 DetaMetrics-0.0.6/DetaMetrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 12:58:43.000000 DetaMetrics-0.0.6/DetaMetrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-06 12:58:43.000000 DetaMetrics-0.0.6/DetaMetrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-06 12:58:43.000000 DetaMetrics-0.0.6/DetaMetrics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1075 2023-06-30 12:12:35.000000 DetaMetrics-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1801 2023-07-06 12:58:43.345186 DetaMetrics-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1423 2023-07-06 12:57:05.000000 DetaMetrics-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 12:58:43.326337 DetaMetrics-0.0.6/detametrics/
--rw-rw-rw-   0        0        0       28 2023-06-30 12:00:58.000000 DetaMetrics-0.0.6/detametrics/__init__.py
--rw-rw-rw-   0        0        0      781 2023-07-01 09:58:35.000000 DetaMetrics-0.0.6/detametrics/sdk.py
--rw-rw-rw-   0        0        0     1444 2023-07-06 12:56:52.000000 DetaMetrics-0.0.6/detametrics/tf.py
--rw-rw-rw-   0        0        0      497 2023-07-06 12:58:23.000000 DetaMetrics-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 12:58:43.349221 DetaMetrics-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 13:15:29.488563 DetaMetrics-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-07-06 13:15:29.479565 DetaMetrics-0.0.7/DetaMetrics.egg-info/
+-rw-rw-rw-   0        0        0     1801 2023-07-06 13:15:29.000000 DetaMetrics-0.0.7/DetaMetrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-06 13:15:29.000000 DetaMetrics-0.0.7/DetaMetrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 13:15:29.000000 DetaMetrics-0.0.7/DetaMetrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-06 13:15:29.000000 DetaMetrics-0.0.7/DetaMetrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-06 13:15:29.000000 DetaMetrics-0.0.7/DetaMetrics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1075 2023-06-30 12:12:35.000000 DetaMetrics-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1801 2023-07-06 13:15:29.486565 DetaMetrics-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1423 2023-07-06 12:57:05.000000 DetaMetrics-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 13:15:29.485567 DetaMetrics-0.0.7/detametrics/
+-rw-rw-rw-   0        0        0       28 2023-06-30 12:00:58.000000 DetaMetrics-0.0.7/detametrics/__init__.py
+-rw-rw-rw-   0        0        0      781 2023-07-01 09:58:35.000000 DetaMetrics-0.0.7/detametrics/sdk.py
+-rw-rw-rw-   0        0        0     1449 2023-07-06 13:14:20.000000 DetaMetrics-0.0.7/detametrics/tf.py
+-rw-rw-rw-   0        0        0      497 2023-07-06 13:14:37.000000 DetaMetrics-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 13:15:29.488563 DetaMetrics-0.0.7/setup.cfg
```

### Comparing `DetaMetrics-0.0.6/DetaMetrics.egg-info/PKG-INFO` & `DetaMetrics-0.0.7/DetaMetrics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DetaMetrics
-Version: 0.0.6
+Version: 0.0.7
 Summary: SDK for DetaMetrics TensorBoard alternative.
 Author: SamTheProgrammer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `DetaMetrics-0.0.6/LICENSE` & `DetaMetrics-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `DetaMetrics-0.0.6/PKG-INFO` & `DetaMetrics-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DetaMetrics
-Version: 0.0.6
+Version: 0.0.7
 Summary: SDK for DetaMetrics TensorBoard alternative.
 Author: SamTheProgrammer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `DetaMetrics-0.0.6/README.md` & `DetaMetrics-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `DetaMetrics-0.0.6/detametrics/sdk.py` & `DetaMetrics-0.0.7/detametrics/sdk.py`

 * *Files identical despite different names*

### Comparing `DetaMetrics-0.0.6/detametrics/tf.py` & `DetaMetrics-0.0.7/detametrics/tf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import tensorflow as tf
 import multiprocessing as mp
 from .sdk import DetaMetrics
 
+def background(queue: mp.Queue, backend: DetaMetrics):
+    while True:
+        metric, value, mode = queue.get()
+        backend.set(metric, mode, value)
+
 class DetaMetricsTFCallback(tf.keras.callbacks.Callback):
     def __init__(self, urlId: str, apiKey: str, log_batch: bool=False) -> None:
         self.__deta_backend = DetaMetrics(urlId, apiKey)
         self.__log_batch = log_batch
     
     def on_train_begin(self, logs=None):
         self.__queue = mp.Queue()
-        self.__process = mp.Process(target=self.__background, args=(self.__queue,))
+        self.__process = mp.Process(target=background, args=(self.__queue, self.__deta_backend))
         self.__process.start()
     
     def on_train_end(self, logs=None):
         self.__process.terminate()
         self.__process.join()
-
-    def __background(self):
-        while True:
-            metric, value, mode = self.__queue.get()
-            self.__deta_backend.set(metric, mode, value)
     
     def on_train_batch_end(self, batch, logs=None):
         if self.__log_batch:
             for metric, value in logs.items():
                 if metric.startswith("val_"):
                     self.__queue.put((metric[4:], value, "Validation"))
                 else:
                     self.__queue.put((metric, value, "Training"))
 
     def on_epoch_end(self, epoch, logs=None):
         for metric, value in logs.items():
             if metric.startswith("val_"):
-                self.__deta_backend.set(metric[4:], "Validation", value)
+                self.__queue.put((metric[4:], value, "Validation"))
             else:
-                self.__deta_backend.set(metric, "Training", value)
+                self.__queue.put((metric[4:], value, "Validation"))
```

