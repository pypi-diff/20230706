# Comparing `tmp/audio-stats-0.0.3.tar.gz` & `tmp/audio-stats-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio-stats-0.0.3.tar", last modified: Thu Jul  6 07:48:04 2023, max compression
+gzip compressed data, was "audio-stats-0.0.4.tar", last modified: Thu Jul  6 10:48:19 2023, max compression
```

## Comparing `audio-stats-0.0.3.tar` & `audio-stats-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-x---   0 khanh     (1004) asr      (10001)        0 2023-07-06 07:48:04.815002 audio-stats-0.0.3/
--rw-r-----   0 khanh     (1004) asr      (10001)     1069 2023-07-06 04:25:14.000000 audio-stats-0.0.3/LICENSE
--rw-r-----   0 khanh     (1004) asr      (10001)      363 2023-07-06 07:48:04.815002 audio-stats-0.0.3/PKG-INFO
--rw-r-----   0 khanh     (1004) asr      (10001)      110 2023-07-06 04:42:07.000000 audio-stats-0.0.3/README.md
-drwxr-x---   0 khanh     (1004) asr      (10001)        0 2023-07-06 07:48:04.815002 audio-stats-0.0.3/audio_stats/
--rw-r-----   0 khanh     (1004) asr      (10001)       36 2023-07-06 04:31:50.000000 audio-stats-0.0.3/audio_stats/__init__.py
--rw-r-----   0 khanh     (1004) asr      (10001)     2241 2023-07-06 07:47:42.000000 audio-stats-0.0.3/audio_stats/audio_stats.py
--rw-r-----   0 khanh     (1004) asr      (10001)     3819 2023-07-06 07:41:14.000000 audio-stats-0.0.3/audio_stats/flac_reader.py
--rw-r-----   0 khanh     (1004) asr      (10001)      253 2023-07-06 07:40:54.000000 audio-stats-0.0.3/audio_stats/wav_reader.py
-drwxr-x---   0 khanh     (1004) asr      (10001)        0 2023-07-06 07:48:04.815002 audio-stats-0.0.3/audio_stats.egg-info/
--rw-r-----   0 khanh     (1004) asr      (10001)      363 2023-07-06 07:48:04.000000 audio-stats-0.0.3/audio_stats.egg-info/PKG-INFO
--rw-r-----   0 khanh     (1004) asr      (10001)      304 2023-07-06 07:48:04.000000 audio-stats-0.0.3/audio_stats.egg-info/SOURCES.txt
--rw-r-----   0 khanh     (1004) asr      (10001)        1 2023-07-06 07:48:04.000000 audio-stats-0.0.3/audio_stats.egg-info/dependency_links.txt
--rw-r-----   0 khanh     (1004) asr      (10001)       13 2023-07-06 07:48:04.000000 audio-stats-0.0.3/audio_stats.egg-info/requires.txt
--rw-r-----   0 khanh     (1004) asr      (10001)       12 2023-07-06 07:48:04.000000 audio-stats-0.0.3/audio_stats.egg-info/top_level.txt
--rw-r-----   0 khanh     (1004) asr      (10001)       38 2023-07-06 07:48:04.815002 audio-stats-0.0.3/setup.cfg
--rw-r-----   0 khanh     (1004) asr      (10001)      574 2023-07-06 07:48:02.000000 audio-stats-0.0.3/setup.py
+drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-07-06 10:48:19.051908 audio-stats-0.0.4/
+-rw-r--r--   0 khanh      (501) staff       (20)     1069 2023-07-06 10:45:04.000000 audio-stats-0.0.4/LICENSE
+-rw-r--r--   0 khanh      (501) staff       (20)      363 2023-07-06 10:48:19.051729 audio-stats-0.0.4/PKG-INFO
+-rw-r--r--   0 khanh      (501) staff       (20)      110 2023-07-06 10:45:04.000000 audio-stats-0.0.4/README.md
+drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-07-06 10:48:19.050664 audio-stats-0.0.4/audio_stats/
+-rw-r--r--   0 khanh      (501) staff       (20)       36 2023-07-06 10:45:04.000000 audio-stats-0.0.4/audio_stats/__init__.py
+-rw-r--r--   0 khanh      (501) staff       (20)     2202 2023-07-06 10:48:11.000000 audio-stats-0.0.4/audio_stats/audio_stats.py
+-rw-r--r--   0 khanh      (501) staff       (20)     3769 2023-07-06 10:48:12.000000 audio-stats-0.0.4/audio_stats/flac_reader.py
+-rw-r--r--   0 khanh      (501) staff       (20)      254 2023-07-06 10:48:11.000000 audio-stats-0.0.4/audio_stats/wav_reader.py
+drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-07-06 10:48:19.051423 audio-stats-0.0.4/audio_stats.egg-info/
+-rw-r--r--   0 khanh      (501) staff       (20)      363 2023-07-06 10:48:19.000000 audio-stats-0.0.4/audio_stats.egg-info/PKG-INFO
+-rw-r--r--   0 khanh      (501) staff       (20)      304 2023-07-06 10:48:19.000000 audio-stats-0.0.4/audio_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 khanh      (501) staff       (20)        1 2023-07-06 10:48:19.000000 audio-stats-0.0.4/audio_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 khanh      (501) staff       (20)       13 2023-07-06 10:48:19.000000 audio-stats-0.0.4/audio_stats.egg-info/requires.txt
+-rw-r--r--   0 khanh      (501) staff       (20)       12 2023-07-06 10:48:19.000000 audio-stats-0.0.4/audio_stats.egg-info/top_level.txt
+-rw-r--r--   0 khanh      (501) staff       (20)       38 2023-07-06 10:48:19.052096 audio-stats-0.0.4/setup.cfg
+-rw-r--r--   0 khanh      (501) staff       (20)      574 2023-07-06 10:48:16.000000 audio-stats-0.0.4/setup.py
```

### Comparing `audio-stats-0.0.3/LICENSE` & `audio-stats-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `audio-stats-0.0.3/audio_stats/audio_stats.py` & `audio-stats-0.0.4/audio_stats/audio_stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 from __future__ import annotations
-from typing import *
-import os
+
 import json
+import os
+from typing import *
+
 from tqdm import tqdm
 
-from .wav_reader import get_wav_duration
 from .flac_reader import get_flac_duration
+from .wav_reader import get_wav_duration
 
 get_duration = {
     ".wav": get_wav_duration,
     ".flac": get_flac_duration,
 }
 
+
 class AudioStats:
     def __init__(self, cache_path: str = "/tmp/audio_stats.tmp"):
         self.cache_path = cache_path
         self.cache = {}
-        
+
         self.opened = False
         self.f = None
 
-    def __enter__(self) -> WavStats:
+    def __enter__(self) -> AudioStats:
         if self.opened:
             raise RuntimeError("context cannot be entered multiple times")
 
         self.opened = True
         # init cache
         cache_dir = os.path.dirname(self.cache_path)
         if not os.path.exists(cache_dir):
             os.makedirs(cache_dir)
-            
+
         if os.path.exists(self.cache_path):
             # read cache
             with open(self.cache_path) as f:
                 for line in tqdm(list(f), desc=f"loading cache {self.cache_path}"):
                     o = json.loads(line)
                     path, frame_count, sample_rate = o["path"], o["frame_count"], o["sample_rate"]
                     self.cache[path] = {
                         "frame_count": frame_count,
                         "sample_rate": sample_rate,
                     }
         # open file
         self.f = open(self.cache_path, "a")
         return self
-    
+
     def __exit__(self, exc_type, exc_val, exc_tb):
         if not self.opened:
             raise RuntimeError("context cannot be exited without entering")
 
         self.opened = False
         self.f.close()
         self.f = None
-    
+
     def read(self, path: str) -> Dict[str, Union[int, float]]:
         if not self.opened:
             raise RuntimeError("read only within context")
-        
+
         path = os.path.realpath(path)
-        
+
         if path not in self.cache:
             ext = os.path.splitext(path)[1]
             frame_count, sample_rate = get_duration[ext](path)
 
             o = {
                 "path": path,
                 "frame_count": frame_count,
```

