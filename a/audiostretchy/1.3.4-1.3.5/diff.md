# Comparing `tmp/audiostretchy-1.3.4.tar.gz` & `tmp/audiostretchy-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostretchy-1.3.4.tar", last modified: Thu Jul  6 11:13:45 2023, max compression
+gzip compressed data, was "audiostretchy-1.3.5.tar", last modified: Thu Jul  6 12:15:28 2023, max compression
```

## Comparing `audiostretchy-1.3.4.tar` & `audiostretchy-1.3.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:13:45.052719 audiostretchy-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:13:45.024719 audiostretchy-1.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:13:45.032719 audiostretchy-1.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-06 11:13:45.056719 audiostretchy-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:13:45.036719 audiostretchy-1.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:13:45.036719 audiostretchy-1.3.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-06 11:13:45.056719 audiostretchy-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:13:45.024719 audiostretchy-1.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:13:45.036719 audiostretchy-1.3.4/src/audiostretchy/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/src/audiostretchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/src/audiostretchy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:13:45.040719 audiostretchy-1.3.4/src/audiostretchy/interface/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:13:45.044719 audiostretchy-1.3.4/src/audiostretchy/interface/linux/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/src/audiostretchy/interface/linux/_stretch.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:13:45.044719 audiostretchy-1.3.4/src/audiostretchy/interface/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/src/audiostretchy/interface/mac/_stretch.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/src/audiostretchy/interface/tdhs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:13:45.044719 audiostretchy-1.3.4/src/audiostretchy/interface/win/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/src/audiostretchy/interface/win/_stretch.def
--rw-r--r--   0 runner    (1001) docker     (123)   140288 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/src/audiostretchy/interface/win/_stretch.dll
--rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/src/audiostretchy/stretch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:13:45.040719 audiostretchy-1.3.4/src/audiostretchy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-06 11:13:44.000000 audiostretchy-1.3.4/src/audiostretchy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-06 11:13:45.000000 audiostretchy-1.3.4/src/audiostretchy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:13:44.000000 audiostretchy-1.3.4/src/audiostretchy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 11:13:44.000000 audiostretchy-1.3.4/src/audiostretchy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:13:44.000000 audiostretchy-1.3.4/src/audiostretchy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-06 11:13:44.000000 audiostretchy-1.3.4/src/audiostretchy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 11:13:44.000000 audiostretchy-1.3.4/src/audiostretchy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:13:45.052719 audiostretchy-1.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   198991 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/tests/audio-1.2.mp3
--rw-r--r--   0 runner    (1001) docker     (123)  1091644 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/tests/audio-1.2.wav
--rw-r--r--   0 runner    (1001) docker     (123)   132118 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/tests/audio.mp3
--rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/tests/audio.wav
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-06 11:13:26.000000 audiostretchy-1.3.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:15:28.302526 audiostretchy-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:15:28.290526 audiostretchy-1.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:15:28.294526 audiostretchy-1.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-07-06 12:15:28.302526 audiostretchy-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:15:28.298526 audiostretchy-1.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:15:28.298526 audiostretchy-1.3.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-06 12:15:28.306526 audiostretchy-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:15:28.290526 audiostretchy-1.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:15:28.298526 audiostretchy-1.3.5/src/audiostretchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/src/audiostretchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/src/audiostretchy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:15:28.298526 audiostretchy-1.3.5/src/audiostretchy/interface/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:15:28.298526 audiostretchy-1.3.5/src/audiostretchy/interface/linux/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/src/audiostretchy/interface/linux/_stretch.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:15:28.298526 audiostretchy-1.3.5/src/audiostretchy/interface/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/src/audiostretchy/interface/mac/_stretch.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/src/audiostretchy/interface/tdhs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:15:28.298526 audiostretchy-1.3.5/src/audiostretchy/interface/win/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/src/audiostretchy/interface/win/_stretch.def
+-rw-r--r--   0 runner    (1001) docker     (123)   140288 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/src/audiostretchy/interface/win/_stretch.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/src/audiostretchy/stretch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:15:28.298526 audiostretchy-1.3.5/src/audiostretchy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-07-06 12:15:28.000000 audiostretchy-1.3.5/src/audiostretchy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-06 12:15:28.000000 audiostretchy-1.3.5/src/audiostretchy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:15:28.000000 audiostretchy-1.3.5/src/audiostretchy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 12:15:28.000000 audiostretchy-1.3.5/src/audiostretchy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:15:27.000000 audiostretchy-1.3.5/src/audiostretchy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-06 12:15:28.000000 audiostretchy-1.3.5/src/audiostretchy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 12:15:28.000000 audiostretchy-1.3.5/src/audiostretchy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:15:28.302526 audiostretchy-1.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   198991 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/tests/audio-1.2.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)  1091644 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/tests/audio-1.2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   132118 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/tests/audio.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/tests/audio.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-06 12:15:11.000000 audiostretchy-1.3.5/tests/conftest.py
```

### Comparing `audiostretchy-1.3.4/.coveragerc` & `audiostretchy-1.3.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/.github/workflows/ci.yaml` & `audiostretchy-1.3.5/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/.gitignore` & `audiostretchy-1.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/.pre-commit-config.yaml` & `audiostretchy-1.3.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/.readthedocs.yml` & `audiostretchy-1.3.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/LICENSE.txt` & `audiostretchy-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/PKG-INFO` & `audiostretchy-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.3.4
+Version: 1.3.5
 Summary: AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. AudioStretchy is a wrapper around the audio-stretch C library by David Bryant.
 Home-page: https://github.com/twardoch/audiostretchy
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -26,15 +26,15 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # AudioStretchy
 
 AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-_Version: 1.3.4_
