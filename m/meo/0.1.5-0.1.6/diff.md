# Comparing `tmp/meo-0.1.5.tar.gz` & `tmp/meo-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meo-0.1.5.tar", last modified: Mon Jun 26 07:34:16 2023, max compression
+gzip compressed data, was "meo-0.1.6.tar", last modified: Thu Jul  6 11:56:02 2023, max compression
```

## Comparing `meo-0.1.5.tar` & `meo-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-26 07:34:16.606138 meo-0.1.5/
--rw-r--r--   0 meo       (1000) meo       (1000)     1066 2023-06-24 09:52:08.000000 meo-0.1.5/LICENSE
--rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-26 07:34:16.606138 meo-0.1.5/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)      317 2023-06-24 09:52:08.000000 meo-0.1.5/README.md
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-26 07:34:16.602805 meo-0.1.5/meo/
--rw-r--r--   0 meo       (1000) meo       (1000)      134 2023-06-26 06:49:06.000000 meo-0.1.5/meo/__init__.py
--rw-r--r--   0 meo       (1000) meo       (1000)      302 2023-06-26 07:34:02.000000 meo-0.1.5/meo/__version__.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-26 07:34:16.602805 meo-0.1.5/meo/crack/
--rw-r--r--   0 meo       (1000) meo       (1000)      237 2023-06-26 07:10:23.000000 meo-0.1.5/meo/crack/__init__.py
--rw-r--r--   0 meo       (1000) meo       (1000)     4833 2023-06-26 06:40:46.000000 meo-0.1.5/meo/crack/cracker.py
--rw-r--r--   0 meo       (1000) meo       (1000)      749 2023-06-26 07:31:01.000000 meo-0.1.5/meo/crack/pdf.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1076 2023-06-25 19:31:21.000000 meo-0.1.5/meo/crack/utils.py
--rw-r--r--   0 meo       (1000) meo       (1000)      985 2023-06-26 07:29:34.000000 meo-0.1.5/meo/crack/zip.py
--rw-r--r--   0 meo       (1000) meo       (1000)      576 2023-06-24 09:52:08.000000 meo-0.1.5/meo/flask.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2671 2023-06-26 07:24:35.000000 meo-0.1.5/meo/io.py
--rw-r--r--   0 meo       (1000) meo       (1000)      823 2023-06-24 12:10:37.000000 meo-0.1.5/meo/net.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2228 2023-06-24 10:20:41.000000 meo-0.1.5/meo/screen.py
--rw-r--r--   0 meo       (1000) meo       (1000)      167 2023-06-24 09:52:08.000000 meo-0.1.5/meo/utils.py
--rw-r--r--   0 meo       (1000) meo       (1000)      332 2023-06-26 06:59:04.000000 meo-0.1.5/meo/wapper.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-26 07:34:16.602805 meo-0.1.5/meo.egg-info/
--rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-26 07:34:16.000000 meo-0.1.5/meo.egg-info/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)      415 2023-06-26 07:34:16.000000 meo-0.1.5/meo.egg-info/SOURCES.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-06-26 07:34:16.000000 meo-0.1.5/meo.egg-info/dependency_links.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       27 2023-06-26 07:34:16.000000 meo-0.1.5/meo.egg-info/requires.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        4 2023-06-26 07:34:16.000000 meo-0.1.5/meo.egg-info/top_level.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-06-26 07:34:16.606138 meo-0.1.5/setup.cfg
--rwxr-xr-x   0 meo       (1000) meo       (1000)     1361 2023-06-25 19:31:21.000000 meo-0.1.5/setup.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-26 07:34:16.602805 meo-0.1.5/test/
--rw-r--r--   0 meo       (1000) meo       (1000)      310 2023-06-26 07:30:54.000000 meo-0.1.5/test/test.py
--rw-r--r--   0 meo       (1000) meo       (1000)      355 2023-06-25 19:31:21.000000 meo-0.1.5/test/test_crack.py
--rw-r--r--   0 meo       (1000) meo       (1000)      143 2023-06-25 19:31:21.000000 meo-0.1.5/test/test_imp.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-06 11:56:02.589948 meo-0.1.6/
+-rw-r--r--   0 meo       (1000) meo       (1000)     1066 2023-07-01 13:29:07.000000 meo-0.1.6/LICENSE
+-rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-07-06 11:56:02.589948 meo-0.1.6/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      317 2023-07-01 13:29:07.000000 meo-0.1.6/README.md
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-06 11:56:02.586614 meo-0.1.6/meo/
+-rw-r--r--   0 meo       (1000) meo       (1000)      134 2023-07-01 13:29:07.000000 meo-0.1.6/meo/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      302 2023-07-06 11:55:44.000000 meo-0.1.6/meo/__version__.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-06 11:56:02.589948 meo-0.1.6/meo/crack/
+-rw-r--r--   0 meo       (1000) meo       (1000)      237 2023-07-01 13:29:07.000000 meo-0.1.6/meo/crack/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     5317 2023-07-01 13:29:07.000000 meo-0.1.6/meo/crack/cracker.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      725 2023-07-01 13:29:07.000000 meo-0.1.6/meo/crack/pdf.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     1076 2023-07-01 13:29:07.000000 meo-0.1.6/meo/crack/utils.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     1046 2023-07-01 13:29:07.000000 meo-0.1.6/meo/crack/zip.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      576 2023-07-01 13:29:07.000000 meo-0.1.6/meo/flask.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2671 2023-07-01 13:29:07.000000 meo-0.1.6/meo/io.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      823 2023-07-01 13:29:07.000000 meo-0.1.6/meo/net.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2228 2023-07-01 13:29:07.000000 meo-0.1.6/meo/screen.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      375 2023-07-06 11:55:15.000000 meo-0.1.6/meo/utils.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      332 2023-07-01 13:29:07.000000 meo-0.1.6/meo/wapper.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-06 11:56:02.586614 meo-0.1.6/meo.egg-info/
+-rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-07-06 11:56:02.000000 meo-0.1.6/meo.egg-info/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      415 2023-07-06 11:56:02.000000 meo-0.1.6/meo.egg-info/SOURCES.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-07-06 11:56:02.000000 meo-0.1.6/meo.egg-info/dependency_links.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       27 2023-07-06 11:56:02.000000 meo-0.1.6/meo.egg-info/requires.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        4 2023-07-06 11:56:02.000000 meo-0.1.6/meo.egg-info/top_level.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-07-06 11:56:02.589948 meo-0.1.6/setup.cfg
+-rwxr-xr-x   0 meo       (1000) meo       (1000)     1361 2023-07-01 13:29:07.000000 meo-0.1.6/setup.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-06 11:56:02.589948 meo-0.1.6/test/
+-rw-r--r--   0 meo       (1000) meo       (1000)      435 2023-07-01 13:29:07.000000 meo-0.1.6/test/test.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      355 2023-07-01 13:29:07.000000 meo-0.1.6/test/test_crack.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      143 2023-07-01 13:29:07.000000 meo-0.1.6/test/test_imp.py
```

### Comparing `meo-0.1.5/LICENSE` & `meo-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `meo-0.1.5/PKG-INFO` & `meo-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meo
-Version: 0.1.5
+Version: 0.1.6
 Summary: frequently-used function library
 Home-page: http://github.com/miaobuao/meo
 Author: miaobuao
 Author-email: miaobuao@outlook.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `meo-0.1.5/meo/crack/cracker.py` & `meo-0.1.6/meo/crack/cracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,79 @@
 import multiprocessing
 import gc
