# Comparing `tmp/audiostretchy-1.3.1.tar.gz` & `tmp/audiostretchy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostretchy-1.3.1.tar", last modified: Thu Jun 15 16:43:29 2023, max compression
+gzip compressed data, was "audiostretchy-1.3.2.tar", last modified: Thu Jul  6 11:04:15 2023, max compression
```

## Comparing `audiostretchy-1.3.1.tar` & `audiostretchy-1.3.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:43:29.144678 audiostretchy-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:43:29.132677 audiostretchy-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:43:29.140677 audiostretchy-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-06-15 16:43:29.144678 audiostretchy-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:43:29.140677 audiostretchy-1.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:43:29.140677 audiostretchy-1.3.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-15 16:43:29.148678 audiostretchy-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:43:29.136677 audiostretchy-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:43:29.140677 audiostretchy-1.3.1/src/audiostretchy/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/src/audiostretchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/src/audiostretchy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:43:29.140677 audiostretchy-1.3.1/src/audiostretchy/interface/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:43:29.140677 audiostretchy-1.3.1/src/audiostretchy/interface/linux/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/src/audiostretchy/interface/linux/_stretch.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:43:29.140677 audiostretchy-1.3.1/src/audiostretchy/interface/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/src/audiostretchy/interface/mac/_stretch.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/src/audiostretchy/interface/tdhs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:43:29.144678 audiostretchy-1.3.1/src/audiostretchy/interface/win/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/src/audiostretchy/interface/win/_stretch.def
--rw-r--r--   0 runner    (1001) docker     (123)   140288 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/src/audiostretchy/interface/win/_stretch.dll
--rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/src/audiostretchy/stretch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:43:29.140677 audiostretchy-1.3.1/src/audiostretchy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-06-15 16:43:29.000000 audiostretchy-1.3.1/src/audiostretchy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-15 16:43:29.000000 audiostretchy-1.3.1/src/audiostretchy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:43:29.000000 audiostretchy-1.3.1/src/audiostretchy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 16:43:29.000000 audiostretchy-1.3.1/src/audiostretchy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:43:28.000000 audiostretchy-1.3.1/src/audiostretchy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-15 16:43:29.000000 audiostretchy-1.3.1/src/audiostretchy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 16:43:29.000000 audiostretchy-1.3.1/src/audiostretchy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:43:29.144678 audiostretchy-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   198991 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/tests/audio-1.2.mp3
--rw-r--r--   0 runner    (1001) docker     (123)  1091644 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/tests/audio-1.2.wav
--rw-r--r--   0 runner    (1001) docker     (123)   132118 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/tests/audio.mp3
--rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/tests/audio.wav
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-15 16:43:15.000000 audiostretchy-1.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:04:15.414018 audiostretchy-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:04:15.402018 audiostretchy-1.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:04:15.406018 audiostretchy-1.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-07-06 11:04:15.414018 audiostretchy-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:04:15.406018 audiostretchy-1.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:04:15.410018 audiostretchy-1.3.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-06 11:04:15.414018 audiostretchy-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:04:15.402018 audiostretchy-1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:04:15.410018 audiostretchy-1.3.2/src/audiostretchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/src/audiostretchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/src/audiostretchy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:04:15.410018 audiostretchy-1.3.2/src/audiostretchy/interface/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:04:15.410018 audiostretchy-1.3.2/src/audiostretchy/interface/linux/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/src/audiostretchy/interface/linux/_stretch.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:04:15.410018 audiostretchy-1.3.2/src/audiostretchy/interface/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/src/audiostretchy/interface/mac/_stretch.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/src/audiostretchy/interface/tdhs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:04:15.410018 audiostretchy-1.3.2/src/audiostretchy/interface/win/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/src/audiostretchy/interface/win/_stretch.def
+-rw-r--r--   0 runner    (1001) docker     (123)   140288 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/src/audiostretchy/interface/win/_stretch.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/src/audiostretchy/stretch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:04:15.410018 audiostretchy-1.3.2/src/audiostretchy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-07-06 11:04:15.000000 audiostretchy-1.3.2/src/audiostretchy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-06 11:04:15.000000 audiostretchy-1.3.2/src/audiostretchy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:04:15.000000 audiostretchy-1.3.2/src/audiostretchy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 11:04:15.000000 audiostretchy-1.3.2/src/audiostretchy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:04:15.000000 audiostretchy-1.3.2/src/audiostretchy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-06 11:04:15.000000 audiostretchy-1.3.2/src/audiostretchy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 11:04:15.000000 audiostretchy-1.3.2/src/audiostretchy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:04:15.414018 audiostretchy-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   198991 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/tests/audio-1.2.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)  1091644 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/tests/audio-1.2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   132118 2023-07-06 11:04:01.000000 audiostretchy-1.3.2/tests/audio.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-07-06 11:04:02.000000 audiostretchy-1.3.2/tests/audio.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-06 11:04:02.000000 audiostretchy-1.3.2/tests/conftest.py
```

### Comparing `audiostretchy-1.3.1/.coveragerc` & `audiostretchy-1.3.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/.github/workflows/ci.yaml` & `audiostretchy-1.3.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/.gitignore` & `audiostretchy-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/.pre-commit-config.yaml` & `audiostretchy-1.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/.readthedocs.yml` & `audiostretchy-1.3.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/LICENSE.txt` & `audiostretchy-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/PKG-INFO` & `audiostretchy-1.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.3.1
+Version: 1.3.2
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
 
