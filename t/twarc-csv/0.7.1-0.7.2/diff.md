# Comparing `tmp/twarc-csv-0.7.1.tar.gz` & `tmp/twarc-csv-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/twarc-csv-0.7.1.tar", last modified: Sun Jan  8 23:35:17 2023, max compression
+gzip compressed data, was "dist/twarc-csv-0.7.2.tar", last modified: Thu Jul  6 11:45:04 2023, max compression
```

## Comparing `twarc-csv-0.7.1.tar` & `twarc-csv-0.7.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 t495      (1000) t495      (1000)        0 2023-01-08 23:35:17.000000 twarc-csv-0.7.1/
--rw-rw-r--   0 t495      (1000) t495      (1000)     5057 2023-01-08 23:35:17.000000 twarc-csv-0.7.1/PKG-INFO
--rw-rw-r--   0 t495      (1000) t495      (1000)     3979 2023-01-08 23:31:39.000000 twarc-csv-0.7.1/README.md
--rw-rw-r--   0 t495      (1000) t495      (1000)     2638 2023-01-06 02:40:43.000000 twarc-csv-0.7.1/csv_writer.py
--rw-rw-r--   0 t495      (1000) t495      (1000)    18197 2023-01-08 23:23:44.000000 twarc-csv-0.7.1/dataframe_converter.py
--rw-rw-r--   0 t495      (1000) t495      (1000)      104 2023-01-08 23:35:17.000000 twarc-csv-0.7.1/setup.cfg
--rw-rw-r--   0 t495      (1000) t495      (1000)      798 2023-01-08 23:14:31.000000 twarc-csv-0.7.1/setup.py
-drwxrwxr-x   0 t495      (1000) t495      (1000)        0 2023-01-08 23:35:17.000000 twarc-csv-0.7.1/twarc_csv.egg-info/
--rw-rw-r--   0 t495      (1000) t495      (1000)     5057 2023-01-08 23:35:17.000000 twarc-csv-0.7.1/twarc_csv.egg-info/PKG-INFO
--rw-rw-r--   0 t495      (1000) t495      (1000)      278 2023-01-08 23:35:17.000000 twarc-csv-0.7.1/twarc_csv.egg-info/SOURCES.txt
--rw-rw-r--   0 t495      (1000) t495      (1000)        1 2023-01-08 23:35:17.000000 twarc-csv-0.7.1/twarc_csv.egg-info/dependency_links.txt
--rw-rw-r--   0 t495      (1000) t495      (1000)       55 2023-01-08 23:35:17.000000 twarc-csv-0.7.1/twarc_csv.egg-info/entry_points.txt
--rw-rw-r--   0 t495      (1000) t495      (1000)       63 2023-01-08 23:35:17.000000 twarc-csv-0.7.1/twarc_csv.egg-info/requires.txt
--rw-rw-r--   0 t495      (1000) t495      (1000)       41 2023-01-08 23:35:17.000000 twarc-csv-0.7.1/twarc_csv.egg-info/top_level.txt
--rw-rw-r--   0 t495      (1000) t495      (1000)     7509 2023-01-06 02:40:43.000000 twarc-csv-0.7.1/twarc_csv.py
+drwxrwxr-x   0 t495      (1000) t495      (1000)        0 2023-07-06 11:45:04.000000 twarc-csv-0.7.2/
+-rw-rw-r--   0 t495      (1000) t495      (1000)     5057 2023-07-06 11:45:04.000000 twarc-csv-0.7.2/PKG-INFO
+-rw-rw-r--   0 t495      (1000) t495      (1000)     3979 2023-07-06 11:40:23.000000 twarc-csv-0.7.2/README.md
+-rw-rw-r--   0 t495      (1000) t495      (1000)     2638 2023-01-06 02:40:43.000000 twarc-csv-0.7.2/csv_writer.py
+-rw-rw-r--   0 t495      (1000) t495      (1000)    18227 2023-07-06 11:44:10.000000 twarc-csv-0.7.2/dataframe_converter.py
+-rw-rw-r--   0 t495      (1000) t495      (1000)      104 2023-07-06 11:45:04.000000 twarc-csv-0.7.2/setup.cfg
+-rw-rw-r--   0 t495      (1000) t495      (1000)      798 2023-07-06 11:44:10.000000 twarc-csv-0.7.2/setup.py
+drwxrwxr-x   0 t495      (1000) t495      (1000)        0 2023-07-06 11:45:04.000000 twarc-csv-0.7.2/twarc_csv.egg-info/
+-rw-rw-r--   0 t495      (1000) t495      (1000)     5057 2023-07-06 11:45:04.000000 twarc-csv-0.7.2/twarc_csv.egg-info/PKG-INFO
+-rw-rw-r--   0 t495      (1000) t495      (1000)      278 2023-07-06 11:45:04.000000 twarc-csv-0.7.2/twarc_csv.egg-info/SOURCES.txt
+-rw-rw-r--   0 t495      (1000) t495      (1000)        1 2023-07-06 11:45:04.000000 twarc-csv-0.7.2/twarc_csv.egg-info/dependency_links.txt
+-rw-rw-r--   0 t495      (1000) t495      (1000)       55 2023-07-06 11:45:04.000000 twarc-csv-0.7.2/twarc_csv.egg-info/entry_points.txt
+-rw-rw-r--   0 t495      (1000) t495      (1000)       63 2023-07-06 11:45:04.000000 twarc-csv-0.7.2/twarc_csv.egg-info/requires.txt
+-rw-rw-r--   0 t495      (1000) t495      (1000)       41 2023-07-06 11:45:04.000000 twarc-csv-0.7.2/twarc_csv.egg-info/top_level.txt
+-rw-rw-r--   0 t495      (1000) t495      (1000)     7509 2023-01-06 02:40:43.000000 twarc-csv-0.7.2/twarc_csv.py
```

### Comparing `twarc-csv-0.7.1/PKG-INFO` & `twarc-csv-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twarc-csv
-Version: 0.7.1
+Version: 0.7.2
 Summary: A twarc plugin to output Twitter data as CSV
 Home-page: https://github.com/docnow/twarc-csv
 Author: Igor Brigadir
 Author-email: igor.brigadir@gmail.com
 License: UNKNOWN
 Description: # twarc-csv
