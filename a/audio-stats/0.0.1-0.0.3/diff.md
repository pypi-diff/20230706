# Comparing `tmp/audio-stats-0.0.1.tar.gz` & `tmp/audio-stats-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio-stats-0.0.1.tar", last modified: Thu Jul  6 04:42:20 2023, max compression
+gzip compressed data, was "audio-stats-0.0.3.tar", last modified: Thu Jul  6 07:48:04 2023, max compression
```

## Comparing `audio-stats-0.0.1.tar` & `audio-stats-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-x---   0 khanh     (1004) asr      (10001)        0 2023-07-06 04:42:20.959079 audio-stats-0.0.1/
--rw-r-----   0 khanh     (1004) asr      (10001)     1069 2023-07-06 04:25:14.000000 audio-stats-0.0.1/LICENSE
--rw-r-----   0 khanh     (1004) asr      (10001)      363 2023-07-06 04:42:20.959079 audio-stats-0.0.1/PKG-INFO
--rw-r-----   0 khanh     (1004) asr      (10001)      110 2023-07-06 04:42:07.000000 audio-stats-0.0.1/README.md
-drwxr-x---   0 khanh     (1004) asr      (10001)        0 2023-07-06 04:42:20.959079 audio-stats-0.0.1/audio_stats/
--rw-r-----   0 khanh     (1004) asr      (10001)       36 2023-07-06 04:31:50.000000 audio-stats-0.0.1/audio_stats/__init__.py
--rw-r-----   0 khanh     (1004) asr      (10001)     2145 2023-07-06 04:31:27.000000 audio-stats-0.0.1/audio_stats/audio_stats.py
--rw-r-----   0 khanh     (1004) asr      (10001)     4107 2023-07-06 04:30:41.000000 audio-stats-0.0.1/audio_stats/reader.py
-drwxr-x---   0 khanh     (1004) asr      (10001)        0 2023-07-06 04:42:20.959079 audio-stats-0.0.1/audio_stats.egg-info/
--rw-r-----   0 khanh     (1004) asr      (10001)      363 2023-07-06 04:42:20.000000 audio-stats-0.0.1/audio_stats.egg-info/PKG-INFO
--rw-r-----   0 khanh     (1004) asr      (10001)      239 2023-07-06 04:42:20.000000 audio-stats-0.0.1/audio_stats.egg-info/SOURCES.txt
--rw-r-----   0 khanh     (1004) asr      (10001)        1 2023-07-06 04:42:20.000000 audio-stats-0.0.1/audio_stats.egg-info/dependency_links.txt
--rw-r-----   0 khanh     (1004) asr      (10001)       12 2023-07-06 04:42:20.000000 audio-stats-0.0.1/audio_stats.egg-info/top_level.txt
--rw-r-----   0 khanh     (1004) asr      (10001)       38 2023-07-06 04:42:20.959079 audio-stats-0.0.1/setup.cfg
--rw-r-----   0 khanh     (1004) asr      (10001)      538 2023-07-06 04:41:36.000000 audio-stats-0.0.1/setup.py
+drwxr-x---   0 khanh     (1004) asr      (10001)        0 2023-07-06 07:48:04.815002 audio-stats-0.0.3/
+-rw-r-----   0 khanh     (1004) asr      (10001)     1069 2023-07-06 04:25:14.000000 audio-stats-0.0.3/LICENSE
+-rw-r-----   0 khanh     (1004) asr      (10001)      363 2023-07-06 07:48:04.815002 audio-stats-0.0.3/PKG-INFO
+-rw-r-----   0 khanh     (1004) asr      (10001)      110 2023-07-06 04:42:07.000000 audio-stats-0.0.3/README.md
+drwxr-x---   0 khanh     (1004) asr      (10001)        0 2023-07-06 07:48:04.815002 audio-stats-0.0.3/audio_stats/
+-rw-r-----   0 khanh     (1004) asr      (10001)       36 2023-07-06 04:31:50.000000 audio-stats-0.0.3/audio_stats/__init__.py
+-rw-r-----   0 khanh     (1004) asr      (10001)     2241 2023-07-06 07:47:42.000000 audio-stats-0.0.3/audio_stats/audio_stats.py
+-rw-r-----   0 khanh     (1004) asr      (10001)     3819 2023-07-06 07:41:14.000000 audio-stats-0.0.3/audio_stats/flac_reader.py
+-rw-r-----   0 khanh     (1004) asr      (10001)      253 2023-07-06 07:40:54.000000 audio-stats-0.0.3/audio_stats/wav_reader.py
+drwxr-x---   0 khanh     (1004) asr      (10001)        0 2023-07-06 07:48:04.815002 audio-stats-0.0.3/audio_stats.egg-info/
+-rw-r-----   0 khanh     (1004) asr      (10001)      363 2023-07-06 07:48:04.000000 audio-stats-0.0.3/audio_stats.egg-info/PKG-INFO
+-rw-r-----   0 khanh     (1004) asr      (10001)      304 2023-07-06 07:48:04.000000 audio-stats-0.0.3/audio_stats.egg-info/SOURCES.txt
+-rw-r-----   0 khanh     (1004) asr      (10001)        1 2023-07-06 07:48:04.000000 audio-stats-0.0.3/audio_stats.egg-info/dependency_links.txt
+-rw-r-----   0 khanh     (1004) asr      (10001)       13 2023-07-06 07:48:04.000000 audio-stats-0.0.3/audio_stats.egg-info/requires.txt
+-rw-r-----   0 khanh     (1004) asr      (10001)       12 2023-07-06 07:48:04.000000 audio-stats-0.0.3/audio_stats.egg-info/top_level.txt
+-rw-r-----   0 khanh     (1004) asr      (10001)       38 2023-07-06 07:48:04.815002 audio-stats-0.0.3/setup.cfg
+-rw-r-----   0 khanh     (1004) asr      (10001)      574 2023-07-06 07:48:02.000000 audio-stats-0.0.3/setup.py
```

### Comparing `audio-stats-0.0.1/LICENSE` & `audio-stats-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `audio-stats-0.0.1/audio_stats/reader.py` & `audio-stats-0.0.3/audio_stats/flac_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from __future__ import annotations
 from typing import *
-import os
-import wave
-import contextlib
 from tqdm import tqdm
 
 import struct
 
 def bytes_to_int(bytes: list) -> int:
         result = 0
         for byte in bytes:
@@ -74,16 +71,7 @@
                 samplerate = bytes_to_int(unpacked[4:7]) >> 4
                 sample_bytes = [(unpacked[7] & 0x0F)] + list(unpacked[8:12])
                 total_samples = bytes_to_int(sample_bytes)
                 return total_samples, samplerate
             
             header = f.read(4)
 
-def get_wav_duration(filename: str) -> Tuple[int, int]:
-    with contextlib.closing(wave.open(filename, "rb")) as f:
-        return f.getnframes(), f.getframerate()
-
-get_duration = {
-    ".wav": get_wav_duration,
-    ".flac": get_flac_duration,
-}
-
```

### Comparing `audio-stats-0.0.1/setup.py` & `audio-stats-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 if __name__ == "__main__":
     with open("README.md") as f:
         long_description = f.read()
 
     setuptools.setup(
         name="audio-stats",
-        version="0.0.1",
+        version="0.0.3",
         author="Nguyen Ngoc Khanh",
         author_email="khanh.nguyen.contact@gmail.com",
         long_description=long_description,
         long_description_content_type="text/markdown",
-        url="https://github.com/khanh101/audio_stats",
+        url="https://github.com/khanh101/audio-stats",
         packages=setuptools.find_packages(),
         license="MIT",
-        install_requires=[],
+        install_requires=[
+            "tqdm==4.65.0"
+        ],
     )
```

