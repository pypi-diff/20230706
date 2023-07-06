# Comparing `tmp/google_play_developer_api-0.6.0.tar.gz` & `tmp/google_play_developer_api-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_play_developer_api-0.6.0.tar", max compression
+gzip compressed data, was "google_play_developer_api-0.6.1.tar", max compression
```

## Comparing `google_play_developer_api-0.6.0.tar` & `google_play_developer_api-0.6.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-07-06 10:22:25.838872 google_play_developer_api-0.6.0/LICENSE
--rw-r--r--   0        0        0      858 2023-07-06 10:22:25.838872 google_play_developer_api-0.6.0/README.md
--rw-r--r--   0        0        0       78 2023-07-06 10:22:25.838872 google_play_developer_api-0.6.0/google_play_developer_api/__init__.py
--rw-r--r--   0        0        0    16184 2023-07-06 10:22:25.838872 google_play_developer_api-0.6.0/google_play_developer_api/reporting.py
--rw-r--r--   0        0        0     2697 2023-07-06 10:22:25.838872 google_play_developer_api-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-07-06 10:22:25.838872 google_play_developer_api-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     4037 2023-07-06 10:22:25.838872 google_play_developer_api-0.6.0/tests/test_reporting_apis.py
--rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 google_play_developer_api-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-06 10:46:39.691999 google_play_developer_api-0.6.1/LICENSE
+-rw-r--r--   0        0        0      934 2023-07-06 10:46:39.691999 google_play_developer_api-0.6.1/README.md
+-rw-r--r--   0        0        0       78 2023-07-06 10:46:39.695999 google_play_developer_api-0.6.1/google_play_developer_api/__init__.py
+-rw-r--r--   0        0        0    16184 2023-07-06 10:46:39.695999 google_play_developer_api-0.6.1/google_play_developer_api/reporting.py
+-rw-r--r--   0        0        0     2697 2023-07-06 10:46:39.695999 google_play_developer_api-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-07-06 10:46:39.695999 google_play_developer_api-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0     4037 2023-07-06 10:46:39.695999 google_play_developer_api-0.6.1/tests/test_reporting_apis.py
+-rw-r--r--   0        0        0     3043 1970-01-01 00:00:00.000000 google_play_developer_api-0.6.1/PKG-INFO
```

### Comparing `google_play_developer_api-0.6.0/LICENSE` & `google_play_developer_api-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google_play_developer_api-0.6.0/README.md` & `google_play_developer_api-0.6.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,8 +5,9 @@
 [![develop](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/dev.yml/badge.svg)](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/dev.yml)
 [![main](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/release.yml/badge.svg)](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/release.yml)
 
 Wrapper for APIs
 
 ## Features
 
-* Crash rate hourly report from Google Play Developer API
+* Crash rate hourly and daily report from Google Play Developer API
+* ANR rate hourly and daily report from Google Play Developer API
```

### Comparing `google_play_developer_api-0.6.0/google_play_developer_api/reporting.py` & `google_play_developer_api-0.6.1/google_play_developer_api/reporting.py`

 * *Files identical despite different names*

### Comparing `google_play_developer_api-0.6.0/pyproject.toml` & `google_play_developer_api-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "google-play-developer-api"
-version = "0.6.0"
+version = "0.6.1"
 homepage = "https://github.com/ikameglobal/google-play-developer-api"
 description = "Wrapper for APIs"
 authors = ["ikameglobal <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `google_play_developer_api-0.6.0/tests/test_reporting_apis.py` & `google_play_developer_api-0.6.1/tests/test_reporting_apis.py`

 * *Files identical despite different names*

### Comparing `google_play_developer_api-0.6.0/PKG-INFO` & `google_play_developer_api-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-play-developer-api
-Version: 0.6.0
+Version: 0.6.1
 Summary: Wrapper for APIs
 Home-page: https://github.com/ikameglobal/google-play-developer-api
 License: MIT
 Author: ikameglobal
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -50,9 +50,10 @@
 [![develop](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/dev.yml/badge.svg)](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/dev.yml)
 [![main](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/release.yml/badge.svg)](https://github.com/ikameglobal/google-play-developer-api/actions/workflows/release.yml)
 
 Wrapper for APIs
 
 ## Features
 
-* Crash rate hourly report from Google Play Developer API
+* Crash rate hourly and daily report from Google Play Developer API
+* ANR rate hourly and daily report from Google Play Developer API
```