### Comparing `audio-stats-0.0.3/audio_stats/flac_reader.py` & `audio-stats-0.0.4/audio_stats/flac_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
-from typing import *
-from tqdm import tqdm
 
 import struct
+from typing import *
+
 
 def bytes_to_int(bytes: list) -> int:
-        result = 0
-        for byte in bytes:
-            result = (result << 8) + byte
-        return result
+    result = 0
+    for byte in bytes:
+        result = (result << 8) + byte
+    return result
 
 
 def get_flac_duration(filename: str) -> Tuple[int, int]:
     """
     Returns the duration of a FLAC file in seconds
 
     https://xiph.org/flac/format.html
@@ -68,10 +68,9 @@
                                        result in an invalid bitstream.
                 """
 
                 samplerate = bytes_to_int(unpacked[4:7]) >> 4
                 sample_bytes = [(unpacked[7] & 0x0F)] + list(unpacked[8:12])
                 total_samples = bytes_to_int(sample_bytes)
                 return total_samples, samplerate
-            
-            header = f.read(4)
 
+            header = f.read(4)
```

### Comparing `audio-stats-0.0.3/setup.py` & `audio-stats-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 if __name__ == "__main__":
     with open("README.md") as f:
         long_description = f.read()
 
     setuptools.setup(
         name="audio-stats",
-        version="0.0.3",
+        version="0.0.4",
         author="Nguyen Ngoc Khanh",
         author_email="khanh.nguyen.contact@gmail.com",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/khanh101/audio-stats",
         packages=setuptools.find_packages(),
         license="MIT",
```

