# Comparing `tmp/magnify-0.3.3.tar.gz` & `tmp/magnify-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnify-0.3.3.tar", max compression
+gzip compressed data, was "magnify-0.3.4.tar", max compression
```

## Comparing `magnify-0.3.3.tar` & `magnify-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.3.3/README.md
--rw-r--r--   0        0        0     1650 2023-06-09 01:57:44.109149 magnify-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      246 2023-06-09 01:57:51.201276 magnify-0.3.3/src/magnify/__init__.py
--rw-r--r--   0        0        0     4571 2023-06-02 00:21:13.635636 magnify-0.3.3/src/magnify/filter.py
--rw-r--r--   0        0        0    26578 2023-06-02 00:21:04.883425 magnify-0.3.3/src/magnify/find.py
--rw-r--r--   0        0        0     3794 2023-06-09 01:57:30.532905 magnify-0.3.3/src/magnify/identify.py
--rw-r--r--   0        0        0     1406 2023-04-14 21:30:07.711891 magnify-0.3.3/src/magnify/pipeline.py
--rw-r--r--   0        0        0      317 2023-05-31 18:04:36.204183 magnify-0.3.3/src/magnify/plot/__init__.py
--rw-r--r--   0        0        0     2339 2023-06-02 00:19:24.832979 magnify-0.3.3/src/magnify/plot/image.py
--rw-r--r--   0        0        0     1855 2023-05-11 01:21:29.027397 magnify-0.3.3/src/magnify/plot/ndplot.py
--rw-r--r--   0        0        0     2483 2023-05-31 18:00:09.258919 magnify-0.3.3/src/magnify/plot/relation.py
--rw-r--r--   0        0        0      650 2023-05-11 02:30:53.591879 magnify-0.3.3/src/magnify/plot/style.py
--rw-r--r--   0        0        0     1017 2023-06-02 00:16:42.972866 magnify-0.3.3/src/magnify/postprocess.py
--rw-r--r--   0        0        0     1736 2023-04-14 21:30:15.276066 magnify-0.3.3/src/magnify/preprocess.py
--rw-r--r--   0        0        0    15093 2023-05-31 01:36:36.512603 magnify-0.3.3/src/magnify/reader.py
--rw-r--r--   0        0        0     3339 2023-06-02 00:16:33.476618 magnify-0.3.3/src/magnify/registry.py
--rw-r--r--   0        0        0     1077 2023-05-23 23:12:37.145369 magnify-0.3.3/src/magnify/stitch.py
--rw-r--r--   0        0        0     2639 2023-06-02 00:20:14.442200 magnify-0.3.3/src/magnify/utils.py
--rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 magnify-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.3.4/README.md
+-rw-r--r--   0        0        0     1650 2023-07-05 22:13:08.287843 magnify-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-07-05 22:13:20.828112 magnify-0.3.4/src/magnify/__init__.py
+-rw-r--r--   0        0        0     4571 2023-06-30 21:12:54.595829 magnify-0.3.4/src/magnify/filter.py
+-rw-r--r--   0        0        0    26578 2023-06-02 00:21:04.883425 magnify-0.3.4/src/magnify/find.py
+-rw-r--r--   0        0        0     7542 2023-06-30 20:57:39.570528 magnify-0.3.4/src/magnify/identify.py
+-rw-r--r--   0        0        0     1406 2023-04-14 21:30:07.711891 magnify-0.3.4/src/magnify/pipeline.py
+-rw-r--r--   0        0        0      317 2023-05-31 18:04:36.204183 magnify-0.3.4/src/magnify/plot/__init__.py
+-rw-r--r--   0        0        0     2339 2023-06-02 00:19:24.832979 magnify-0.3.4/src/magnify/plot/image.py
+-rw-r--r--   0        0        0     1855 2023-05-11 01:21:29.027397 magnify-0.3.4/src/magnify/plot/ndplot.py
+-rw-r--r--   0        0        0     2483 2023-05-31 18:00:09.258919 magnify-0.3.4/src/magnify/plot/relation.py
+-rw-r--r--   0        0        0      650 2023-05-11 02:30:53.591879 magnify-0.3.4/src/magnify/plot/style.py
+-rw-r--r--   0        0        0     1017 2023-06-02 00:16:42.972866 magnify-0.3.4/src/magnify/postprocess.py
+-rw-r--r--   0        0        0     1736 2023-04-14 21:30:15.276066 magnify-0.3.4/src/magnify/preprocess.py
+-rw-r--r--   0        0        0    15093 2023-07-05 22:12:57.343609 magnify-0.3.4/src/magnify/reader.py
+-rw-r--r--   0        0        0     3339 2023-06-30 21:12:59.455923 magnify-0.3.4/src/magnify/registry.py
+-rw-r--r--   0        0        0     1077 2023-05-23 23:12:37.145369 magnify-0.3.4/src/magnify/stitch.py
+-rw-r--r--   0        0        0     2639 2023-06-02 00:20:14.442200 magnify-0.3.4/src/magnify/utils.py
+-rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 magnify-0.3.4/PKG-INFO
```

### Comparing `magnify-0.3.3/pyproject.toml` & `magnify-0.3.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnify"
-version = "0.3.3"
+version = "0.3.4"
 description = "A microscopy image processing toolkit."
 authors = ["Karl Krauth <karl.krauth@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 opencv-python = [
```

### Comparing `magnify-0.3.3/src/magnify/filter.py` & `magnify-0.3.4/src/magnify/filter.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.3/src/magnify/find.py` & `magnify-0.3.4/src/magnify/find.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.3/src/magnify/pipeline.py` & `magnify-0.3.4/src/magnify/pipeline.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.3/src/magnify/plot/image.py` & `magnify-0.3.4/src/magnify/plot/image.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.3/src/magnify/plot/ndplot.py` & `magnify-0.3.4/src/magnify/plot/ndplot.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.3/src/magnify/plot/relation.py` & `magnify-0.3.4/src/magnify/plot/relation.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.3/src/magnify/plot/style.py` & `magnify-0.3.4/src/magnify/plot/style.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.3/src/magnify/postprocess.py` & `magnify-0.3.4/src/magnify/postprocess.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.3/src/magnify/preprocess.py` & `magnify-0.3.4/src/magnify/preprocess.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.3/src/magnify/reader.py` & `magnify-0.3.4/src/magnify/reader.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.3/src/magnify/registry.py` & `magnify-0.3.4/src/magnify/registry.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.3/src/magnify/stitch.py` & `magnify-0.3.4/src/magnify/stitch.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.3/src/magnify/utils.py` & `magnify-0.3.4/src/magnify/utils.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.3/PKG-INFO` & `magnify-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnify
-Version: 0.3.3
+Version: 0.3.4
 Summary: A microscopy image processing toolkit.
 Author: Karl Krauth
 Author-email: karl.krauth@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

