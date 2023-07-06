# Comparing `tmp/lyrics_transcriber-0.4.1.tar.gz` & `tmp/lyrics_transcriber-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrics_transcriber-0.4.1.tar", max compression
+gzip compressed data, was "lyrics_transcriber-0.5.0.tar", max compression
```

## Comparing `lyrics_transcriber-0.4.1.tar` & `lyrics_transcriber-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-01 00:07:55.170976 lyrics_transcriber-0.4.1/LICENSE
--rw-r--r--   0        0        0     3523 2023-07-03 03:34:02.162763 lyrics_transcriber-0.4.1/README.md
--rw-r--r--   0        0        0       94 2023-07-01 16:43:51.383557 lyrics_transcriber-0.4.1/lyrics_transcriber/__init__.py
--rw-r--r--   0        0        0    10321 2023-07-03 04:09:45.243605 lyrics_transcriber-0.4.1/lyrics_transcriber/transcriber.py
--rw-r--r--   0        0        0        0 2023-06-30 23:05:50.978048 lyrics_transcriber-0.4.1/lyrics_transcriber/utils/__init__.py
--rwxr-xr-x   0        0        0     3532 2023-07-03 04:10:21.670806 lyrics_transcriber-0.4.1/lyrics_transcriber/utils/cli.py
--rw-r--r--   0        0        0     1206 2023-07-03 03:33:02.897814 lyrics_transcriber-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4543 1970-01-01 00:00:00.000000 lyrics_transcriber-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-01 00:07:55.170976 lyrics_transcriber-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3523 2023-07-03 03:34:02.162763 lyrics_transcriber-0.5.0/README.md
+-rw-r--r--   0        0        0       94 2023-07-01 16:43:51.383557 lyrics_transcriber-0.5.0/lyrics_transcriber/__init__.py
+-rw-r--r--   0        0        0    12922 2023-07-06 06:52:16.605838 lyrics_transcriber-0.5.0/lyrics_transcriber/transcriber.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:05:50.978048 lyrics_transcriber-0.5.0/lyrics_transcriber/utils/__init__.py
+-rwxr-xr-x   0        0        0     3849 2023-07-06 06:29:00.769390 lyrics_transcriber-0.5.0/lyrics_transcriber/utils/cli.py
+-rw-r--r--   0        0        0     1244 2023-07-06 06:54:28.197151 lyrics_transcriber-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4574 1970-01-01 00:00:00.000000 lyrics_transcriber-0.5.0/PKG-INFO
```

### Comparing `lyrics_transcriber-0.4.1/LICENSE` & `lyrics_transcriber-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.4.1/README.md` & `lyrics_transcriber-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.4.1/lyrics_transcriber/transcriber.py` & `lyrics_transcriber-0.5.0/lyrics_transcriber/transcriber.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,44 +4,50 @@
 import logging
 import shutil
 import hashlib
 import subprocess
 import slugify
 import whisper_timestamped as whisper
 import lyricsgenius
+import syrics.api
 
 
 class LyricsTranscriber:
     def __init__(
         self,
         audio_filepath,
         song_artist=None,
         song_title=None,
         genius_api_token=None,
+        spotify_cookie=None,
         output_dir=None,
         cache_dir="/tmp/lyrics-transcriber-cache/",
         log_level=logging.DEBUG,
-        log_format="%(asctime)s - %(module)s - %(levelname)s - %(message)s",
+        log_format="%(asctime)s - %(levelname)s - %(module)s - %(message)s",
     ):
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(log_level)
 
         log_handler = logging.StreamHandler()
         log_formatter = logging.Formatter(log_format)
         log_handler.setFormatter(log_formatter)
         self.logger.addHandler(log_handler)
 
         self.logger.debug(f"LyricsTranscriber instantiating with input file: {audio_filepath}")
 
         self.cache_dir = cache_dir
         self.output_dir = output_dir
         self.audio_filepath = audio_filepath
