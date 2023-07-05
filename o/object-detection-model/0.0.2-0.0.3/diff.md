# Comparing `tmp/object_detection_model-0.0.2-py3-none-any.whl.zip` & `tmp/object_detection_model-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3461 bytes, number of entries: 7
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-05 20:59 object_detection_model/__init__.py
--rw-r--r--  2.0 unx     2105 b- defN 23-Jul-05 20:59 object_detection_model/model.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Jul-05 21:02 object_detection_model-0.0.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      493 b- defN 23-Jul-05 21:02 object_detection_model-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-05 21:02 object_detection_model-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       23 b- defN 23-Jul-05 21:02 object_detection_model-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      641 b- defN 23-Jul-05 21:02 object_detection_model-0.0.2.dist-info/RECORD
-7 files, 4449 bytes uncompressed, 2301 bytes compressed:  48.3%
+Zip file size: 3463 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-05 22:20 object_detection_model/__init__.py
+-rw-r--r--  2.0 unx     2130 b- defN 23-Jul-05 22:20 object_detection_model/model.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jul-05 22:24 object_detection_model-0.0.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      528 b- defN 23-Jul-05 22:24 object_detection_model-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-05 22:24 object_detection_model-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       23 b- defN 23-Jul-05 22:24 object_detection_model-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      641 b- defN 23-Jul-05 22:24 object_detection_model-0.0.3.dist-info/RECORD
+7 files, 4509 bytes uncompressed, 2303 bytes compressed:  48.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: object_detection_model/__init__.py
 Comment: 
 
 Filename: object_detection_model/model.py
 Comment: 
 
-Filename: object_detection_model-0.0.2.dist-info/LICENSE.txt
+Filename: object_detection_model-0.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: object_detection_model-0.0.2.dist-info/METADATA
+Filename: object_detection_model-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: object_detection_model-0.0.2.dist-info/WHEEL
+Filename: object_detection_model-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: object_detection_model-0.0.2.dist-info/top_level.txt
+Filename: object_detection_model-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: object_detection_model-0.0.2.dist-info/RECORD
+Filename: object_detection_model-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## object_detection_model/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

## object_detection_model/model.py

```diff
@@ -6,20 +6,19 @@
 import matplotlib.pyplot as plt
 from numpy.typing import ArrayLike
 
 matplotlib.use("Agg")  # Solves some error
 
 
 class ModelConfig:
-    config_file_path: str = (
-        "object_detection/ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt"
+    config_file_path: str = "object_detection_model/object_detection/ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt"
+    frozen_model_path: str = (
+        "object_detection_model/object_detection/frozen_inference_graph.pb"
     )
-    frozen_model_path: str = "object_detection/frozen_inference_graph.pb"
-    labels_path: str = "object_detection/coco.names"
-    output_filename: str = "prediction.png"
+    labels_path: str = "object_detection_model/object_detection/coco.names"
 
 
 @dataclass
 class Model:
     config: ModelConfig
 
     def __init__(self, config: ModelConfig):
```

## Comparing `object_detection_model-0.0.2.dist-info/LICENSE.txt` & `object_detection_model-0.0.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `object_detection_model-0.0.2.dist-info/RECORD` & `object_detection_model-0.0.3.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-object_detection_model/__init__.py,sha256=QvlVh4JTl3JL7jQAja76yKtT-IvF4631ASjWY1wS6AQ,22
-object_detection_model/model.py,sha256=sHCVRWP0a_Fka-joCVjhpjZArWa_1rR7OSRn4s9J9MM,2105
-object_detection_model-0.0.2.dist-info/LICENSE.txt,sha256=BzhLY9Bs5tjH9RiNLyNZ4UqGs0RW-cZdvRSMTZuP_GM,1073
-object_detection_model-0.0.2.dist-info/METADATA,sha256=cgxorsCeErn9p5MKIcoJ1tquFXG3ZuaEl9_JUwmL3QM,493
-object_detection_model-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-object_detection_model-0.0.2.dist-info/top_level.txt,sha256=RnQz6TKnoVu-pc69VtIkVzUH13JhE5TRtzRYOGrXmGY,23
-object_detection_model-0.0.2.dist-info/RECORD,,
+object_detection_model/__init__.py,sha256=4GZKi13lDTD25YBkGakhZyEQZWTER_OWQMNPoH_UM2c,22
+object_detection_model/model.py,sha256=nb-oxpW7vkdt_oopv8sqoTqwU9yYzBh5nKcYXdUhELA,2130
+object_detection_model-0.0.3.dist-info/LICENSE.txt,sha256=BzhLY9Bs5tjH9RiNLyNZ4UqGs0RW-cZdvRSMTZuP_GM,1073
+object_detection_model-0.0.3.dist-info/METADATA,sha256=G6qjtOd-zniRk2DdstQ2Dbd2rDwh3g2cdkiRS4LdfLA,528
+object_detection_model-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+object_detection_model-0.0.3.dist-info/top_level.txt,sha256=RnQz6TKnoVu-pc69VtIkVzUH13JhE5TRtzRYOGrXmGY,23
+object_detection_model-0.0.3.dist-info/RECORD,,
```

