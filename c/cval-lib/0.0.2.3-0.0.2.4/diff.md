# Comparing `tmp/cval-lib-0.0.2.3.tar.gz` & `tmp/cval-lib-0.0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cval-lib-0.0.2.3.tar", last modified: Tue Jul  4 09:06:41 2023, max compression
+gzip compressed data, was "cval-lib-0.0.2.4.tar", last modified: Thu Jul  6 15:54:11 2023, max compression
```

## Comparing `cval-lib-0.0.2.3.tar` & `cval-lib-0.0.2.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-04 09:06:41.012082 cval-lib-0.0.2.3/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)    11357 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/LICENSE
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-04 09:06:41.012082 cval-lib-0.0.2.3/PKG-INFO
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5555 2023-07-02 18:44:46.000000 cval-lib-0.0.2.3/README.md
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-04 09:06:41.008082 cval-lib-0.0.2.3/cval_lib/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:05:48.000000 cval-lib-0.0.2.3/cval_lib/__init__.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-04 09:06:41.008082 cval-lib-0.0.2.3/cval_lib/configs/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/configs/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      137 2023-07-02 13:22:21.000000 cval-lib-0.0.2.3/cval_lib/configs/main_config.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1428 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/connection.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-04 09:06:41.008082 cval-lib-0.0.2.3/cval_lib/examples/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/examples/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1685 2023-07-02 18:45:46.000000 cval-lib-0.0.2.3/cval_lib/examples/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      820 2023-07-02 18:35:48.000000 cval-lib-0.0.2.3/cval_lib/examples/embeddings.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1313 2023-07-02 18:34:57.000000 cval-lib-0.0.2.3/cval_lib/examples/monkey_patch.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2012 2023-07-02 18:34:57.000000 cval-lib-0.0.2.3/cval_lib/examples/on_pemise.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1306 2023-07-02 18:45:46.000000 cval-lib-0.0.2.3/cval_lib/examples/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-04 09:06:41.008082 cval-lib-0.0.2.3/cval_lib/handlers/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1260 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/handlers/__async.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/handlers/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2898 2023-07-02 19:12:34.000000 cval-lib-0.0.2.3/cval_lib/handlers/_abstract_handler.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5155 2023-07-02 18:28:19.000000 cval-lib-0.0.2.3/cval_lib/handlers/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1884 2023-07-04 09:05:59.000000 cval-lib-0.0.2.3/cval_lib/handlers/detection.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5250 2023-07-02 18:30:35.000000 cval-lib-0.0.2.3/cval_lib/handlers/embedding.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      946 2023-07-02 19:17:24.000000 cval-lib-0.0.2.3/cval_lib/handlers/frame.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2487 2023-07-04 09:05:59.000000 cval-lib-0.0.2.3/cval_lib/handlers/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-04 09:06:41.012082 cval-lib-0.0.2.3/cval_lib/models/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/models/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1914 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/models/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     3040 2023-07-02 14:57:53.000000 cval-lib-0.0.2.3/cval_lib/models/detection.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1404 2023-07-02 18:41:52.000000 cval-lib-0.0.2.3/cval_lib/models/embedding.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2214 2023-07-02 18:22:01.000000 cval-lib-0.0.2.3/cval_lib/models/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-04 09:06:41.012082 cval-lib-0.0.2.3/cval_lib/patterns/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/patterns/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      240 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/patterns/singleton.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-04 09:06:41.012082 cval-lib-0.0.2.3/cval_lib.egg-info/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-04 09:06:40.000000 cval-lib-0.0.2.3/cval_lib.egg-info/PKG-INFO
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1022 2023-07-04 09:06:40.000000 cval-lib-0.0.2.3/cval_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        1 2023-07-04 09:06:40.000000 cval-lib-0.0.2.3/cval_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)       18 2023-07-04 09:06:40.000000 cval-lib-0.0.2.3/cval_lib.egg-info/requires.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        9 2023-07-04 09:06:40.000000 cval-lib-0.0.2.3/cval_lib.egg-info/top_level.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)       38 2023-07-04 09:06:41.012082 cval-lib-0.0.2.3/setup.cfg
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      446 2023-07-04 09:06:30.000000 cval-lib-0.0.2.3/setup.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-06 15:54:11.402924 cval-lib-0.0.2.4/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)    11357 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/LICENSE
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-06 15:54:11.402924 cval-lib-0.0.2.4/PKG-INFO
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5622 2023-07-06 15:50:50.000000 cval-lib-0.0.2.4/README.md
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-06 15:54:11.390924 cval-lib-0.0.2.4/cval_lib/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:05:48.000000 cval-lib-0.0.2.4/cval_lib/__init__.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-06 15:54:11.390924 cval-lib-0.0.2.4/cval_lib/configs/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/configs/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      137 2023-07-02 13:22:21.000000 cval-lib-0.0.2.4/cval_lib/configs/main_config.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1428 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/connection.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-06 15:54:11.394924 cval-lib-0.0.2.4/cval_lib/examples/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/examples/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1689 2023-07-06 06:27:41.000000 cval-lib-0.0.2.4/cval_lib/examples/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      820 2023-07-02 18:35:48.000000 cval-lib-0.0.2.4/cval_lib/examples/embeddings.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1313 2023-07-02 18:34:57.000000 cval-lib-0.0.2.4/cval_lib/examples/monkey_patch.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2012 2023-07-02 18:34:57.000000 cval-lib-0.0.2.4/cval_lib/examples/on_pemise.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1306 2023-07-02 18:45:46.000000 cval-lib-0.0.2.4/cval_lib/examples/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-06 15:54:11.398924 cval-lib-0.0.2.4/cval_lib/handlers/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1260 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/handlers/__async.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/handlers/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2521 2023-07-06 15:50:50.000000 cval-lib-0.0.2.4/cval_lib/handlers/_abstract_handler.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5076 2023-07-06 06:28:17.000000 cval-lib-0.0.2.4/cval_lib/handlers/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1884 2023-07-04 09:05:59.000000 cval-lib-0.0.2.4/cval_lib/handlers/detection.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5250 2023-07-02 18:30:35.000000 cval-lib-0.0.2.4/cval_lib/handlers/embedding.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      946 2023-07-02 19:17:24.000000 cval-lib-0.0.2.4/cval_lib/handlers/frame.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2487 2023-07-04 09:05:59.000000 cval-lib-0.0.2.4/cval_lib/handlers/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-06 15:54:11.398924 cval-lib-0.0.2.4/cval_lib/models/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/models/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1914 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/models/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     3014 2023-07-06 15:53:23.000000 cval-lib-0.0.2.4/cval_lib/models/detection.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1404 2023-07-02 18:41:52.000000 cval-lib-0.0.2.4/cval_lib/models/embedding.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2214 2023-07-02 18:22:01.000000 cval-lib-0.0.2.4/cval_lib/models/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-06 15:54:11.402924 cval-lib-0.0.2.4/cval_lib/patterns/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/patterns/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      240 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/patterns/singleton.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-06 15:54:11.402924 cval-lib-0.0.2.4/cval_lib.egg-info/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-06 15:54:11.000000 cval-lib-0.0.2.4/cval_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1022 2023-07-06 15:54:11.000000 cval-lib-0.0.2.4/cval_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        1 2023-07-06 15:54:11.000000 cval-lib-0.0.2.4/cval_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)       18 2023-07-06 15:54:11.000000 cval-lib-0.0.2.4/cval_lib.egg-info/requires.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        9 2023-07-06 15:54:11.000000 cval-lib-0.0.2.4/cval_lib.egg-info/top_level.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)       38 2023-07-06 15:54:11.402924 cval-lib-0.0.2.4/setup.cfg
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      446 2023-07-06 15:53:54.000000 cval-lib-0.0.2.4/setup.py
```

### Comparing `cval-lib-0.0.2.3/LICENSE` & `cval-lib-0.0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.3/README.md` & `cval-lib-0.0.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -145,21 +145,22 @@
 ```python3
 import random
 import uuid
 from cval_lib.models.detection import BBoxScores, FramePrediction
 
 # :NOTE: example only
 frames_predictions = list(
-  map(
-  lambda x: FramePrediction(
-  frame_id=str(uuid.uuid4()), 
-  predictions=list(map(lambda x: BBoxScores(category_id=str(uuid.uuid4()), random.random()), range(100)))
-  ), 
-  range(100)
- )
+    map(
+        lambda x: FramePrediction(
+            frame_id=str(uuid.uuid4().hex),
+            predictions=list(
+                map(lambda x: BBoxScores(category_id=str(uuid.uuid4()), score=random.random()), range(100)))
+        ),
+        range(10)
+    )
 )
 
 print(frames_predictions)
 
 
 ```
