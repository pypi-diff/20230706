# Comparing `tmp/hydrusvideodeduplicator-0.2.0.tar.gz` & `tmp/hydrusvideodeduplicator-0.2.1.tar.gz`

## Comparing `hydrusvideodeduplicator-0.2.0.tar` & `hydrusvideodeduplicator-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/Dockerfile
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/docker-compose.yml
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/docker-entrypoint.sh
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/__init__.py
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/__main__.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/config.py
--rw-r--r--   0        0        0    15720 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/dedup.py
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/dedup_util.py
--rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/hydrus_api/LICENSE
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/hydrus_api/README.md
--rw-r--r--   0        0        0    36873 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/hydrus_api/__init__.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/hydrus_api/utils.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/__init__.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/hasher/__init__.py
--rw-r--r--   0        0        0    24236 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/hasher/pdq_hasher.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/tests/__init__.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/tests/hash256_test.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/tests/matrix_test.py
--rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/tests/pdq_test.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/tools/__init__.py
--rw-r--r--   0        0        0    12530 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/tools/pdq_photo_hasher_tool.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/types/__init__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/types/containers.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/types/exceptions.py
--rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/types/hash256.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/utils/__init__.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/utils/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/vpdqpy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/vpdqpy/__main__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/vpdqpy/typing_utils.py
--rw-r--r--   0        0        0     6420 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/vpdqpy/vpdqpy.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/LICENSE
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/README.md
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/Dockerfile
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/docker-compose.yml
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/docker-entrypoint.sh
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/__init__.py
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/__main__.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/config.py
+-rw-r--r--   0        0        0    15957 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/dedup.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/dedup_util.py
+-rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/hydrus_api/LICENSE
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/hydrus_api/README.md
+-rw-r--r--   0        0        0    36873 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/hydrus_api/__init__.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/hydrus_api/utils.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/__init__.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/hasher/__init__.py
+-rw-r--r--   0        0        0    24209 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tests/__init__.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tests/matrix_test.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tools/__init__.py
+-rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/types/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/types/containers.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/types/exceptions.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/utils/__init__.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/vpdqpy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/vpdqpy/__main__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/vpdqpy/typing_utils.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/README.md
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.1/PKG-INFO
```

### Comparing `hydrusvideodeduplicator-0.2.0/docker-compose.yml` & `hydrusvideodeduplicator-0.2.1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.0/docker-entrypoint.sh` & `hydrusvideodeduplicator-0.2.1/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.0/.github/workflows/python-publish.yml` & `hydrusvideodeduplicator-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/__main__.py` & `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/__main__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/config.py` & `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/config.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/dedup.py` & `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/dedup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from tqdm import tqdm
 
 if TYPE_CHECKING:
     pass
 
 import hydrusvideodeduplicator.hydrus_api as hydrus_api
 import hydrusvideodeduplicator.hydrus_api.utils
-from vpdqpy.vpdqpy import Vpdq
+from .vpdqpy.vpdqpy import Vpdq
 
 from .config import DEDUP_DATABASE_DIR, DEDUP_DATABASE_FILE, DEDUP_DATABASE_NAME
 from .dedup_util import database_accessible, find_tag_in_tags, get_file_names_hydrus
 
 
 class HydrusVideoDeduplicator:
     hydlog = logging.getLogger("hydlog")
@@ -61,18 +61,24 @@
 
         video_hashes = None
         if skip_hashing:
             rprint("[yellow] Skipping perceptual hashing")
             if query:
                 video_hashes = set(self._retrieve_video_hashes(search_tags))
         else:
-            video_hashes = self._retrieve_video_hashes(search_tags)
-            self._add_perceptual_hashes_to_db(overwrite=overwrite, video_hashes=video_hashes)
+            all_video_hashes = self._retrieve_video_hashes(search_tags)
+            self._add_perceptual_hashes_to_db(overwrite=overwrite, video_hashes=all_video_hashes)
+        
+        if query and not skip_hashing:
+            video_hashes = set(self._retrieve_video_hashes(search_tags))
 
-        self._find_potential_duplicates(limited_video_hashes=video_hashes)
+        if query:
+            self._find_potential_duplicates(limited_video_hashes=video_hashes)
+        else:
+            self._find_potential_duplicates(limited_video_hashes=None)
 
         self.hydlog.info("Deduplication done.")
 
     @staticmethod
     def _calculate_perceptual_hash(video: str | bytes) -> str:
         perceptual_hash = Vpdq.vpdq_to_json(Vpdq.computeHash(video))
         assert perceptual_hash != "[]"
```

### Comparing `hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/dedup_util.py` & `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/dedup_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/hydrus_api/LICENSE` & `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/hydrus_api/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/hydrus_api/__init__.py` & `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/hydrus_api/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/hydrus_api/utils.py` & `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/hydrus_api/utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.0/src/pdqhashing/hasher/pdq_hasher.py` & `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 import math
 import time
 from typing import List
 
 from PIL import Image
 
