# Comparing `tmp/aquariumlearning-1.0.4.tar.gz` & `tmp/aquariumlearning-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aquariumlearning-1.0.4.tar", last modified: Thu May  4 19:40:12 2023, max compression
+gzip compressed data, was "dist/aquariumlearning-1.0.5.tar", last modified: Thu Jul  6 21:34:17 2023, max compression
```

## Comparing `aquariumlearning-1.0.4.tar` & `aquariumlearning-1.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/
--rw-r--r--   0 robinyang   (501) staff       (20)      642 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/PKG-INFO
--rw-r--r--   0 robinyang   (501) staff       (20)      125 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/README.md
-drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/aquariumlearning/
--rw-r--r--   0 robinyang   (501) staff       (20)     5264 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/__init__.py
--rw-r--r--   0 robinyang   (501) staff       (20)    27894 2023-05-04 19:32:27.000000 aquariumlearning-1.0.4/aquariumlearning/base_labels.py
--rw-r--r--   0 robinyang   (501) staff       (20)    19772 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/class_map.py
--rw-r--r--   0 robinyang   (501) staff       (20)    82456 2023-05-04 19:32:27.000000 aquariumlearning-1.0.4/aquariumlearning/client.py
--rw-r--r--   0 robinyang   (501) staff       (20)    37335 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/collection_client.py
--rw-r--r--   0 robinyang   (501) staff       (20)    13675 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/coordinate_frames.py
--rw-r--r--   0 robinyang   (501) staff       (20)     4221 2023-04-20 18:28:38.000000 aquariumlearning-1.0.4/aquariumlearning/dataset_client.py
--rw-r--r--   0 robinyang   (501) staff       (20)    45024 2023-03-27 18:45:55.000000 aquariumlearning-1.0.4/aquariumlearning/datasets.py
--rw-r--r--   0 robinyang   (501) staff       (20)     4405 2023-03-27 18:45:55.000000 aquariumlearning-1.0.4/aquariumlearning/datasharing.py
--rw-r--r--   0 robinyang   (501) staff       (20)     5319 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/embedding_distance_sampling.py
--rw-r--r--   0 robinyang   (501) staff       (20)    36142 2023-05-04 17:33:24.000000 aquariumlearning-1.0.4/aquariumlearning/frames.py
--rw-r--r--   0 robinyang   (501) staff       (20)    17446 2023-04-24 23:38:39.000000 aquariumlearning-1.0.4/aquariumlearning/inferences.py
--rw-r--r--   0 robinyang   (501) staff       (20)    21566 2023-05-04 19:32:27.000000 aquariumlearning-1.0.4/aquariumlearning/labels.py
--rw-r--r--   0 robinyang   (501) staff       (20)    23775 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/metrics_manager.py
--rw-r--r--   0 robinyang   (501) staff       (20)    17181 2023-04-24 23:38:39.000000 aquariumlearning-1.0.4/aquariumlearning/modified_labels.py
--rw-r--r--   0 robinyang   (501) staff       (20)     1768 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/sampling_agent.py
--rw-r--r--   0 robinyang   (501) staff       (20)    28949 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/segments.py
--rw-r--r--   0 robinyang   (501) staff       (20)    19457 2023-04-10 17:47:19.000000 aquariumlearning-1.0.4/aquariumlearning/sensor_data.py
--rw-r--r--   0 robinyang   (501) staff       (20)     8622 2023-02-08 03:39:31.000000 aquariumlearning-1.0.4/aquariumlearning/turbo.py
--rw-r--r--   0 robinyang   (501) staff       (20)    18412 2023-05-04 19:32:27.000000 aquariumlearning-1.0.4/aquariumlearning/util.py
--rw-r--r--   0 robinyang   (501) staff       (20)     9477 2023-02-08 03:39:31.000000 aquariumlearning-1.0.4/aquariumlearning/viridis.py
--rw-r--r--   0 robinyang   (501) staff       (20)    10213 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/work_queues.py
-drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/aquariumlearning.egg-info/
--rw-r--r--   0 robinyang   (501) staff       (20)      642 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/aquariumlearning.egg-info/PKG-INFO
--rw-r--r--   0 robinyang   (501) staff       (20)      919 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/aquariumlearning.egg-info/SOURCES.txt
--rw-r--r--   0 robinyang   (501) staff       (20)        1 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/aquariumlearning.egg-info/dependency_links.txt
--rw-r--r--   0 robinyang   (501) staff       (20)      349 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/aquariumlearning.egg-info/requires.txt
--rw-r--r--   0 robinyang   (501) staff       (20)       17 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/aquariumlearning.egg-info/top_level.txt
--rw-r--r--   0 robinyang   (501) staff       (20)       38 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/setup.cfg
--rw-r--r--   0 robinyang   (501) staff       (20)     1373 2023-05-04 19:32:56.000000 aquariumlearning-1.0.4/setup.py
+drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-07-06 21:34:17.000000 aquariumlearning-1.0.5/
+-rw-r--r--   0 robinyang   (501) staff       (20)      642 2023-07-06 21:34:17.000000 aquariumlearning-1.0.5/PKG-INFO
+-rw-r--r--   0 robinyang   (501) staff       (20)      125 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/README.md
+drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-07-06 21:34:17.000000 aquariumlearning-1.0.5/aquariumlearning/
+-rw-r--r--   0 robinyang   (501) staff       (20)     5264 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/__init__.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    27894 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/base_labels.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    19772 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/class_map.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    82456 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/client.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    37335 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/collection_client.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    13675 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/coordinate_frames.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     4221 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/dataset_client.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    45024 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/datasets.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     4405 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/datasharing.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     5319 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/embedding_distance_sampling.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    36286 2023-07-06 20:24:08.000000 aquariumlearning-1.0.5/aquariumlearning/frames.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    17446 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/inferences.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    21566 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/labels.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    23775 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/metrics_manager.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    17181 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/modified_labels.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     1768 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/sampling_agent.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    28949 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/segments.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    19457 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/sensor_data.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     8622 2023-02-08 03:39:31.000000 aquariumlearning-1.0.5/aquariumlearning/turbo.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    18415 2023-06-27 21:26:51.000000 aquariumlearning-1.0.5/aquariumlearning/util.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     9477 2023-02-08 03:39:31.000000 aquariumlearning-1.0.5/aquariumlearning/viridis.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    10213 2023-06-21 02:06:18.000000 aquariumlearning-1.0.5/aquariumlearning/work_queues.py
+drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-07-06 21:34:17.000000 aquariumlearning-1.0.5/aquariumlearning.egg-info/
+-rw-r--r--   0 robinyang   (501) staff       (20)      642 2023-07-06 21:34:17.000000 aquariumlearning-1.0.5/aquariumlearning.egg-info/PKG-INFO
+-rw-r--r--   0 robinyang   (501) staff       (20)      919 2023-07-06 21:34:17.000000 aquariumlearning-1.0.5/aquariumlearning.egg-info/SOURCES.txt
+-rw-r--r--   0 robinyang   (501) staff       (20)        1 2023-07-06 21:34:17.000000 aquariumlearning-1.0.5/aquariumlearning.egg-info/dependency_links.txt
+-rw-r--r--   0 robinyang   (501) staff       (20)      349 2023-07-06 21:34:17.000000 aquariumlearning-1.0.5/aquariumlearning.egg-info/requires.txt
+-rw-r--r--   0 robinyang   (501) staff       (20)       17 2023-07-06 21:34:17.000000 aquariumlearning-1.0.5/aquariumlearning.egg-info/top_level.txt
+-rw-r--r--   0 robinyang   (501) staff       (20)       38 2023-07-06 21:34:17.000000 aquariumlearning-1.0.5/setup.cfg
+-rw-r--r--   0 robinyang   (501) staff       (20)     1373 2023-07-06 20:25:16.000000 aquariumlearning-1.0.5/setup.py
```

### Comparing `aquariumlearning-1.0.4/PKG-INFO` & `aquariumlearning-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquariumlearning
-Version: 1.0.4
+Version: 1.0.5
 Summary: Aquarium Learning Python Client
 Home-page: https://www.aquariumlearning.com
 Author: Quinn Johnson
 Author-email: quinn@aquarium-learn.com
 License: UNKNOWN
 Description: # Aquarium Learning Python Client Library