-_Version: **1.3.1** (actually working on Windows as well)_
+_Version: **1.3.2** 
 
 ## Features
 
 - Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
@@ -46,16 +46,16 @@
 
 The library gives very good results with speech recordings, especially with modest stretching at the ratio between 0.9 (10% slower) and 1.1 (10% faster). AudioStretchy is a Python wrapper around that library. The Python package also offers some additional, optional functionality: supports MP3 (in addition to WAV), and allows you to preform resampling.
 
 ## Demo
 
 Below are links to a short audio file (as WAV and MP3), with the same file stretched at 1.2 (20% slower):
 
-| Input                                                                              | Stretched                                                                                  |
-| ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
+| Input                                                                             | Stretched                                                                                 |
+| --------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
 | [`audio.wav`](https://github.com/twardoch/audiostretchy/raw/main/tests/audio.wav) | [`audio-1.2.wav`](https://github.com/twardoch/audiostretchy/raw/main/tests/audio-1.2.wav) |
 | [`audio.mp3`](https://github.com/twardoch/audiostretchy/raw/main/tests/audio.mp3) | [`audio-1.2.mp3`](https://github.com/twardoch/audiostretchy/raw/main/tests/audio-1.2.mp3) |
 
 
 ## Installation
 
 ### Full installation
@@ -173,14 +173,15 @@
 # This needs [all] installation for soxr support
 audio_stretch.resample(sample_rate=44100) 
 audio_stretch.save(file=WAVDataAsBytesIO, format="wav")
 ```
 
 ## Changelog
 
+- v1.3.2: fix for MP3 opening
 - v1.3.0: actually working on Windows as well
 - v1.2.x: working on macOS and Linux
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
 - [Python code](https://github.com/twardoch/audiostretchy): Copyright (c) 2023 Adam Twardoch
```

### Comparing `audiostretchy-1.3.1/README.md` & `audiostretchy-1.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AudioStretchy
 
 AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-_Version: **1.3.1** (actually working on Windows as well)_
+_Version: **1.3.2** 
 
 ## Features
 
 - Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
@@ -18,16 +18,16 @@
 
 The library gives very good results with speech recordings, especially with modest stretching at the ratio between 0.9 (10% slower) and 1.1 (10% faster). AudioStretchy is a Python wrapper around that library. The Python package also offers some additional, optional functionality: supports MP3 (in addition to WAV), and allows you to preform resampling.
 
 ## Demo
 
 Below are links to a short audio file (as WAV and MP3), with the same file stretched at 1.2 (20% slower):
 
-| Input                                                                              | Stretched                                                                                  |
-| ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
+| Input                                                                             | Stretched                                                                                 |
+| --------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
 | [`audio.wav`](https://github.com/twardoch/audiostretchy/raw/main/tests/audio.wav) | [`audio-1.2.wav`](https://github.com/twardoch/audiostretchy/raw/main/tests/audio-1.2.wav) |
 | [`audio.mp3`](https://github.com/twardoch/audiostretchy/raw/main/tests/audio.mp3) | [`audio-1.2.mp3`](https://github.com/twardoch/audiostretchy/raw/main/tests/audio-1.2.mp3) |
 
 
 ## Installation
 
 ### Full installation
@@ -145,14 +145,15 @@
 # This needs [all] installation for soxr support
 audio_stretch.resample(sample_rate=44100) 
 audio_stretch.save(file=WAVDataAsBytesIO, format="wav")
 ```
 
 ## Changelog
 
+- v1.3.2: fix for MP3 opening
 - v1.3.0: actually working on Windows as well
 - v1.2.x: working on macOS and Linux
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
 - [Python code](https://github.com/twardoch/audiostretchy): Copyright (c) 2023 Adam Twardoch
```

### Comparing `audiostretchy-1.3.1/docs/Makefile` & `audiostretchy-1.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/docs/conf.py` & `audiostretchy-1.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/docs/index.md` & `audiostretchy-1.3.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/setup.cfg` & `audiostretchy-1.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/setup.py` & `audiostretchy-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/src/audiostretchy/__init__.py` & `audiostretchy-1.3.2/src/audiostretchy/__init__.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/src/audiostretchy/interface/linux/_stretch.so` & `audiostretchy-1.3.2/src/audiostretchy/interface/linux/_stretch.so`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/src/audiostretchy/interface/mac/_stretch.dylib` & `audiostretchy-1.3.2/src/audiostretchy/interface/mac/_stretch.dylib`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/src/audiostretchy/interface/tdhs.py` & `audiostretchy-1.3.2/src/audiostretchy/interface/tdhs.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/src/audiostretchy/interface/win/_stretch.dll` & `audiostretchy-1.3.2/src/audiostretchy/interface/win/_stretch.dll`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/src/audiostretchy/stretch.py` & `audiostretchy-1.3.2/src/audiostretchy/stretch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from wave import Wave_read, Wave_write
 import wave
-import numpy as np
 from io import BytesIO
 from pathlib import Path
-from typing import Union, Tuple, BinaryIO, Optional
+from typing import BinaryIO, Optional, Tuple, Union
+from wave import Wave_read, Wave_write
+
+import numpy as np
+
 from .interface.tdhs import TDHSAudioStretch
 
 
 class AudioStretch:
     """
     Class to perform audio stretching operations.
     """
@@ -65,20 +67,21 @@
         Args:
             audio_file (BinaryIO): Binary I/O object of the audio file.
         """
         try:
             import mp3
 
             decoder = mp3.Decoder(audio_file)
-            with open(BytesIO(), "wb") as wav_io:
-                wav_file = Wave_write(wav_io)
-                wav_file.setnchannels(decoder.get_channels())
-                wav_file.setsampwidth(2)
-                wav_file.setframerate(decoder.get_sample_rate())
-                wav_file.writeframes(decoder.read())
+            wav_io = BytesIO()
+            wav_file = Wave_write(wav_io)
+            wav_file.setnchannels(decoder.get_channels())
+            wav_file.setsampwidth(2)
+            wav_file.setframerate(decoder.get_sample_rate())
+            wav_file.writeframes(decoder.read())
+            wav_io.seek(0)
             self.open_wav(wav_io)
         except ImportError:
             from pydub import AudioSegment
 
             audio = AudioSegment.from_file(audio_file, format="mp3")
             wav_io = BytesIO()
             audio.export(wav_io, format="wav")
@@ -327,31 +330,31 @@
     lower_freq: int = 55,
     buffer_ms: float = 25,
     threshold_gap_db: float = -40,
     double_range: bool = False,
     fast_detection: bool = False,
     normal_detection: bool = False,
     sample_rate: int = 0,
-    ):
+):
     """Stretches the input audio file and saves the result to the output path.
 
-Args:
-    input_path (str): The path to the input WAV or MP3 audio file.
-    output_path (str): The path to save the stretched WAV or MP3 audio file.
-    ratio (float, optional): The stretch ratio, where values greater than 1.0 will extend the audio and values less than 1.0 will shorten the audio. From 0.5 to 2.0, or with `-d` from 0.25 to 4.0. Default is 1.0 = no stretching.
-    gap_ratio (float, optional): The stretch ratio for gaps (silence) in the audio. Default is 0.0 = uses ratio.
-    upper_freq (int, optional): The upper frequency limit for period detection in Hz. Default is 333 Hz.
-    lower_freq (int, optional): The lower frequency limit. Default is 55 Hz.
-    buffer_ms (float, optional): The buffer size in milliseconds for processing the audio in chunks (useful with `-g`). Default is 25 ms.
-    threshold_gap_db (float, optional): The threshold level in dB to determine if a section of audio is considered a gap (for `-g`). Default is -40 dB.
-    double_range (bool, optional): If set, doubles the min/max range of stretching from 0.5-2.0 to 0.25-4.0. 
-    fast_detection (bool, optional): If set, enables fast period detection, which may speed up processing but reduce the quality of the stretched audio. 
-    normal_detection (bool, optional): If set, forces the algorithm to use normal period detection instead of fast period detection.
-    sample_rate (int, optional): The target sample rate for resampling the stretched audio in Hz (if installed with `[all]`). Default is 0 = use sample rate of the input audio.
-"""
+    Args:
+        input_path (str): The path to the input WAV or MP3 audio file.
+        output_path (str): The path to save the stretched WAV or MP3 audio file.
+        ratio (float, optional): The stretch ratio, where values greater than 1.0 will extend the audio and values less than 1.0 will shorten the audio. From 0.5 to 2.0, or with `-d` from 0.25 to 4.0. Default is 1.0 = no stretching.
+        gap_ratio (float, optional): The stretch ratio for gaps (silence) in the audio. Default is 0.0 = uses ratio.
+        upper_freq (int, optional): The upper frequency limit for period detection in Hz. Default is 333 Hz.
+        lower_freq (int, optional): The lower frequency limit. Default is 55 Hz.
+        buffer_ms (float, optional): The buffer size in milliseconds for processing the audio in chunks (useful with `-g`). Default is 25 ms.
+        threshold_gap_db (float, optional): The threshold level in dB to determine if a section of audio is considered a gap (for `-g`). Default is -40 dB.
+        double_range (bool, optional): If set, doubles the min/max range of stretching from 0.5-2.0 to 0.25-4.0.
+        fast_detection (bool, optional): If set, enables fast period detection, which may speed up processing but reduce the quality of the stretched audio.
+        normal_detection (bool, optional): If set, forces the algorithm to use normal period detection instead of fast period detection.
+        sample_rate (int, optional): The target sample rate for resampling the stretched audio in Hz (if installed with `[all]`). Default is 0 = use sample rate of the input audio.
+    """
     audio_stretch = AudioStretch()
     audio_stretch.open(input_path)
     audio_stretch.stretch(
         ratio,
         gap_ratio,
         upper_freq,
         lower_freq,
```

### Comparing `audiostretchy-1.3.1/src/audiostretchy.egg-info/PKG-INFO` & `audiostretchy-1.3.2/src/audiostretchy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.3.1
+Version: 1.3.2
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
 
-_Version: **1.3.1** (actually working on Windows as well)_
+_Version: **1.3.2** 
 
 ## Features
 
 - Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
@@ -46,16 +46,16 @@
 
 The library gives very good results with speech recordings, especially with modest stretching at the ratio between 0.9 (10% slower) and 1.1 (10% faster). AudioStretchy is a Python wrapper around that library. The Python package also offers some additional, optional functionality: supports MP3 (in addition to WAV), and allows you to preform resampling.
 
 ## Demo
 
 Below are links to a short audio file (as WAV and MP3), with the same file stretched at 1.2 (20% slower):
 
-| Input                                                                              | Stretched                                                                                  |
-| ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
+| Input                                                                             | Stretched                                                                                 |
+| --------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
 | [`audio.wav`](https://github.com/twardoch/audiostretchy/raw/main/tests/audio.wav) | [`audio-1.2.wav`](https://github.com/twardoch/audiostretchy/raw/main/tests/audio-1.2.wav) |
 | [`audio.mp3`](https://github.com/twardoch/audiostretchy/raw/main/tests/audio.mp3) | [`audio-1.2.mp3`](https://github.com/twardoch/audiostretchy/raw/main/tests/audio-1.2.mp3) |
 
 
 ## Installation
 
 ### Full installation
@@ -173,14 +173,15 @@
 # This needs [all] installation for soxr support
 audio_stretch.resample(sample_rate=44100) 
 audio_stretch.save(file=WAVDataAsBytesIO, format="wav")
 ```
 
 ## Changelog
 
+- v1.3.2: fix for MP3 opening
 - v1.3.0: actually working on Windows as well
 - v1.2.x: working on macOS and Linux
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
 - [Python code](https://github.com/twardoch/audiostretchy): Copyright (c) 2023 Adam Twardoch
```

### Comparing `audiostretchy-1.3.1/src/audiostretchy.egg-info/SOURCES.txt` & `audiostretchy-1.3.2/src/audiostretchy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/tests/audio-1.2.mp3` & `audiostretchy-1.3.2/tests/audio-1.2.mp3`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/tests/audio-1.2.wav` & `audiostretchy-1.3.2/tests/audio-1.2.wav`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/tests/audio.mp3` & `audiostretchy-1.3.2/tests/audio.mp3`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.3.1/tests/audio.wav` & `audiostretchy-1.3.2/tests/audio.wav`

 * *Files identical despite different names*