```

#### html2text {}

```diff
@@ -50,21 +50,21 @@
 ImageEmbeddingModel(id=img_id_2, image_embedding=list(map(lambda x: random(),
 range(1000)))), ] print(embeddings) ``` ##### Upload & check embeddings
 ```python3 emb = cval.embedding(ds_id, 'training') emb.upload_many(embeddings)
 print(emb.get_many()) ``` > The following example is used to invoke active
 learning ### Active learning ##### Get predictions data ```python3 import
 random import uuid from cval_lib.models.detection import BBoxScores,
 FramePrediction # :NOTE: example only frames_predictions = list( map( lambda x:
-FramePrediction( frame_id=str(uuid.uuid4()), predictions=list(map(lambda x:
-BBoxScores(category_id=str(uuid.uuid4()), random.random()), range(100))) ),
-range(100) ) ) print(frames_predictions) ``` ##### Construct config ```python3
-from cval_lib.models.detection import DetectionSamplingOnPremise request =
-DetectionSamplingOnPremise( num_of_samples=200, bbox_selection_policy='min',
-selection_strategy='margin', sort_strategy='ascending',
-frames=frames_predictions, ) ``` ##### Run active learning ```python3 emb =
-cval.detection() print(emd.on_premise_sampling(response_model)) ``` > The
-following method is most relevant when we are dealing with long-term tasks and,
-accordingly, with asynchronous interaction. ##### Polling > refers to actively
-sampling the status of an external device by a client program as a synchronous
-activity. ```python3 from time import sleep result = None sleep_sec = 1 while
-result is None: result = emb.result.get_result() sleep(sleep_sec) sleep_sec *=
-2 print(result) ```
+FramePrediction( frame_id=str(uuid.uuid4().hex), predictions=list( map(lambda
+x: BBoxScores(category_id=str(uuid.uuid4()), score=random.random()), range
+(100))) ), range(10) ) ) print(frames_predictions) ``` ##### Construct config
+```python3 from cval_lib.models.detection import DetectionSamplingOnPremise
+request = DetectionSamplingOnPremise( num_of_samples=200,
+bbox_selection_policy='min', selection_strategy='margin',
+sort_strategy='ascending', frames=frames_predictions, ) ``` ##### Run active
+learning ```python3 emb = cval.detection() print(emd.on_premise_sampling
+(response_model)) ``` > The following method is most relevant when we are
+dealing with long-term tasks and, accordingly, with asynchronous interaction.
+##### Polling > refers to actively sampling the status of an external device by
+a client program as a synchronous activity. ```python3 from time import sleep
+result = None sleep_sec = 1 while result is None: result =
+emb.result.get_result() sleep(sleep_sec) sleep_sec *= 2 print(result) ```
```

### Comparing `cval-lib-0.0.2.3/cval_lib/connection.py` & `cval-lib-0.0.2.4/cval_lib/connection.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.3/cval_lib/examples/dataset.py` & `cval-lib-0.0.2.4/cval_lib/examples/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     # choose strategy
     ds = cval.dataset()
     # create your dataset
     ds_id = ds.create()
     print(ds_id)
     # update your dataset
     update = ds.update(name='any')