```

### Comparing `aquariumlearning-1.0.4/aquariumlearning/__init__.py` & `aquariumlearning-1.0.5/aquariumlearning/__init__.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/base_labels.py` & `aquariumlearning-1.0.5/aquariumlearning/base_labels.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/class_map.py` & `aquariumlearning-1.0.5/aquariumlearning/class_map.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/client.py` & `aquariumlearning-1.0.5/aquariumlearning/client.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/collection_client.py` & `aquariumlearning-1.0.5/aquariumlearning/collection_client.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/coordinate_frames.py` & `aquariumlearning-1.0.5/aquariumlearning/coordinate_frames.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/dataset_client.py` & `aquariumlearning-1.0.5/aquariumlearning/dataset_client.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/datasets.py` & `aquariumlearning-1.0.5/aquariumlearning/datasets.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/datasharing.py` & `aquariumlearning-1.0.5/aquariumlearning/datasharing.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/embedding_distance_sampling.py` & `aquariumlearning-1.0.5/aquariumlearning/embedding_distance_sampling.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/frames.py` & `aquariumlearning-1.0.5/aquariumlearning/frames.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,25 +388,23 @@
         for sensor_datum in sensor_data:
             if sensor_datum.id in seen_sensor_ids:
                 raise Exception(
                     f"Encountered multiple sensor_data with the same id {sensor_datum.id}"
                 )
             seen_sensor_ids.add(sensor_datum.id)
             if not sensor_datum.coordinate_frame:
+                # check if there are explicitly passed coordinate frames that this could feasibly belong to
+                # in the case of someone just wanting to pass coordinates and sensors without having to predefine them
                 existing = _find_first_instance(
                     coordinate_frames, sensor_datum._default_cf_class
                 )
-                new = _find_first_instance(
-                    new_coordinate_frames, sensor_datum._default_cf_class
-                )
                 if existing:
                     sensor_datum._set_coordinate_frame(existing)
-                elif new:
-                    sensor_datum._set_coordinate_frame(new)
                 else:
+                    # otherwise, assume that this is a separate sensor from other sensors that is looking at a different part of the world
                     new_cf = sensor_datum._default_cf_class(sensor_datum.id)
                     sensor_datum._set_coordinate_frame(new_cf)
                     new_coordinate_frames.append(new_cf)
         return new_coordinate_frames
 
     def _validate_and_parent_cf(
         self,
```

### Comparing `aquariumlearning-1.0.4/aquariumlearning/inferences.py` & `aquariumlearning-1.0.5/aquariumlearning/inferences.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/labels.py` & `aquariumlearning-1.0.5/aquariumlearning/labels.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/metrics_manager.py` & `aquariumlearning-1.0.5/aquariumlearning/metrics_manager.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/modified_labels.py` & `aquariumlearning-1.0.5/aquariumlearning/modified_labels.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/sampling_agent.py` & `aquariumlearning-1.0.5/aquariumlearning/sampling_agent.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/segments.py` & `aquariumlearning-1.0.5/aquariumlearning/segments.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/sensor_data.py` & `aquariumlearning-1.0.5/aquariumlearning/sensor_data.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/turbo.py` & `aquariumlearning-1.0.5/aquariumlearning/turbo.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/util.py` & `aquariumlearning-1.0.5/aquariumlearning/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
 
 
 def extract_illegal_characters(el_id: str) -> List[str]:
     # prohibit characters that violate https://cloud.google.com/storage/docs/naming-objects#objectnames
     # and commas and slashes as they are used for internal aquarium aggregations
     # also ban all non-ascii characters
     matches = re.findall(
-        "[^\x00-\xFF]|#|[[]|[]]|[?]|[*]|,|/|[\x7F-\x84]|[\x86-\x9F]", el_id
+        r"[^\x00-\xFF]|#|[\[]|[\]]|[?]|[*]|,|/|[\x7F-\x84]|[\x86-\x9F]", el_id
     )
     return list(set(matches))
 
 
 def validate_id(el_id: str, el_type: str) -> None:
     if not isinstance(el_id, str):
         raise Exception(f"{el_type} id must be a string")
```

### Comparing `aquariumlearning-1.0.4/aquariumlearning/viridis.py` & `aquariumlearning-1.0.5/aquariumlearning/viridis.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning/work_queues.py` & `aquariumlearning-1.0.5/aquariumlearning/work_queues.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/aquariumlearning.egg-info/PKG-INFO` & `aquariumlearning-1.0.5/aquariumlearning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquariumlearning
-Version: 1.0.4
+Version: 1.0.5
 Summary: Aquarium Learning Python Client
 Home-page: https://www.aquariumlearning.com
 Author: Quinn Johnson
 Author-email: quinn@aquarium-learn.com
 License: UNKNOWN
 Description: # Aquarium Learning Python Client Library
```

### Comparing `aquariumlearning-1.0.4/aquariumlearning.egg-info/SOURCES.txt` & `aquariumlearning-1.0.5/aquariumlearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.4/setup.py` & `aquariumlearning-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aquariumlearning",  # Replace with your own username
-    version="1.0.4",
+    version="1.0.5",
     author="Quinn Johnson",
     author_email="quinn@aquarium-learn.com",
     description="Aquarium Learning Python Client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.aquariumlearning.com",
     packages=setuptools.find_packages(
```

