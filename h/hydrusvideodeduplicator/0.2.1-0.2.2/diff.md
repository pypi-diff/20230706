# Comparing `tmp/hydrusvideodeduplicator-0.2.1.tar.gz` & `tmp/hydrusvideodeduplicator-0.2.2.tar.gz`

## Comparing `hydrusvideodeduplicator-0.2.1.tar` & `hydrusvideodeduplicator-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,37 @@
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/Dockerfile
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/docker-compose.yml
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/docker-entrypoint.sh
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/__init__.py
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/__main__.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/config.py
--rw-r--r--   0        0        0    15957 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/dedup.py
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/dedup_util.py
--rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/hydrus_api/LICENSE
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/hydrus_api/README.md
--rw-r--r--   0        0        0    36873 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/hydrus_api/__init__.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/hydrus_api/utils.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/__init__.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/hasher/__init__.py
--rw-r--r--   0        0        0    24209 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tests/__init__.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tests/matrix_test.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tools/__init__.py
--rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/types/__init__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/types/containers.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/types/exceptions.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/utils/__init__.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/vpdqpy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/vpdqpy/__main__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/vpdqpy/typing_utils.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/LICENSE
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/README.md
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/Dockerfile
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/docker-compose.yml
+-rwxr-xr-x   0        0        0      825 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/docker-entrypoint.sh
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/__init__.py
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/__main__.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/config.py
+-rw-r--r--   0        0        0    15957 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/dedup.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/dedup_util.py
+-rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/hydrus_api/LICENSE
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/hydrus_api/README.md
+-rw-r--r--   0        0        0    36873 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/hydrus_api/__init__.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/hydrus_api/utils.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/__init__.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/hasher/__init__.py
+-rw-r--r--   0        0        0    24209 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tests/__init__.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tests/matrix_test.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tools/__init__.py
+-rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/types/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/types/containers.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/types/exceptions.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/utils/__init__.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/vpdqpy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/vpdqpy/__main__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/vpdqpy/typing_utils.py
+-rw-r--r--   0        0        0     7086 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/README.md
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/PKG-INFO
```

### Comparing `hydrusvideodeduplicator-0.2.1/docker-compose.yml` & `hydrusvideodeduplicator-0.2.2/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/docker-entrypoint.sh` & `hydrusvideodeduplicator-0.2.2/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/__main__.py` & `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/__main__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/config.py` & `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/config.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/dedup.py` & `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/dedup.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/dedup_util.py` & `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/dedup_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/hydrus_api/LICENSE` & `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/hydrus_api/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/hydrus_api/__init__.py` & `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/hydrus_api/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/hydrus_api/utils.py` & `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/hydrus_api/utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py` & `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py` & `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py` & `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py` & `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/types/containers.py` & `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/types/containers.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py` & `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py` & `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py` & `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import io
 import json
 from dataclasses import dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING
+import logging
 
 import av
 from PIL import Image
 
 from ..pdqhashing.hasher.pdq_hasher import PDQHasher
 
 if TYPE_CHECKING:
@@ -118,18 +119,31 @@
 
         result = Vpdq.feature_match_count(query_filtered, target_filtered, distance_tolerance)
         return result * 100 / len(query_filtered)
 
     @staticmethod
     def frame_extract_pyav(video: bytes) -> Generator[Image.Image]:
         with av.open(io.BytesIO(video), metadata_encoding='utf-8', metadata_errors='ignore') as container:
+            # Check for video in video container
+            video_streams = container.streams.video
+            if len(video_streams) < 1:
+                logging.error("Video stream not found.")
+                raise ValueError("Video stream not found.")
+
             video = container.streams.video[0]
             video.thread_type = "AUTO"
 
-            average_fps: int = round(video.average_rate)
+            average_fps = video.average_rate
+            # Some videos, like small GIFs, will have a NoneType FPS
+            # If this happens or if the average FPS is below 1, every frame will be hashed
+            if average_fps is None:
+                average_fps = 1
+                logging.warning("Average FPS not found. Every frame will be hashed.")
+            else:
+                average_fps: int = int(max(round(average_fps), 1))
 
             for index, frame in enumerate(container.decode(video)):
                 if index % average_fps == 0:
                     yield frame
 
     # Perceptually hash video from a file path or the bytes
     @staticmethod
