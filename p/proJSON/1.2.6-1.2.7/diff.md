# Comparing `tmp/proJSON-1.2.6.tar.gz` & `tmp/proJSON-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proJSON-1.2.6.tar", last modified: Sun Jun 25 13:47:16 2023, max compression
+gzip compressed data, was "proJSON-1.2.7.tar", last modified: Thu Jul  6 20:44:47 2023, max compression
```

## Comparing `proJSON-1.2.6.tar` & `proJSON-1.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:47:16.493633 proJSON-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-25 13:47:06.000000 proJSON-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-25 13:47:16.493633 proJSON-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-25 13:47:06.000000 proJSON-1.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-25 13:47:06.000000 proJSON-1.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 13:47:16.493633 proJSON-1.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:47:16.493633 proJSON-1.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:47:16.493633 proJSON-1.2.6/src/proJSON/
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-06-25 13:47:06.000000 proJSON-1.2.6/src/proJSON/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:47:16.493633 proJSON-1.2.6/src/proJSON.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-25 13:47:16.000000 proJSON-1.2.6/src/proJSON.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-25 13:47:16.000000 proJSON-1.2.6/src/proJSON.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 13:47:16.000000 proJSON-1.2.6/src/proJSON.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-25 13:47:16.000000 proJSON-1.2.6/src/proJSON.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 13:47:16.000000 proJSON-1.2.6/src/proJSON.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:47:16.493633 proJSON-1.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-25 13:47:06.000000 proJSON-1.2.6/tests/test_projson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:47.595867 proJSON-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-06 20:44:37.000000 proJSON-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-06 20:44:47.595867 proJSON-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-06 20:44:37.000000 proJSON-1.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-06 20:44:37.000000 proJSON-1.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:44:47.595867 proJSON-1.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:47.591867 proJSON-1.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:47.595867 proJSON-1.2.7/src/proJSON/
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-06 20:44:37.000000 proJSON-1.2.7/src/proJSON/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:47.595867 proJSON-1.2.7/src/proJSON.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-06 20:44:47.000000 proJSON-1.2.7/src/proJSON.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-06 20:44:47.000000 proJSON-1.2.7/src/proJSON.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:44:47.000000 proJSON-1.2.7/src/proJSON.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 20:44:47.000000 proJSON-1.2.7/src/proJSON.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 20:44:47.000000 proJSON-1.2.7/src/proJSON.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:47.595867 proJSON-1.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-06 20:44:37.000000 proJSON-1.2.7/tests/test_projson.py
```

### Comparing `proJSON-1.2.6/LICENSE` & `proJSON-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `proJSON-1.2.6/PKG-INFO` & `proJSON-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proJSON
-Version: 1.2.6
+Version: 1.2.7
 Summary: A python library to compress a dict into a bytearray.
 Author-email: JKinc <communications@jkinc.co.uk>
 Project-URL: Homepage, https://github.com/The-Geiger-Network-Project/proJSON/tree/main
 Project-URL: Bug Tracker, https://github.com/The-Geiger-Network-Project/proJSON/tree/main/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proJSON-1.2.6/README.md` & `proJSON-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `proJSON-1.2.6/pyproject.toml` & `proJSON-1.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proJSON"
-version = "1.2.6"
+version = "1.2.7"
 authors = [
   { name="JKinc", email="communications@jkinc.co.uk" },
 ]
 description = "A python library to compress a dict into a bytearray."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `proJSON-1.2.6/src/proJSON/__init__.py` & `proJSON-1.2.7/src/proJSON/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,36 +2,27 @@
 from zlib import compress, decompress
 from math import floor
 
 class Crafter:
     def __init__(self, proJSON, compression="lz4"):
         self.proJSON = proJSON
         if compression != "lz4" and compression != "zlib" and compression != "dev":
-            print(f"The compression type {self.compression} is not supported. The current options are lz4, zlib and dev (no compression)")
+            print(f"The compression type {compression} is not supported. The current options are lz4, zlib and dev (no compression)")
             print("If you believe this is an error, please submit a bug report at https://github.com/The-Geiger-Network-Project/proJSON/issues")
             print("Defaulting to lz4 compression")
             self.compression = "lz4"
         else:
             self.compression = compression
 
     def decode(self, data: bytes):
 
         if self.compression == "zlib":
             data = decompress(data)
         elif self.compression == "lz4":
-            if len(data) > 256:
-                context = frame.create_decompression_context()
-                decompressed = b""
-                for i in range(floor(len(data) / 256)):
-                    x, _, _ = frame.decompress_chunk(context, data[i*256:(i+1)*256])
-                    decompressed += x
-                x, _, _ = frame.decompress_chunk(context, data[floor(len(data) / 256):floor(len(data) / 256)+(len(data) % 256)])
-                decompressed += x
-            else:
-                decompressed = frame.decompress(data)
+            decompressed = frame.decompress(data)
                 
             data = decompressed
 
         ret = {}
         offset = 0
         for k, v in self.proJSON.items():
             if v["type"] == "int":
@@ -201,23 +192,15 @@
                         ret += b"\x01" if i else b"\x00"
 
                 ret += b"\xff"
 
         if self.compression == "zlib":
             ret = compress(ret)
         elif self.compression == "lz4":
-            if len(ret) > 256:
-                context = frame.create_compression_context()
-                compressed = frame.compress_begin(context)
-                for i in range(floor(len(ret) / 256)):
-                    compressed += frame.compress_chunk(context, ret[i*256:(i+1)*256])
-                compressed += frame.compress_chunk(context, ret[floor(len(ret) / 256):floor(len(ret) / 256)+(len(ret) % 256)])
-                compressed += frame.compress_flush(context)
-            else:
-                compressed = frame.compress(ret)
+            compressed = frame.compress(ret)
                 
             ret = compressed
                         
         return ret
     
 
 class InvalidType(BaseException):
```

### Comparing `proJSON-1.2.6/src/proJSON.egg-info/PKG-INFO` & `proJSON-1.2.7/src/proJSON.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proJSON
-Version: 1.2.6
+Version: 1.2.7
 Summary: A python library to compress a dict into a bytearray.
 Author-email: JKinc <communications@jkinc.co.uk>
 Project-URL: Homepage, https://github.com/The-Geiger-Network-Project/proJSON/tree/main
 Project-URL: Bug Tracker, https://github.com/The-Geiger-Network-Project/proJSON/tree/main/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proJSON-1.2.6/tests/test_projson.py` & `proJSON-1.2.7/tests/test_projson.py`

 * *Files identical despite different names*