+
         self.song_artist = song_artist
         self.song_title = song_title
-        self.genius_api_token = genius_api_token
+        self.song_known = self.song_artist is not None and self.song_title is not None
+
+        self.genius_api_token = os.getenv("GENIUS_API_TOKEN", default=genius_api_token)
+        self.spotify_cookie = os.getenv("SPOTIFY_COOKIE_SP_DC", default=spotify_cookie)
 
         self.whisper_result_dict = None
 
         self.result_metadata = {
             "whisper_json_filepath": None,
             "genius_lyrics": None,
             "genius_lyrics_filepath": None,
@@ -58,46 +64,96 @@
 
     def generate(self):
         self.logger.debug(f"audio_filepath is set: {self.audio_filepath}, beginning initial whisper transcription")
 
         self.result_metadata["whisper_json_filepath"] = self.get_cache_filepath(".json")
         self.whisper_result_dict = self.transcribe()
 
-        self.result_metadata["midico_lrc_filepath"] = self.get_cache_filepath(".lrc")
-        self.write_midico_lrc_file()
-
         self.calculate_singing_percentage()
 
-        if self.genius_api_token and self.song_artist and self.song_title:
-            self.logger.debug(
-                f"fetching lyrics from Genius as genius_api_token: {self.genius_api_token}, song_artist: {self.song_artist} and song_title: {self.song_title} were set"
-            )
-            self.result_metadata["genius_lyrics_filepath"] = self.get_cache_filepath("-genius.txt")
-            self.write_genius_lyrics_file()
-        else:
-            self.logger.debug(
-                f"not fetching lyrics from Genius as not all genius params were set: genius_api_token: {self.genius_api_token}, song_artist: {self.song_artist} and song_title: {self.song_title}"
-            )
+        self.write_genius_lyrics_file()
+        self.write_spotify_lyrics_file()
 
         # TODO: attempt to match up segments from genius lyrics with whisper segments
 
         # TODO: output synced lyrics from self.whisper_result_dict in ASS format too, using code from the_tuul
 
+        self.result_metadata["midico_lrc_filepath"] = self.get_cache_filepath(".lrc")
+        self.write_midico_lrc_file()
+
+        self.copy_files_to_output_dir()
+
+        return self.result_metadata
+
+    def copy_files_to_output_dir(self):
         if self.output_dir is None:
             self.output_dir = os.getcwd()
 
         self.result_metadata["whisper_json_filepath"] = shutil.copy(self.result_metadata["whisper_json_filepath"], self.output_dir)
         self.result_metadata["midico_lrc_filepath"] = shutil.copy(self.result_metadata["midico_lrc_filepath"], self.output_dir)
 
         if self.result_metadata["genius_lyrics_filepath"] is not None:
             self.result_metadata["genius_lyrics_filepath"] = shutil.copy(self.result_metadata["genius_lyrics_filepath"], self.output_dir)
 
-        return self.result_metadata
+        if self.result_metadata["spotify_lyrics_filepath"] is not None:
+            self.result_metadata["spotify_lyrics_filepath"] = shutil.copy(self.result_metadata["spotify_lyrics_filepath"], self.output_dir)
+
+    def write_spotify_lyrics_file(self):
+        if self.spotify_cookie and self.song_known:
+            self.logger.debug(f"attempting spotify fetch as spotify_cookie and song name was set")
+        else:
+            self.logger.warning(f"skipping spotify fetch as not all spotify params were set")
+            return
+
+        spotify_lyrics_cache_filepath = os.path.join(self.cache_dir, self.get_song_slug() + "-spotify.json")
+
+        if os.path.isfile(spotify_lyrics_cache_filepath):
+            self.logger.debug(f"found existing file at spotify_lyrics_cache_filepath, reading: {spotify_lyrics_cache_filepath}")
+
+            with open(spotify_lyrics_cache_filepath, "r") as cached_lyrics:
+                self.result_metadata["spotify_lyrics_filepath"] = spotify_lyrics_cache_filepath
+                self.result_metadata["spotify_lyrics"] = cached_lyrics
+                return cached_lyrics
+
+        self.logger.debug(
+            f"no cached lyrics found at spotify_lyrics_cache_filepath: {spotify_lyrics_cache_filepath}, attempting to fetch from spotify"
+        )
+
+        spotify_lyrics_json = None
+
+        try:
+            spotify_client = syrics.api.Spotify(self.spotify_cookie)
+            spotify_search_query = f"{self.song_title} - {self.song_artist}"
+            spotify_search_results = spotify_client.search(spotify_search_query, type="track", limit=5)
+
+            spotify_top_result = spotify_search_results["tracks"]["items"][0]
+            self.logger.debug(
+                f"spotify_top_result: {spotify_top_result['artists'][0]['name']} - {spotify_top_result['name']} ({spotify_top_result['external_urls']['spotify']})"
+            )
+
+            spotify_lyrics_dict = spotify_client.get_lyrics(spotify_top_result["id"])
+            spotify_lyrics_json = json.dumps(spotify_lyrics_dict, indent=4)
+
+            self.logger.debug(f"writing lyrics to spotify_lyrics_cache_filepath: {spotify_lyrics_cache_filepath}")
+            with open(spotify_lyrics_cache_filepath, "w") as f:
+                f.write(spotify_lyrics_json)
+        except Exception as e:
+            self.logger.warn(f"caught exception while attempting to fetch from spotify: ", e)
+
+        self.result_metadata["spotify_lyrics_filepath"] = spotify_lyrics_cache_filepath
+        self.result_metadata["spotify_lyrics"] = spotify_lyrics_json
+        return spotify_lyrics_json
 
     def write_genius_lyrics_file(self):
+        if self.genius_api_token and self.song_known:
+            self.logger.debug(f"attempting genius fetch as genius_api_token and song name was set")
+        else:
+            self.logger.warning(f"skipping genius fetch as not all genius params were set")
+            return
+
         genius_lyrics_cache_filepath = os.path.join(self.cache_dir, self.get_song_slug() + "-genius.txt")
 
         if os.path.isfile(genius_lyrics_cache_filepath):
             self.logger.debug(f"found existing file at genius_lyrics_cache_filepath, reading: {genius_lyrics_cache_filepath}")
 
             with open(genius_lyrics_cache_filepath, "r") as cached_lyrics:
                 self.result_metadata["genius_lyrics_filepath"] = genius_lyrics_cache_filepath
@@ -196,15 +252,15 @@
         self.logger.debug(f"no cached transcription file found, running whisper transcribe")
         audio = whisper.load_audio(self.audio_filepath)
         model = whisper.load_model("medium.en", device="cpu")
         result = whisper.transcribe(model, audio, language="en")
 
         self.logger.debug(f"whisper transcription complete, writing JSON to cache file: {whisper_cache_filepath}")
         with open(whisper_cache_filepath, "w") as cache_file:
-            json.dump(result, cache_file, indent=2)
+            json.dump(result, cache_file, indent=4)
 
         return result
 
     def get_cache_filepath(self, extension):
         filename = os.path.split(self.audio_filepath)[1]
         filename_slug = slugify.slugify(filename)
         hash_value = self.get_file_hash(self.audio_filepath)
```

### Comparing `lyrics_transcriber-0.4.1/lyrics_transcriber/utils/cli.py` & `lyrics_transcriber-0.5.0/lyrics_transcriber/utils/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def main():
     logger = logging.getLogger(__name__)
     logger.setLevel(logging.DEBUG)
 
     log_handler = logging.StreamHandler()
-    log_formatter = logging.Formatter("%(asctime)s - %(module)s - %(levelname)s - %(message)s")
+    log_formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(module)s - %(message)s")
     log_handler.setFormatter(log_formatter)
     logger.addHandler(log_handler)
 
     logger.debug("Parsing CLI args")
 
     parser = argparse.ArgumentParser(
         description="Create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, from any input song file"
@@ -33,14 +33,19 @@
         help="Optional: specify song title for Genius lyrics lookup and auto-correction",
     )
     parser.add_argument(
         "--genius_api_token",
         default=None,
         help="Optional: specify Genius API token for lyrics lookup and auto-correction",
     )
+    parser.add_argument(
+        "--spotify_cookie",
+        default=None,
+        help="Optional: specify Spotify sp_dc cookie value for lyrics lookup and auto-correction",
+    )
 
     parser.add_argument("--cache_dir", default="/tmp/lyrics-transcriber-cache/", help="Optional cache directory.")
 
     parser.add_argument(
         "--output_dir",
         default=None,
         help="Optional directory where the resulting lyrics files will be saved. If not specified, outputs to current dir.",
@@ -64,14 +69,15 @@
         exit(1)
 
     logger.debug("Loading LyricsTranscriber class")
 
     transcriber = LyricsTranscriber(
         args.audio_filepath,
         genius_api_token=args.genius_api_token,
+        spotify_cookie=args.spotify_cookie,
         song_artist=args.song_artist,
         song_title=args.song_title,
         output_dir=args.output_dir,
         cache_dir=args.cache_dir,
     )
 
     result_metadata = transcriber.generate()
@@ -87,11 +93,12 @@
     logger.info(f"Total Singing Duration: {formatted_singing_duration}")
     logger.info(f"Singing Percentage: {result_metadata['singing_percentage']}%")
 
     logger.info(f"*** Outputs: ***")
     logger.info(f"Whisper transcription output JSON file: {result_metadata['whisper_json_filepath']}")
     logger.info(f"MidiCo LRC output file: {result_metadata['midico_lrc_filepath']}")
     logger.info(f"Genius lyrics output file: {result_metadata['genius_lyrics_filepath']}")
+    logger.info(f"Spotify lyrics output file: {result_metadata['spotify_lyrics_filepath']}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `lyrics_transcriber-0.4.1/pyproject.toml` & `lyrics_transcriber-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lyrics-transcriber"
-version = "0.4.1"
+version = "0.5.0"
 description = "Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "lyrics_transcriber" }]
 
 [tool.poetry.dependencies]
@@ -16,19 +16,20 @@
 numpy = "^1"
 onnx = "^1"
 onnxruntime = "^1"
 torch = "^1"
 tqdm = "^4"
 lyricsgenius = "^3"
 python-slugify = "^8"
+syrics = "^0"
 openai-whisper = "20230314"
-# Note: after adding openai-whisper with poetry lock, I then removed all traces of triton
+whisper-timestamped = "^1"
+# Note: after adding openai-whisper and whisper-timestamped with poetry lock, I then removed all traces of triton
 # from poetry.lock before running poetry install, as triton doesn't support macOS but isn't actually needed for whisper.
 # This was the only way I was able to get a working cross-platform build published to PyPI.
-whisper-timestamped = "^1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 
 [tool.black]
 line-length = 140
```

### Comparing `lyrics_transcriber-0.4.1/PKG-INFO` & `lyrics_transcriber-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrics-transcriber
-Version: 0.4.1
+Version: 0.5.0
 Summary: Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Requires-Dist: lyricsgenius (>=3,<4)
 Requires-Dist: numba (>=0.57,<0.58)
 Requires-Dist: numpy (>=1,<2)
 Requires-Dist: onnx (>=1,<2)
 Requires-Dist: onnxruntime (>=1,<2)
 Requires-Dist: openai-whisper (==20230314)
 Requires-Dist: python-slugify (>=8,<9)
+Requires-Dist: syrics (>=0,<1)
 Requires-Dist: torch (>=1,<2)
 Requires-Dist: tqdm (>=4,<5)
 Requires-Dist: whisper-timestamped (>=1,<2)
 Description-Content-Type: text/markdown
 
 # Lyrics Transcriber 🎶
```