```

### Comparing `hydrusvideodeduplicator-0.2.1/.gitignore` & `hydrusvideodeduplicator-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/LICENSE` & `hydrusvideodeduplicator-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.1/README.md` & `hydrusvideodeduplicator-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,24 +21,20 @@
 The accuracy is extremely good because of [vpdq](https://github.com/facebook/ThreatExchange/tree/main/vpdq). You can adjust the threshold of similarity using `--threshold`. The default is 75%.
 
 For more information check out the [wiki](https://github.com/appleappleapplenanner/hydrus-video-deduplicator/wiki) and the [FAQ](https://github.com/appleappleapplenanner/hydrus-video-deduplicator/wiki/faq)
 
 ---
 
 ## Installation:
-
-[Windows requires WSL](https://github.com/appleappleapplenanner/hydrus-video-deduplicator/wiki/Installation#Windows)
-
-### Linux:
-[Install dependencies](https://github.com/appleappleapplenanner/hydrus-video-deduplicator/wiki/Installation#Linux)
-
-Then install with pip:
+#### Dependencies:
+- Python >=3.10
+- FFmpeg
 
 ```sh
-pip install hydrusvideodeduplicator
+python3 -m pip install hydrusvideodeduplicator
 ```
 
 ---
 
 ## [Usage:](https://github.com/appleappleapplenanner/hydrus-video-deduplicator/wiki/Usage)
 
 ```sh
@@ -50,24 +46,24 @@
 ## TODO:
 - [ ] Option to rollback and remove potential duplicates
 - [ ] OR predicates for --query
 - [ ] Parallelize hashing and duplicate search
 - [ ] Automatically generate access key with Hydrus API
 - [x] Docker container
 - [ ] Upload Docker container to Docker Hub (GitHub Action)
-- [ ] Pure Python port of vpdq
-- [ ] Windows compatibility without WSL or Docker
+- [x] Pure Python port of vpdq
+- [x] Windows compatibility without WSL or Docker
 
-Please create an issue on Github if you have any problems or questions! Pull requests also welcome on this or my VideoHash fork. 
-
-There is a lot to improve and cleanup and I'm more experienced in C than Python, so fix stuff please.
+Please create an issue on Github if you have any problems or questions! Pull requests are also welcome.
 
 ---
 
 ## Credits:
 [Hydrus Network](https://github.com/hydrusnetwork/hydrus) by dev
 
 [Hydrus API Library](https://gitlab.com/cryzed/hydrus-api) by Cryzed
 
-[vpdq](https://github.com/facebook/ThreatExchange/tree/main/vpdq) by Meta
+[pdq](https://github.com/facebook/ThreatExchange/tree/main/pdq) by Meta
+
+vpdq by Meta, ported to Python by me.
 
-various other files from threatexchange by Meta
+[Big Buck Bunny](https://peach.blender.org/about) clips by Blender Foundation (CC BY 3.0)
```

### Comparing `hydrusvideodeduplicator-0.2.1/pyproject.toml` & `hydrusvideodeduplicator-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,21 @@
 Issues = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues"
 Source = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator"
 
 [tool.hatch.dependencies]
 hydrus_api = {path = "src/hydrusvideodeduplicator/hydrus_api"}
 vpdqpy = {path = "src/hydrusvideodeduplicator/vpdqpy"}
 
+[tool.hatch.build]
+exclude = [
+  "/.*",
+  "/docs",
+  "/tests",
+]
+
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.version]
 path = "src/hydrusvideodeduplicator/__about__.py"
 
 [tool.hatch.envs.default]
```

### Comparing `hydrusvideodeduplicator-0.2.1/PKG-INFO` & `hydrusvideodeduplicator-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrusvideodeduplicator
-Version: 0.2.1
+Version: 0.2.2
 Summary: Video deduplicator utility for Hydrus Network
 Project-URL: Documentation, https://github.com/appleappleapplenanner/hydrus-video-deduplicator#readme
 Project-URL: Issues, https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues
 Project-URL: Source, https://github.com/appleappleapplenanner/hydrus-video-deduplicator
 Author-email: appleappleapplenanner <applenannerapple@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -51,24 +51,20 @@
 The accuracy is extremely good because of [vpdq](https://github.com/facebook/ThreatExchange/tree/main/vpdq). You can adjust the threshold of similarity using `--threshold`. The default is 75%.
 
 For more information check out the [wiki](https://github.com/appleappleapplenanner/hydrus-video-deduplicator/wiki) and the [FAQ](https://github.com/appleappleapplenanner/hydrus-video-deduplicator/wiki/faq)
 
 ---
 
 ## Installation:
-
-[Windows requires WSL](https://github.com/appleappleapplenanner/hydrus-video-deduplicator/wiki/Installation#Windows)
-
-### Linux:
-[Install dependencies](https://github.com/appleappleapplenanner/hydrus-video-deduplicator/wiki/Installation#Linux)
-
-Then install with pip:
+#### Dependencies:
+- Python >=3.10
+- FFmpeg
 
 ```sh
-pip install hydrusvideodeduplicator
+python3 -m pip install hydrusvideodeduplicator
 ```
 
 ---
 
 ## [Usage:](https://github.com/appleappleapplenanner/hydrus-video-deduplicator/wiki/Usage)
 
 ```sh
@@ -80,24 +76,24 @@
 ## TODO:
 - [ ] Option to rollback and remove potential duplicates
 - [ ] OR predicates for --query
 - [ ] Parallelize hashing and duplicate search
 - [ ] Automatically generate access key with Hydrus API
 - [x] Docker container
 - [ ] Upload Docker container to Docker Hub (GitHub Action)
-- [ ] Pure Python port of vpdq
-- [ ] Windows compatibility without WSL or Docker
+- [x] Pure Python port of vpdq
+- [x] Windows compatibility without WSL or Docker
 
-Please create an issue on Github if you have any problems or questions! Pull requests also welcome on this or my VideoHash fork. 
-
-There is a lot to improve and cleanup and I'm more experienced in C than Python, so fix stuff please.
+Please create an issue on Github if you have any problems or questions! Pull requests are also welcome.
 
 ---
 
 ## Credits:
 [Hydrus Network](https://github.com/hydrusnetwork/hydrus) by dev
 
 [Hydrus API Library](https://gitlab.com/cryzed/hydrus-api) by Cryzed
 
-[vpdq](https://github.com/facebook/ThreatExchange/tree/main/vpdq) by Meta
+[pdq](https://github.com/facebook/ThreatExchange/tree/main/pdq) by Meta
+
+vpdq by Meta, ported to Python by me.
 
-various other files from threatexchange by Meta
+[Big Buck Bunny](https://peach.blender.org/about) clips by Blender Foundation (CC BY 3.0)
```