+import threading
 import os
-from .utils import *
 from tqdm.asyncio import tqdm
 import itertools
 import asyncio
+import time
+from .utils import *
+
+
 
 class Cracker:
     
     def __init__(self, path: str) -> None:
         assert os.path.exists(path)
         self.path = path
 
-    def in_multiprocess_by_seed(self, seed=PWD_SEED_COMPLEX, min_length=None, max_length=None, n_processes=8, slice_size=500, progressbar=False):
+    def in_multiprocess_by_seed(self, seed=PWD_SEED_COMPLEX, 
+            min_length=None, max_length=None, n_processes=None, slice_size=500,
+            gc_interval=2, progressbar=False):
         pool = multiprocessing.Pool(n_processes)
         it = key_generator(seed, min_length, max_length)
         manager = multiprocessing.Manager()
         info = manager.dict()
         info['key'] = None
         if progressbar:
             bar = tqdm(mininterval=0.25)
         def cb(re):
             if progressbar:
                 bar.update(slice_size)
             if re:
                 info['key'] = re
                 pool.terminate()
+        def create_gc_timer():
+            gc_timer = threading.Timer(gc_interval, create_gc_timer)
+            gc_timer.start()
+            gc.collect()
+        # create_gc_timer()
+        gc_cnt = 1
         while True:
             try:
