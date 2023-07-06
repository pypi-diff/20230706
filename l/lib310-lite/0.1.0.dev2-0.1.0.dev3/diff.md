# Comparing `tmp/lib310_lite-0.1.0.dev2.tar.gz` & `tmp/lib310_lite-0.1.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.1.0.dev2.tar", max compression
+gzip compressed data, was "lib310_lite-0.1.0.dev3.tar", max compression
```

## Comparing `lib310_lite-0.1.0.dev2.tar` & `lib310_lite-0.1.0.dev3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      253 2023-07-06 11:48:04.613198 lib310_lite-0.1.0.dev2/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.1.0.dev2/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7479 2023-05-12 13:53:49.135436 lib310_lite-0.1.0.dev2/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.1.0.dev2/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0    11688 2023-07-06 11:48:04.621257 lib310_lite-0.1.0.dev2/lib310_lite/laser/laser.py
--rw-r--r--   0        0        0      778 2023-07-06 11:48:04.617089 lib310_lite-0.1.0.dev2/pyproject.toml
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev2/setup.py
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0      253 2023-07-06 11:48:04.613198 lib310_lite-0.1.0.dev3/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.1.0.dev3/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7479 2023-05-12 13:53:49.135436 lib310_lite-0.1.0.dev3/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.1.0.dev3/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0    11752 2023-07-06 12:50:42.285615 lib310_lite-0.1.0.dev3/lib310_lite/laser/laser.py
+-rw-r--r--   0        0        0      778 2023-07-06 12:51:21.380002 lib310_lite-0.1.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev3/setup.py
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev3/PKG-INFO
```

### Comparing `lib310_lite-0.1.0.dev2/lib310_lite/bigquery/client.py` & `lib310_lite-0.1.0.dev3/lib310_lite/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.1.0.dev2/lib310_lite/bigquery/constants.py` & `lib310_lite-0.1.0.dev3/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.1.0.dev2/lib310_lite/laser/laser.py` & `lib310_lite-0.1.0.dev3/lib310_lite/laser/laser.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,8 +296,10 @@
 
         self.kill_fill_request_queue_thread.clear()
         self.kill_fill_response_queue_thread.clear()
 
         self.is_buffering = False
 
     def __del__(self):
+        if self.is_buffering:
+            self.stop_buffering()
         Laser.instances -= 1
```

### Comparing `lib310_lite-0.1.0.dev2/pyproject.toml` & `lib310_lite-0.1.0.dev3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.1.0.dev2"
+version = "0.1.0.dev3"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
```

### Comparing `lib310_lite-0.1.0.dev2/setup.py` & `lib310_lite-0.1.0.dev3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
  'mysqlclient>=2.0.0',
  'numpy<1.23.0']
 
 setup_kwargs = {
     'name': 'lib310-lite',
-    'version': '0.1.0.dev2',
+    'version': '0.1.0.dev3',
     'description': 'lib310 Lite Python Package',
     'long_description': 'None',
     'author': '310',
     'author_email': 'info@310.ai',
     'maintainer': 'Saman Fekri',
     'maintainer_email': 'saman@310.ai',
     'url': 'None',
```

### Comparing `lib310_lite-0.1.0.dev2/PKG-INFO` & `lib310_lite-0.1.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.1.0.dev2
+Version: 0.1.0.dev3
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
```

