# Comparing `tmp/lib310_lite-0.1.0.dev1.tar.gz` & `tmp/lib310_lite-0.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.1.0.dev1.tar", max compression
+gzip compressed data, was "lib310_lite-0.1.0.dev2.tar", max compression
```

## Comparing `lib310_lite-0.1.0.dev1.tar` & `lib310_lite-0.1.0.dev2.tar`

### file list

```diff
@@ -1,12 +1,8 @@
--rw-r--r--   0        0        0      289 2023-07-05 13:20:23.360374 lib310_lite-0.1.0.dev1/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.1.0.dev1/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7479 2023-05-12 13:53:49.135436 lib310_lite-0.1.0.dev1/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.1.0.dev1/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.1.0.dev1/lib310_lite/fucntion.py
--rw-r--r--   0        0        0    11378 2023-07-05 14:19:15.712417 lib310_lite-0.1.0.dev1/lib310_lite/laser/laser.py
--rw-r--r--   0        0        0    12905 2023-05-31 18:31:27.737763 lib310_lite-0.1.0.dev1/lib310_lite/mldl/mldl.py
--rw-r--r--   0        0        0     1528 2023-05-12 10:35:08.523571 lib310_lite-0.1.0.dev1/lib310_lite/mldl/models/InteractionModel.py
--rw-r--r--   0        0        0     2818 2023-05-12 10:35:08.531397 lib310_lite-0.1.0.dev1/lib310_lite/mldl/models/SeqLangModel.py
--rw-r--r--   0        0        0      828 2023-07-06 08:28:45.013372 lib310_lite-0.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0      987 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev1/setup.py
--rw-r--r--   0        0        0      934 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0      253 2023-07-06 11:48:04.613198 lib310_lite-0.1.0.dev2/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.1.0.dev2/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7479 2023-05-12 13:53:49.135436 lib310_lite-0.1.0.dev2/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.1.0.dev2/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0    11688 2023-07-06 11:48:04.621257 lib310_lite-0.1.0.dev2/lib310_lite/laser/laser.py
+-rw-r--r--   0        0        0      778 2023-07-06 11:48:04.617089 lib310_lite-0.1.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev2/setup.py
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev2/PKG-INFO
```

### Comparing `lib310_lite-0.1.0.dev1/lib310_lite/bigquery/client.py` & `lib310_lite-0.1.0.dev2/lib310_lite/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.1.0.dev1/lib310_lite/bigquery/constants.py` & `lib310_lite-0.1.0.dev2/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.1.0.dev1/lib310_lite/laser/laser.py` & `lib310_lite-0.1.0.dev2/lib310_lite/laser/laser.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,14 @@
         pass
         self.pool_hash = h
 
         cnx = None
         cursor = None
         try:
             # Establish a connection to the database
-            print("Getting pool 1")
             cnx = MySQLdb.connect(**self.db_config)
             cursor = cnx.cursor()
             # check if the query is already in the database
             cursor.execute("SELECT * FROM cached WHERE hash = %s", (h,))
             result = cursor.fetchone()
             if result is None:
                 raise Exception("Pool does not exist")
@@ -280,18 +279,25 @@
         """
         self.kill_fill_request_queue_thread.set()
         self.kill_fill_response_queue_thread.set()
 
         if self.fill_request_queue_thread is not None:
             if not self.request_queue.empty():
                 self.request_queue.get()
-            self.fill_request_queue_thread.join()
+            self.fill_request_queue_thread.join(10)
+            if self.fill_request_queue_thread.is_alive():
+                self.fill_request_queue_thread.terminate()
 
         if self.fill_response_queue_thread is not None:
             if not self.response_queue.empty():
                 self.response_queue.get()
-            self.fill_response_queue_thread.join()
+            self.fill_response_queue_thread.join(10)
+            if self.fill_response_queue_thread.is_alive():
+                self.fill_response_queue_thread.terminate()
+
+        self.kill_fill_request_queue_thread.clear()
+        self.kill_fill_response_queue_thread.clear()
 
         self.is_buffering = False
 
     def __del__(self):
         Laser.instances -= 1
```

### Comparing `lib310_lite-0.1.0.dev1/pyproject.toml` & `lib310_lite-0.1.0.dev2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.1.0.dev1"
+version = "0.1.0.dev2"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
@@ -17,16 +17,14 @@
 db-dtypes = ">=1.0.0"
 numpy = "<1.23.0"
 bounded_pool_executor = ">=0.0.0"
 dask = ">=2022.11.0"
 distributed = ">=2022.11.0"
 dask-sql = ">=2022.11.0"
 gcsfs = ">=2022.11.0"
-SQLAlchemy = ">=2.0.0"
-psycopg2-binary= ">=2.9.0"
 mysqlclient = ">=2.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">7.1.2"
 python-dotenv = ">=0.19.0"
```

### Comparing `lib310_lite-0.1.0.dev1/setup.py` & `lib310_lite-0.1.0.dev2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['lib310_lite',
- 'lib310_lite.bigquery',
- 'lib310_lite.laser',
- 'lib310_lite.mldl',
- 'lib310_lite.mldl.models']
+['lib310_lite', 'lib310_lite.bigquery', 'lib310_lite.laser']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['SQLAlchemy>=2.0.0',
- 'bounded_pool_executor>=0.0.0',
+['bounded_pool_executor>=0.0.0',
  'dask-sql>=2022.11.0',
  'dask>=2022.11.0',
  'db-dtypes>=1.0.0',
  'distributed>=2022.11.0',
  'gcsfs>=2022.11.0',
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
  'mysqlclient>=2.0.0',
- 'numpy<1.23.0',
- 'psycopg2-binary>=2.9.0']
+ 'numpy<1.23.0']
 
 setup_kwargs = {
     'name': 'lib310-lite',
-    'version': '0.1.0.dev1',
+    'version': '0.1.0.dev2',
     'description': 'lib310 Lite Python Package',
     'long_description': 'None',
     'author': '310',
     'author_email': 'info@310.ai',
     'maintainer': 'Saman Fekri',
     'maintainer_email': 'saman@310.ai',
     'url': 'None',
```

### Comparing `lib310_lite-0.1.0.dev1/PKG-INFO` & `lib310_lite-0.1.0.dev2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: SQLAlchemy (>=2.0.0)
 Requires-Dist: bounded_pool_executor (>=0.0.0)
 Requires-Dist: dask (>=2022.11.0)
 Requires-Dist: dask-sql (>=2022.11.0)
 Requires-Dist: db-dtypes (>=1.0.0)
 Requires-Dist: distributed (>=2022.11.0)
 Requires-Dist: gcsfs (>=2022.11.0)
 Requires-Dist: google-cloud (>=0.34.0)
 Requires-Dist: google-cloud-bigquery (>=3.2.0)
 Requires-Dist: mysqlclient (>=2.0.0)
 Requires-Dist: numpy (<1.23.0)
-Requires-Dist: psycopg2-binary (>=2.9.0)
```