-                pwds = itertools.islice(it, 0, slice_size)
-                if pwds := list(pwds):
-                    pwds, char_sizes = list(zip(*pwds))
+                pwds_slice = itertools.islice(it, 0, slice_size)
+                if pwds_list := list(pwds_slice):
+                    pwds, char_sizes = list(zip(*pwds_list))
                     char_size = char_sizes[-1]
                     pool.apply_async(self.step_some, (*pwds, ), callback=cb, error_callback=print)
                     del pwds
+                    del pwds_list
                     del char_sizes
                 else:
                     pool.close()
                     pool.join()
                     pool.terminate()
                     return info['key']
+                del pwds_slice
             except Exception as e:
                 if e.args[0] == 'Pool not running':
                     return info['key']
                 else:
                     raise e
             if progressbar:
                 bar.set_postfix({
                     "char": char_size
                 }, refresh=False)
-            gc.collect()
+            if gc_cnt % gc_interval == 0:
+                gc.collect()
+                gc_cnt = 1
+            else:
+                gc_cnt += 1
 
-    def in_multiprocess_by_book(self, book:list, n_processes=8, chunksize=1000):
+    def in_multiprocess_by_book(self, book:list, n_processes=None, chunksize=1000):
         pool = multiprocessing.Pool(n_processes)
         manager = multiprocessing.Manager()
         info = manager.dict()
         info['key'] = None
         def cb(pwds):
             pwds = filter(None, pwds)
             for pwd in pwds:
```

### Comparing `meo-0.1.5/meo/crack/pdf.py` & `meo-0.1.6/meo/crack/pdf.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from pikepdf import Pdf, PasswordError
 from .cracker import Cracker
-from ..io import encode
 
 class PdfCracker(Cracker):
     def remove_pdf_password(self, output_path: str, pwd=b''):
         with Pdf.open(self.path, password=pwd) as f:
             f.save(output_path)
             
     def test(self, pwd=b''):
```

### Comparing `meo-0.1.5/meo/crack/utils.py` & `meo-0.1.6/meo/crack/utils.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.5/meo/crack/zip.py` & `meo-0.1.6/meo/crack/zip.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,21 @@
         except:
             return False
 
     def step_once(self, pwd: bytes) -> bytes | None:
         zfile = ZipFile(self.path)
         mem = zfile.filelist[0].filename
         if self.test(zfile, pwd, mem):
+            del pwd
             return pwd
+        del pwd
         return None
     
     def step_some(self, *pwds: bytes) -> bytes | None:
         zfile = ZipFile(self.path)
         mem = zfile.filelist[0].filename
         for pwd in pwds:
             if self.test(zfile, pwd, mem):
+                del pwds
                 return pwd
         del pwds
         return None
```

### Comparing `meo-0.1.5/meo/flask.py` & `meo-0.1.6/meo/flask.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.5/meo/io.py` & `meo-0.1.6/meo/io.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.5/meo/net.py` & `meo-0.1.6/meo/net.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.5/meo/screen.py` & `meo-0.1.6/meo/screen.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.5/meo.egg-info/PKG-INFO` & `meo-0.1.6/meo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meo
-Version: 0.1.5
+Version: 0.1.6
 Summary: frequently-used function library
 Home-page: http://github.com/miaobuao/meo
 Author: miaobuao
 Author-email: miaobuao@outlook.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `meo-0.1.5/setup.py` & `meo-0.1.6/setup.py`

 * *Files identical despite different names*

