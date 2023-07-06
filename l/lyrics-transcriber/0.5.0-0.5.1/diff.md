# Comparing `tmp/lyrics_transcriber-0.5.0.tar.gz` & `tmp/lyrics_transcriber-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrics_transcriber-0.5.0.tar", max compression
+gzip compressed data, was "lyrics_transcriber-0.5.1.tar", max compression
```

## Comparing `lyrics_transcriber-0.5.0.tar` & `lyrics_transcriber-0.5.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-01 00:07:55.170976 lyrics_transcriber-0.5.0/LICENSE
--rw-r--r--   0        0        0     3523 2023-07-03 03:34:02.162763 lyrics_transcriber-0.5.0/README.md
--rw-r--r--   0        0        0       94 2023-07-01 16:43:51.383557 lyrics_transcriber-0.5.0/lyrics_transcriber/__init__.py
--rw-r--r--   0        0        0    12922 2023-07-06 06:52:16.605838 lyrics_transcriber-0.5.0/lyrics_transcriber/transcriber.py
--rw-r--r--   0        0        0        0 2023-06-30 23:05:50.978048 lyrics_transcriber-0.5.0/lyrics_transcriber/utils/__init__.py
--rwxr-xr-x   0        0        0     3849 2023-07-06 06:29:00.769390 lyrics_transcriber-0.5.0/lyrics_transcriber/utils/cli.py
--rw-r--r--   0        0        0     1244 2023-07-06 06:54:28.197151 lyrics_transcriber-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4574 1970-01-01 00:00:00.000000 lyrics_transcriber-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-01 00:07:55.170976 lyrics_transcriber-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3523 2023-07-03 03:34:02.162763 lyrics_transcriber-0.5.1/README.md
+-rw-r--r--   0        0        0       94 2023-07-01 16:43:51.383557 lyrics_transcriber-0.5.1/lyrics_transcriber/__init__.py
+-rw-r--r--   0        0        0    13003 2023-07-06 07:05:57.554203 lyrics_transcriber-0.5.1/lyrics_transcriber/transcriber.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:05:50.978048 lyrics_transcriber-0.5.1/lyrics_transcriber/utils/__init__.py
+-rwxr-xr-x   0        0        0     3849 2023-07-06 06:29:00.769390 lyrics_transcriber-0.5.1/lyrics_transcriber/utils/cli.py
+-rw-r--r--   0        0        0     1244 2023-07-06 07:06:01.865876 lyrics_transcriber-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4574 1970-01-01 00:00:00.000000 lyrics_transcriber-0.5.1/PKG-INFO
```

### Comparing `lyrics_transcriber-0.5.0/LICENSE` & `lyrics_transcriber-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.5.0/README.md` & `lyrics_transcriber-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.5.0/lyrics_transcriber/transcriber.py` & `lyrics_transcriber-0.5.1/lyrics_transcriber/transcriber.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 
         self.whisper_result_dict = None
 
         self.result_metadata = {
             "whisper_json_filepath": None,
             "genius_lyrics": None,
             "genius_lyrics_filepath": None,
+            "spotify_lyrics": None,
+            "spotify_lyrics_filepath": None,
             "midico_lrc_filepath": None,
             "singing_percentage": None,
             "total_singing_duration": None,
             "song_duration": None,
         }
 
         if self.audio_filepath is None:
```

### Comparing `lyrics_transcriber-0.5.0/lyrics_transcriber/utils/cli.py` & `lyrics_transcriber-0.5.1/lyrics_transcriber/utils/cli.py`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.5.0/pyproject.toml` & `lyrics_transcriber-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lyrics-transcriber"
-version = "0.5.0"
+version = "0.5.1"
 description = "Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "lyrics_transcriber" }]
 
 [tool.poetry.dependencies]
```

### Comparing `lyrics_transcriber-0.5.0/PKG-INFO` & `lyrics_transcriber-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrics-transcriber
-Version: 0.5.0
+Version: 0.5.1
 Summary: Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