-from pdqhashing.types.containers import HashAndQuality, HashesAndQuality
-from pdqhashing.types.hash256 import Hash256
-from pdqhashing.utils.matrix import MatrixUtil
+from ..types.containers import HashAndQuality, HashesAndQuality
+from ..types.hash256 import Hash256
+from ..utils.matrix import MatrixUtil
 
 
 class PDQHasher:
     """The only class state is the DCT matrix, so this class may either be
     instantiated once per image, or instantiated once and used for all images;
     the latter will be slightly faster as the DCT matrix will not need to be
     recomputed once per image. Methods are threadsafe."""
```

### Comparing `hydrusvideodeduplicator-0.2.0/src/pdqhashing/tests/hash256_test.py` & `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pyre-strict
 # Copyright (c) Meta Platforms, Inc. and affiliates.
-from pdqhashing.types.exceptions import PDQHashFormatException
-from pdqhashing.types.hash256 import Hash256
+from ..types.exceptions import PDQHashFormatException
+from ..types.hash256 import Hash256
 import unittest
 
 
 class Hash256Test(unittest.TestCase):
     SAMPLE_HASH = "9c151c3af838278e3ef57c180c7d031c07aefd12f2ccc1e18f2a1e1c7d0ff163"
 
     def test_incorrect_hex_length(self) -> None:
```

### Comparing `hydrusvideodeduplicator-0.2.0/src/pdqhashing/tests/pdq_test.py` & `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 
-from pdqhashing.hasher.pdq_hasher import PDQHasher
-from pdqhashing.types.hash256 import Hash256
+from ..hasher.pdq_hasher import PDQHasher
+from ..types.hash256 import Hash256
 import unittest
 
 SAMPLE_MEDIA = os.path.dirname(__file__) + "/../../../../data/"
 
 
 class PdqTest(unittest.TestCase):
     def get_data(self):
```

### Comparing `hydrusvideodeduplicator-0.2.0/src/pdqhashing/tools/pdq_photo_hasher_tool.py` & `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import argparse
 import os
 import sys
 
 sys.path.append(os.path.join(os.path.dirname(__file__), "../.."))
 
-from pdqhashing.hasher.pdq_hasher import PDQHasher
-from pdqhashing.types.hash256 import Hash256
+from ..hasher.pdq_hasher import PDQHasher
+from ..types.hash256 import Hash256
 
 
 class PDQPhotoHasherTool:
     """Tool for computing PDQ hashes of image files (JPEG, PNG, etc.).
     Example use from within pdqhashing directory in Instagram Container:
     python tools/pdq_photo_hasher_tool.py ../media/sample_data/pdq/misc-images/b.jpg --pdq"""
```

### Comparing `hydrusvideodeduplicator-0.2.0/src/pdqhashing/types/containers.py` & `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/types/containers.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.0/src/pdqhashing/types/hash256.py` & `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 
 from random import randint
 
-from pdqhashing.types.exceptions import PDQHashFormatException
+from ..types.exceptions import PDQHashFormatException
 
 
 class Hash256:
     """256-bit hashes with Hamming distance"""
 
     # 16 slots of 16 bits each.
     # See hashing/pdq/README-MIH.md in this repo for why not 8x32 or 32x8, etc.
```

### Comparing `hydrusvideodeduplicator-0.2.0/src/pdqhashing/utils/matrix.py` & `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.0/src/vpdqpy/vpdqpy.py` & `hydrusvideodeduplicator-0.2.1/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import av
 from PIL import Image
 
-from pdqhashing.hasher.pdq_hasher import PDQHasher
+from ..pdqhashing.hasher.pdq_hasher import PDQHasher
 
 if TYPE_CHECKING:
     from typing import Annotated, Generator
 
     from .typing_utils import ValueRange
 
-    from pdqhashing.types.containers import HashAndQuality
+    from ..pdqhashing.types.containers import HashAndQuality
 
-from pdqhashing.types.hash256 import Hash256
+from ..pdqhashing.types.hash256 import Hash256
 
 
 @dataclass(slots=True)
 class VpdqFeature:
     pdq_hash: Hash256  # 64 char hex string
     quality: float  # 0 to 100
     frame_number: int
```

### Comparing `hydrusvideodeduplicator-0.2.0/.gitignore` & `hydrusvideodeduplicator-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.0/LICENSE` & `hydrusvideodeduplicator-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.0/README.md` & `hydrusvideodeduplicator-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.0/pyproject.toml` & `hydrusvideodeduplicator-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 
 [project.urls]
 Documentation = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator#readme"
 Issues = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues"
 Source = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator"
 
 [tool.hatch.dependencies]
-local_dependency = {path = "src/hydrusvideodeduplicator/hydrus_api"}
+hydrus_api = {path = "src/hydrusvideodeduplicator/hydrus_api"}
+vpdqpy = {path = "src/hydrusvideodeduplicator/vpdqpy"}
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.version]
 path = "src/hydrusvideodeduplicator/__about__.py"
```

### Comparing `hydrusvideodeduplicator-0.2.0/PKG-INFO` & `hydrusvideodeduplicator-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrusvideodeduplicator
-Version: 0.2.0
+Version: 0.2.1
 Summary: Video deduplicator utility for Hydrus Network
 Project-URL: Documentation, https://github.com/appleappleapplenanner/hydrus-video-deduplicator#readme
 Project-URL: Issues, https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues
 Project-URL: Source, https://github.com/appleappleapplenanner/hydrus-video-deduplicator
 Author-email: appleappleapplenanner <applenannerapple@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