+_Version: 1.3.5_
 
 ## Features
 
 - Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
@@ -173,14 +173,15 @@
 # This needs [all] installation for soxr support
 audio_stretch.resample(sample_rate=44100) 
 audio_stretch.save(file=WAVDataAsBytesIO, format="wav")
 ```
 
 ## Changelog
 
+- v1.3.5: fix for MP3 writing
 - v1.3.2: fix for MP3 opening
 - v1.3.0: actually working on Windows as well
 - v1.2.x: working on macOS and Linux
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
```

### Comparing `audiostretchy-1.3.4/README.md` & `audiostretchy-1.3.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AudioStretchy
 
 AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-_Version: 1.3.4_
+_Version: 1.3.5_
 
 ## Features
 
 - Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
@@ -145,14 +145,15 @@
 # This needs [all] installation for soxr support
 audio_stretch.resample(sample_rate=44100) 
 audio_stretch.save(file=WAVDataAsBytesIO, format="wav")
 ```
 
 ## Changelog
 
+- v1.3.5: fix for MP3 writing
 - v1.3.2: fix for MP3 opening
 - v1.3.0: actually working on Windows as well
 - v1.2.x: working on macOS and Linux
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
```

### Comparing `audiostretchy-1.3.4/docs/Makefile` & `audiostretchy-1.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/docs/conf.py` & `audiostretchy-1.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/docs/index.md` & `audiostretchy-1.3.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/setup.cfg` & `audiostretchy-1.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/setup.py` & `audiostretchy-1.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/src/audiostretchy/__init__.py` & `audiostretchy-1.3.5/src/audiostretchy/__init__.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/src/audiostretchy/interface/linux/_stretch.so` & `audiostretchy-1.3.5/src/audiostretchy/interface/linux/_stretch.so`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/src/audiostretchy/interface/mac/_stretch.dylib` & `audiostretchy-1.3.5/src/audiostretchy/interface/mac/_stretch.dylib`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/src/audiostretchy/interface/tdhs.py` & `audiostretchy-1.3.5/src/audiostretchy/interface/tdhs.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/src/audiostretchy/interface/win/_stretch.dll` & `audiostretchy-1.3.5/src/audiostretchy/interface/win/_stretch.dll`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/src/audiostretchy/stretch.py` & `audiostretchy-1.3.5/src/audiostretchy/stretch.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
             import mp3
 
             encoder = mp3.Encoder(audio_file)
             encoder.set_bit_rate(bit_rate)
             encoder.set_sample_rate(self.framerate)
             encoder.set_channels(self.nchannels)
             encoder.set_quality(quality)
-            encoder.set_mod(
+            encoder.set_mode(
                 mp3.MODE_STEREO if nchannels == 2 else mp3.MODE_SINGLE_CHANNEL
             )
             encoder.write(self.pcm)
         except ImportError:
             from pydub import AudioSegment
 
             wav_io = BytesIO()
```

### Comparing `audiostretchy-1.3.4/src/audiostretchy.egg-info/PKG-INFO` & `audiostretchy-1.3.5/src/audiostretchy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.3.4
+Version: 1.3.5
 Summary: AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. AudioStretchy is a wrapper around the audio-stretch C library by David Bryant.
 Home-page: https://github.com/twardoch/audiostretchy
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -26,15 +26,15 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # AudioStretchy
 
 AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-_Version: 1.3.4_
+_Version: 1.3.5_
 
 ## Features
 
 - Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
@@ -173,14 +173,15 @@
 # This needs [all] installation for soxr support
 audio_stretch.resample(sample_rate=44100) 
 audio_stretch.save(file=WAVDataAsBytesIO, format="wav")
 ```
 
 ## Changelog
 
+- v1.3.5: fix for MP3 writing
 - v1.3.2: fix for MP3 opening
 - v1.3.0: actually working on Windows as well
 - v1.2.x: working on macOS and Linux
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
```

### Comparing `audiostretchy-1.3.4/src/audiostretchy.egg-info/SOURCES.txt` & `audiostretchy-1.3.5/src/audiostretchy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/tests/audio-1.2.mp3` & `audiostretchy-1.3.5/tests/audio-1.2.mp3`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/tests/audio-1.2.wav` & `audiostretchy-1.3.5/tests/audio-1.2.wav`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/tests/audio.mp3` & `audiostretchy-1.3.5/tests/audio.mp3`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.4/tests/audio.wav` & `audiostretchy-1.3.5/tests/audio.wav`

 * *Files identical despite different names*