-    print(update)
+    print('', update)
     # watch changes
     get = ds.get()
     print(get)
     # also you can use dataset_id for watch changes
     get = ds.get(ds_id)
     print(get)
     # get all datasets
```

### Comparing `cval-lib-0.0.2.3/cval_lib/examples/embeddings.py` & `cval-lib-0.0.2.4/cval_lib/examples/embeddings.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.3/cval_lib/examples/monkey_patch.py` & `cval-lib-0.0.2.4/cval_lib/examples/monkey_patch.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.3/cval_lib/examples/on_pemise.py` & `cval-lib-0.0.2.4/cval_lib/examples/on_pemise.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.3/cval_lib/examples/result.py` & `cval-lib-0.0.2.4/cval_lib/examples/result.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.3/cval_lib/handlers/__async.py` & `cval-lib-0.0.2.4/cval_lib/handlers/__async.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.3/cval_lib/handlers/_abstract_handler.py` & `cval-lib-0.0.2.4/cval_lib/handlers/_abstract_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,23 +55,13 @@
     def _put(self, url: str, json=None, params=None, stream=False, **files):
         self._post(url, json, params, stream=stream, **files)
         self.method = 'put'
 
     @staticmethod
     def validate_response(resp: Response):
         if resp.status_code >= 400:
-            match resp.status_code:
-                case 422:
-                    raise ValueError(resp.json())
-                case 403:
-                    raise PermissionError(resp.json())
-                case 409:
-                    raise ValueError(resp.json())
-                case 400:
-                    raise ValueError(resp.json())
-                case _:
-                    raise Exception(resp.json() if resp.status_code != 500 else 'Internal Server Error :(')
+            raise Exception(resp.json() if resp.status_code != 500 else 'Internal Server Error :(')
 
     def send(self):
         resp = self.session.send(self.prepare())
         self.validate_response(resp)
         return resp