```

### Comparing `twarc-csv-0.7.1/README.md` & `twarc-csv-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `twarc-csv-0.7.1/csv_writer.py` & `twarc-csv-0.7.2/csv_writer.py`

 * *Files identical despite different names*

### Comparing `twarc-csv-0.7.1/dataframe_converter.py` & `twarc-csv-0.7.2/dataframe_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 lang
 source
 public_metrics.impression_count
 public_metrics.reply_count
 public_metrics.retweet_count
 public_metrics.quote_count
 public_metrics.like_count
+public_metrics.bookmark_count
 reply_settings
 edit_history_tweet_ids
 edit_controls.edits_remaining
 edit_controls.editable_until
 edit_controls.is_edit_eligible
 possibly_sensitive
 withheld.scope
```

### Comparing `twarc-csv-0.7.1/setup.py` & `twarc-csv-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="twarc-csv",
-    version="0.7.1",
+    version="0.7.2",
     url="https://github.com/docnow/twarc-csv",
     author="Igor Brigadir",
     author_email="igor.brigadir@gmail.com",
     py_modules=["twarc_csv", "csv_writer", "dataframe_converter"],
     description="A twarc plugin to output Twitter data as CSV",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `twarc-csv-0.7.1/twarc_csv.egg-info/PKG-INFO` & `twarc-csv-0.7.2/twarc_csv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twarc-csv
-Version: 0.7.1
+Version: 0.7.2
 Summary: A twarc plugin to output Twitter data as CSV
 Home-page: https://github.com/docnow/twarc-csv
 Author: Igor Brigadir
 Author-email: igor.brigadir@gmail.com
 License: UNKNOWN
 Description: # twarc-csv
```

### Comparing `twarc-csv-0.7.1/twarc_csv.py` & `twarc-csv-0.7.2/twarc_csv.py`

 * *Files identical despite different names*