```

### Comparing `cval-lib-0.0.2.3/cval_lib/handlers/dataset.py` & `cval-lib-0.0.2.4/cval_lib/handlers/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,28 +30,28 @@
 class Dataset(AbstractHandler):
     """
     Within the framework of the created system,
     datasets are spaces in which data for machine learning is stored.
     Creating a dataset is similar to creating a folder.
     """
     def __init__(self, session: Session):
-        self.dataset_request = DatasetModel
+        self.dataset_request = DatasetModel()
         self.route = f'{MainConfig().main_url}/dataset'
         self.dataset_id = None
         self.result = Result(session)
         self._embedding = Embedding(session, _is_not_second=False)
         self.embedding = self._embedding.monkey_patch_url
         self.detection = Detection(session)
         super().__init__(session)
 
     def __repr__(self):
         return f'<dataset {self.dataset_id}>'
 
     def _construct_request(self, name: str, description: str):
-        self.dataset_request = DatasetModel
+        self.dataset_request = DatasetModel()
         if name is not None:
             self.dataset_request.dataset_name = name
         if description is not None:
             self.dataset_request.dataset_description = description
 
     def create(
             self,
@@ -61,15 +61,15 @@
         """
         this method creates a dataset
         :param name: the name of dataset
         :param description: the name of dataset
         :return: id of dataset (dataset_id)
         """
         self._construct_request(name, description)
-        self._post(url=self.route, json=self.dataset_request().dict())
+        self._post(url=self.route, json=self.dataset_request.dict())
         self.dataset_id = self.send().json().get('dataset_id')
         self._embedding.dataset_id = self.dataset_id
         return self.dataset_id
 
     def update(
             self,
             dataset_id: str = None,
@@ -81,17 +81,16 @@
         :param dataset_id: id of dataset
         :param name: the name of dataset
         :param description: the description of dataset
         :return: DatasetResponse model with updates
         """
         dataset_id = self.set_dataset_id(dataset_id)
         self._construct_request(name, description)
-        self.dataset_request.dataset_id = dataset_id
-        self._put(url=self.route+f'/{dataset_id}', json=self.dataset_request().dict(), )
-        self.dataset_request = DatasetModel.parse_obj(self.send().json())
+        self._put(url=self.route+f'/{dataset_id}', json=self.dataset_request.dict(), )
+        self.dataset_request = self.send().json()
         return self.dataset_request
 
     def set_dataset_id(self, dataset_id: str = None):
         if dataset_id is None:
             dataset_id = self.dataset_id
         self.dataset_id = dataset_id
         if self.dataset_id is None:
@@ -120,9 +119,9 @@
         """
         this method returns a dataset name and description by dataset_id
         :param name: the name of dataset. regexp
         :param description: the description of dataset. regexp
         :return: DatasetResponse model with updates
         """
         self._construct_request(name, description)
-        self._get(url=self.route+'s/all', params=self.dataset_request().dict())
+        self._get(url=self.route+'s/all', params=self.dataset_request.dict())
         return [DatasetResponse.parse_obj(i) for i in self.send().json()]
```

### Comparing `cval-lib-0.0.2.3/cval_lib/handlers/detection.py` & `cval-lib-0.0.2.4/cval_lib/handlers/detection.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.3/cval_lib/handlers/embedding.py` & `cval-lib-0.0.2.4/cval_lib/handlers/embedding.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.3/cval_lib/handlers/frame.py` & `cval-lib-0.0.2.4/cval_lib/handlers/frame.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.3/cval_lib/handlers/result.py` & `cval-lib-0.0.2.4/cval_lib/handlers/result.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.3/cval_lib/models/dataset.py` & `cval-lib-0.0.2.4/cval_lib/models/dataset.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.3/cval_lib/models/detection.py` & `cval-lib-0.0.2.4/cval_lib/models/detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     :type frames: List[FramePrediction]
     :raises ValueError if value not in allowed
     """
     num_of_samples: int
     bbox_selection_policy: str
     selection_strategy: str
     sort_strategy: str
-    frames: List[FramePrediction] = Field(max_items=10_000)
+    frames: List[FramePrediction]
 
     @validator('bbox_selection_policy')
     def validate_bbox_selection_policy(cls, value):
         allowed = ['min', 'max', 'sum', 'mean']
         if value not in allowed:
             raise ValueError(f"allowed bbox_selection_policy = {allowed}")
         return value
```

### Comparing `cval-lib-0.0.2.3/cval_lib/models/embedding.py` & `cval-lib-0.0.2.4/cval_lib/models/embedding.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.3/cval_lib/models/result.py` & `cval-lib-0.0.2.4/cval_lib/models/result.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.3/cval_lib.egg-info/SOURCES.txt` & `cval-lib-0.0.2.4/cval_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

