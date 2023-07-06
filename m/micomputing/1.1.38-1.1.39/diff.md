# Comparing `tmp/micomputing-1.1.38.tar.gz` & `tmp/micomputing-1.1.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micomputing-1.1.38.tar", last modified: Thu Jul  6 12:58:09 2023, max compression
+gzip compressed data, was "micomputing-1.1.39.tar", last modified: Thu Jul  6 15:29:04 2023, max compression
```

## Comparing `micomputing-1.1.38.tar` & `micomputing-1.1.39.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:09.231960 micomputing-1.1.38/
--rw-r--r--   0 admin      (501) staff       (20)       99 2023-07-06 12:58:09.000000 micomputing-1.1.38/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-06 12:58:09.231828 micomputing-1.1.38/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-06 12:58:09.000000 micomputing-1.1.38/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:09.229625 micomputing-1.1.38/micomputing/
--rw-r--r--   0 admin      (501) staff       (20)     2360 2023-07-06 12:58:08.000000 micomputing-1.1.38/micomputing/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing/data.py
--rw-r--r--   0 admin      (501) staff       (20)    38276 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing/funcs.py
--rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-06 12:58:08.000000 micomputing-1.1.38/micomputing/metrics.py
--rwxr-xr-x   0 admin      (501) staff       (20)    33404 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing/micfunctions.so
--rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing/network.py
--rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-06 12:58:08.000000 micomputing-1.1.38/micomputing/plot.py
--rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing/stdio.py
--rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing/test.py
--rw-r--r--   0 admin      (501) staff       (20)    98904 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing/trans.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:09.231029 micomputing-1.1.38/micomputing/zxhtools/
--rw-r--r--   0 admin      (501) staff       (20)     7454 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing/zxhtools/TRS.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:09.231616 micomputing-1.1.38/micomputing/zxhtools/__pycache__/
--rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     9153 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc
--rw-r--r--   0 admin      (501) staff       (20)     8988 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     8071 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing/zxhtools/exec.py
--rw-r--r--   0 admin      (501) staff       (20)      507 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing/zxhtools/image2.AFF
--rw-r--r--   0 admin      (501) staff       (20)    21032 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing/zxhtools/image2.FFD
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:09.230512 micomputing-1.1.38/micomputing.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       72 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       12 2023-07-06 12:58:09.000000 micomputing-1.1.38/micomputing.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-06 12:58:09.232012 micomputing-1.1.38/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1482 2023-07-06 12:58:09.000000 micomputing-1.1.38/setup_micomputing.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 15:29:04.044078 micomputing-1.1.39/
+-rw-r--r--   0 admin      (501) staff       (20)       99 2023-07-06 15:29:03.000000 micomputing-1.1.39/MANIFEST.in
+-rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-06 15:29:04.043914 micomputing-1.1.39/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-06 15:29:03.000000 micomputing-1.1.39/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 15:29:04.041682 micomputing-1.1.39/micomputing/
+-rw-r--r--   0 admin      (501) staff       (20)     2360 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/data.py
+-rw-r--r--   0 admin      (501) staff       (20)    38276 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/funcs.py
+-rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/metrics.py
+-rwxr-xr-x   0 admin      (501) staff       (20)    33404 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/micfunctions.so
+-rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/network.py
+-rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/plot.py
+-rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/stdio.py
+-rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/test.py
+-rw-r--r--   0 admin      (501) staff       (20)    98915 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/trans.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 15:29:04.043037 micomputing-1.1.39/micomputing/zxhtools/
+-rw-r--r--   0 admin      (501) staff       (20)     7454 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/zxhtools/TRS.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 15:29:04.043624 micomputing-1.1.39/micomputing/zxhtools/__pycache__/
+-rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     9153 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     8988 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     8071 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/zxhtools/exec.py
+-rw-r--r--   0 admin      (501) staff       (20)      507 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/zxhtools/image2.AFF
+-rw-r--r--   0 admin      (501) staff       (20)    21032 2023-07-06 15:29:03.000000 micomputing-1.1.39/micomputing/zxhtools/image2.FFD
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 15:29:04.042467 micomputing-1.1.39/micomputing.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-06 15:29:04.000000 micomputing-1.1.39/micomputing.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-06 15:29:04.000000 micomputing-1.1.39/micomputing.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-06 15:29:04.000000 micomputing-1.1.39/micomputing.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       72 2023-07-06 15:29:04.000000 micomputing-1.1.39/micomputing.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       12 2023-07-06 15:29:04.000000 micomputing-1.1.39/micomputing.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-06 15:29:04.044134 micomputing-1.1.39/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1482 2023-07-06 15:29:03.000000 micomputing-1.1.39/setup_micomputing.py
```

### Comparing `micomputing-1.1.38/PKG-INFO` & `micomputing-1.1.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micomputing
-Version: 1.1.38
+Version: 1.1.39
 Summary: 'micomputing' is a package for medical image computing. 
 Home-page: https://github.com/Bertie97/PyZMyc/micomputing
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # MIComputing
```

### Comparing `micomputing-1.1.38/README.md` & `micomputing-1.1.39/README.md`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/micomputing/__init__.py` & `micomputing-1.1.39/micomputing/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = 'micomputing',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.1.37',
+    version = '1.1.38',
     contact = 'bertiezhou@163.com',
     keywords = ['medical image', 'image registration', 'image similarities'],
     description = "'micomputing' is a package for medical image computing. ",
     requires = ['numpy', 'torch>=1.5.1', 'batorch', 'pycamia', 'pyoverload', 'nibabel', 'pydicom', 'SimpleITK'],
-    update = '2023-07-05 17:05:57',
+    update = '2023-07-06 20:58:08',
     package_data = True
 ).check()
 
 from . import plot as plt
 from .stdio import IMG, dcm2nii, nii2dcm #*
 from .data import Info, Subject, ImageObject, Dataset, MedicalDataset #*
 from .network import U_Net, CNN, FCN
```

### Comparing `micomputing-1.1.38/micomputing/data.py` & `micomputing-1.1.39/micomputing/data.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/micomputing/funcs.py` & `micomputing-1.1.39/micomputing/funcs.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/micomputing/metrics.py` & `micomputing-1.1.39/micomputing/metrics.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/micomputing/micfunctions.so` & `micomputing-1.1.39/micomputing/micfunctions.so`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/micomputing/network.py` & `micomputing-1.1.39/micomputing/network.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/micomputing/plot.py` & `micomputing-1.1.39/micomputing/plot.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/micomputing/stdio.py` & `micomputing-1.1.39/micomputing/stdio.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/micomputing/test.py` & `micomputing-1.1.39/micomputing/test.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/micomputing/trans.py` & `micomputing-1.1.39/micomputing/trans.py`

 * *Files 0% similar despite different names*

```diff
@@ -4901,1282 +4901,1283 @@
 00013240: 2020 2072 6574 7572 6e20 696e 7465 7270     return interp
 00013250: 6f6c 6174 696f 6e5f 666f 7277 6172 6428  olation_forward(
 00013260: 696d 6167 652c 2074 7261 6e73 2c20 6d65  image, trans, me
 00013270: 7468 6f64 203d 206d 6574 686f 642c 2074  thod = method, t
 00013280: 6172 6765 745f 7370 6163 6520 3d20 7461  arget_space = ta
 00013290: 7267 6574 5f73 7061 6365 2c20 6669 6c6c  rget_space, fill
 000132a0: 203d 2066 696c 6c29 0a20 2020 2069 6d61   = fill).    ima
-000132b0: 6765 203d 2062 6174 6f72 6368 5f74 656e  ge = batorch_ten
-000132c0: 736f 7228 696d 6167 6529 0a20 2020 2073  sor(image).    s
-000132d0: 6861 7065 5f6f 7574 203d 2069 6d61 6765  hape_out = image
-000132e0: 2e73 6861 7065 0a20 2020 2069 6620 7472  .shape.    if tr
-000132f0: 616e 7320 6973 204e 6f6e 6520 6f72 2074  ans is None or t
-00013300: 7261 6e73 2e6e 5f64 696d 2069 7320 4e6f  rans.n_dim is No
-00013310: 6e65 3a0a 2020 2020 2020 2020 6966 206e  ne:.        if n
-00013320: 6f74 2069 6d61 6765 2e68 6173 5f62 6174  ot image.has_bat
-00013330: 6368 3a20 696d 6167 652e 756e 7371 7565  ch: image.unsque
-00013340: 657a 655f 285b 5d29 0a20 2020 2020 2020  eze_([]).       
-00013350: 2069 6620 6e6f 7420 696d 6167 652e 6861   if not image.ha
-00013360: 735f 6368 616e 6e65 6c3a 2069 6d61 6765  s_channel: image
-00013370: 2e73 7461 6e64 6172 645f 2829 2e75 6e73  .standard_().uns
-00013380: 7175 6565 7a65 5f28 7b31 7d29 0a20 2020  queeze_({1}).   
-00013390: 2020 2020 206e 5f64 696d 203d 2069 6d61       n_dim = ima
-000133a0: 6765 2e6e 5f73 7061 6365 2023 2047 6574  ge.n_space # Get
-000133b0: 2074 6865 2073 7061 7469 616c 2072 616e   the spatial ran
-000133c0: 6b2e 0a20 2020 2065 6c73 653a 0a20 2020  k..    else:.   
-000133d0: 2020 2020 206e 5f64 696d 203d 2074 7261       n_dim = tra
-000133e0: 6e73 2e6e 5f64 696d 0a20 2020 2020 2020  ns.n_dim.       
-000133f0: 2069 6620 696d 6167 652e 6e5f 6469 6d20   if image.n_dim 
-00013400: 3d3d 206e 5f64 696d 3a0a 2020 2020 2020  == n_dim:.      
-00013410: 2020 2020 2020 6966 2069 6d61 6765 2e68        if image.h
-00013420: 6173 5f73 7065 6369 616c 3a0a 2020 2020  as_special:.    
-00013430: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00013440: 7428 6622 5761 726e 696e 673a 2027 696e  t(f"Warning: 'in
-00013450: 7465 7270 6f6c 6174 696f 6e27 2074 7279  terpolation' try
-00013460: 696e 6720 746f 2074 7261 6e73 666f 726d  ing to transform
-00013470: 207b 696d 6167 652e 6e5f 7370 6163 657d   {image.n_space}
-00013480: 2b7b 696d 6167 652e 6e5f 7370 6563 6961  +{image.n_specia
-00013490: 6c7d 4420 696d 6167 6520 2877 6974 6820  l}D image (with 
-000134a0: 6261 7463 6820 6f72 2063 6861 6e6e 656c  batch or channel
-000134b0: 2920 6279 207b 6e5f 6469 6d7d 4420 7472  ) by {n_dim}D tr
-000134c0: 616e 7366 6f72 6d61 7469 6f6e 2c20 6175  ansformation, au
-000134d0: 746f 2d72 656d 6f76 696e 6720 7370 6563  to-removing spec
-000134e0: 6961 6c20 6469 6d65 6e73 696f 6e73 2e22  ial dimensions."
-000134f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00013500: 2020 696d 6167 652e 7265 6d6f 7665 5f73    image.remove_s
-00013510: 7065 6369 616c 5f28 290a 2020 2020 2020  pecial_().      
-00013520: 2020 2020 2020 696d 6167 652e 756e 7371        image.unsq
-00013530: 7565 657a 655f 285b 5d29 2e75 6e73 7175  ueeze_([]).unsqu
-00013540: 6565 7a65 5f28 7b7d 290a 2020 2020 2020  eeze_({}).      
-00013550: 2020 656c 6966 2069 6d61 6765 2e6e 5f64    elif image.n_d
-00013560: 696d 203d 3d20 6e5f 6469 6d20 2b20 313a  im == n_dim + 1:
-00013570: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00013580: 6e6f 7420 696d 6167 652e 6861 735f 6261  not image.has_ba
-00013590: 7463 683a 0a20 2020 2020 2020 2020 2020  tch:.           
-000135a0: 2020 2020 2069 6620 696d 6167 652e 6861       if image.ha
-000135b0: 735f 6368 616e 6e65 6c3a 2069 6d61 6765  s_channel: image
-000135c0: 2e75 6e73 7175 6565 7a65 5f28 5b5d 290a  .unsqueeze_([]).
-000135d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135e0: 656c 7365 3a20 696d 6167 652e 7769 7468  else: image.with
-000135f0: 5f62 6174 6368 6469 6d28 3029 2e75 6e73  _batchdim(0).uns
-00013600: 7175 6565 7a65 5f28 7b31 7d29 0a20 2020  queeze_({1}).   
-00013610: 2020 2020 2020 2020 2065 6c69 6620 6e6f           elif no
-00013620: 7420 696d 6167 652e 6861 735f 6368 616e  t image.has_chan
-00013630: 6e65 6c3a 2069 6d61 6765 2e75 6e73 7175  nel: image.unsqu
-00013640: 6565 7a65 5f28 7b7d 290a 2020 2020 2020  eeze_({}).      
-00013650: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00013660: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00013670: 7428 6622 5761 726e 696e 673a 2027 696e  t(f"Warning: 'in
-00013680: 7465 7270 6f6c 6174 696f 6e27 2074 7279  terpolation' try
-00013690: 696e 6720 746f 2074 7261 6e73 666f 726d  ing to transform
-000136a0: 207b 696d 6167 652e 6e5f 7370 6163 657d   {image.n_space}
-000136b0: 2b7b 696d 6167 652e 6e5f 7370 6563 6961  +{image.n_specia
-000136c0: 6c7d 4420 696d 6167 6520 2877 6974 6820  l}D image (with 
-000136d0: 6261 7463 6820 6f72 2063 6861 6e6e 656c  batch or channel
-000136e0: 2920 6279 207b 6e5f 6469 6d7d 4420 7472  ) by {n_dim}D tr
-000136f0: 616e 7366 6f72 6d61 7469 6f6e 2c20 6175  ansformation, au
-00013700: 746f 2d72 656d 6f76 696e 6720 7468 6520  to-removing the 
-00013710: 6368 616e 6e65 6c20 6469 6d65 6e73 696f  channel dimensio
-00013720: 6e73 2e22 290a 2020 2020 2020 2020 2020  ns.").          
-00013730: 2020 2020 2020 696d 6167 652e 7769 7468        image.with
-00013740: 5f63 6861 6e6e 656c 6469 6d28 4e6f 6e65  _channeldim(None
-00013750: 292e 756e 7371 7565 657a 655f 287b 7d29  ).unsqueeze_({})
-00013760: 0a20 2020 2020 2020 2065 6c69 6620 696d  .        elif im
-00013770: 6167 652e 6e5f 6469 6d20 3d3d 206e 5f64  age.n_dim == n_d
-00013780: 696d 202b 2032 3a0a 2020 2020 2020 2020  im + 2:.        
-00013790: 2020 2020 2320 5f63 6861 6e6e 616c 2f62      # _channal/b
-000137a0: 6174 6368 2064 696d 656e 7369 6f6e 7320  atch dimensions 
-000137b0: 7573 6564 2068 6572 6520 6173 2074 6865  used here as the
-000137c0: 7920 6172 6520 6e5f 6469 6d20 7768 656e  y are n_dim when
-000137d0: 206e 6f74 2065 7869 7374 6564 2e20 0a20   not existed. . 
-000137e0: 2020 2020 2020 2020 2020 2069 6620 696d             if im
-000137f0: 6167 652e 6e5f 7370 6563 6961 6c20 3d3d  age.n_special ==
-00013800: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-00013810: 2020 2020 7072 696e 7428 6622 5761 726e      print(f"Warn
-00013820: 696e 673a 2027 696e 7465 7270 6f6c 6174  ing: 'interpolat
-00013830: 696f 6e27 2074 7279 696e 6720 746f 2074  ion' trying to t
-00013840: 7261 6e73 666f 726d 207b 696d 6167 652e  ransform {image.
-00013850: 6e5f 7370 6163 657d 2b31 4420 696d 6167  n_space}+1D imag
-00013860: 6520 2877 6974 6820 6261 7463 6820 6f72  e (with batch or
-00013870: 2063 6861 6e6e 656c 2920 6279 207b 6e5f   channel) by {n_
-00013880: 6469 6d7d 4420 7472 616e 7366 6f72 6d61  dim}D transforma
-00013890: 7469 6f6e 2c20 6175 746f 2d69 6e73 6572  tion, auto-inser
-000138a0: 7469 6e67 206e 6577 2073 7065 6369 616c  ting new special
-000138b0: 2064 696d 656e 7369 6f6e 2e22 290a 2020   dimension.").  
-000138c0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-000138d0: 2069 6d61 6765 2e68 6173 5f62 6174 6368   image.has_batch
-000138e0: 3a20 696d 6167 652e 6261 7463 685f 6469  : image.batch_di
-000138f0: 6d65 6e73 696f 6e20 3d20 3020 6966 2069  mension = 0 if i
-00013900: 6d61 6765 2e5f 6368 616e 6e65 6c5f 6469  mage._channel_di
-00013910: 6d65 6e73 696f 6e20 3e20 3020 656c 7365  mension > 0 else
-00013920: 2031 0a20 2020 2020 2020 2020 2020 2069   1.            i
-00013930: 6620 6e6f 7420 696d 6167 652e 6861 735f  f not image.has_
-00013940: 6368 616e 6e65 6c3a 2069 6d61 6765 2e63  channel: image.c
-00013950: 6861 6e6e 656c 5f64 696d 656e 7369 6f6e  hannel_dimension
-00013960: 203d 2030 2069 6620 696d 6167 652e 5f62   = 0 if image._b
-00013970: 6174 6368 5f64 696d 656e 7369 6f6e 203e  atch_dimension >
-00013980: 2030 2065 6c73 6520 310a 2020 2020 6176   0 else 1.    av
-00013990: 6f75 6368 2869 6d61 6765 2e68 6173 5f62  ouch(image.has_b
-000139a0: 6174 6368 2061 6e64 2069 6d61 6765 2e68  atch and image.h
-000139b0: 6173 5f63 6861 6e6e 656c 2c20 2250 6c65  as_channel, "Ple
-000139c0: 6173 6520 7573 6520 6261 746f 7263 6820  ase use batorch 
-000139d0: 7465 6e73 6f72 206f 6620 7369 7a65 2022  tensor of size "
-000139e0: 202b 0a20 2020 2020 2020 2020 2020 2022   +.            "
-000139f0: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f63  ([n_batch], {n_c
-00013a00: 6861 6e6e 656c 2f6e 5f66 6561 7475 7265  hannel/n_feature
-00013a10: 3a6f 7074 696f 6e61 6c7d 2c20 6d5f 312c  :optional}, m_1,
-00013a20: 206d 5f32 2c20 2e2e 2e2c 206d 5f72 2920   m_2, ..., m_r) 
-00013a30: 5b72 3d6e 5f64 696d 5d20 666f 7220 2220  [r=n_dim] for " 
-00013a40: 2b20 0a20 2020 2020 2020 2020 2020 2066  + .            f
-00013a50: 2264 6174 6120 746f 2062 6520 7370 6174  "data to be spat
-00013a60: 6961 6c6c 7920 696e 7465 7270 6f6c 6174  ially interpolat
-00013a70: 6564 2c20 696e 7374 6561 6420 6f66 207b  ed, instead of {
-00013a80: 696d 6167 652e 7368 6170 657d 2e20 2229  image.shape}. ")
-00013a90: 0a20 2020 2069 6620 7472 616e 7320 6973  .    if trans is
-00013aa0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00013ab0: 2020 2061 766f 7563 6828 696d 6167 652e     avouch(image.
-00013ac0: 6e5f 6261 7463 6820 3d3d 2031 206f 7220  n_batch == 1 or 
-00013ad0: 7472 616e 732e 6e5f 6261 7463 6820 696e  trans.n_batch in
-00013ae0: 2028 4e6f 6e65 2c20 696d 6167 652e 6e5f   (None, image.n_
-00013af0: 6261 7463 682c 2031 292c 2022 506c 6561  batch, 1), "Plea
-00013b00: 7365 2075 7365 2074 7261 6e73 666f 726d  se use transform
-00013b10: 6174 696f 6e20 6f66 2061 2022 202b 0a20  ation of a " +. 
-00013b20: 2020 2020 2020 2020 2020 2066 2273 7569             f"sui
-00013b30: 7461 626c 6520 6e5f 6261 7463 6820 746f  table n_batch to
-00013b40: 2074 7261 6e73 666f 726d 2069 6d61 6765   transform image
-00013b50: 2077 6974 6820 6261 7463 6873 697a 6520   with batchsize 
-00013b60: 7b69 6d61 6765 2e6e 5f62 6174 6368 7d2c  {image.n_batch},
-00013b70: 2063 7572 7265 6e74 6c79 207b 7472 616e   currently {tran
-00013b80: 732e 6e5f 6261 7463 687d 2e22 290a 0a20  s.n_batch}.").. 
-00013b90: 2020 206e 5f62 6174 6368 203d 2069 6d61     n_batch = ima
-00013ba0: 6765 2e6e 5f62 6174 6368 0a20 2020 2069  ge.n_batch.    i
-00013bb0: 6620 6e5f 6261 7463 6820 3d3d 2031 2061  f n_batch == 1 a
-00013bc0: 6e64 2074 7261 6e73 2069 7320 6e6f 7420  nd trans is not 
-00013bd0: 4e6f 6e65 2061 6e64 2074 7261 6e73 2e6e  None and trans.n
-00013be0: 5f62 6174 6368 2069 7320 6e6f 7420 4e6f  _batch is not No
-00013bf0: 6e65 2061 6e64 2074 7261 6e73 2e6e 5f62  ne and trans.n_b
-00013c00: 6174 6368 203e 2031 3a20 6e5f 6261 7463  atch > 1: n_batc
-00013c10: 6820 3d20 7472 616e 732e 6e5f 6261 7463  h = trans.n_batc
-00013c20: 680a 2020 2020 6966 206e 5f62 6174 6368  h.    if n_batch
-00013c30: 203d 3d20 3120 616e 6420 6973 696e 7374   == 1 and isinst
-00013c40: 616e 6365 2874 6172 6765 745f 7370 6163  ance(target_spac
-00013c50: 652c 2062 742e 5465 6e73 6f72 2920 616e  e, bt.Tensor) an
-00013c60: 6420 7461 7267 6574 5f73 7061 6365 2e68  d target_space.h
-00013c70: 6173 5f62 6174 6368 2061 6e64 2074 6172  as_batch and tar
-00013c80: 6765 745f 7370 6163 652e 6e5f 6261 7463  get_space.n_batc
-00013c90: 6820 3e20 313a 206e 5f62 6174 6368 203d  h > 1: n_batch =
-00013ca0: 2074 6172 6765 745f 7370 6163 652e 6e5f   target_space.n_
-00013cb0: 6261 7463 680a 2020 2020 6966 2069 6d61  batch.    if ima
-00013cc0: 6765 2e6e 5f62 6174 6368 203d 3d20 313a  ge.n_batch == 1:
-00013cd0: 2069 6d61 6765 203d 2069 6d61 6765 2e72   image = image.r
-00013ce0: 6570 6561 7465 6428 6e5f 6261 7463 682c  epeated(n_batch,
-00013cf0: 205b 5d29 0a20 2020 206e 5f66 6561 7475   []).    n_featu
-00013d00: 7265 203d 2069 6d61 6765 2e6e 5f63 6861  re = image.n_cha
-00013d10: 6e6e 656c 0a20 2020 2073 697a 6520 3d20  nnel.    size = 
-00013d20: 6274 2e63 6861 6e6e 656c 5f74 656e 736f  bt.channel_tenso
-00013d30: 7228 696d 6167 652e 7370 6163 6529 2e69  r(image.space).i
-00013d40: 6e74 2829 0a20 2020 2069 6620 6e5f 6261  nt().    if n_ba
-00013d50: 7463 6820 3e20 3120 616e 6420 6e6f 7420  tch > 1 and not 
-00013d60: 7368 6170 655f 6f75 742e 6861 735f 6261  shape_out.has_ba
-00013d70: 7463 683a 2073 6861 7065 5f6f 7574 203d  tch: shape_out =
-00013d80: 2062 742e 5369 7a65 285b 6e5f 6261 7463   bt.Size([n_batc
-00013d90: 685d 2920 2b20 7368 6170 655f 6f75 740a  h]) + shape_out.
-00013da0: 2020 2020 6966 2074 6172 6765 745f 7370      if target_sp
-00013db0: 6163 6520 6973 204e 6f6e 653a 0a20 2020  ace is None:.   
-00013dc0: 2020 2020 2073 6361 6c65 2c20 2a70 6169       scale, *pai
-00013dd0: 7273 203d 2074 7261 6e73 2e72 6573 6861  rs = trans.resha
-00013de0: 7065 0a20 2020 2020 2020 2069 6620 6c65  pe.        if le
-00013df0: 6e28 7363 616c 6529 203d 3d20 313a 2073  n(scale) == 1: s
-00013e00: 6361 6c65 202a 3d20 6e5f 6469 6d0a 2020  cale *= n_dim.  
-00013e10: 2020 2020 2020 7461 7267 6574 5f73 7061        target_spa
-00013e20: 6365 203d 205b 696e 7428 7820 2a20 7929  ce = [int(x * y)
-00013e30: 2066 6f72 2078 2c20 7920 696e 207a 6970   for x, y in zip
-00013e40: 2869 6d61 6765 2e73 7061 6365 2c20 7363  (image.space, sc
-00013e50: 616c 6529 5d0a 2020 2020 2020 2020 666f  ale)].        fo
-00013e60: 7220 702c 2071 2069 6e20 7061 6972 733a  r p, q in pairs:
-00013e70: 2074 6172 6765 745f 7370 6163 655b 705d   target_space[p]
-00013e80: 2c20 7461 7267 6574 5f73 7061 6365 5b71  , target_space[q
-00013e90: 5d20 3d20 7461 7267 6574 5f73 7061 6365  ] = target_space
-00013ea0: 5b71 5d2c 2074 6172 6765 745f 7370 6163  [q], target_spac
-00013eb0: 655b 705d 0a20 2020 2020 2020 2074 6172  e[p].        tar
-00013ec0: 6765 745f 7370 6163 6520 3d20 7475 706c  get_space = tupl
-00013ed0: 6528 7461 7267 6574 5f73 7061 6365 290a  e(target_space).
-00013ee0: 2020 2020 2020 2020 7368 6170 655f 6f75          shape_ou
-00013ef0: 7420 3d20 7368 6170 655f 6f75 742e 7265  t = shape_out.re
-00013f00: 7365 745f 7370 6163 6528 7461 7267 6574  set_space(target
-00013f10: 5f73 7061 6365 290a 2020 2020 6966 2069  _space).    if i
-00013f20: 7369 6e73 7461 6e63 6528 7461 7267 6574  sinstance(target
-00013f30: 5f73 7061 6365 2c20 7475 706c 6529 2061  _space, tuple) a
-00013f40: 6e64 206c 656e 2874 6172 6765 745f 7370  nd len(target_sp
-00013f50: 6163 6529 203d 3d20 6e5f 6469 6d3a 2070  ace) == n_dim: p
-00013f60: 6173 730a 2020 2020 656c 6966 2069 7369  ass.    elif isi
-00013f70: 6e73 7461 6e63 6528 7461 7267 6574 5f73  nstance(target_s
-00013f80: 7061 6365 2c20 6274 2e74 6f72 6368 2e54  pace, bt.torch.T
-00013f90: 656e 736f 7229 3a20 7061 7373 0a20 2020  ensor): pass.   
-00013fa0: 2065 6c73 653a 2072 6169 7365 2054 7970   else: raise Typ
-00013fb0: 6545 7272 6f72 2866 2257 726f 6e67 2074  eError(f"Wrong t
-00013fc0: 6172 6765 7420 7370 6163 6520 666f 7220  arget space for 
-00013fd0: 696e 7465 7270 6f6c 6174 696f 6e3a 207b  interpolation: {
-00013fe0: 7461 7267 6574 5f73 7061 6365 7d2e 2022  target_space}. "
-00013ff0: 290a 2020 2020 6966 2069 7369 6e73 7461  ).    if isinsta
-00014000: 6e63 6528 7461 7267 6574 5f73 7061 6365  nce(target_space
-00014010: 2c20 7475 706c 6529 3a20 0a20 2020 2020  , tuple): .     
-00014020: 2020 2023 2043 7265 6174 6520 6120 6772     # Create a gr
-00014030: 6964 2058 2077 6974 6820 7369 7a65 2028  id X with size (
-00014040: 7b6e 5f64 696d 7d2c 2073 697a 655f 312c  {n_dim}, size_1,
-00014050: 2073 697a 655f 322c 202e 2e2e 2c20 7369   size_2, ..., si
-00014060: 7a65 5f72 2920 5b72 3d6e 5f64 696d 5d2e  ze_r) [r=n_dim].
-00014070: 0a20 2020 2020 2020 2058 203d 2062 742e  .        X = bt.
-00014080: 696d 6167 655f 6772 6964 2874 6172 6765  image_grid(targe
-00014090: 745f 7370 6163 6529 2e66 6c6f 6174 2829  t_space).float()
-000140a0: 2023 202b 2062 742e 6368 616e 6e65 6c5f   # + bt.channel_
-000140b0: 7465 6e73 6f72 285b 666c 6f61 7428 612d  tensor([float(a-
-000140c0: 6229 2f32 2066 6f72 2061 2c20 6220 696e  b)/2 for a, b in
-000140d0: 207a 6970 2869 6d61 6765 2e73 7061 6365   zip(image.space
-000140e0: 2c20 7461 7267 6574 5f73 7061 6365 295d  , target_space)]
-000140f0: 290a 2020 2020 2020 2020 2320 436f 6d70  ).        # Comp
-00014100: 7574 6520 7468 6520 7472 616e 7366 6f72  ute the transfor
-00014110: 6d65 6420 636f 6f72 6469 6e61 7465 732e  med coordinates.
-00014120: 2059 3a20 285b 6e5f 6261 7463 685d 2c20   Y: ([n_batch], 
-00014130: 7b6e 5f64 696d 7d2c 2073 697a 655f 312c  {n_dim}, size_1,
-00014140: 2073 697a 655f 322c 202e 2e2e 2c20 7369   size_2, ..., si
-00014150: 7a65 5f72 2920 5b72 3d6e 5f64 696d 5d2e  ze_r) [r=n_dim].
-00014160: 0a20 2020 2020 2020 2069 6620 7472 616e  .        if tran
-00014170: 7320 6973 204e 6f6e 653a 2074 7261 6e73  s is None: trans
-00014180: 203d 2049 6465 6e74 6974 7928 290a 2020   = Identity().  
-00014190: 2020 2020 2020 5920 3d20 7472 616e 7328        Y = trans(
-000141a0: 5829 0a20 2020 2020 2020 2069 6620 6e6f  X).        if no
-000141b0: 7420 592e 6861 735f 6261 7463 683a 2059  t Y.has_batch: Y
-000141c0: 203d 2059 2e6d 756c 7469 706c 7928 6e5f   = Y.multiply(n_
-000141d0: 6261 7463 682c 205b 5d29 0a20 2020 2020  batch, []).     
-000141e0: 2020 2069 6620 592e 6e5f 6261 7463 6820     if Y.n_batch 
-000141f0: 3d3d 2031 3a20 5920 3d20 592e 7265 7065  == 1: Y = Y.repe
-00014200: 6174 6564 286e 5f62 6174 6368 2c20 5b5d  ated(n_batch, []
-00014210: 290a 2020 2020 2020 2020 5920 3d20 592e  ).        Y = Y.
-00014220: 616d 706c 6966 7928 6e5f 6665 6174 7572  amplify(n_featur
-00014230: 652c 205b 5d29 0a20 2020 2020 2020 2073  e, []).        s
-00014240: 6861 7065 5f6f 7574 203d 2073 6861 7065  hape_out = shape
-00014250: 5f6f 7574 2e72 6573 6574 5f73 7061 6365  _out.reset_space
-00014260: 2874 6172 6765 745f 7370 6163 6529 0a20  (target_space). 
-00014270: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00014280: 2074 6172 6765 745f 7370 6163 6520 3d20   target_space = 
-00014290: 6261 746f 7263 685f 7465 6e73 6f72 2874  batorch_tensor(t
-000142a0: 6172 6765 745f 7370 6163 6529 0a20 2020  arget_space).   
-000142b0: 2020 2020 2069 6620 6e6f 7420 7461 7267       if not targ
-000142c0: 6574 5f73 7061 6365 2e68 6173 5f62 6174  et_space.has_bat
-000142d0: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
-000142e0: 6966 2074 6172 6765 745f 7370 6163 652e  if target_space.
-000142f0: 7369 7a65 2830 2920 3d3d 206e 5f62 6174  size(0) == n_bat
-00014300: 6368 2061 6e64 206e 5f62 6174 6368 2021  ch and n_batch !
-00014310: 3d20 6e5f 6469 6d20 6f72 206c 656e 285b  = n_dim or len([
-00014320: 7820 666f 7220 7820 696e 2074 6172 6765  x for x in targe
-00014330: 745f 7370 6163 652e 7368 6170 6520 6966  t_space.shape if
-00014340: 2078 203d 3d20 6e5f 6469 6d5d 2920 3e3d   x == n_dim]) >=
-00014350: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-00014360: 2020 2020 7461 7267 6574 5f73 7061 6365      target_space
-00014370: 2e77 6974 685f 6261 7463 6864 696d 2830  .with_batchdim(0
-00014380: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00014390: 7365 3a20 7461 7267 6574 5f73 7061 6365  se: target_space
-000143a0: 2e75 6e73 7175 6565 7a65 5f28 5b5d 290a  .unsqueeze_([]).
-000143b0: 2020 2020 2020 2020 6966 206e 6f74 2074          if not t
-000143c0: 6172 6765 745f 7370 6163 652e 6861 735f  arget_space.has_
-000143d0: 6368 616e 6e65 6c3a 0a20 2020 2020 2020  channel:.       
-000143e0: 2020 2020 2069 6620 7461 7267 6574 5f73       if target_s
-000143f0: 7061 6365 2e62 6174 6368 5f64 696d 656e  pace.batch_dimen
-00014400: 7369 6f6e 2021 3d20 3020 616e 6420 7461  sion != 0 and ta
-00014410: 7267 6574 5f73 7061 6365 2e73 697a 6528  rget_space.size(
-00014420: 3029 203d 3d20 6e5f 6469 6d3a 2074 6172  0) == n_dim: tar
-00014430: 6765 745f 7370 6163 652e 7769 7468 5f63  get_space.with_c
-00014440: 6861 6e6e 656c 6469 6d28 3029 0a20 2020  hanneldim(0).   
-00014450: 2020 2020 2020 2020 2065 6c69 6620 7461           elif ta
-00014460: 7267 6574 5f73 7061 6365 2e62 6174 6368  rget_space.batch
-00014470: 5f64 696d 656e 7369 6f6e 2021 3d20 3120  _dimension != 1 
-00014480: 616e 6420 7461 7267 6574 5f73 7061 6365  and target_space
-00014490: 2e73 697a 6528 3129 203d 3d20 6e5f 6469  .size(1) == n_di
-000144a0: 6d3a 2074 6172 6765 745f 7370 6163 652e  m: target_space.
-000144b0: 7769 7468 5f63 6861 6e6e 656c 6469 6d28  with_channeldim(
-000144c0: 3129 0a20 2020 2020 2020 2020 2020 2065  1).            e
-000144d0: 6c69 6620 7461 7267 6574 5f73 7061 6365  lif target_space
-000144e0: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
-000144f0: 2021 3d20 7461 7267 6574 5f73 7061 6365   != target_space
-00014500: 2e6e 5f64 696d 202d 2031 2061 6e64 2074  .n_dim - 1 and t
-00014510: 6172 6765 745f 7370 6163 652e 7369 7a65  arget_space.size
-00014520: 282d 3129 203d 3d20 6e5f 6469 6d3a 2074  (-1) == n_dim: t
-00014530: 6172 6765 745f 7370 6163 652e 7769 7468  arget_space.with
-00014540: 5f63 6861 6e6e 656c 6469 6d28 2d31 290a  _channeldim(-1).
-00014550: 2020 2020 2020 2020 6176 6f75 6368 2874          avouch(t
-00014560: 6172 6765 745f 7370 6163 652e 6861 735f  arget_space.has_
-00014570: 6368 616e 6e65 6c20 616e 6420 7461 7267  channel and targ
-00014580: 6574 5f73 7061 6365 2e6e 5f63 6861 6e6e  et_space.n_chann
-00014590: 656c 203d 3d20 6e5f 6469 6d2c 2022 2774  el == n_dim, "'t
-000145a0: 6172 6765 745f 7370 6163 6527 2066 6f72  arget_space' for
-000145b0: 2069 6e74 6572 706f 6c61 7469 6f6e 2073   interpolation s
-000145c0: 686f 756c 6420 6861 7665 2061 2063 6861  hould have a cha
-000145d0: 6e6e 656c 2064 696d 656e 7369 6f6e 2066  nnel dimension f
-000145e0: 6f72 2063 6f6f 7264 696e 6174 6573 2e20  or coordinates. 
-000145f0: 2229 0a20 2020 2020 2020 2059 203d 2074  ").        Y = t
-00014600: 6172 6765 745f 7370 6163 652e 7265 7065  arget_space.repe
-00014610: 6174 6564 286e 5f62 6174 6368 202f 2f20  ated(n_batch // 
-00014620: 7461 7267 6574 5f73 7061 6365 2e6e 5f62  target_space.n_b
-00014630: 6174 6368 2c20 5b5d 292e 616d 706c 6966  atch, []).amplif
-00014640: 7928 6e5f 6665 6174 7572 652c 205b 5d29  y(n_feature, [])
-00014650: 0a20 2020 2020 2020 2073 6861 7065 5f6f  .        shape_o
-00014660: 7574 203d 2073 6861 7065 5f6f 7574 2e72  ut = shape_out.r
-00014670: 6573 6574 5f73 7061 6365 2874 6172 6765  eset_space(targe
-00014680: 745f 7370 6163 652e 7370 6163 6529 0a20  t_space.space). 
-00014690: 2020 2020 2020 200a 2020 2020 696d 6167         .    imag
-000146a0: 6520 3d20 696d 6167 652e 6d65 7267 6564  e = image.merged
-000146b0: 696d 7328 7b7d 2c20 5b5d 290a 2020 2020  ims({}, []).    
-000146c0: 6e5f 6261 7463 6820 3d20 696d 6167 652e  n_batch = image.
-000146d0: 6e5f 6261 7463 680a 0a20 2020 2069 6620  n_batch..    if 
-000146e0: 6d65 7468 6f64 2e6c 6f77 6572 2829 203d  method.lower() =
-000146f0: 3d20 2762 7370 6c69 6e65 273a 0a20 2020  = 'bspline':.   
-00014700: 2020 2020 2069 6620 6465 7269 7661 7469       if derivati
-00014710: 7665 3a20 7261 6973 6520 5479 7065 4572  ve: raise TypeEr
-00014720: 726f 7228 224e 6f20 6465 7269 7661 7469  ror("No derivati
-00014730: 7665 7320 666f 7220 6273 706c 696e 6520  ves for bspline 
-00014740: 696e 7465 7270 6f6c 6174 696f 6e73 2061  interpolations a
-00014750: 7265 2061 7661 696c 6162 6c65 2073 6f20  re available so 
-00014760: 6661 722e 2050 6c65 6173 6520 7772 6974  far. Please writ
-00014770: 6520 6974 2062 7920 796f 7572 7365 6c66  e it by yourself
-00014780: 2e20 2229 0a20 2020 2020 2020 2023 2054  . ").        # T
-00014790: 4f44 4f3a 2046 4644 0a20 2020 2020 2020  ODO: FFD.       
-000147a0: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-000147b0: 2822 4273 706c 696e 6520 696e 7465 7270  ("Bspline interp
-000147c0: 6f6c 6174 696f 6e20 6973 206e 6f74 2061  olation is not a
-000147d0: 7661 696c 6162 6c65 2073 6f20 6661 722e  vailable so far.
-000147e0: 2050 6c65 6173 6520 7772 6974 6520 6974   Please write it
-000147f0: 2062 7920 796f 7572 7365 6c66 2e20 2229   by yourself. ")
-00014800: 0a0a 2020 2020 6959 203d 2062 742e 666c  ..    iY = bt.fl
-00014810: 6f6f 7228 5929 2e6c 6f6e 6728 2920 2320  oor(Y).long() # 
-00014820: 4765 6e65 7261 7465 2074 6865 2069 6e74  Generate the int
-00014830: 6567 6572 2070 6172 7420 6f66 2059 0a20  eger part of Y. 
-00014840: 2020 206a 5920 3d20 6959 202b 2031 2023     jY = iY + 1 #
-00014850: 2061 6e64 2074 6865 2069 6e74 6567 6572   and the integer
-00014860: 2070 6172 7420 706c 7573 206f 6e65 2e0a   part plus one..
-00014870: 2020 2020 6966 206d 6574 686f 642e 6c6f      if method.lo
-00014880: 7765 7228 2920 3d3d 2027 6c69 6e65 6172  wer() == 'linear
-00014890: 273a 2066 5920 3d20 5920 2d20 6959 2e66  ': fY = Y - iY.f
-000148a0: 6c6f 6174 2829 2023 2054 6865 2064 6563  loat() # The dec
-000148b0: 696d 616c 2070 6172 7420 6f66 2059 2e0a  imal part of Y..
-000148c0: 2020 2020 656c 6966 206d 6574 686f 642e      elif method.
-000148d0: 6c6f 7765 7228 2920 3d3d 2027 6e65 6172  lower() == 'near
-000148e0: 6573 7427 3a20 6659 203d 2062 742e 666c  est': fY = bt.fl
-000148f0: 6f6f 7228 5920 2d20 6959 2e66 6c6f 6174  oor(Y - iY.float
-00014900: 2829 202b 2030 2e35 2920 2320 5468 6520  () + 0.5) # The 
-00014910: 6465 6369 6d61 6c20 7061 7274 206f 6620  decimal part of 
-00014920: 592e 0a20 2020 2065 6c73 653a 2072 6169  Y..    else: rai
-00014930: 7365 2054 7970 6545 7272 6f72 2822 556e  se TypeError("Un
-00014940: 7265 636f 676e 697a 6564 2061 7267 756d  recognized argum
-00014950: 656e 7420 276d 6574 686f 6427 2e20 2229  ent 'method'. ")
-00014960: 0a20 2020 2062 5920 3d20 6274 2e73 7461  .    bY = bt.sta
-00014970: 636b 2828 6959 2c20 6a59 292c 2031 292e  ck((iY, jY), 1).
-00014980: 7669 6577 285b 6e5f 6261 7463 685d 2c20  view([n_batch], 
-00014990: 322c 207b 6e5f 6469 6d7d 2c20 2d31 2920  2, {n_dim}, -1) 
-000149a0: 2320 285b 6e5f 6261 7463 685d 2c20 322c  # ([n_batch], 2,
-000149b0: 207b 6e5f 6469 6d7d 2c20 6e5f 6461 7461   {n_dim}, n_data
-000149c0: 292e 0a20 2020 2057 203d 2062 742e 7374  )..    W = bt.st
-000149d0: 6163 6b28 2831 202d 2066 592c 2066 5929  ack((1 - fY, fY)
-000149e0: 2c20 3129 2e76 6965 7728 5b6e 5f62 6174  , 1).view([n_bat
-000149f0: 6368 5d2c 2032 2c20 7b6e 5f64 696d 7d2c  ch], 2, {n_dim},
-00014a00: 202d 3129 2023 2028 5b6e 5f62 6174 6368   -1) # ([n_batch
-00014a10: 5d2c 2032 2c20 7b6e 5f64 696d 7d2c 206e  ], 2, {n_dim}, n
-00014a20: 5f64 6174 6129 2e0a 2020 2020 6e5f 6461  _data)..    n_da
-00014a30: 7461 203d 2062 592e 7369 7a65 282d 3129  ta = bY.size(-1)
-00014a40: 0a0a 2020 2020 2320 5072 6570 6172 6520  ..    # Prepare 
-00014a50: 666f 7220 7468 6520 6f75 7470 7574 2073  for the output s
-00014a60: 7061 6365 3a20 6e5f 6261 7463 682c 206d  pace: n_batch, m
-00014a70: 5f31 2c20 2e2e 2e2c 206d 5f73 0a20 2020  _1, ..., m_s.   
-00014a80: 2069 6620 6465 7269 7661 7469 7665 3a20   if derivative: 
-00014a90: 6f75 7470 7574 203d 2062 742e 7a65 726f  output = bt.zero
-00014aa0: 7328 5b6e 5f62 6174 6368 5d2c 207b 6e5f  s([n_batch], {n_
-00014ab0: 6469 6d7d 2c20 2a73 6861 7065 5f6f 7574  dim}, *shape_out
-00014ac0: 2e73 7061 6365 290a 2020 2020 656c 7365  .space).    else
-00014ad0: 3a20 6f75 7470 7574 203d 2062 742e 7a65  : output = bt.ze
-00014ae0: 726f 7328 7368 6170 655f 6f75 7429 0a20  ros(shape_out). 
-00014af0: 2020 2066 6f72 2047 2069 6e20 6274 2e69     for G in bt.i
-00014b00: 6d61 6765 5f67 7269 6428 5b32 5d2a 6e5f  mage_grid([2]*n_
-00014b10: 6469 6d29 2e66 6c61 7474 656e 2829 2e74  dim).flatten().t
-00014b20: 7261 6e73 706f 7365 2830 2c20 3129 3a0a  ranspose(0, 1):.
-00014b30: 2020 2020 2020 2020 2320 4765 7420 7468          # Get th
-00014b40: 6520 696e 6469 6365 7320 666f 7220 7468  e indices for th
-00014b50: 6520 7465 726d 3a20 6259 5b3a 2c20 475b  e term: bY[:, G[
-00014b60: 445d 2c20 442c 203a 5d2c 2073 697a 653d  D], D, :], size=
-00014b70: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f64  ([n_batch], {n_d
-00014b80: 696d 7d2c 206e 5f64 6174 6129 0a20 2020  im}, n_data).   
-00014b90: 2020 2020 2049 6e64 203d 2062 592e 6761       Ind = bY.ga
-00014ba0: 7468 6572 2831 2c20 472e 6578 7061 6e64  ther(1, G.expand
-00014bb0: 5f74 6f28 5b6e 5f62 6174 6368 5d2c 2031  _to([n_batch], 1
-00014bc0: 2c20 7b6e 5f64 696d 7d2c 206e 5f64 6174  , {n_dim}, n_dat
-00014bd0: 6129 292e 7371 7565 657a 6528 3129 0a20  a)).squeeze(1). 
-00014be0: 2020 2020 2020 2023 2043 6c61 6d70 2074         # Clamp t
-00014bf0: 6865 2069 6e64 6963 6573 2069 6e20 7468  he indices in th
-00014c00: 6520 636f 7272 6563 7420 7261 6e67 6520  e correct range 
-00014c10: 2620 436f 6d70 7574 6520 7468 6520 626f  & Compute the bo
-00014c20: 7264 6572 2063 6f6e 6469 7469 6f6e 0a20  rder condition. 
-00014c30: 2020 2020 2020 2063 6f6e 6469 7469 6f6e         condition
-00014c40: 203d 2062 742e 7375 6d28 2849 6e64 203c   = bt.sum((Ind <
-00014c50: 2030 2920 2b20 2849 6e64 203e 2073 697a   0) + (Ind > siz
-00014c60: 6520 2d20 3129 2c20 3129 0a20 2020 2020  e - 1), 1).     
-00014c70: 2020 2049 6e64 203d 2062 742e 6d69 6e28     Ind = bt.min(
-00014c80: 6274 2e63 6c61 6d70 2849 6e64 2c20 6d69  bt.clamp(Ind, mi
-00014c90: 6e3d 3029 2c20 2873 697a 6520 2d20 3129  n=0), (size - 1)
-00014ca0: 2e65 7870 616e 645f 746f 2849 6e64 2929  .expand_to(Ind))
-00014cb0: 0a20 2020 2020 2020 2023 2043 6f6e 7665  .        # Conve
-00014cc0: 7274 2074 6865 2069 6e64 6963 6573 2074  rt the indices t
-00014cd0: 6f20 3120 6469 6d65 6e73 696f 6e61 6c2e  o 1 dimensional.
-00014ce0: 2044 6f74 3a20 285b 6e5f 6261 7463 685d   Dot: ([n_batch]
-00014cf0: 2c20 6e5f 6461 7461 290a 2020 2020 2020  , n_data).      
-00014d00: 2020 446f 7420 3d20 496e 645b 3a2c 2030    Dot = Ind[:, 0
-00014d10: 5d0a 2020 2020 2020 2020 666f 7220 7220  ].        for r 
-00014d20: 696e 2072 616e 6765 2831 2c20 6e5f 6469  in range(1, n_di
-00014d30: 6d29 3a20 446f 7420 2a3d 2073 697a 655b  m): Dot *= size[
-00014d40: 725d 3b20 446f 7420 2b3d 2049 6e64 5b3a  r]; Dot += Ind[:
-00014d50: 2c20 725d 0a20 2020 2020 2020 2023 2047  , r].        # G
-00014d60: 6574 2074 6865 2069 6d61 6765 2076 616c  et the image val
-00014d70: 7565 7320 4956 3a20 285b 6e5f 6261 7463  ues IV: ([n_batc
-00014d80: 685d 2c20 6e5f 6461 7461 290a 2020 2020  h], n_data).    
-00014d90: 2020 2020 4956 203d 204e 6f6e 650a 2020      IV = None.  
-00014da0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00014db0: 6e63 6528 6669 6c6c 2c20 7374 7229 3a0a  nce(fill, str):.
-00014dc0: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-00014dd0: 696c 6c2e 6c6f 7765 7228 2920 3d3d 2027  ill.lower() == '
-00014de0: 6e65 6172 6573 7427 3a0a 2020 2020 2020  nearest':.      
-00014df0: 2020 2020 2020 2020 2020 4956 203d 2069            IV = i
-00014e00: 6d61 6765 2e66 6c61 7474 656e 2829 2e67  mage.flatten().g
-00014e10: 6174 6865 7228 312c 2044 6f74 290a 2020  ather(1, Dot).  
-00014e20: 2020 2020 2020 2020 2020 656c 6966 2066            elif f
-00014e30: 696c 6c2e 6c6f 7765 7228 2920 3d3d 2027  ill.lower() == '
-00014e40: 6261 636b 6772 6f75 6e64 273a 0a20 2020  background':.   
-00014e50: 2020 2020 2020 2020 2020 2020 2062 6b5f               bk_
-00014e60: 7661 6c75 6520 3d20 6274 2e73 7461 636b  value = bt.stack
-00014e70: 285b 696d 6167 655b 2873 6c69 6365 284e  ([image[(slice(N
-00014e80: 6f6e 6529 2c29 202b 2074 7570 6c65 2867  one),) + tuple(g
-00014e90: 295d 2066 6f72 2067 2069 6e20 2862 742e  )] for g in (bt.
-00014ea0: 696d 6167 655f 6772 6964 285b 325d 2a6e  image_grid([2]*n
-00014eb0: 5f64 696d 2920 2a20 6274 2e63 6861 6e6e  _dim) * bt.chann
-00014ec0: 656c 5f74 656e 736f 7228 7369 7a65 2d31  el_tensor(size-1
-00014ed0: 2929 2e66 6c61 7474 656e 2829 2e74 7261  )).flatten().tra
-00014ee0: 6e73 706f 7365 2830 2c31 295d 2c20 3129  nspose(0,1)], 1)
-00014ef0: 2e6d 6564 6961 6e28 3129 2e76 616c 7565  .median(1).value
-00014f00: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00014f10: 2020 6261 636b 6772 6f75 6e64 203d 2062    background = b
-00014f20: 6b5f 7661 6c75 6520 2a20 6274 2e6f 6e65  k_value * bt.one
-00014f30: 735f 6c69 6b65 2844 6f74 290a 2020 2020  s_like(Dot).    
-00014f40: 2020 2020 2020 2020 656c 6966 2066 696c          elif fil
-00014f50: 6c2e 6c6f 7765 7228 2920 3d3d 2027 7a65  l.lower() == 'ze
-00014f60: 726f 273a 0a20 2020 2020 2020 2020 2020  ro':.           
-00014f70: 2020 2020 2062 6163 6b67 726f 756e 6420       background 
-00014f80: 3d20 6274 2e7a 6572 6f73 5f6c 696b 6528  = bt.zeros_like(
-00014f90: 446f 7429 0a20 2020 2020 2020 2065 6c73  Dot).        els
-00014fa0: 653a 0a20 2020 2020 2020 2020 2020 2062  e:.            b
-00014fb0: 6163 6b67 726f 756e 6420 3d20 6669 6c6c  ackground = fill
-00014fc0: 202a 2062 742e 6f6e 6573 5f6c 696b 6528   * bt.ones_like(
-00014fd0: 446f 7429 0a20 2020 2020 2020 2069 6620  Dot).        if 
-00014fe0: 4956 2069 7320 4e6f 6e65 3a20 4956 203d  IV is None: IV =
-00014ff0: 2062 742e 7768 6572 6528 636f 6e64 6974   bt.where(condit
-00015000: 696f 6e20 3e3d 2031 2c20 6261 636b 6772  ion >= 1, backgr
-00015010: 6f75 6e64 2e66 6c6f 6174 2829 2c20 696d  ound.float(), im
-00015020: 6167 652e 666c 6174 7465 6e28 292e 6761  age.flatten().ga
-00015030: 7468 6572 2831 2c20 446f 7429 2e66 6c6f  ther(1, Dot).flo
-00015040: 6174 2829 290a 2020 2020 2020 2020 2320  at()).        # 
-00015050: 5765 6967 6874 7320 666f 7220 6561 6368  Weights for each
-00015060: 2070 6f69 6e74 3a20 5b70 726f 6475 6374   point: [product
-00015070: 206f 6620 575b 3a2c 2047 5b44 5d2c 2044   of W[:, G[D], D
-00015080: 2c20 785d 2066 6f72 2044 2069 6e20 7261  , x] for D in ra
-00015090: 6e67 6528 6e5f 6469 6d29 5d20 666f 7220  nge(n_dim)] for 
-000150a0: 706f 696e 7420 782e 0a20 2020 2020 2020  point x..       
-000150b0: 2023 2057 673a 2028 5b6e 5f62 6174 6368   # Wg: ([n_batch
-000150c0: 5d2c 207b 6e5f 6469 6d7d 2c20 6e5f 6461  ], {n_dim}, n_da
-000150d0: 7461 290a 2020 2020 2020 2020 5767 203d  ta).        Wg =
-000150e0: 2057 2e67 6174 6865 7228 312c 2047 2e65   W.gather(1, G.e
-000150f0: 7870 616e 645f 746f 285b 6e5f 6261 7463  xpand_to([n_batc
-00015100: 685d 2c20 312c 207b 6e5f 6469 6d7d 2c20  h], 1, {n_dim}, 
-00015110: 6e5f 6461 7461 2929 2e73 7175 6565 7a65  n_data)).squeeze
-00015120: 2831 290a 2020 2020 2020 2020 6966 206e  (1).        if n
-00015130: 6f74 2064 6572 6976 6174 6976 653a 0a20  ot derivative:. 
-00015140: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-00015150: 7420 2b3d 2028 5767 2e70 726f 6428 3129  t += (Wg.prod(1)
-00015160: 202a 2049 5629 2e76 6965 775f 6173 286f   * IV).view_as(o
-00015170: 7574 7075 7429 0a20 2020 2020 2020 2065  utput).        e
-00015180: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00015190: 2074 656d 7057 674d 6174 203d 2057 672e   tempWgMat = Wg.
-000151a0: 6d75 6c74 6970 6c79 286e 5f64 696d 2c20  multiply(n_dim, 
-000151b0: 3129 2023 2028 5b6e 5f62 6174 6368 5d2c  1) # ([n_batch],
-000151c0: 206e 5f64 696d 2c20 7b6e 5f64 696d 7d2c   n_dim, {n_dim},
-000151d0: 206e 5f64 6174 6129 0a20 2020 2020 2020   n_data).       
-000151e0: 2020 2020 2074 656d 7057 674d 6174 5b3a       tempWgMat[:
-000151f0: 2c20 6274 2e61 7261 6e67 6528 6e5f 6469  , bt.arange(n_di
-00015200: 6d29 2c20 6274 2e61 7261 6e67 6528 6e5f  m), bt.arange(n_
-00015210: 6469 6d29 5d20 3d20 310a 2020 2020 2020  dim)] = 1.      
-00015220: 2020 2020 2020 6457 6720 3d20 7465 6d70        dWg = temp
-00015230: 5767 4d61 742e 7072 6f64 2831 2920 2a20  WgMat.prod(1) * 
-00015240: 2847 202a 2032 202d 2031 292e 666c 6f61  (G * 2 - 1).floa
-00015250: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00015260: 6f75 7470 7574 202b 3d20 2864 5767 202a  output += (dWg *
-00015270: 2049 562e 756e 7371 7565 657a 6528 3129   IV.unsqueeze(1)
-00015280: 292e 7669 6577 5f61 7328 6f75 7470 7574  ).view_as(output
-00015290: 290a 2020 2020 6274 2e74 6f72 6368 2e63  ).    bt.torch.c
-000152a0: 7564 612e 656d 7074 795f 6361 6368 6528  uda.empty_cache(
-000152b0: 290a 2020 2020 6570 7320 3d20 3165 2d36  ).    eps = 1e-6
-000152c0: 0a20 2020 206d 203d 2030 2069 6620 696d  .    m = 0 if im
-000152d0: 6167 652e 6d69 6e28 2920 3e20 2d65 7073  age.min() > -eps
-000152e0: 2065 6c73 6520 696d 6167 652e 6d69 6e28   else image.min(
-000152f0: 292e 6974 656d 2829 0a20 2020 204d 203d  ).item().    M =
-00015300: 2031 2069 6620 696d 6167 652e 6d61 7828   1 if image.max(
-00015310: 2920 3c20 3120 2b20 6570 7320 656c 7365  ) < 1 + eps else
-00015320: 2069 6d61 6765 2e6d 6178 2829 2e69 7465   image.max().ite
-00015330: 6d28 290a 2020 2020 7265 7475 726e 206f  m().    return o
-00015340: 7574 7075 742e 636c 616d 7028 6d2c 204d  utput.clamp(m, M
-00015350: 290a 0a40 616c 6961 7328 2272 6573 616d  )..@alias("resam
-00015360: 706c 655f 666f 7277 6172 6422 290a 6465  ple_forward").de
-00015370: 6620 696e 7465 7270 6f6c 6174 696f 6e5f  f interpolation_
-00015380: 666f 7277 6172 6428 0a20 2020 2020 2020  forward(.       
-00015390: 2069 6d61 6765 2c20 0a20 2020 2020 2020   image, .       
-000153a0: 2074 7261 6e73 203d 204e 6f6e 652c 200a   trans = None, .
-000153b0: 2020 2020 2020 2020 6d65 7468 6f64 203d          method =
-000153c0: 2027 4c69 6e65 6172 272c 200a 2020 2020   'Linear', .    
-000153d0: 2020 2020 7461 7267 6574 5f73 7061 6365      target_space
-000153e0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000153f0: 2066 696c 6c20 3d20 277a 6572 6f27 2c0a   fill = 'zero',.
-00015400: 2020 2020 2020 2020 6465 7269 7661 7469          derivati
-00015410: 7665 203d 2046 616c 7365 0a20 2020 2029  ve = False.    )
-00015420: 3a0a 2020 2020 2727 270a 2020 2020 496e  :.    '''.    In
-00015430: 7465 7270 6f6c 6174 6520 7573 696e 6720  terpolate using 
-00015440: 666f 7277 6172 6420 7472 616e 7366 6f72  forward transfor
-00015450: 6d61 7469 6f6e 2e20 4974 2069 7320 6e6f  mation. It is no
-00015460: 7420 7965 7420 696d 706c 656d 656e 7465  t yet implemente
-00015470: 642e 200a 2020 2020 692e 652e 2043 6f6d  d. .    i.e. Com
-00015480: 7075 7465 2074 6865 2069 6d61 6765 2049  pute the image I
-00015490: 2073 2e74 2e20 7472 616e 7328 7829 203d   s.t. trans(x) =
-000154a0: 2079 2066 6f72 2078 2069 6e20 696e 7075   y for x in inpu
-000154b0: 7420 696d 6167 6520 616e 6420 7920 696e  t image and y in
-000154c0: 2074 6865 206f 7574 7075 7420 4920 7573   the output I us
-000154d0: 696e 6720 696e 7465 7270 6f6c 6174 696f  ing interpolatio
-000154e0: 6e20 6d65 7468 6f64 3a0a 2020 2020 2020  n method:.      
-000154f0: 2020 6d65 7468 6f64 203d 204c 696e 6561    method = Linea
-00015500: 7220 5b4e 4f20 4752 4144 4945 4e54 2121  r [NO GRADIENT!!
-00015510: 215d 3a20 4269 6c69 6e65 6172 2069 6e74  !]: Bilinear int
-00015520: 6572 706f 6c61 7469 6f6e 0a20 2020 2020  erpolation.     
-00015530: 2020 206d 6574 686f 6420 3d20 4e65 6172     method = Near
-00015540: 6573 7420 5b4e 4f20 4752 4144 4945 4e54  est [NO GRADIENT
-00015550: 2121 215d 3a20 4e65 6172 6573 7420 696e  !!!]: Nearest in
-00015560: 7465 7270 6f6c 6174 696f 6e0a 0a20 2020  terpolation..   
-00015570: 2050 6172 616d 733a 0a20 2020 2020 2020   Params:.       
-00015580: 2069 6d61 6765 205b 6274 2e54 656e 736f   image [bt.Tenso
-00015590: 725d 3a20 5468 6520 7461 7267 6574 2069  r]: The target i
-000155a0: 6d61 6765 2e0a 2020 2020 2020 2020 2020  mage..          
-000155b0: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
-000155c0: 683a 6f70 7469 6f6e 616c 5d2c 207b 6e5f  h:optional], {n_
-000155d0: 6368 616e 6e65 6c3a 6f70 7469 6f6e 616c  channel:optional
-000155e0: 7d2c 206d 4031 2c20 6d40 322c 202e 2e2e  }, m@1, m@2, ...
-000155f0: 2c20 6d40 6e5f 6469 6d29 0a20 2020 2020  , m@n_dim).     
-00015600: 2020 2074 7261 6e73 205b 4675 6e63 7469     trans [Functi
-00015610: 6f6e 206f 7220 6d69 636f 6d70 7574 696e  on or micomputin
-00015620: 672e 5370 6174 6961 6c54 7261 6e73 666f  g.SpatialTransfo
-00015630: 726d 6174 696f 6e5d 3a20 5472 616e 7366  rmation]: Transf
-00015640: 6f72 6d61 7469 6f6e 2066 756e 6374 696f  ormation functio
-00015650: 6e2c 206d 6170 7069 6e67 0a20 2020 2020  n, mapping.     
-00015660: 2020 2020 2020 2073 697a 653a 2028 5b6e         size: ([n
-00015670: 5f62 6174 6368 3a6f 7074 696f 6e61 6c5d  _batch:optional]
-00015680: 2c20 7b6e 5f64 696d 7d2c 206e 4031 2c20  , {n_dim}, n@1, 
-00015690: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
-000156a0: 6d29 2074 6f20 285b 6e5f 6261 7463 685d  m) to ([n_batch]
-000156b0: 2c20 7b6e 5f64 696d 7d2c 206e 4031 2c20  , {n_dim}, n@1, 
-000156c0: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
-000156d0: 6d29 0a20 2020 2020 2020 206d 6574 686f  m).        metho
-000156e0: 6420 5b73 7472 3a20 6c69 6e65 6172 7c6e  d [str: linear|n
-000156f0: 6561 7265 7374 5d3a 2054 6865 2069 6e74  earest]: The int
-00015700: 6572 706f 6c61 7469 6f6e 206d 6574 686f  erpolation metho
-00015710: 642e 200a 2020 2020 2020 2020 7461 7267  d. .        targ
-00015720: 6574 5f73 7061 6365 205b 7475 706c 6520  et_space [tuple 
-00015730: 6f72 2062 742e 5465 6e73 6f72 5d3a 0a20  or bt.Tensor]:. 
-00015740: 2020 2020 2020 2020 2020 2053 697a 6520             Size 
-00015750: 2874 7570 6c65 2920 6f66 2061 2074 6172  (tuple) of a tar
-00015760: 6765 7420 524f 4920 6174 2074 6865 2063  get ROI at the c
-00015770: 656e 7465 7220 6f66 2069 6d61 6765 2e20  enter of image. 
-00015780: 0a20 2020 2020 2020 2020 2020 204f 5220  .            OR 
-00015790: 5472 616e 7366 6f72 6d65 6420 636f 6f72  Transformed coor
-000157a0: 6469 6e61 7465 2073 7061 6365 2028 6274  dinate space (bt
-000157b0: 2e54 656e 736f 7229 206f 6620 7468 6520  .Tensor) of the 
-000157c0: 6f75 7470 7574 2069 6d61 6765 2e20 0a20  output image. . 
-000157d0: 2020 2020 2020 2020 2020 2073 697a 653a             size:
-000157e0: 206c 656e 6774 6828 6e5f 6469 6d29 206f   length(n_dim) o
-000157f0: 7220 285b 6e5f 6261 7463 683a 6f70 7469  r ([n_batch:opti
-00015800: 6f6e 616c 5d2c 207b 6e5f 6469 6d3a 6f70  onal], {n_dim:op
-00015810: 7469 6f6e 616c 7d2c 2073 697a 6540 312c  tional}, size@1,
-00015820: 2073 697a 6540 322c 202e 2e2e 2c20 7369   size@2, ..., si
-00015830: 7a65 406e 5f64 696d 290a 2020 2020 2020  ze@n_dim).      
-00015840: 2020 6669 6c6c 205b 7374 723a 206e 6561    fill [str: nea
-00015850: 7265 7374 7c62 6163 6b67 726f 756e 6420  rest|background 
-00015860: 6f72 2069 6e74 206f 7220 666c 6f61 7428  or int or float(
-00015870: 6e75 6d62 6572 295d 3a20 496e 6469 6361  number)]: Indica
-00015880: 7465 2074 6865 2077 6179 2074 6f20 6669  te the way to fi
-00015890: 6c6c 2062 6163 6b67 726f 756e 6420 6f75  ll background ou
-000158a0: 7473 6964 6520 6053 7572 726f 756e 6469  tside `Surroundi
-000158b0: 6e67 602e 200a 2020 2020 2020 2020 6465  ng`. .        de
-000158c0: 7269 7661 7469 7665 205b 626f 6f6c 5d3a  rivative [bool]:
-000158d0: 2057 6865 7468 6572 2074 6f20 7265 7475   Whether to retu
-000158e0: 726e 2074 6865 2067 7261 6469 656e 742e  rn the gradient.
-000158f0: 204f 6e65 2063 616e 206f 6d69 7420 6974   One can omit it
-00015900: 2077 6865 6e20 7573 696e 6720 746f 7263   when using torc
-00015910: 682e 6175 746f 6772 6164 2e0a 0a20 2020  h.autograd...   
-00015920: 2020 2020 206f 7574 7075 7420 5b62 742e       output [bt.
-00015930: 5465 6e73 6f72 5d3a 2054 6865 2074 7261  Tensor]: The tra
-00015940: 6e73 666f 726d 6564 2069 6d61 6765 2e0a  nsformed image..
-00015950: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-00015960: 3a20 285b 6e5f 6261 7463 685d 2c20 7b6e  : ([n_batch], {n
-00015970: 5f63 6861 6e6e 656c 3a6f 7074 696f 6e61  _channel:optiona
-00015980: 6c7d 2c20 6d40 312c 206d 4032 2c20 2e2e  l}, m@1, m@2, ..
-00015990: 2e2c 206d 406e 5f64 696d 290a 2020 2020  ., m@n_dim).    
-000159a0: 2020 2020 2020 2020 6f72 2077 6865 6e20          or when 
-000159b0: 6074 6172 6765 745f 7370 6163 6560 2069  `target_space` i
-000159c0: 7320 6465 6669 6e65 6420 6279 2074 656e  s defined by ten
-000159d0: 736f 722e 200a 2020 2020 2020 2020 2020  sor. .          
-000159e0: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
-000159f0: 685d 2c20 7369 7a65 4031 2c20 7369 7a65  h], size@1, size
-00015a00: 4032 2c20 2e2e 2e2c 2073 697a 6540 6e5f  @2, ..., size@n_
-00015a10: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
-00015a20: 206f 7220 7468 6520 6465 7269 7661 7469   or the derivati
-00015a30: 7665 2066 6f72 2074 6865 2069 6e74 6572  ve for the inter
-00015a40: 706f 6c61 7469 6f6e 2e20 2869 6620 6064  polation. (if `d
-00015a50: 6572 6976 6174 6976 6520 3d20 5472 7565  erivative = True
-00015a60: 6029 0a20 2020 2020 2020 2020 2020 2073  `).            s
-00015a70: 697a 653a 2028 5b6e 5f62 6174 6368 5d2c  ize: ([n_batch],
-00015a80: 207b 6e5f 6469 6d7d 2c20 7369 7a65 4031   {n_dim}, size@1
-00015a90: 2c20 7369 7a65 4032 2c20 2e2e 2e2c 2073  , size@2, ..., s
-00015aa0: 697a 6540 6e5f 6469 6d29 0a0a 2020 2020  ize@n_dim)..    
-00015ab0: 4578 616d 706c 6573 3a0a 2020 2020 2d2d  Examples:.    --
-00015ac0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 203e 3e3e  --------.    >>>
-00015ad0: 2049 6d61 6765 203d 2062 742e 7261 6e64   Image = bt.rand
-00015ae0: 2833 2c20 3130 302c 2031 3230 2c20 3830  (3, 100, 120, 80
-00015af0: 290a 2020 2020 3e3e 3e20 414d 203d 2062  ).    >>> AM = b
-00015b00: 742e 7261 6e64 2834 2c20 3429 0a20 2020  t.rand(4, 4).   
-00015b10: 203e 3e3e 2041 4d5b 332c 203a 5d20 3d20   >>> AM[3, :] = 
-00015b20: 6274 2e6f 6e65 5f68 6f74 282d 312c 2034  bt.one_hot(-1, 4
-00015b30: 290a 2020 2020 3e3e 3e20 696e 7465 7270  ).    >>> interp
-00015b40: 6f6c 6174 696f 6e28 496d 6167 652c 2041  olation(Image, A
-00015b50: 6666 696e 6528 414d 292c 206d 6574 686f  ffine(AM), metho
-00015b60: 643d 274c 696e 6561 7227 290a 2020 2020  d='Linear').    
-00015b70: 2727 270a 2020 2020 6966 2074 7261 6e73  '''.    if trans
-00015b80: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-00015b90: 2074 7261 6e73 2e62 6163 6b77 6172 643a   trans.backward:
-00015ba0: 0a20 2020 2020 2020 2069 6620 6861 7361  .        if hasa
-00015bb0: 7474 7228 7472 616e 732c 2027 696e 7627  ttr(trans, 'inv'
-00015bc0: 293a 2074 7261 6e73 203d 2074 7261 6e73  ): trans = trans
-00015bd0: 2e69 6e76 2829 2e66 616b 655f 696e 7628  .inv().fake_inv(
-00015be0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00015bf0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00015c00: 7428 2257 6172 6e69 6e67 3a20 4261 636b  t("Warning: Back
-00015c10: 7761 7264 2074 7261 6e73 666f 726d 6174  ward transformat
-00015c20: 696f 6e20 666f 756e 6420 696e 206d 6574  ion found in met
-00015c30: 686f 6420 6069 6e74 6572 706f 6c61 7469  hod `interpolati
-00015c40: 6f6e 5f66 6f72 7761 7264 602e 2055 7369  on_forward`. Usi
-00015c50: 6e67 2060 696e 7465 7270 6f6c 6174 696f  ng `interpolatio
-00015c60: 6e60 2069 6e73 7465 6164 2e20 2229 0a20  n` instead. "). 
-00015c70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00015c80: 6e20 696e 7465 7270 6f6c 6174 696f 6e28  n interpolation(
-00015c90: 696d 6167 652c 2074 7261 6e73 2c20 6d65  image, trans, me
-00015ca0: 7468 6f64 203d 206d 6574 686f 642c 2074  thod = method, t
-00015cb0: 6172 6765 745f 7370 6163 6520 3d20 7461  arget_space = ta
-00015cc0: 7267 6574 5f73 7061 6365 2c20 6669 6c6c  rget_space, fill
-00015cd0: 203d 2066 696c 6c29 0a20 2020 2072 6574   = fill).    ret
-00015ce0: 7572 6e20 4e6f 7449 6d70 6c65 6d65 6e74  urn NotImplement
-00015cf0: 6564 0a0a 2323 2323 2323 2323 2323 2323  ed..############
-00015d00: 2049 6d61 6765 2054 7261 6e73 666f 726d   Image Transform
-00015d10: 6174 696f 6e73 2023 2323 2323 2323 2323  ations #########
-00015d20: 2323 230a 0a63 6c61 7373 2049 6d61 6765  ###..class Image
-00015d30: 5472 616e 7366 6f72 6d61 7469 6f6e 2854  Transformation(T
-00015d40: 7261 6e73 666f 726d 6174 696f 6e29 3a0a  ransformation):.
-00015d50: 2020 2020 2020 2020 0a20 2020 2064 6566          .    def
-00015d60: 205f 5f63 616c 6c5f 5f28 7365 6c66 2c20   __call__(self, 
-00015d70: 5829 3a0a 2020 2020 2020 2020 2727 270a  X):.        '''.
-00015d80: 2020 2020 2020 2020 5820 5b62 742e 5465          X [bt.Te
-00015d90: 6e73 6f72 5d3a 2049 6d61 6765 2074 6f20  nsor]: Image to 
-00015da0: 6265 2074 7261 6e73 666f 726d 6564 2e0a  be transformed..
-00015db0: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-00015dc0: 3a20 285b 6e5f 6261 7463 683a 6f70 7469  : ([n_batch:opti
-00015dd0: 6f6e 616c 5d2c 207b 6e5f 6368 616e 6e65  onal], {n_channe
-00015de0: 6c3a 6f70 7469 6f6e 616c 7d2c 206e 4031  l:optional}, n@1
-00015df0: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
-00015e00: 6469 6d29 0a20 2020 2020 2020 206f 7574  dim).        out
-00015e10: 7075 7420 5b62 742e 5465 6e73 6f72 5d3a  put [bt.Tensor]:
-00015e20: 2054 6865 2074 7261 6e73 666f 726d 6564   The transformed
-00015e30: 2069 6d61 6765 2e0a 2020 2020 2020 2020   image..        
-00015e40: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
-00015e50: 7463 685d 2c20 7b6e 5f63 6861 6e6e 656c  tch], {n_channel
-00015e60: 7d2c 206e 4031 2c20 6e40 322c 202e 2e2e  }, n@1, n@2, ...
-00015e70: 2c20 6e40 6e5f 6469 6d29 0a20 2020 2020  , n@n_dim).     
-00015e80: 2020 2027 2727 0a20 2020 2020 2020 2058     '''.        X
-00015e90: 203d 2062 6174 6f72 6368 5f74 656e 736f   = batorch_tenso
-00015ea0: 7228 5829 0a20 2020 2020 2020 2069 6620  r(X).        if 
-00015eb0: 7365 6c66 2e6e 5f64 696d 2069 7320 4e6f  self.n_dim is No
-00015ec0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00015ed0: 6966 206e 6f74 2058 2e68 6173 5f62 6174  if not X.has_bat
-00015ee0: 6368 3a20 5820 3d20 582e 756e 7371 7565  ch: X = X.unsque
-00015ef0: 657a 6528 5b5d 290a 2020 2020 2020 2020  eze([]).        
-00015f00: 2020 2020 6966 206e 6f74 2058 2e68 6173      if not X.has
-00015f10: 5f63 6861 6e6e 656c 3a20 5820 3d20 582e  _channel: X = X.
-00015f20: 7374 616e 6461 7264 2829 2e75 6e73 7175  standard().unsqu
-00015f30: 6565 7a65 287b 317d 290a 2020 2020 2020  eeze({1}).      
-00015f40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00015f50: 2020 2020 6966 2058 2e6e 5f64 696d 203d      if X.n_dim =
-00015f60: 3d20 7365 6c66 2e6e 5f64 696d 3a20 5820  = self.n_dim: X 
-00015f70: 3d20 582e 7265 6d6f 7665 5f73 7065 6369  = X.remove_speci
-00015f80: 616c 5f28 292e 756e 7371 7565 657a 6528  al_().unsqueeze(
-00015f90: 5b5d 292e 756e 7371 7565 657a 6528 7b31  []).unsqueeze({1
-00015fa0: 7d29 0a20 2020 2020 2020 2020 2020 2065  }).            e
-00015fb0: 6c69 6620 582e 6e5f 6469 6d20 3d3d 2073  lif X.n_dim == s
-00015fc0: 656c 662e 6e5f 6469 6d20 2b20 313a 0a20  elf.n_dim + 1:. 
-00015fd0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00015fe0: 6620 582e 6861 735f 6261 7463 683a 2058  f X.has_batch: X
-00015ff0: 2e63 6861 6e6e 656c 5f64 696d 656e 7369  .channel_dimensi
-00016000: 6f6e 203d 204e 6f6e 653b 2058 203d 2058  on = None; X = X
-00016010: 2e75 6e73 7175 6565 7a65 287b 3020 6966  .unsqueeze({0 if
-00016020: 2058 2e62 6174 6368 5f64 696d 656e 7369   X.batch_dimensi
-00016030: 6f6e 203e 2030 2065 6c73 6520 317d 290a  on > 0 else 1}).
-00016040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016050: 656c 6966 2058 2e68 6173 5f63 6861 6e6e  elif X.has_chann
-00016060: 656c 3a20 5820 3d20 582e 756e 7371 7565  el: X = X.unsque
-00016070: 657a 6528 5b5d 290a 2020 2020 2020 2020  eze([]).        
-00016080: 2020 2020 2020 2020 656c 7365 3a20 5820          else: X 
-00016090: 3d20 582e 6261 7463 685f 6469 6d65 6e73  = X.batch_dimens
-000160a0: 696f 6e5f 2830 292e 756e 7371 7565 657a  ion_(0).unsqueez
-000160b0: 6528 7b31 7d29 0a20 2020 2020 2020 2020  e({1}).         
-000160c0: 2020 2065 6c69 6620 582e 6e5f 6469 6d20     elif X.n_dim 
-000160d0: 3d3d 2073 656c 662e 6e5f 6469 6d20 2b20  == self.n_dim + 
-000160e0: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
-000160f0: 2020 2023 205f 6368 616e 6e61 6c2f 6261     # _channal/ba
-00016100: 7463 6820 6469 6d65 6e73 696f 6e73 2075  tch dimensions u
-00016110: 7365 6420 6865 7265 2061 7320 7468 6579  sed here as they
-00016120: 2061 7265 206e 5f64 696d 2077 6865 6e20   are n_dim when 
-00016130: 6e6f 7420 6578 6973 7465 642e 200a 2020  not existed. .  
-00016140: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00016150: 206e 6f74 2058 2e68 6173 5f62 6174 6368   not X.has_batch
-00016160: 3a20 582e 6261 7463 685f 6469 6d65 6e73  : X.batch_dimens
-00016170: 696f 6e20 3d20 3020 6966 2058 2e5f 6368  ion = 0 if X._ch
-00016180: 616e 6e65 6c5f 6469 6d65 6e73 696f 6e20  annel_dimension 
-00016190: 3e20 3020 656c 7365 2031 0a20 2020 2020  > 0 else 1.     
-000161a0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-000161b0: 7420 582e 6861 735f 6368 616e 6e65 6c3a  t X.has_channel:
-000161c0: 2058 2e63 6861 6e6e 656c 5f64 696d 656e   X.channel_dimen
-000161d0: 7369 6f6e 203d 2030 2069 6620 582e 5f62  sion = 0 if X._b
-000161e0: 6174 6368 5f64 696d 656e 7369 6f6e 203e  atch_dimension >
-000161f0: 2030 2065 6c73 6520 310a 2020 2020 2020   0 else 1.      
-00016200: 2020 6176 6f75 6368 2858 2e68 6173 5f62    avouch(X.has_b
-00016210: 6174 6368 2061 6e64 2058 2e68 6173 5f63  atch and X.has_c
-00016220: 6861 6e6e 656c 2c20 6622 506c 6561 7365  hannel, f"Please
-00016230: 2075 7365 2062 6174 6f72 6368 2074 656e   use batorch ten
-00016240: 736f 7220 6f66 2073 697a 6520 5c0a 2020  sor of size \.  
-00016250: 2020 2020 2020 2020 2020 285b 6e5f 6261            ([n_ba
-00016260: 7463 685d 2c20 7b7b 6e5f 6368 616e 6e65  tch], {{n_channe
-00016270: 6c2f 6e5f 6665 6174 7572 653a 6f70 7469  l/n_feature:opti
-00016280: 6f6e 616c 7d7d 2c20 6d5f 312c 206d 5f32  onal}}, m_1, m_2
-00016290: 2c20 2e2e 2e2c 206d 5f72 2920 5b72 3d6e  , ..., m_r) [r=n
-000162a0: 5f64 696d 5d20 666f 7220 5c0a 2020 2020  _dim] for \.    
-000162b0: 2020 2020 2020 2020 2020 2020 7b73 656c              {sel
-000162c0: 662e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  f.__class__.__na
-000162d0: 6d65 5f5f 2e73 706c 6974 2827 2e27 295b  me__.split('.')[
-000162e0: 2d31 5d7d 2054 7261 6e73 666f 726d 6174  -1]} Transformat
-000162f0: 696f 6e2c 2069 6e73 7465 6164 206f 6620  ion, instead of 
-00016300: 7b58 2e73 6861 7065 7d2e 2022 290a 2020  {X.shape}. ").  
-00016310: 2020 2020 2020 7265 7475 726e 2058 2e63        return X.c
-00016320: 6c6f 6e65 2829 0a0a 636c 6173 7320 4e6f  lone()..class No
-00016330: 726d 616c 697a 6528 496d 6167 6554 7261  rmalize(ImageTra
-00016340: 6e73 666f 726d 6174 696f 6e29 3a0a 2020  nsformation):.  
-00016350: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00016360: 656c 662c 202a 5f72 616e 6765 293a 0a20  elf, *_range):. 
-00016370: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00016380: 2020 204e 6f72 6d61 6c69 7a65 2074 6865     Normalize the
-00016390: 2069 6e74 656e 7369 7479 206f 6620 616e   intensity of an
-000163a0: 2069 6d61 6765 2e0a 2020 2020 2020 2020   image..        
-000163b0: 0a20 2020 2020 2020 2050 6172 616d 733a  .        Params:
-000163c0: 0a20 2020 2020 2020 2020 2020 205f 7261  .            _ra
-000163d0: 6e67 6520 3d20 286c 6f77 2c20 6869 6768  nge = (low, high
-000163e0: 2920 5b69 6e74 206f 7220 666c 6f61 7420  ) [int or float 
-000163f0: 6f72 2062 742e 5465 6e73 6f72 5d3a 2054  or bt.Tensor]: T
-00016400: 6865 206c 6f77 6573 7420 2861 6e64 2068  he lowest (and h
-00016410: 6967 6865 7374 2920 696e 7465 6e73 6974  ighest) intensit
-00016420: 792e 200a 2020 2020 2020 2020 2020 2020  y. .            
-00016430: 2020 2020 7369 7a65 3a20 6c65 6e67 7468      size: length
-00016440: 2832 2920 6f72 2028 5b6e 5f62 6174 6368  (2) or ([n_batch
-00016450: 5d2c 207b 327d 290a 2020 2020 2020 2020  ], {2}).        
-00016460: 2020 2020 0a20 2020 2020 2020 2057 6865      .        Whe
-00016470: 6e20 6974 2069 7320 6361 6c6c 6564 3a0a  n it is called:.
-00016480: 2020 2020 2020 2020 2020 2020 5820 5b62              X [b
-00016490: 742e 5465 6e73 6f72 5d3a 2049 6d61 6765  t.Tensor]: Image
-000164a0: 2074 6f20 6265 2074 7261 6e73 666f 726d   to be transform
-000164b0: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-000164c0: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
-000164d0: 7463 683a 6f70 7469 6f6e 616c 5d2c 207b  tch:optional], {
-000164e0: 6e5f 6368 616e 6e65 6c3a 6f70 7469 6f6e  n_channel:option
-000164f0: 616c 7d2c 206e 4031 2c20 6e40 322c 202e  al}, n@1, n@2, .
-00016500: 2e2e 2c20 6e40 6e5f 6469 6d29 0a20 2020  .., n@n_dim).   
-00016510: 2020 2020 2020 2020 206f 7574 7075 7420           output 
-00016520: 5b62 742e 5465 6e73 6f72 5d3a 2054 6865  [bt.Tensor]: The
-00016530: 2074 7261 6e73 666f 726d 6564 2069 6d61   transformed ima
-00016540: 6765 2e0a 2020 2020 2020 2020 2020 2020  ge..            
-00016550: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
-00016560: 7463 685d 2c20 7b6e 5f63 6861 6e6e 656c  tch], {n_channel
-00016570: 7d2c 206e 4031 2c20 6e40 322c 202e 2e2e  }, n@1, n@2, ...
-00016580: 2c20 6e40 6e5f 6469 6d29 0a20 2020 2020  , n@n_dim).     
-00016590: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
-000165a0: 6620 6c65 6e28 5f72 616e 6765 2920 3d3d  f len(_range) ==
-000165b0: 2030 3a20 5f72 616e 6765 203d 204e 6f6e   0: _range = Non
-000165c0: 650a 2020 2020 2020 2020 656c 6966 206c  e.        elif l
-000165d0: 656e 285f 7261 6e67 6529 203d 3d20 3120  en(_range) == 1 
-000165e0: 616e 6420 6973 696e 7374 616e 6365 285f  and isinstance(_
-000165f0: 7261 6e67 655b 305d 2c20 286c 6973 742c  range[0], (list,
-00016600: 2074 7570 6c65 2929 3a20 5f72 616e 6765   tuple)): _range
-00016610: 203d 2062 6174 6f72 6368 5f74 656e 736f   = batorch_tenso
-00016620: 7228 6c69 7374 285f 7261 6e67 655b 305d  r(list(_range[0]
-00016630: 2929 0a20 2020 2020 2020 2065 6c69 6620  )).        elif 
-00016640: 6c65 6e28 5f72 616e 6765 2920 3d3d 2031  len(_range) == 1
-00016650: 2061 6e64 2069 7369 6e73 7461 6e63 6528   and isinstance(
-00016660: 5f72 616e 6765 5b30 5d2c 2062 742e 5465  _range[0], bt.Te
-00016670: 6e73 6f72 293a 205f 7261 6e67 6520 3d20  nsor): _range = 
-00016680: 5f72 616e 6765 5b30 5d0a 2020 2020 2020  _range[0].      
-00016690: 2020 656c 6966 206c 656e 285f 7261 6e67    elif len(_rang
-000166a0: 6529 203d 3d20 313a 205f 7261 6e67 6520  e) == 1: _range 
-000166b0: 3d20 6274 2e63 6861 6e6e 656c 5f74 656e  = bt.channel_ten
-000166c0: 736f 7228 2830 2c20 5f72 616e 6765 2929  sor((0, _range))
-000166d0: 0a20 2020 2020 2020 2065 6c69 6620 6c65  .        elif le
-000166e0: 6e28 5f72 616e 6765 2920 3d3d 2032 3a20  n(_range) == 2: 
-000166f0: 5f72 616e 6765 203d 2062 742e 6368 616e  _range = bt.chan
-00016700: 6e65 6c5f 7465 6e73 6f72 285f 7261 6e67  nel_tensor(_rang
-00016710: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
-00016720: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-00016730: 2866 2249 6e76 616c 6964 2072 616e 6765  (f"Invalid range
-00016740: 2066 6f72 204e 6f72 6d61 6c69 7a65 3a20   for Normalize: 
-00016750: 7b5f 7261 6e67 657d 2e20 2229 0a20 2020  {_range}. ").   
-00016760: 2020 2020 2069 6620 5f72 616e 6765 2069       if _range i
-00016770: 7320 4e6f 6e65 3a20 7061 7373 0a20 2020  s None: pass.   
-00016780: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00016790: 2020 2020 2020 2069 6620 5f72 616e 6765         if _range
-000167a0: 2e6e 5f64 696d 203c 2032 3a20 5f72 616e  .n_dim < 2: _ran
-000167b0: 6765 203d 205f 7261 6e67 652e 756e 7371  ge = _range.unsq
-000167c0: 7565 657a 6528 5b5d 290a 2020 2020 2020  ueeze([]).      
-000167d0: 2020 2020 2020 6966 206e 6f74 205f 7261        if not _ra
-000167e0: 6e67 652e 6861 735f 6261 7463 683a 205f  nge.has_batch: _
-000167f0: 7261 6e67 652e 6261 7463 685f 6469 6d65  range.batch_dime
-00016800: 6e73 696f 6e20 3d20 300a 2020 2020 2020  nsion = 0.      
-00016810: 2020 2020 2020 6966 206e 6f74 205f 7261        if not _ra
-00016820: 6e67 652e 6861 735f 6368 616e 6e65 6c3a  nge.has_channel:
-00016830: 205f 7261 6e67 652e 6368 616e 6e65 6c5f   _range.channel_
-00016840: 6469 6d65 6e73 696f 6e20 3d20 310a 2020  dimension = 1.  
-00016850: 2020 2020 2020 2020 2020 6176 6f75 6368            avouch
-00016860: 285f 7261 6e67 652e 6861 735f 6261 7463  (_range.has_batc
-00016870: 6820 616e 6420 5f72 616e 6765 2e68 6173  h and _range.has
-00016880: 5f63 6861 6e6e 656c 2c20 6622 506c 6561  _channel, f"Plea
-00016890: 7365 2075 7365 2062 6174 6f72 6368 2074  se use batorch t
-000168a0: 656e 736f 7220 6f66 2073 697a 6520 5c0a  ensor of size \.
-000168b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168c0: 285b 6e5f 6261 7463 683a 6f70 7469 6f6e  ([n_batch:option
-000168d0: 616c 5d2c 207b 7b32 7d7d 2920 666f 7220  al], {{2}}) for 
-000168e0: 4e6f 726d 616c 697a 696e 6720 7061 7261  Normalizing para
-000168f0: 6d65 7465 7273 2c20 696e 7374 6561 6420  meters, instead 
-00016900: 6f66 207b 5f72 616e 6765 2e73 6861 7065  of {_range.shape
-00016910: 7d2e 2022 290a 2020 2020 2020 2020 7375  }. ").        su
-00016920: 7065 7228 292e 5f5f 696e 6974 5f5f 285f  per().__init__(_
-00016930: 7261 6e67 6529 0a20 2020 2020 2020 2073  range).        s
-00016940: 656c 662e 7261 6e67 6520 3d20 5f72 616e  elf.range = _ran
-00016950: 6765 0a20 2020 2020 2020 2073 656c 662e  ge.        self.
-00016960: 5f72 616e 6765 203d 204e 6f6e 650a 0a20  _range = None.. 
-00016970: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
-00016980: 7365 6c66 2c20 5829 3a0a 2020 2020 2020  self, X):.      
-00016990: 2020 5820 3d20 7375 7065 7228 292e 5f5f    X = super().__
-000169a0: 6361 6c6c 5f5f 2858 290a 2020 2020 2020  call__(X).      
-000169b0: 2020 5f72 616e 6765 203d 2073 656c 662e    _range = self.
-000169c0: 7261 6e67 650a 2020 2020 2020 2020 6966  range.        if
-000169d0: 205f 7261 6e67 6520 6973 204e 6f6e 653a   _range is None:
-000169e0: 0a20 2020 2020 2020 2020 2020 205f 7261  .            _ra
-000169f0: 6e67 6520 3d20 6274 2e71 7561 6e74 696c  nge = bt.quantil
-00016a00: 6528 582e 666c 6174 7465 6e28 292e 666c  e(X.flatten().fl
-00016a10: 6f61 7428 292c 2062 6174 6f72 6368 5f74  oat(), batorch_t
-00016a20: 656e 736f 7228 5b30 2e30 3235 2c20 302e  ensor([0.025, 0.
-00016a30: 3937 355d 292c 2061 7869 733d 2d31 292e  975]), axis=-1).
-00016a40: 6d6f 7665 6469 6d28 302c 202d 3129 2e73  movedim(0, -1).s
-00016a50: 7065 6369 616c 5f66 726f 6d5f 2858 290a  pecial_from_(X).
-00016a60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016a70: 2e5f 7261 6e67 6520 3d20 5f72 616e 6765  ._range = _range
-00016a80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00016a90: 2828 5820 2d20 5f72 616e 6765 5b2e 2e2e  ((X - _range[...
-00016aa0: 2c20 305d 2920 2f20 285f 7261 6e67 655b  , 0]) / (_range[
-00016ab0: 2e2e 2e2c 2031 5d20 2d20 5f72 616e 6765  ..., 1] - _range
-00016ac0: 5b2e 2e2e 2c20 305d 2929 2e63 6c61 6d70  [..., 0])).clamp
-00016ad0: 2830 2e2c 2031 2e29 0a20 2020 200a 2020  (0., 1.).    .  
-00016ae0: 2020 6465 6620 696e 7628 7365 6c66 293a    def inv(self):
-00016af0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00016b00: 2e72 616e 6765 2069 7320 6e6f 7420 4e6f  .range is not No
-00016b10: 6e65 3a20 5f72 616e 6765 203d 2073 656c  ne: _range = sel
-00016b20: 662e 7261 6e67 650a 2020 2020 2020 2020  f.range.        
-00016b30: 656c 6966 2073 656c 662e 5f72 616e 6765  elif self._range
-00016b40: 2069 7320 6e6f 7420 4e6f 6e65 3a20 5f72   is not None: _r
-00016b50: 616e 6765 203d 2073 656c 662e 5f72 616e  ange = self._ran
-00016b60: 6765 0a20 2020 2020 2020 2065 6c73 653a  ge.        else:
-00016b70: 2072 6574 7572 6e20 4e6f 726d 616c 697a   return Normaliz
-00016b80: 6528 4e6f 6e65 290a 2020 2020 2020 2020  e(None).        
-00016b90: 6465 6e20 3d20 5f72 616e 6765 5b2e 2e2e  den = _range[...
-00016ba0: 2c20 315d 202d 205f 7261 6e67 655b 2e2e  , 1] - _range[..
-00016bb0: 2e2c 2030 5d0a 2020 2020 2020 2020 5f72  ., 0].        _r
-00016bc0: 616e 6765 203d 2062 742e 7374 6163 6b28  ange = bt.stack(
-00016bd0: 2d5f 7261 6e67 655b 2e2e 2e2c 2030 5d2c  -_range[..., 0],
-00016be0: 2031 2d5f 7261 6e67 655b 2e2e 2e2c 2030   1-_range[..., 0
-00016bf0: 5d2c 202d 3129 202f 2064 656e 0a20 2020  ], -1) / den.   
-00016c00: 2020 2020 2072 6574 7572 6e20 4e6f 726d       return Norm
-00016c10: 616c 697a 6528 5f72 616e 6765 290a 0a23  alize(_range)..#
-00016c20: 2323 2323 2323 2323 2323 2323 2053 7570  ############ Sup
-00016c30: 706f 7274 696e 6720 4675 6e63 7469 6f6e  porting Function
-00016c40: 7320 2323 2323 2323 2323 2323 2323 0a0a  s ############..
-00016c50: 6465 6620 4273 706c 696e 6528 692c 2055  def Bspline(i, U
-00016c60: 293a 0a20 2020 2022 2222 0a20 2020 2043  ):.    """.    C
-00016c70: 7562 6963 2042 2d73 706c 696e 6520 6675  ubic B-spline fu
-00016c80: 6e63 7469 6f6e 2e20 0a20 2020 204e 6f74  nction. .    Not
-00016c90: 653a 2041 7320 6c6f 6e67 2061 7320 6920  e: As long as i 
-00016ca0: 616e 6420 5520 6861 7665 2074 6865 2073  and U have the s
-00016cb0: 616d 6520 7369 7a65 2c20 616e 7920 7368  ame size, any sh
-00016cc0: 6170 6520 6f66 2074 656e 736f 7273 2077  ape of tensors w
-00016cd0: 6f75 6c64 2064 6f2e 0a20 2020 200a 2020  ould do..    .  
-00016ce0: 2020 5061 7261 6d73 3a0a 2020 2020 2020    Params:.      
-00016cf0: 2020 6920 5b62 742e 5465 6e73 6f72 5d3a    i [bt.Tensor]:
-00016d00: 2074 6865 2069 6e64 6578 206f 6620 7365   the index of se
-00016d10: 676d 656e 7420 6675 6e63 7469 6f6e 206f  gment function o
-00016d20: 6620 422d 7370 6c69 6e65 2e0a 2020 2020  f B-spline..    
-00016d30: 2020 2020 2020 2020 5468 6520 7661 6c75          The valu
-00016d40: 6520 6f66 2065 6163 6820 656c 656d 656e  e of each elemen
-00016d50: 7420 6361 6e20 6265 2063 686f 7365 6e20  t can be chosen 
-00016d60: 696e 2028 2d31 2c20 302c 2031 2c20 3229  in (-1, 0, 1, 2)
-00016d70: 2e20 0a20 2020 2020 2020 2055 205b 6274  . .        U [bt
-00016d80: 2e54 656e 736f 725d 3a20 7468 6520 6465  .Tensor]: the de
-00016d90: 6369 6d61 6c20 6172 6775 6d65 6e74 206f  cimal argument o
-00016da0: 6620 422d 7370 6c69 6e65 2066 756e 6374  f B-spline funct
-00016db0: 696f 6e2e 2049 7420 7368 6f75 6c64 2062  ion. It should b
-00016dc0: 6520 7769 7468 696e 2072 616e 6765 205b  e within range [
-00016dd0: 302c 2031 292e 0a20 2020 2022 2222 0a20  0, 1)..    """. 
-00016de0: 2020 2069 203d 2062 6174 6f72 6368 5f74     i = batorch_t
-00016df0: 656e 736f 7228 6929 3b20 5520 3d20 6261  ensor(i); U = ba
-00016e00: 746f 7263 685f 7465 6e73 6f72 2855 290a  torch_tensor(U).
-00016e10: 2020 2020 7265 7475 726e 2028 0a20 2020      return (.   
-00016e20: 2020 2020 2062 742e 7768 6572 6528 6920       bt.where(i 
-00016e30: 3d3d 202d 312c 2028 3120 2d20 5529 202a  == -1, (1 - U) *
-00016e40: 2a20 3320 2f20 362c 0a20 2020 2020 2020  * 3 / 6,.       
-00016e50: 2062 742e 7768 6572 6528 6920 3d3d 2030   bt.where(i == 0
-00016e60: 2c20 5520 2a2a 2033 202f 2032 202d 2055  , U ** 3 / 2 - U
-00016e70: 202a 2055 202b 2032 202f 2033 2c0a 2020   * U + 2 / 3,.  
-00016e80: 2020 2020 2020 6274 2e77 6865 7265 2869        bt.where(i
-00016e90: 203d 3d20 312c 2028 2d20 3320 2a20 5520   == 1, (- 3 * U 
-00016ea0: 2a2a 2033 202b 2033 202a 2055 202a 2055  ** 3 + 3 * U * U
-00016eb0: 202b 2033 202a 2055 202b 2031 2920 2f20   + 3 * U + 1) / 
-00016ec0: 362c 0a20 2020 2020 2020 2062 742e 7768  6,.        bt.wh
-00016ed0: 6572 6528 6920 3d3d 2032 2c20 5520 2a2a  ere(i == 2, U **
-00016ee0: 2033 202f 2036 2c0a 2020 2020 2020 2020   3 / 6,.        
-00016ef0: 6274 2e7a 6572 6f73 5f6c 696b 6528 5529  bt.zeros_like(U)
-00016f00: 2929 2929 0a20 2020 2029 0a0a 6465 6620  )))).    )..def 
-00016f10: 6442 7370 6c69 6e65 2869 2c20 5529 3a0a  dBspline(i, U):.
-00016f20: 2020 2020 2222 220a 2020 2020 5468 6520      """.    The 
-00016f30: 6465 7269 7661 7469 7665 206f 6620 422d  derivative of B-
-00016f40: 7370 6c69 6e65 2066 756e 6374 696f 6e2c  spline function,
-00016f50: 2077 6974 6820 7265 7370 6563 7420 746f   with respect to
-00016f60: 2055 2e20 0a20 2020 204e 6f74 653a 2041   U. .    Note: A
-00016f70: 7320 6c6f 6e67 2061 7320 6920 616e 6420  s long as i and 
-00016f80: 5520 6861 7665 2074 6865 2073 616d 6520  U have the same 
-00016f90: 7369 7a65 2c20 616e 7920 7368 6170 6520  size, any shape 
-00016fa0: 6f66 2074 656e 736f 7273 2077 6f75 6c64  of tensors would
-00016fb0: 2064 6f2e 0a20 2020 200a 2020 2020 5061   do..    .    Pa
-00016fc0: 7261 6d73 3a0a 2020 2020 2020 2020 6920  rams:.        i 
-00016fd0: 5b62 742e 5465 6e73 6f72 5d3a 2074 6865  [bt.Tensor]: the
-00016fe0: 2069 6e64 6578 206f 6620 7365 676d 656e   index of segmen
-00016ff0: 7420 6675 6e63 7469 6f6e 206f 6620 422d  t function of B-
-00017000: 7370 6c69 6e65 2e0a 2020 2020 2020 2020  spline..        
-00017010: 2020 2020 5468 6520 7661 6c75 6520 6f66      The value of
-00017020: 2065 6163 6820 656c 656d 656e 7420 6361   each element ca
-00017030: 6e20 6265 2063 686f 7365 6e20 696e 2028  n be chosen in (
-00017040: 2d31 2c20 302c 2031 2c20 3229 2e20 0a20  -1, 0, 1, 2). . 
-00017050: 2020 2020 2020 2055 205b 6274 2e54 656e         U [bt.Ten
-00017060: 736f 725d 3a20 7468 6520 6465 6369 6d61  sor]: the decima
-00017070: 6c20 6172 6775 6d65 6e74 206f 6620 422d  l argument of B-
-00017080: 7370 6c69 6e65 2066 756e 6374 696f 6e2e  spline function.
-00017090: 2049 7420 7368 6f75 6c64 2062 6520 7769   It should be wi
-000170a0: 7468 696e 2072 616e 6765 205b 302c 2031  thin range [0, 1
-000170b0: 292e 0a20 2020 2022 2222 0a20 2020 2069  )..    """.    i
-000170c0: 203d 2062 6174 6f72 6368 5f74 656e 736f   = batorch_tenso
-000170d0: 7228 6929 3b20 5520 3d20 6261 746f 7263  r(i); U = batorc
-000170e0: 685f 7465 6e73 6f72 2855 290a 2020 2020  h_tensor(U).    
-000170f0: 7265 7475 726e 2028 0a20 2020 2020 2020  return (.       
-00017100: 2062 742e 7768 6572 6528 6920 3d3d 202d   bt.where(i == -
-00017110: 312c 202d 2033 202a 2028 3120 2d20 5529  1, - 3 * (1 - U)
-00017120: 202a 2a20 3220 2f20 362c 0a20 2020 2020   ** 2 / 6,.     
-00017130: 2020 2062 742e 7768 6572 6528 6920 3d3d     bt.where(i ==
-00017140: 2030 2c20 3320 2a20 5520 2a2a 2032 202f   0, 3 * U ** 2 /
-00017150: 2032 202d 2032 202a 2055 2c0a 2020 2020   2 - 2 * U,.    
-00017160: 2020 2020 6274 2e77 6865 7265 2869 203d      bt.where(i =
-00017170: 3d20 312c 2028 2d20 3320 2a20 5520 2a2a  = 1, (- 3 * U **
-00017180: 2032 202b 2032 202a 2055 202b 2031 2920   2 + 2 * U + 1) 
-00017190: 2f20 322c 0a20 2020 2020 2020 2062 742e  / 2,.        bt.
-000171a0: 7768 6572 6528 6920 3d3d 2032 2c20 3320  where(i == 2, 3 
-000171b0: 2a20 5520 2a2a 2032 202f 2036 2c0a 2020  * U ** 2 / 6,.  
-000171c0: 2020 2020 2020 6274 2e7a 6572 6f73 5f6c        bt.zeros_l
-000171d0: 696b 6528 5529 2929 2929 0a20 2020 2029  ike(U))))).    )
-000171e0: 0a0a 6465 6620 6642 7370 6c69 6e65 2863  ..def fBspline(c
-000171f0: 2c20 7829 3a0a 2020 2020 6320 3d20 6261  , x):.    c = ba
-00017200: 746f 7263 685f 7465 6e73 6f72 2863 293b  torch_tensor(c);
-00017210: 2078 203d 2062 6174 6f72 6368 5f74 656e   x = batorch_ten
-00017220: 736f 7228 7829 0a20 2020 2064 203d 2078  sor(x).    d = x
-00017230: 202d 2063 0a20 2020 2072 6574 7572 6e20   - c.    return 
-00017240: 280a 2020 2020 2020 2020 6274 2e77 6865  (.        bt.whe
-00017250: 7265 2828 2d32 203c 3d20 6429 202a 2028  re((-2 <= d) * (
-00017260: 6420 3c20 2d31 292c 2064 202a 2a20 3320  d < -1), d ** 3 
-00017270: 2b20 3620 2a20 6420 2a2a 2032 202b 2031  + 6 * d ** 2 + 1
-00017280: 3220 2a20 6420 2b20 382c 0a20 2020 2020  2 * d + 8,.     
-00017290: 2020 2062 742e 7768 6572 6528 282d 3120     bt.where((-1 
-000172a0: 3c3d 2064 2920 2a20 2864 203c 2030 292c  <= d) * (d < 0),
-000172b0: 202d 2033 202a 2064 202a 2a20 3320 2d20   - 3 * d ** 3 - 
-000172c0: 3620 2a20 6420 2a2a 2032 202b 2034 2c0a  6 * d ** 2 + 4,.
-000172d0: 2020 2020 2020 2020 6274 2e77 6865 7265          bt.where
-000172e0: 2828 3020 3c3d 2064 2920 2a20 2864 203c  ((0 <= d) * (d <
-000172f0: 2031 292c 2033 202a 2064 202a 2a20 3320   1), 3 * d ** 3 
-00017300: 2d20 3620 2a20 6420 2a2a 2032 202b 2034  - 6 * d ** 2 + 4
-00017310: 2c0a 2020 2020 2020 2020 6274 2e77 6865  ,.        bt.whe
-00017320: 7265 2828 3120 3c3d 2064 2920 2a20 2864  re((1 <= d) * (d
-00017330: 203c 2032 292c 202d 2064 202a 2a20 3320   < 2), - d ** 3 
-00017340: 2b20 3620 2a20 6420 2a2a 2032 202d 2031  + 6 * d ** 2 - 1
-00017350: 3220 2a20 6420 2b20 382c 0a20 2020 2020  2 * d + 8,.     
-00017360: 2020 2062 742e 7a65 726f 735f 6c69 6b65     bt.zeros_like
-00017370: 2864 2929 2929 2920 2f20 360a 2020 2020  (d))))) / 6.    
-00017380: 290a 0a64 6566 2041 6666 696e 6532 4432  )..def Affine2D2
-00017390: 4d61 7472 6978 2870 6172 616d 7329 3a0a  Matrix(params):.
-000173a0: 2020 2020 2222 220a 2020 2020 7431 2c20      """.    t1, 
-000173b0: 7432 2c20 ceb8 2c20 7331 2c20 7332 2c20  t2, .., s1, s2, 
-000173c0: cf81 312c 20cf 8132 2069 6e20 7369 7a65  ..1, ..2 in size
-000173d0: 3a20 285b 6e5f 6261 7463 685d 2c20 7b37  : ([n_batch], {7
-000173e0: 7d29 0a20 2020 2074 312c 2074 322c 2063  }).    t1, t2, c
-000173f0: 312c 2063 322c 20ce b82c 2073 312c 2073  1, c2, .., s1, s
-00017400: 322c 20cf 8131 2c20 cf81 3220 696e 2073  2, ..1, ..2 in s
-00017410: 697a 653a 2028 5b6e 5f62 6174 6368 5d2c  ize: ([n_batch],
-00017420: 207b 397d 290a 2020 2020 6f75 7470 7574   {9}).    output
-00017430: 2069 6e20 7369 7a65 3a20 285b 6e5f 6261   in size: ([n_ba
-00017440: 7463 685d 2c20 332c 2033 290a 2020 2020  tch], 3, 3).    
-00017450: 2222 220a 2020 2020 7061 7261 6d73 203d  """.    params =
-00017460: 2062 6174 6f72 6368 5f74 656e 736f 7228   batorch_tensor(
-00017470: 7061 7261 6d73 290a 2020 2020 6966 2070  params).    if p
-00017480: 6172 616d 732e 6e5f 6469 6d20 3c3d 2031  arams.n_dim <= 1
-00017490: 2061 6e64 206e 6f74 2070 6172 616d 732e   and not params.
-000174a0: 6861 735f 6261 7463 683a 2070 6172 616d  has_batch: param
-000174b0: 7320 3d20 7061 7261 6d73 2e75 6e73 7175  s = params.unsqu
-000174c0: 6565 7a65 285b 5d29 0a20 2020 2069 6620  eeze([]).    if 
-000174d0: 7061 7261 6d73 2e6e 5f64 696d 203c 3d20  params.n_dim <= 
-000174e0: 3120 616e 6420 6e6f 7420 7061 7261 6d73  1 and not params
-000174f0: 2e68 6173 5f63 6861 6e6e 656c 3a20 7061  .has_channel: pa
-00017500: 7261 6d73 203d 2070 6172 616d 732e 756e  rams = params.un
-00017510: 7371 7565 657a 6528 7b31 7d29 0a20 2020  squeeze({1}).   
-00017520: 2069 6620 7061 7261 6d73 2e6e 5f64 696d   if params.n_dim
-00017530: 203d 3d20 3220 616e 6420 6e6f 7420 7061   == 2 and not pa
-00017540: 7261 6d73 2e68 6173 5f62 6174 6368 3a20  rams.has_batch: 
-00017550: 7061 7261 6d73 2e62 6174 6368 5f64 696d  params.batch_dim
-00017560: 656e 7369 6f6e 203d 2030 0a20 2020 2069  ension = 0.    i
-00017570: 6620 7061 7261 6d73 2e6e 5f64 696d 203d  f params.n_dim =
-00017580: 3d20 3220 616e 6420 6e6f 7420 7061 7261  = 2 and not para
-00017590: 6d73 2e68 6173 5f63 6861 6e6e 656c 3a20  ms.has_channel: 
-000175a0: 7061 7261 6d73 2e63 6861 6e6e 656c 5f64  params.channel_d
-000175b0: 696d 656e 7369 6f6e 203d 2031 0a20 2020  imension = 1.   
-000175c0: 2061 766f 7563 6828 7061 7261 6d73 2e68   avouch(params.h
-000175d0: 6173 5f62 6174 6368 2c20 6622 506c 6561  as_batch, f"Plea
-000175e0: 7365 2075 7365 2062 6174 6f72 6368 2074  se use batorch t
-000175f0: 656e 736f 7220 6f66 2073 697a 6520 285b  ensor of size ([
-00017600: 6e5f 6261 7463 685d 2c20 7b37 206f 7220  n_batch], {7 or 
-00017610: 397d 2920 5c0a 2020 2020 2020 2020 666f  9}) \.        fo
-00017620: 7220 4166 6669 6e65 2070 6172 616d 6574  r Affine paramet
-00017630: 6572 732c 2069 6e73 7465 6164 206f 6620  ers, instead of 
-00017640: 7b70 6172 616d 732e 7368 6170 657d 2e20  {params.shape}. 
-00017650: 2229 0a20 2020 206e 5f62 6174 6368 203d  ").    n_batch =
-00017660: 2070 6172 616d 732e 6e5f 6261 7463 680a   params.n_batch.
-00017670: 2020 2020 6966 2070 6172 616d 732e 7369      if params.si
-00017680: 7a65 2831 2920 3d3d 2037 3a0a 2020 2020  ze(1) == 7:.    
-00017690: 2020 2020 7431 2c20 7432 2c20 ceb8 2c20      t1, t2, .., 
-000176a0: 7331 2c20 7332 2c20 cf81 312c 20cf 8132  s1, s2, ..1, ..2
-000176b0: 203d 2070 6172 616d 732e 7370 6c69 7428   = params.split(
-000176c0: 290a 2020 2020 2020 2020 6331 203d 2062  ).        c1 = b
-000176d0: 742e 7a65 726f 7328 5b6e 5f62 6174 6368  t.zeros([n_batch
-000176e0: 5d2c 2031 293b 2063 3220 3d20 6274 2e7a  ], 1); c2 = bt.z
-000176f0: 6572 6f73 285b 6e5f 6261 7463 685d 2c20  eros([n_batch], 
-00017700: 3129 0a20 2020 2069 6620 7061 7261 6d73  1).    if params
-00017710: 2e73 697a 6528 3129 203d 3d20 393a 0a20  .size(1) == 9:. 
-00017720: 2020 2020 2020 2074 312c 2074 322c 2063         t1, t2, c
-00017730: 312c 2063 322c 20ce b82c 2073 312c 2073  1, c2, .., s1, s
-00017740: 322c 20cf 8131 2c20 cf81 3220 3d20 7061  2, ..1, ..2 = pa
-00017750: 7261 6d73 2e73 706c 6974 2829 0a20 2020  rams.split().   
-00017760: 2061 203d 2028 cf81 3120 2a20 cf81 3220   a = (..1 * ..2 
-00017770: 2b20 3129 202a 2073 3120 2a20 6274 2e63  + 1) * s1 * bt.c
-00017780: 6f73 28ce b829 202b 20cf 8131 202a 2073  os(..) + ..1 * s
-00017790: 3220 2a20 6274 2e73 696e 28ce b829 0a20  2 * bt.sin(..). 
-000177a0: 2020 2062 203d 202d 2028 cf81 3120 2a20     b = - (..1 * 
-000177b0: cf81 3220 2b20 3129 202a 2073 3120 2a20  ..2 + 1) * s1 * 
-000177c0: 6274 2e73 696e 28ce b829 202b 20cf 8131  bt.sin(..) + ..1
-000177d0: 202a 2073 3220 2a20 6274 2e63 6f73 28ce   * s2 * bt.cos(.
-000177e0: b829 0a20 2020 2063 203d 20cf 8132 202a  .).    c = ..2 *
-000177f0: 2073 3120 2a20 6274 2e63 6f73 28ce b829   s1 * bt.cos(..)
-00017800: 202b 2073 3220 2a20 6274 2e73 696e 28ce   + s2 * bt.sin(.
-00017810: b829 0a20 2020 2064 203d 202d 20cf 8132  .).    d = - ..2
-00017820: 202a 2073 3120 2a20 6274 2e73 696e 28ce   * s1 * bt.sin(.
-00017830: b829 202b 2073 3220 2a20 6274 2e63 6f73  .) + s2 * bt.cos
-00017840: 28ce b829 0a20 2020 2072 6574 7572 6e20  (..).    return 
-00017850: 6274 2e63 6174 280a 2020 2020 2020 2020  bt.cat(.        
-00017860: 6274 2e63 6174 2828 612c 2062 2c20 7431  bt.cat((a, b, t1
-00017870: 202d 2061 202a 2063 3120 2d20 6220 2a20   - a * c1 - b * 
-00017880: 6332 202b 2063 312c 2063 2c20 642c 2074  c2 + c1, c, d, t
-00017890: 3220 2d20 6320 2a20 6331 202d 2064 202a  2 - c * c1 - d *
-000178a0: 2063 3220 2b20 6332 292c 207b 7d29 2e76   c2 + c2), {}).v
-000178b0: 6965 7728 5b6e 5f62 6174 6368 5d2c 2032  iew([n_batch], 2
-000178c0: 2c20 3329 2c20 0a20 2020 2020 2020 2062  , 3), .        b
-000178d0: 742e 6f6e 655f 686f 7428 2d31 2c20 3329  t.one_hot(-1, 3)
-000178e0: 2e6d 756c 7469 706c 7928 6e5f 6261 7463  .multiply(n_batc
-000178f0: 682c 205b 5d29 2e76 6965 7728 5b6e 5f62  h, []).view([n_b
-00017900: 6174 6368 5d2c 2031 2c20 3329 2c20 310a  atch], 1, 3), 1.
-00017910: 2020 2020 290a 0a64 6566 2051 7561 7465      )..def Quate
-00017920: 726e 7332 4d61 7472 6978 2870 6172 616d  rns2Matrix(param
-00017930: 7329 3a0a 2020 2020 2222 220a 2020 2020  s):.    """.    
-00017940: 2020 2020 5175 6174 6572 6e3a 2071 622c      Quatern: qb,
-00017950: 2071 632c 2071 642c 2070 782c 2070 792c   qc, qd, px, py,
-00017960: 2070 7a20 696e 2073 697a 653a 2028 5b6e   pz in size: ([n
-00017970: 5f62 6174 6368 5d2c 207b 367d 290a 2020  _batch], {6}).  
-00017980: 2020 2020 2020 4d61 7472 6978 3a20 285b        Matrix: ([
-00017990: 6e5f 6261 7463 685d 2c20 342c 2034 290a  n_batch], 4, 4).
-000179a0: 2020 2020 2222 220a 2020 2020 7061 7261      """.    para
-000179b0: 6d73 203d 2062 6174 6f72 6368 5f74 656e  ms = batorch_ten
-000179c0: 736f 7228 7061 7261 6d73 290a 2020 2020  sor(params).    
-000179d0: 6966 2070 6172 616d 732e 6e5f 6469 6d20  if params.n_dim 
-000179e0: 3c3d 2031 2061 6e64 206e 6f74 2070 6172  <= 1 and not par
-000179f0: 616d 732e 6861 735f 6261 7463 683a 2070  ams.has_batch: p
-00017a00: 6172 616d 7320 3d20 7061 7261 6d73 2e75  arams = params.u
-00017a10: 6e73 7175 6565 7a65 285b 5d29 0a20 2020  nsqueeze([]).   
-00017a20: 2069 6620 7061 7261 6d73 2e6e 5f64 696d   if params.n_dim
-00017a30: 203c 3d20 3120 616e 6420 6e6f 7420 7061   <= 1 and not pa
-00017a40: 7261 6d73 2e68 6173 5f63 6861 6e6e 656c  rams.has_channel
-00017a50: 3a20 7061 7261 6d73 203d 2070 6172 616d  : params = param
-00017a60: 732e 756e 7371 7565 657a 6528 7b31 7d29  s.unsqueeze({1})
-00017a70: 0a20 2020 2069 6620 7061 7261 6d73 2e6e  .    if params.n
-00017a80: 5f64 696d 203d 3d20 3220 616e 6420 6e6f  _dim == 2 and no
-00017a90: 7420 7061 7261 6d73 2e68 6173 5f62 6174  t params.has_bat
-00017aa0: 6368 3a20 7061 7261 6d73 2e62 6174 6368  ch: params.batch
-00017ab0: 5f64 696d 656e 7369 6f6e 203d 2030 0a20  _dimension = 0. 
-00017ac0: 2020 2069 6620 7061 7261 6d73 2e6e 5f64     if params.n_d
-00017ad0: 696d 203d 3d20 3220 616e 6420 6e6f 7420  im == 2 and not 
-00017ae0: 7061 7261 6d73 2e68 6173 5f63 6861 6e6e  params.has_chann
-00017af0: 656c 3a20 7061 7261 6d73 2e63 6861 6e6e  el: params.chann
-00017b00: 656c 5f64 696d 656e 7369 6f6e 203d 2031  el_dimension = 1
-00017b10: 0a20 2020 2061 766f 7563 6828 7061 7261  .    avouch(para
-00017b20: 6d73 2e6e 5f64 696d 203d 3d20 3220 616e  ms.n_dim == 2 an
-00017b30: 6420 7061 7261 6d73 2e68 6173 5f62 6174  d params.has_bat
-00017b40: 6368 2061 6e64 2070 6172 616d 732e 6861  ch and params.ha
-00017b50: 735f 6368 616e 6e65 6c2c 200a 2020 2020  s_channel, .    
-00017b60: 2020 2020 2020 2066 2250 6c65 6173 6520         f"Please 
-00017b70: 7573 6520 6261 746f 7263 6820 7465 6e73  use batorch tens
-00017b80: 6f72 206f 6620 7369 7a65 2028 5b6e 5f62  or of size ([n_b
-00017b90: 6174 6368 5d2c 207b 7b36 7d7d 2920 666f  atch], {{6}}) fo
-00017ba0: 7220 4166 6669 6e65 2070 6172 616d 6574  r Affine paramet
-00017bb0: 6572 732c 2069 6e73 7465 6164 206f 6620  ers, instead of 
-00017bc0: 7b70 6172 616d 732e 7368 6170 657d 2e20  {params.shape}. 
-00017bd0: 2229 0a20 2020 206e 5f62 6174 6368 203d  ").    n_batch =
-00017be0: 2070 6172 616d 732e 6e5f 6261 7463 680a   params.n_batch.
-00017bf0: 2020 2020 622c 2063 2c20 642c 2078 2c20      b, c, d, x, 
-00017c00: 792c 207a 203d 2070 6172 616d 732e 7370  y, z = params.sp
-00017c10: 6c69 7428 290a 2020 2020 6120 3d20 6274  lit().    a = bt
-00017c20: 2e73 7172 7428 2831 2d62 2a62 2d63 2a63  .sqrt((1-b*b-c*c
-00017c30: 2d64 2a64 292e 636c 616d 7028 3029 290a  -d*d).clamp(0)).
-00017c40: 2020 2020 5231 3120 3d20 612a 612b 622a      R11 = a*a+b*
-00017c50: 622d 632a 632d 642a 640a 2020 2020 5231  b-c*c-d*d.    R1
-00017c60: 3220 3d20 322a 622a 632d 322a 612a 640a  2 = 2*b*c-2*a*d.
-00017c70: 2020 2020 5231 3320 3d20 322a 622a 642b      R13 = 2*b*d+
-00017c80: 322a 612a 630a 2020 2020 5232 3120 3d20  2*a*c.    R21 = 
-00017c90: 322a 622a 632b 322a 612a 640a 2020 2020  2*b*c+2*a*d.    
-00017ca0: 5232 3220 3d20 612a 612b 632a 632d 622a  R22 = a*a+c*c-b*
-00017cb0: 622d 642a 640a 2020 2020 5232 3320 3d20  b-d*d.    R23 = 
-00017cc0: 322a 632a 642d 322a 612a 620a 2020 2020  2*c*d-2*a*b.    
-00017cd0: 5233 3120 3d20 322a 622a 642d 322a 612a  R31 = 2*b*d-2*a*
-00017ce0: 630a 2020 2020 5233 3220 3d20 322a 632a  c.    R32 = 2*c*
-00017cf0: 642b 322a 612a 620a 2020 2020 5233 3320  d+2*a*b.    R33 
-00017d00: 3d20 612a 612b 642a 642d 632a 632d 622a  = a*a+d*d-c*c-b*
-00017d10: 620a 2020 2020 7265 7475 726e 2062 742e  b.    return bt.
-00017d20: 6361 7428 0a20 2020 2020 2020 2062 742e  cat(.        bt.
-00017d30: 6361 7428 2852 3131 2c20 5231 322c 2052  cat((R11, R12, R
-00017d40: 3133 2c20 782c 2052 3231 2c20 5232 322c  13, x, R21, R22,
-00017d50: 2052 3233 2c20 792c 2052 3331 2c20 5233   R23, y, R31, R3
-00017d60: 322c 2052 3333 2c20 7a29 2c20 3129 2e76  2, R33, z), 1).v
-00017d70: 6965 7728 5b6e 5f62 6174 6368 5d2c 2033  iew([n_batch], 3
-00017d80: 2c20 3429 2c0a 2020 2020 2020 2020 6274  , 4),.        bt
-00017d90: 2e6f 6e65 5f68 6f74 282d 312c 2034 292e  .one_hot(-1, 4).
-00017da0: 6d75 6c74 6970 6c79 286e 5f62 6174 6368  multiply(n_batch
-00017db0: 2c20 5b5d 292e 7669 6577 285b 6e5f 6261  , []).view([n_ba
-00017dc0: 7463 685d 2c20 312c 2034 292c 2031 0a20  tch], 1, 4), 1. 
-00017dd0: 2020 2029 0a0a 6465 6620 4d61 7472 6978     )..def Matrix
-00017de0: 3251 7561 7465 726e 7328 7061 7261 6d73  2Quaterns(params
-00017df0: 293a 0a20 2020 2022 2222 0a20 2020 2020  ):.    """.     
-00017e00: 2020 204d 6174 7269 783a 2028 5b6e 5f62     Matrix: ([n_b
-00017e10: 6174 6368 5d2c 2034 2c20 3429 0a20 2020  atch], 4, 4).   
-00017e20: 2020 2020 2051 7561 7465 726e 3a20 7162       Quatern: qb
-00017e30: 2c20 7163 2c20 7164 2c20 7078 2c20 7079  , qc, qd, px, py
-00017e40: 2c20 707a 2069 6e20 7369 7a65 3a20 285b  , pz in size: ([
-00017e50: 6e5f 6261 7463 685d 2c20 7b36 7d29 0a20  n_batch], {6}). 
-00017e60: 2020 2022 2222 0a20 2020 2070 6172 616d     """.    param
-00017e70: 7320 3d20 6261 746f 7263 685f 7465 6e73  s = batorch_tens
-00017e80: 6f72 2870 6172 616d 7329 0a20 2020 2069  or(params).    i
-00017e90: 6620 7061 7261 6d73 2e6e 5f64 696d 203c  f params.n_dim <
-00017ea0: 3d20 3220 616e 6420 6e6f 7420 7061 7261  = 2 and not para
-00017eb0: 6d73 2e68 6173 5f62 6174 6368 3a20 7061  ms.has_batch: pa
-00017ec0: 7261 6d73 203d 2070 6172 616d 732e 756e  rams = params.un
-00017ed0: 7371 7565 657a 6528 5b5d 290a 2020 2020  squeeze([]).    
-00017ee0: 6966 2070 6172 616d 732e 6e5f 6469 6d20  if params.n_dim 
-00017ef0: 3d3d 2033 2061 6e64 206e 6f74 2070 6172  == 3 and not par
-00017f00: 616d 732e 6861 735f 6261 7463 683a 2070  ams.has_batch: p
-00017f10: 6172 616d 732e 6261 7463 685f 6469 6d65  arams.batch_dime
-00017f20: 6e73 696f 6e20 3d20 300a 2020 2020 6966  nsion = 0.    if
-00017f30: 2070 6172 616d 732e 6e5f 6469 6d20 3d3d   params.n_dim ==
-00017f40: 2033 2061 6e64 2070 6172 616d 732e 6861   3 and params.ha
-00017f50: 735f 6368 616e 6e65 6c3a 2070 6172 616d  s_channel: param
-00017f60: 732e 6368 616e 6e65 6c5f 6469 6d65 6e73  s.channel_dimens
-00017f70: 696f 6e20 3d20 4e6f 6e65 0a20 2020 2061  ion = None.    a
-00017f80: 766f 7563 6828 7061 7261 6d73 2e6e 5f64  vouch(params.n_d
-00017f90: 696d 203d 3d20 3320 616e 6420 7061 7261  im == 3 and para
-00017fa0: 6d73 2e68 6173 5f62 6174 6368 2061 6e64  ms.has_batch and
-00017fb0: 206e 6f74 2070 6172 616d 732e 6861 735f   not params.has_
-00017fc0: 6368 616e 6e65 6c2c 200a 2020 2020 2020  channel, .      
-00017fd0: 2020 2020 2066 2250 6c65 6173 6520 7573       f"Please us
-00017fe0: 6520 6261 746f 7263 6820 7465 6e73 6f72  e batorch tensor
-00017ff0: 206f 6620 7369 7a65 2028 5b6e 5f62 6174   of size ([n_bat
-00018000: 6368 5d2c 2034 2c20 3429 2066 6f72 2041  ch], 4, 4) for A
-00018010: 6666 696e 6520 6d61 7472 6978 2c20 696e  ffine matrix, in
-00018020: 7374 6561 6420 6f66 207b 7061 7261 6d73  stead of {params
-00018030: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
-00018040: 6e5f 6261 7463 6820 3d20 7061 7261 6d73  n_batch = params
-00018050: 2e6e 5f62 6174 6368 0a20 2020 2078 2c20  .n_batch.    x, 
-00018060: 792c 207a 203d 2070 6172 616d 735b 2e2e  y, z = params[..
-00018070: 2e2c 203a 332c 202d 315d 2e63 6861 6e6e  ., :3, -1].chann
-00018080: 656c 5f64 696d 5f28 3129 2e73 706c 6974  el_dim_(1).split
-00018090: 2831 2c20 3129 0a20 2020 2061 3220 3d20  (1, 1).    a2 = 
-000180a0: 2862 742e 6469 6167 2870 6172 616d 7329  (bt.diag(params)
-000180b0: 2e73 756d 2829 2e75 6e73 7175 6565 7a65  .sum().unsqueeze
-000180c0: 287b 7d29 202b 2031 2920 2f20 340a 2020  ({}) + 1) / 4.  
-000180d0: 2020 6120 3d20 6274 2e73 7172 7428 6132    a = bt.sqrt(a2
-000180e0: 290a 2020 2020 6232 203d 2061 3220 2d20  ).    b2 = a2 - 
-000180f0: 2870 6172 616d 735b 2e2e 2e2c 2031 2c20  (params[..., 1, 
-00018100: 315d 202b 2070 6172 616d 735b 2e2e 2e2c  1] + params[...,
-00018110: 2032 2c20 325d 2920 2f20 320a 2020 2020   2, 2]) / 2.    
-00018120: 6332 203d 2061 3220 2d20 2870 6172 616d  c2 = a2 - (param
-00018130: 735b 2e2e 2e2c 2032 2c20 325d 202b 2070  s[..., 2, 2] + p
-00018140: 6172 616d 735b 2e2e 2e2c 2030 2c20 305d  arams[..., 0, 0]
-00018150: 2920 2f20 320a 2020 2020 6432 203d 2061  ) / 2.    d2 = a
-00018160: 3220 2d20 2870 6172 616d 735b 2e2e 2e2c  2 - (params[...,
-00018170: 2030 2c20 305d 202b 2070 6172 616d 735b   0, 0] + params[
-00018180: 2e2e 2e2c 2031 2c20 315d 2920 2f20 320a  ..., 1, 1]) / 2.
-00018190: 2020 2020 4420 3d20 7061 7261 6d73 202d      D = params -
-000181a0: 2070 6172 616d 732e 540a 2020 2020 6220   params.T.    b 
-000181b0: 3d20 6274 2e73 6967 6e28 445b 2e2e 2e2c  = bt.sign(D[...,
-000181c0: 2032 2c20 315d 2920 2a20 6274 2e73 7172   2, 1]) * bt.sqr
-000181d0: 7428 6232 290a 2020 2020 6320 3d20 2d20  t(b2).    c = - 
-000181e0: 6274 2e73 6967 6e28 445b 2e2e 2e2c 2032  bt.sign(D[..., 2
-000181f0: 2c20 305d 2920 2a20 6274 2e73 7172 7428  , 0]) * bt.sqrt(
-00018200: 6332 290a 2020 2020 6420 3d20 6274 2e73  c2).    d = bt.s
-00018210: 6967 6e28 445b 2e2e 2e2c 2031 2c20 305d  ign(D[..., 1, 0]
-00018220: 2920 2a20 6274 2e73 7172 7428 6432 290a  ) * bt.sqrt(d2).
-00018230: 2020 2020 7265 7475 726e 2062 742e 6361      return bt.ca
-00018240: 7428 622c 2063 2c20 642c 2078 2c20 792c  t(b, c, d, x, y,
-00018250: 207a 2c20 7b7d 290a                       z, {}).
+000132b0: 6765 203d 2074 6f5f 6465 7669 6365 2862  ge = to_device(b
+000132c0: 6174 6f72 6368 5f74 656e 736f 7228 696d  atorch_tensor(im
+000132d0: 6167 6529 290a 2020 2020 7368 6170 655f  age)).    shape_
+000132e0: 6f75 7420 3d20 696d 6167 652e 7368 6170  out = image.shap
+000132f0: 650a 2020 2020 6966 2074 7261 6e73 2069  e.    if trans i
+00013300: 7320 4e6f 6e65 206f 7220 7472 616e 732e  s None or trans.
+00013310: 6e5f 6469 6d20 6973 204e 6f6e 653a 0a20  n_dim is None:. 
+00013320: 2020 2020 2020 2069 6620 6e6f 7420 696d         if not im
+00013330: 6167 652e 6861 735f 6261 7463 683a 2069  age.has_batch: i
+00013340: 6d61 6765 2e75 6e73 7175 6565 7a65 5f28  mage.unsqueeze_(
+00013350: 5b5d 290a 2020 2020 2020 2020 6966 206e  []).        if n
+00013360: 6f74 2069 6d61 6765 2e68 6173 5f63 6861  ot image.has_cha
+00013370: 6e6e 656c 3a20 696d 6167 652e 7374 616e  nnel: image.stan
+00013380: 6461 7264 5f28 292e 756e 7371 7565 657a  dard_().unsqueez
+00013390: 655f 287b 317d 290a 2020 2020 2020 2020  e_({1}).        
+000133a0: 6e5f 6469 6d20 3d20 696d 6167 652e 6e5f  n_dim = image.n_
+000133b0: 7370 6163 6520 2320 4765 7420 7468 6520  space # Get the 
+000133c0: 7370 6174 6961 6c20 7261 6e6b 2e0a 2020  spatial rank..  
+000133d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000133e0: 6e5f 6469 6d20 3d20 7472 616e 732e 6e5f  n_dim = trans.n_
+000133f0: 6469 6d0a 2020 2020 2020 2020 6966 2069  dim.        if i
+00013400: 6d61 6765 2e6e 5f64 696d 203d 3d20 6e5f  mage.n_dim == n_
+00013410: 6469 6d3a 0a20 2020 2020 2020 2020 2020  dim:.           
+00013420: 2069 6620 696d 6167 652e 6861 735f 7370   if image.has_sp
+00013430: 6563 6961 6c3a 0a20 2020 2020 2020 2020  ecial:.         
+00013440: 2020 2020 2020 2070 7269 6e74 2866 2257         print(f"W
+00013450: 6172 6e69 6e67 3a20 2769 6e74 6572 706f  arning: 'interpo
+00013460: 6c61 7469 6f6e 2720 7472 7969 6e67 2074  lation' trying t
+00013470: 6f20 7472 616e 7366 6f72 6d20 7b69 6d61  o transform {ima
+00013480: 6765 2e6e 5f73 7061 6365 7d2b 7b69 6d61  ge.n_space}+{ima
+00013490: 6765 2e6e 5f73 7065 6369 616c 7d44 2069  ge.n_special}D i
+000134a0: 6d61 6765 2028 7769 7468 2062 6174 6368  mage (with batch
+000134b0: 206f 7220 6368 616e 6e65 6c29 2062 7920   or channel) by 
+000134c0: 7b6e 5f64 696d 7d44 2074 7261 6e73 666f  {n_dim}D transfo
+000134d0: 726d 6174 696f 6e2c 2061 7574 6f2d 7265  rmation, auto-re
+000134e0: 6d6f 7669 6e67 2073 7065 6369 616c 2064  moving special d
+000134f0: 696d 656e 7369 6f6e 732e 2229 0a20 2020  imensions.").   
+00013500: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
+00013510: 6765 2e72 656d 6f76 655f 7370 6563 6961  ge.remove_specia
+00013520: 6c5f 2829 0a20 2020 2020 2020 2020 2020  l_().           
+00013530: 2069 6d61 6765 2e75 6e73 7175 6565 7a65   image.unsqueeze
+00013540: 5f28 5b5d 292e 756e 7371 7565 657a 655f  _([]).unsqueeze_
+00013550: 287b 7d29 0a20 2020 2020 2020 2065 6c69  ({}).        eli
+00013560: 6620 696d 6167 652e 6e5f 6469 6d20 3d3d  f image.n_dim ==
+00013570: 206e 5f64 696d 202b 2031 3a0a 2020 2020   n_dim + 1:.    
+00013580: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+00013590: 6d61 6765 2e68 6173 5f62 6174 6368 3a0a  mage.has_batch:.
+000135a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000135b0: 6966 2069 6d61 6765 2e68 6173 5f63 6861  if image.has_cha
+000135c0: 6e6e 656c 3a20 696d 6167 652e 756e 7371  nnel: image.unsq
+000135d0: 7565 657a 655f 285b 5d29 0a20 2020 2020  ueeze_([]).     
+000135e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000135f0: 2069 6d61 6765 2e77 6974 685f 6261 7463   image.with_batc
+00013600: 6864 696d 2830 292e 756e 7371 7565 657a  hdim(0).unsqueez
+00013610: 655f 287b 317d 290a 2020 2020 2020 2020  e_({1}).        
+00013620: 2020 2020 656c 6966 206e 6f74 2069 6d61      elif not ima
+00013630: 6765 2e68 6173 5f63 6861 6e6e 656c 3a20  ge.has_channel: 
+00013640: 696d 6167 652e 756e 7371 7565 657a 655f  image.unsqueeze_
+00013650: 287b 7d29 0a20 2020 2020 2020 2020 2020  ({}).           
+00013660: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00013670: 2020 2020 2020 2070 7269 6e74 2866 2257         print(f"W
+00013680: 6172 6e69 6e67 3a20 2769 6e74 6572 706f  arning: 'interpo
+00013690: 6c61 7469 6f6e 2720 7472 7969 6e67 2074  lation' trying t
+000136a0: 6f20 7472 616e 7366 6f72 6d20 7b69 6d61  o transform {ima
+000136b0: 6765 2e6e 5f73 7061 6365 7d2b 7b69 6d61  ge.n_space}+{ima
+000136c0: 6765 2e6e 5f73 7065 6369 616c 7d44 2069  ge.n_special}D i
+000136d0: 6d61 6765 2028 7769 7468 2062 6174 6368  mage (with batch
+000136e0: 206f 7220 6368 616e 6e65 6c29 2062 7920   or channel) by 
+000136f0: 7b6e 5f64 696d 7d44 2074 7261 6e73 666f  {n_dim}D transfo
+00013700: 726d 6174 696f 6e2c 2061 7574 6f2d 7265  rmation, auto-re
+00013710: 6d6f 7669 6e67 2074 6865 2063 6861 6e6e  moving the chann
+00013720: 656c 2064 696d 656e 7369 6f6e 732e 2229  el dimensions.")
+00013730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013740: 2069 6d61 6765 2e77 6974 685f 6368 616e   image.with_chan
+00013750: 6e65 6c64 696d 284e 6f6e 6529 2e75 6e73  neldim(None).uns
+00013760: 7175 6565 7a65 5f28 7b7d 290a 2020 2020  queeze_({}).    
+00013770: 2020 2020 656c 6966 2069 6d61 6765 2e6e      elif image.n
+00013780: 5f64 696d 203d 3d20 6e5f 6469 6d20 2b20  _dim == n_dim + 
+00013790: 323a 0a20 2020 2020 2020 2020 2020 2023  2:.            #
+000137a0: 205f 6368 616e 6e61 6c2f 6261 7463 6820   _channal/batch 
+000137b0: 6469 6d65 6e73 696f 6e73 2075 7365 6420  dimensions used 
+000137c0: 6865 7265 2061 7320 7468 6579 2061 7265  here as they are
+000137d0: 206e 5f64 696d 2077 6865 6e20 6e6f 7420   n_dim when not 
+000137e0: 6578 6973 7465 642e 200a 2020 2020 2020  existed. .      
+000137f0: 2020 2020 2020 6966 2069 6d61 6765 2e6e        if image.n
+00013800: 5f73 7065 6369 616c 203d 3d20 313a 0a20  _special == 1:. 
+00013810: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00013820: 7269 6e74 2866 2257 6172 6e69 6e67 3a20  rint(f"Warning: 
+00013830: 2769 6e74 6572 706f 6c61 7469 6f6e 2720  'interpolation' 
+00013840: 7472 7969 6e67 2074 6f20 7472 616e 7366  trying to transf
+00013850: 6f72 6d20 7b69 6d61 6765 2e6e 5f73 7061  orm {image.n_spa
+00013860: 6365 7d2b 3144 2069 6d61 6765 2028 7769  ce}+1D image (wi
+00013870: 7468 2062 6174 6368 206f 7220 6368 616e  th batch or chan
+00013880: 6e65 6c29 2062 7920 7b6e 5f64 696d 7d44  nel) by {n_dim}D
+00013890: 2074 7261 6e73 666f 726d 6174 696f 6e2c   transformation,
+000138a0: 2061 7574 6f2d 696e 7365 7274 696e 6720   auto-inserting 
+000138b0: 6e65 7720 7370 6563 6961 6c20 6469 6d65  new special dime
+000138c0: 6e73 696f 6e2e 2229 0a20 2020 2020 2020  nsion.").       
+000138d0: 2020 2020 2069 6620 6e6f 7420 696d 6167       if not imag
+000138e0: 652e 6861 735f 6261 7463 683a 2069 6d61  e.has_batch: ima
+000138f0: 6765 2e62 6174 6368 5f64 696d 656e 7369  ge.batch_dimensi
+00013900: 6f6e 203d 2030 2069 6620 696d 6167 652e  on = 0 if image.
+00013910: 5f63 6861 6e6e 656c 5f64 696d 656e 7369  _channel_dimensi
+00013920: 6f6e 203e 2030 2065 6c73 6520 310a 2020  on > 0 else 1.  
+00013930: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00013940: 2069 6d61 6765 2e68 6173 5f63 6861 6e6e   image.has_chann
+00013950: 656c 3a20 696d 6167 652e 6368 616e 6e65  el: image.channe
+00013960: 6c5f 6469 6d65 6e73 696f 6e20 3d20 3020  l_dimension = 0 
+00013970: 6966 2069 6d61 6765 2e5f 6261 7463 685f  if image._batch_
+00013980: 6469 6d65 6e73 696f 6e20 3e20 3020 656c  dimension > 0 el
+00013990: 7365 2031 0a20 2020 2061 766f 7563 6828  se 1.    avouch(
+000139a0: 696d 6167 652e 6861 735f 6261 7463 6820  image.has_batch 
+000139b0: 616e 6420 696d 6167 652e 6861 735f 6368  and image.has_ch
+000139c0: 616e 6e65 6c2c 2022 506c 6561 7365 2075  annel, "Please u
+000139d0: 7365 2062 6174 6f72 6368 2074 656e 736f  se batorch tenso
+000139e0: 7220 6f66 2073 697a 6520 2220 2b0a 2020  r of size " +.  
+000139f0: 2020 2020 2020 2020 2020 2228 5b6e 5f62            "([n_b
+00013a00: 6174 6368 5d2c 207b 6e5f 6368 616e 6e65  atch], {n_channe
+00013a10: 6c2f 6e5f 6665 6174 7572 653a 6f70 7469  l/n_feature:opti
+00013a20: 6f6e 616c 7d2c 206d 5f31 2c20 6d5f 322c  onal}, m_1, m_2,
+00013a30: 202e 2e2e 2c20 6d5f 7229 205b 723d 6e5f   ..., m_r) [r=n_
+00013a40: 6469 6d5d 2066 6f72 2022 202b 200a 2020  dim] for " + .  
+00013a50: 2020 2020 2020 2020 2020 6622 6461 7461            f"data
+00013a60: 2074 6f20 6265 2073 7061 7469 616c 6c79   to be spatially
+00013a70: 2069 6e74 6572 706f 6c61 7465 642c 2069   interpolated, i
+00013a80: 6e73 7465 6164 206f 6620 7b69 6d61 6765  nstead of {image
+00013a90: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
+00013aa0: 6966 2074 7261 6e73 2069 7320 6e6f 7420  if trans is not 
+00013ab0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6176  None:.        av
+00013ac0: 6f75 6368 2869 6d61 6765 2e6e 5f62 6174  ouch(image.n_bat
+00013ad0: 6368 203d 3d20 3120 6f72 2074 7261 6e73  ch == 1 or trans
+00013ae0: 2e6e 5f62 6174 6368 2069 6e20 284e 6f6e  .n_batch in (Non
+00013af0: 652c 2069 6d61 6765 2e6e 5f62 6174 6368  e, image.n_batch
+00013b00: 2c20 3129 2c20 2250 6c65 6173 6520 7573  , 1), "Please us
+00013b10: 6520 7472 616e 7366 6f72 6d61 7469 6f6e  e transformation
+00013b20: 206f 6620 6120 2220 2b0a 2020 2020 2020   of a " +.      
+00013b30: 2020 2020 2020 6622 7375 6974 6162 6c65        f"suitable
+00013b40: 206e 5f62 6174 6368 2074 6f20 7472 616e   n_batch to tran
+00013b50: 7366 6f72 6d20 696d 6167 6520 7769 7468  sform image with
+00013b60: 2062 6174 6368 7369 7a65 207b 696d 6167   batchsize {imag
+00013b70: 652e 6e5f 6261 7463 687d 2c20 6375 7272  e.n_batch}, curr
+00013b80: 656e 746c 7920 7b74 7261 6e73 2e6e 5f62  ently {trans.n_b
+00013b90: 6174 6368 7d2e 2229 0a0a 2020 2020 6e5f  atch}.")..    n_
+00013ba0: 6261 7463 6820 3d20 696d 6167 652e 6e5f  batch = image.n_
+00013bb0: 6261 7463 680a 2020 2020 6966 206e 5f62  batch.    if n_b
+00013bc0: 6174 6368 203d 3d20 3120 616e 6420 7472  atch == 1 and tr
+00013bd0: 616e 7320 6973 206e 6f74 204e 6f6e 6520  ans is not None 
+00013be0: 616e 6420 7472 616e 732e 6e5f 6261 7463  and trans.n_batc
+00013bf0: 6820 6973 206e 6f74 204e 6f6e 6520 616e  h is not None an
+00013c00: 6420 7472 616e 732e 6e5f 6261 7463 6820  d trans.n_batch 
+00013c10: 3e20 313a 206e 5f62 6174 6368 203d 2074  > 1: n_batch = t
+00013c20: 7261 6e73 2e6e 5f62 6174 6368 0a20 2020  rans.n_batch.   
+00013c30: 2069 6620 6e5f 6261 7463 6820 3d3d 2031   if n_batch == 1
+00013c40: 2061 6e64 2069 7369 6e73 7461 6e63 6528   and isinstance(
+00013c50: 7461 7267 6574 5f73 7061 6365 2c20 6274  target_space, bt
+00013c60: 2e54 656e 736f 7229 2061 6e64 2074 6172  .Tensor) and tar
+00013c70: 6765 745f 7370 6163 652e 6861 735f 6261  get_space.has_ba
+00013c80: 7463 6820 616e 6420 7461 7267 6574 5f73  tch and target_s
+00013c90: 7061 6365 2e6e 5f62 6174 6368 203e 2031  pace.n_batch > 1
+00013ca0: 3a20 6e5f 6261 7463 6820 3d20 7461 7267  : n_batch = targ
+00013cb0: 6574 5f73 7061 6365 2e6e 5f62 6174 6368  et_space.n_batch
+00013cc0: 0a20 2020 2069 6620 696d 6167 652e 6e5f  .    if image.n_
+00013cd0: 6261 7463 6820 3d3d 2031 3a20 696d 6167  batch == 1: imag
+00013ce0: 6520 3d20 696d 6167 652e 7265 7065 6174  e = image.repeat
+00013cf0: 6564 286e 5f62 6174 6368 2c20 5b5d 290a  ed(n_batch, []).
+00013d00: 2020 2020 6e5f 6665 6174 7572 6520 3d20      n_feature = 
+00013d10: 696d 6167 652e 6e5f 6368 616e 6e65 6c0a  image.n_channel.
+00013d20: 2020 2020 7369 7a65 203d 2062 742e 6368      size = bt.ch
+00013d30: 616e 6e65 6c5f 7465 6e73 6f72 2869 6d61  annel_tensor(ima
+00013d40: 6765 2e73 7061 6365 292e 696e 7428 290a  ge.space).int().
+00013d50: 2020 2020 6966 206e 5f62 6174 6368 203e      if n_batch >
+00013d60: 2031 2061 6e64 206e 6f74 2073 6861 7065   1 and not shape
+00013d70: 5f6f 7574 2e68 6173 5f62 6174 6368 3a20  _out.has_batch: 
+00013d80: 7368 6170 655f 6f75 7420 3d20 6274 2e53  shape_out = bt.S
+00013d90: 697a 6528 5b6e 5f62 6174 6368 5d29 202b  ize([n_batch]) +
+00013da0: 2073 6861 7065 5f6f 7574 0a20 2020 2069   shape_out.    i
+00013db0: 6620 7461 7267 6574 5f73 7061 6365 2069  f target_space i
+00013dc0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00013dd0: 7363 616c 652c 202a 7061 6972 7320 3d20  scale, *pairs = 
+00013de0: 7472 616e 732e 7265 7368 6170 650a 2020  trans.reshape.  
+00013df0: 2020 2020 2020 6966 206c 656e 2873 6361        if len(sca
+00013e00: 6c65 2920 3d3d 2031 3a20 7363 616c 6520  le) == 1: scale 
+00013e10: 2a3d 206e 5f64 696d 0a20 2020 2020 2020  *= n_dim.       
+00013e20: 2074 6172 6765 745f 7370 6163 6520 3d20   target_space = 
+00013e30: 5b69 6e74 2878 202a 2079 2920 666f 7220  [int(x * y) for 
+00013e40: 782c 2079 2069 6e20 7a69 7028 696d 6167  x, y in zip(imag
+00013e50: 652e 7370 6163 652c 2073 6361 6c65 295d  e.space, scale)]
+00013e60: 0a20 2020 2020 2020 2066 6f72 2070 2c20  .        for p, 
+00013e70: 7120 696e 2070 6169 7273 3a20 7461 7267  q in pairs: targ
+00013e80: 6574 5f73 7061 6365 5b70 5d2c 2074 6172  et_space[p], tar
+00013e90: 6765 745f 7370 6163 655b 715d 203d 2074  get_space[q] = t
+00013ea0: 6172 6765 745f 7370 6163 655b 715d 2c20  arget_space[q], 
+00013eb0: 7461 7267 6574 5f73 7061 6365 5b70 5d0a  target_space[p].
+00013ec0: 2020 2020 2020 2020 7461 7267 6574 5f73          target_s
+00013ed0: 7061 6365 203d 2074 7570 6c65 2874 6172  pace = tuple(tar
+00013ee0: 6765 745f 7370 6163 6529 0a20 2020 2020  get_space).     
+00013ef0: 2020 2073 6861 7065 5f6f 7574 203d 2073     shape_out = s
+00013f00: 6861 7065 5f6f 7574 2e72 6573 6574 5f73  hape_out.reset_s
+00013f10: 7061 6365 2874 6172 6765 745f 7370 6163  pace(target_spac
+00013f20: 6529 0a20 2020 2069 6620 6973 696e 7374  e).    if isinst
+00013f30: 616e 6365 2874 6172 6765 745f 7370 6163  ance(target_spac
+00013f40: 652c 2074 7570 6c65 2920 616e 6420 6c65  e, tuple) and le
+00013f50: 6e28 7461 7267 6574 5f73 7061 6365 2920  n(target_space) 
+00013f60: 3d3d 206e 5f64 696d 3a20 7061 7373 0a20  == n_dim: pass. 
+00013f70: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+00013f80: 6365 2874 6172 6765 745f 7370 6163 652c  ce(target_space,
+00013f90: 2062 742e 746f 7263 682e 5465 6e73 6f72   bt.torch.Tensor
+00013fa0: 293a 2070 6173 730a 2020 2020 656c 7365  ): pass.    else
+00013fb0: 3a20 7261 6973 6520 5479 7065 4572 726f  : raise TypeErro
+00013fc0: 7228 6622 5772 6f6e 6720 7461 7267 6574  r(f"Wrong target
+00013fd0: 2073 7061 6365 2066 6f72 2069 6e74 6572   space for inter
+00013fe0: 706f 6c61 7469 6f6e 3a20 7b74 6172 6765  polation: {targe
+00013ff0: 745f 7370 6163 657d 2e20 2229 0a20 2020  t_space}. ").   
+00014000: 2069 6620 6973 696e 7374 616e 6365 2874   if isinstance(t
+00014010: 6172 6765 745f 7370 6163 652c 2074 7570  arget_space, tup
+00014020: 6c65 293a 200a 2020 2020 2020 2020 2320  le): .        # 
+00014030: 4372 6561 7465 2061 2067 7269 6420 5820  Create a grid X 
+00014040: 7769 7468 2073 697a 6520 287b 6e5f 6469  with size ({n_di
+00014050: 6d7d 2c20 7369 7a65 5f31 2c20 7369 7a65  m}, size_1, size
+00014060: 5f32 2c20 2e2e 2e2c 2073 697a 655f 7229  _2, ..., size_r)
+00014070: 205b 723d 6e5f 6469 6d5d 2e0a 2020 2020   [r=n_dim]..    
+00014080: 2020 2020 5820 3d20 6274 2e69 6d61 6765      X = bt.image
+00014090: 5f67 7269 6428 7461 7267 6574 5f73 7061  _grid(target_spa
+000140a0: 6365 292e 666c 6f61 7428 2920 2320 2b20  ce).float() # + 
+000140b0: 6274 2e63 6861 6e6e 656c 5f74 656e 736f  bt.channel_tenso
+000140c0: 7228 5b66 6c6f 6174 2861 2d62 292f 3220  r([float(a-b)/2 
+000140d0: 666f 7220 612c 2062 2069 6e20 7a69 7028  for a, b in zip(
+000140e0: 696d 6167 652e 7370 6163 652c 2074 6172  image.space, tar
+000140f0: 6765 745f 7370 6163 6529 5d29 0a20 2020  get_space)]).   
+00014100: 2020 2020 2023 2043 6f6d 7075 7465 2074       # Compute t
+00014110: 6865 2074 7261 6e73 666f 726d 6564 2063  he transformed c
+00014120: 6f6f 7264 696e 6174 6573 2e20 593a 2028  oordinates. Y: (
+00014130: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 6469  [n_batch], {n_di
+00014140: 6d7d 2c20 7369 7a65 5f31 2c20 7369 7a65  m}, size_1, size
+00014150: 5f32 2c20 2e2e 2e2c 2073 697a 655f 7229  _2, ..., size_r)
+00014160: 205b 723d 6e5f 6469 6d5d 2e0a 2020 2020   [r=n_dim]..    
+00014170: 2020 2020 6966 2074 7261 6e73 2069 7320      if trans is 
+00014180: 4e6f 6e65 3a20 7472 616e 7320 3d20 4964  None: trans = Id
+00014190: 656e 7469 7479 2829 0a20 2020 2020 2020  entity().       
+000141a0: 2059 203d 2074 7261 6e73 2858 290a 2020   Y = trans(X).  
+000141b0: 2020 2020 2020 6966 206e 6f74 2059 2e68        if not Y.h
+000141c0: 6173 5f62 6174 6368 3a20 5920 3d20 592e  as_batch: Y = Y.
+000141d0: 6d75 6c74 6970 6c79 286e 5f62 6174 6368  multiply(n_batch
+000141e0: 2c20 5b5d 290a 2020 2020 2020 2020 6966  , []).        if
+000141f0: 2059 2e6e 5f62 6174 6368 203d 3d20 313a   Y.n_batch == 1:
+00014200: 2059 203d 2059 2e72 6570 6561 7465 6428   Y = Y.repeated(
+00014210: 6e5f 6261 7463 682c 205b 5d29 0a20 2020  n_batch, []).   
+00014220: 2020 2020 2059 203d 2059 2e61 6d70 6c69       Y = Y.ampli
+00014230: 6679 286e 5f66 6561 7475 7265 2c20 5b5d  fy(n_feature, []
+00014240: 290a 2020 2020 2020 2020 7368 6170 655f  ).        shape_
+00014250: 6f75 7420 3d20 7368 6170 655f 6f75 742e  out = shape_out.
+00014260: 7265 7365 745f 7370 6163 6528 7461 7267  reset_space(targ
+00014270: 6574 5f73 7061 6365 290a 2020 2020 656c  et_space).    el
+00014280: 7365 3a0a 2020 2020 2020 2020 7461 7267  se:.        targ
+00014290: 6574 5f73 7061 6365 203d 2062 6174 6f72  et_space = bator
+000142a0: 6368 5f74 656e 736f 7228 7461 7267 6574  ch_tensor(target
+000142b0: 5f73 7061 6365 290a 2020 2020 2020 2020  _space).        
+000142c0: 6966 206e 6f74 2074 6172 6765 745f 7370  if not target_sp
+000142d0: 6163 652e 6861 735f 6261 7463 683a 0a20  ace.has_batch:. 
+000142e0: 2020 2020 2020 2020 2020 2069 6620 7461             if ta
+000142f0: 7267 6574 5f73 7061 6365 2e73 697a 6528  rget_space.size(
+00014300: 3029 203d 3d20 6e5f 6261 7463 6820 616e  0) == n_batch an
+00014310: 6420 6e5f 6261 7463 6820 213d 206e 5f64  d n_batch != n_d
+00014320: 696d 206f 7220 6c65 6e28 5b78 2066 6f72  im or len([x for
+00014330: 2078 2069 6e20 7461 7267 6574 5f73 7061   x in target_spa
+00014340: 6365 2e73 6861 7065 2069 6620 7820 3d3d  ce.shape if x ==
+00014350: 206e 5f64 696d 5d29 203e 3d20 323a 0a20   n_dim]) >= 2:. 
+00014360: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00014370: 6172 6765 745f 7370 6163 652e 7769 7468  arget_space.with
+00014380: 5f62 6174 6368 6469 6d28 3029 0a20 2020  _batchdim(0).   
+00014390: 2020 2020 2020 2020 2065 6c73 653a 2074           else: t
+000143a0: 6172 6765 745f 7370 6163 652e 756e 7371  arget_space.unsq
+000143b0: 7565 657a 655f 285b 5d29 0a20 2020 2020  ueeze_([]).     
+000143c0: 2020 2069 6620 6e6f 7420 7461 7267 6574     if not target
+000143d0: 5f73 7061 6365 2e68 6173 5f63 6861 6e6e  _space.has_chann
+000143e0: 656c 3a0a 2020 2020 2020 2020 2020 2020  el:.            
+000143f0: 6966 2074 6172 6765 745f 7370 6163 652e  if target_space.
+00014400: 6261 7463 685f 6469 6d65 6e73 696f 6e20  batch_dimension 
+00014410: 213d 2030 2061 6e64 2074 6172 6765 745f  != 0 and target_
+00014420: 7370 6163 652e 7369 7a65 2830 2920 3d3d  space.size(0) ==
+00014430: 206e 5f64 696d 3a20 7461 7267 6574 5f73   n_dim: target_s
+00014440: 7061 6365 2e77 6974 685f 6368 616e 6e65  pace.with_channe
+00014450: 6c64 696d 2830 290a 2020 2020 2020 2020  ldim(0).        
+00014460: 2020 2020 656c 6966 2074 6172 6765 745f      elif target_
+00014470: 7370 6163 652e 6261 7463 685f 6469 6d65  space.batch_dime
+00014480: 6e73 696f 6e20 213d 2031 2061 6e64 2074  nsion != 1 and t
+00014490: 6172 6765 745f 7370 6163 652e 7369 7a65  arget_space.size
+000144a0: 2831 2920 3d3d 206e 5f64 696d 3a20 7461  (1) == n_dim: ta
+000144b0: 7267 6574 5f73 7061 6365 2e77 6974 685f  rget_space.with_
+000144c0: 6368 616e 6e65 6c64 696d 2831 290a 2020  channeldim(1).  
+000144d0: 2020 2020 2020 2020 2020 656c 6966 2074            elif t
+000144e0: 6172 6765 745f 7370 6163 652e 6261 7463  arget_space.batc
+000144f0: 685f 6469 6d65 6e73 696f 6e20 213d 2074  h_dimension != t
+00014500: 6172 6765 745f 7370 6163 652e 6e5f 6469  arget_space.n_di
+00014510: 6d20 2d20 3120 616e 6420 7461 7267 6574  m - 1 and target
+00014520: 5f73 7061 6365 2e73 697a 6528 2d31 2920  _space.size(-1) 
+00014530: 3d3d 206e 5f64 696d 3a20 7461 7267 6574  == n_dim: target
+00014540: 5f73 7061 6365 2e77 6974 685f 6368 616e  _space.with_chan
+00014550: 6e65 6c64 696d 282d 3129 0a20 2020 2020  neldim(-1).     
+00014560: 2020 2061 766f 7563 6828 7461 7267 6574     avouch(target
+00014570: 5f73 7061 6365 2e68 6173 5f63 6861 6e6e  _space.has_chann
+00014580: 656c 2061 6e64 2074 6172 6765 745f 7370  el and target_sp
+00014590: 6163 652e 6e5f 6368 616e 6e65 6c20 3d3d  ace.n_channel ==
+000145a0: 206e 5f64 696d 2c20 2227 7461 7267 6574   n_dim, "'target
+000145b0: 5f73 7061 6365 2720 666f 7220 696e 7465  _space' for inte
+000145c0: 7270 6f6c 6174 696f 6e20 7368 6f75 6c64  rpolation should
+000145d0: 2068 6176 6520 6120 6368 616e 6e65 6c20   have a channel 
+000145e0: 6469 6d65 6e73 696f 6e20 666f 7220 636f  dimension for co
+000145f0: 6f72 6469 6e61 7465 732e 2022 290a 2020  ordinates. ").  
+00014600: 2020 2020 2020 5920 3d20 7461 7267 6574        Y = target
+00014610: 5f73 7061 6365 2e72 6570 6561 7465 6428  _space.repeated(
+00014620: 6e5f 6261 7463 6820 2f2f 2074 6172 6765  n_batch // targe
+00014630: 745f 7370 6163 652e 6e5f 6261 7463 682c  t_space.n_batch,
+00014640: 205b 5d29 2e61 6d70 6c69 6679 286e 5f66   []).amplify(n_f
+00014650: 6561 7475 7265 2c20 5b5d 290a 2020 2020  eature, []).    
+00014660: 2020 2020 7368 6170 655f 6f75 7420 3d20      shape_out = 
+00014670: 7368 6170 655f 6f75 742e 7265 7365 745f  shape_out.reset_
+00014680: 7370 6163 6528 7461 7267 6574 5f73 7061  space(target_spa
+00014690: 6365 2e73 7061 6365 290a 2020 2020 2020  ce.space).      
+000146a0: 2020 0a20 2020 2069 6d61 6765 203d 2069    .    image = i
+000146b0: 6d61 6765 2e6d 6572 6765 6469 6d73 287b  mage.mergedims({
+000146c0: 7d2c 205b 5d29 0a20 2020 206e 5f62 6174  }, []).    n_bat
+000146d0: 6368 203d 2069 6d61 6765 2e6e 5f62 6174  ch = image.n_bat
+000146e0: 6368 0a0a 2020 2020 6966 206d 6574 686f  ch..    if metho
+000146f0: 642e 6c6f 7765 7228 2920 3d3d 2027 6273  d.lower() == 'bs
+00014700: 706c 696e 6527 3a0a 2020 2020 2020 2020  pline':.        
+00014710: 6966 2064 6572 6976 6174 6976 653a 2072  if derivative: r
+00014720: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
+00014730: 4e6f 2064 6572 6976 6174 6976 6573 2066  No derivatives f
+00014740: 6f72 2062 7370 6c69 6e65 2069 6e74 6572  or bspline inter
+00014750: 706f 6c61 7469 6f6e 7320 6172 6520 6176  polations are av
+00014760: 6169 6c61 626c 6520 736f 2066 6172 2e20  ailable so far. 
+00014770: 506c 6561 7365 2077 7269 7465 2069 7420  Please write it 
+00014780: 6279 2079 6f75 7273 656c 662e 2022 290a  by yourself. ").
+00014790: 2020 2020 2020 2020 2320 544f 444f 3a20          # TODO: 
+000147a0: 4646 440a 2020 2020 2020 2020 7261 6973  FFD.        rais
+000147b0: 6520 5479 7065 4572 726f 7228 2242 7370  e TypeError("Bsp
+000147c0: 6c69 6e65 2069 6e74 6572 706f 6c61 7469  line interpolati
+000147d0: 6f6e 2069 7320 6e6f 7420 6176 6169 6c61  on is not availa
+000147e0: 626c 6520 736f 2066 6172 2e20 506c 6561  ble so far. Plea
+000147f0: 7365 2077 7269 7465 2069 7420 6279 2079  se write it by y
+00014800: 6f75 7273 656c 662e 2022 290a 0a20 2020  ourself. ")..   
+00014810: 2069 5920 3d20 6274 2e66 6c6f 6f72 2859   iY = bt.floor(Y
+00014820: 292e 6c6f 6e67 2829 2023 2047 656e 6572  ).long() # Gener
+00014830: 6174 6520 7468 6520 696e 7465 6765 7220  ate the integer 
+00014840: 7061 7274 206f 6620 590a 2020 2020 6a59  part of Y.    jY
+00014850: 203d 2069 5920 2b20 3120 2320 616e 6420   = iY + 1 # and 
+00014860: 7468 6520 696e 7465 6765 7220 7061 7274  the integer part
+00014870: 2070 6c75 7320 6f6e 652e 0a20 2020 2069   plus one..    i
+00014880: 6620 6d65 7468 6f64 2e6c 6f77 6572 2829  f method.lower()
+00014890: 203d 3d20 276c 696e 6561 7227 3a20 6659   == 'linear': fY
+000148a0: 203d 2059 202d 2069 592e 666c 6f61 7428   = Y - iY.float(
+000148b0: 2920 2320 5468 6520 6465 6369 6d61 6c20  ) # The decimal 
+000148c0: 7061 7274 206f 6620 592e 0a20 2020 2065  part of Y..    e
+000148d0: 6c69 6620 6d65 7468 6f64 2e6c 6f77 6572  lif method.lower
+000148e0: 2829 203d 3d20 276e 6561 7265 7374 273a  () == 'nearest':
+000148f0: 2066 5920 3d20 6274 2e66 6c6f 6f72 2859   fY = bt.floor(Y
+00014900: 202d 2069 592e 666c 6f61 7428 2920 2b20   - iY.float() + 
+00014910: 302e 3529 2023 2054 6865 2064 6563 696d  0.5) # The decim
+00014920: 616c 2070 6172 7420 6f66 2059 2e0a 2020  al part of Y..  
+00014930: 2020 656c 7365 3a20 7261 6973 6520 5479    else: raise Ty
+00014940: 7065 4572 726f 7228 2255 6e72 6563 6f67  peError("Unrecog
+00014950: 6e69 7a65 6420 6172 6775 6d65 6e74 2027  nized argument '
+00014960: 6d65 7468 6f64 272e 2022 290a 2020 2020  method'. ").    
+00014970: 6259 203d 2062 742e 7374 6163 6b28 2869  bY = bt.stack((i
+00014980: 592c 206a 5929 2c20 3129 2e76 6965 7728  Y, jY), 1).view(
+00014990: 5b6e 5f62 6174 6368 5d2c 2032 2c20 7b6e  [n_batch], 2, {n
+000149a0: 5f64 696d 7d2c 202d 3129 2023 2028 5b6e  _dim}, -1) # ([n
+000149b0: 5f62 6174 6368 5d2c 2032 2c20 7b6e 5f64  _batch], 2, {n_d
+000149c0: 696d 7d2c 206e 5f64 6174 6129 2e0a 2020  im}, n_data)..  
+000149d0: 2020 5720 3d20 6274 2e73 7461 636b 2828    W = bt.stack((
+000149e0: 3120 2d20 6659 2c20 6659 292c 2031 292e  1 - fY, fY), 1).
+000149f0: 7669 6577 285b 6e5f 6261 7463 685d 2c20  view([n_batch], 
+00014a00: 322c 207b 6e5f 6469 6d7d 2c20 2d31 2920  2, {n_dim}, -1) 
+00014a10: 2320 285b 6e5f 6261 7463 685d 2c20 322c  # ([n_batch], 2,
+00014a20: 207b 6e5f 6469 6d7d 2c20 6e5f 6461 7461   {n_dim}, n_data
+00014a30: 292e 0a20 2020 206e 5f64 6174 6120 3d20  )..    n_data = 
+00014a40: 6259 2e73 697a 6528 2d31 290a 0a20 2020  bY.size(-1)..   
+00014a50: 2023 2050 7265 7061 7265 2066 6f72 2074   # Prepare for t
+00014a60: 6865 206f 7574 7075 7420 7370 6163 653a  he output space:
+00014a70: 206e 5f62 6174 6368 2c20 6d5f 312c 202e   n_batch, m_1, .
+00014a80: 2e2e 2c20 6d5f 730a 2020 2020 6966 2064  .., m_s.    if d
+00014a90: 6572 6976 6174 6976 653a 206f 7574 7075  erivative: outpu
+00014aa0: 7420 3d20 6274 2e7a 6572 6f73 285b 6e5f  t = bt.zeros([n_
+00014ab0: 6261 7463 685d 2c20 7b6e 5f64 696d 7d2c  batch], {n_dim},
+00014ac0: 202a 7368 6170 655f 6f75 742e 7370 6163   *shape_out.spac
+00014ad0: 6529 0a20 2020 2065 6c73 653a 206f 7574  e).    else: out
+00014ae0: 7075 7420 3d20 6274 2e7a 6572 6f73 2873  put = bt.zeros(s
+00014af0: 6861 7065 5f6f 7574 290a 2020 2020 666f  hape_out).    fo
+00014b00: 7220 4720 696e 2062 742e 696d 6167 655f  r G in bt.image_
+00014b10: 6772 6964 285b 325d 2a6e 5f64 696d 292e  grid([2]*n_dim).
+00014b20: 666c 6174 7465 6e28 292e 7472 616e 7370  flatten().transp
+00014b30: 6f73 6528 302c 2031 293a 0a20 2020 2020  ose(0, 1):.     
+00014b40: 2020 2023 2047 6574 2074 6865 2069 6e64     # Get the ind
+00014b50: 6963 6573 2066 6f72 2074 6865 2074 6572  ices for the ter
+00014b60: 6d3a 2062 595b 3a2c 2047 5b44 5d2c 2044  m: bY[:, G[D], D
+00014b70: 2c20 3a5d 2c20 7369 7a65 3d28 5b6e 5f62  , :], size=([n_b
+00014b80: 6174 6368 5d2c 207b 6e5f 6469 6d7d 2c20  atch], {n_dim}, 
+00014b90: 6e5f 6461 7461 290a 2020 2020 2020 2020  n_data).        
+00014ba0: 496e 6420 3d20 6259 2e67 6174 6865 7228  Ind = bY.gather(
+00014bb0: 312c 2047 2e65 7870 616e 645f 746f 285b  1, G.expand_to([
+00014bc0: 6e5f 6261 7463 685d 2c20 312c 207b 6e5f  n_batch], 1, {n_
+00014bd0: 6469 6d7d 2c20 6e5f 6461 7461 2929 2e73  dim}, n_data)).s
+00014be0: 7175 6565 7a65 2831 290a 2020 2020 2020  queeze(1).      
+00014bf0: 2020 2320 436c 616d 7020 7468 6520 696e    # Clamp the in
+00014c00: 6469 6365 7320 696e 2074 6865 2063 6f72  dices in the cor
+00014c10: 7265 6374 2072 616e 6765 2026 2043 6f6d  rect range & Com
+00014c20: 7075 7465 2074 6865 2062 6f72 6465 7220  pute the border 
+00014c30: 636f 6e64 6974 696f 6e0a 2020 2020 2020  condition.      
+00014c40: 2020 636f 6e64 6974 696f 6e20 3d20 6274    condition = bt
+00014c50: 2e73 756d 2828 496e 6420 3c20 3029 202b  .sum((Ind < 0) +
+00014c60: 2028 496e 6420 3e20 7369 7a65 202d 2031   (Ind > size - 1
+00014c70: 292c 2031 290a 2020 2020 2020 2020 496e  ), 1).        In
+00014c80: 6420 3d20 6274 2e6d 696e 2862 742e 636c  d = bt.min(bt.cl
+00014c90: 616d 7028 496e 642c 206d 696e 3d30 292c  amp(Ind, min=0),
+00014ca0: 2028 7369 7a65 202d 2031 292e 6578 7061   (size - 1).expa
+00014cb0: 6e64 5f74 6f28 496e 6429 290a 2020 2020  nd_to(Ind)).    
+00014cc0: 2020 2020 2320 436f 6e76 6572 7420 7468      # Convert th
+00014cd0: 6520 696e 6469 6365 7320 746f 2031 2064  e indices to 1 d
+00014ce0: 696d 656e 7369 6f6e 616c 2e20 446f 743a  imensional. Dot:
+00014cf0: 2028 5b6e 5f62 6174 6368 5d2c 206e 5f64   ([n_batch], n_d
+00014d00: 6174 6129 0a20 2020 2020 2020 2044 6f74  ata).        Dot
+00014d10: 203d 2049 6e64 5b3a 2c20 305d 0a20 2020   = Ind[:, 0].   
+00014d20: 2020 2020 2066 6f72 2072 2069 6e20 7261       for r in ra
+00014d30: 6e67 6528 312c 206e 5f64 696d 293a 2044  nge(1, n_dim): D
+00014d40: 6f74 202a 3d20 7369 7a65 5b72 5d3b 2044  ot *= size[r]; D
+00014d50: 6f74 202b 3d20 496e 645b 3a2c 2072 5d0a  ot += Ind[:, r].
+00014d60: 2020 2020 2020 2020 2320 4765 7420 7468          # Get th
+00014d70: 6520 696d 6167 6520 7661 6c75 6573 2049  e image values I
+00014d80: 563a 2028 5b6e 5f62 6174 6368 5d2c 206e  V: ([n_batch], n
+00014d90: 5f64 6174 6129 0a20 2020 2020 2020 2049  _data).        I
+00014da0: 5620 3d20 4e6f 6e65 0a20 2020 2020 2020  V = None.       
+00014db0: 2069 6620 6973 696e 7374 616e 6365 2866   if isinstance(f
+00014dc0: 696c 6c2c 2073 7472 293a 0a20 2020 2020  ill, str):.     
+00014dd0: 2020 2020 2020 2069 6620 6669 6c6c 2e6c         if fill.l
+00014de0: 6f77 6572 2829 203d 3d20 276e 6561 7265  ower() == 'neare
+00014df0: 7374 273a 0a20 2020 2020 2020 2020 2020  st':.           
+00014e00: 2020 2020 2049 5620 3d20 696d 6167 652e       IV = image.
+00014e10: 666c 6174 7465 6e28 292e 6761 7468 6572  flatten().gather
+00014e20: 2831 2c20 446f 7429 0a20 2020 2020 2020  (1, Dot).       
+00014e30: 2020 2020 2065 6c69 6620 6669 6c6c 2e6c       elif fill.l
+00014e40: 6f77 6572 2829 203d 3d20 2762 6163 6b67  ower() == 'backg
+00014e50: 726f 756e 6427 3a0a 2020 2020 2020 2020  round':.        
+00014e60: 2020 2020 2020 2020 626b 5f76 616c 7565          bk_value
+00014e70: 203d 2062 742e 7374 6163 6b28 5b69 6d61   = bt.stack([ima
+00014e80: 6765 5b28 736c 6963 6528 4e6f 6e65 292c  ge[(slice(None),
+00014e90: 2920 2b20 7475 706c 6528 6729 5d20 666f  ) + tuple(g)] fo
+00014ea0: 7220 6720 696e 2028 6274 2e69 6d61 6765  r g in (bt.image
+00014eb0: 5f67 7269 6428 5b32 5d2a 6e5f 6469 6d29  _grid([2]*n_dim)
+00014ec0: 202a 2062 742e 6368 616e 6e65 6c5f 7465   * bt.channel_te
+00014ed0: 6e73 6f72 2873 697a 652d 3129 292e 666c  nsor(size-1)).fl
+00014ee0: 6174 7465 6e28 292e 7472 616e 7370 6f73  atten().transpos
+00014ef0: 6528 302c 3129 5d2c 2031 292e 6d65 6469  e(0,1)], 1).medi
+00014f00: 616e 2831 292e 7661 6c75 6573 0a20 2020  an(1).values.   
+00014f10: 2020 2020 2020 2020 2020 2020 2062 6163               bac
+00014f20: 6b67 726f 756e 6420 3d20 626b 5f76 616c  kground = bk_val
+00014f30: 7565 202a 2062 742e 6f6e 6573 5f6c 696b  ue * bt.ones_lik
+00014f40: 6528 446f 7429 0a20 2020 2020 2020 2020  e(Dot).         
+00014f50: 2020 2065 6c69 6620 6669 6c6c 2e6c 6f77     elif fill.low
+00014f60: 6572 2829 203d 3d20 277a 6572 6f27 3a0a  er() == 'zero':.
+00014f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f80: 6261 636b 6772 6f75 6e64 203d 2062 742e  background = bt.
+00014f90: 7a65 726f 735f 6c69 6b65 2844 6f74 290a  zeros_like(Dot).
+00014fa0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00014fb0: 2020 2020 2020 2020 2020 6261 636b 6772            backgr
+00014fc0: 6f75 6e64 203d 2066 696c 6c20 2a20 6274  ound = fill * bt
+00014fd0: 2e6f 6e65 735f 6c69 6b65 2844 6f74 290a  .ones_like(Dot).
+00014fe0: 2020 2020 2020 2020 6966 2049 5620 6973          if IV is
+00014ff0: 204e 6f6e 653a 2049 5620 3d20 6274 2e77   None: IV = bt.w
+00015000: 6865 7265 2863 6f6e 6469 7469 6f6e 203e  here(condition >
+00015010: 3d20 312c 2062 6163 6b67 726f 756e 642e  = 1, background.
+00015020: 666c 6f61 7428 292c 2069 6d61 6765 2e66  float(), image.f
+00015030: 6c61 7474 656e 2829 2e67 6174 6865 7228  latten().gather(
+00015040: 312c 2044 6f74 292e 666c 6f61 7428 2929  1, Dot).float())
+00015050: 0a20 2020 2020 2020 2023 2057 6569 6768  .        # Weigh
+00015060: 7473 2066 6f72 2065 6163 6820 706f 696e  ts for each poin
+00015070: 743a 205b 7072 6f64 7563 7420 6f66 2057  t: [product of W
+00015080: 5b3a 2c20 475b 445d 2c20 442c 2078 5d20  [:, G[D], D, x] 
+00015090: 666f 7220 4420 696e 2072 616e 6765 286e  for D in range(n
+000150a0: 5f64 696d 295d 2066 6f72 2070 6f69 6e74  _dim)] for point
+000150b0: 2078 2e0a 2020 2020 2020 2020 2320 5767   x..        # Wg
+000150c0: 3a20 285b 6e5f 6261 7463 685d 2c20 7b6e  : ([n_batch], {n
+000150d0: 5f64 696d 7d2c 206e 5f64 6174 6129 0a20  _dim}, n_data). 
+000150e0: 2020 2020 2020 2057 6720 3d20 572e 6761         Wg = W.ga
+000150f0: 7468 6572 2831 2c20 472e 6578 7061 6e64  ther(1, G.expand
+00015100: 5f74 6f28 5b6e 5f62 6174 6368 5d2c 2031  _to([n_batch], 1
+00015110: 2c20 7b6e 5f64 696d 7d2c 206e 5f64 6174  , {n_dim}, n_dat
+00015120: 6129 292e 7371 7565 657a 6528 3129 0a20  a)).squeeze(1). 
+00015130: 2020 2020 2020 2069 6620 6e6f 7420 6465         if not de
+00015140: 7269 7661 7469 7665 3a0a 2020 2020 2020  rivative:.      
+00015150: 2020 2020 2020 6f75 7470 7574 202b 3d20        output += 
+00015160: 2857 672e 7072 6f64 2831 2920 2a20 4956  (Wg.prod(1) * IV
+00015170: 292e 7669 6577 5f61 7328 6f75 7470 7574  ).view_as(output
+00015180: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00015190: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+000151a0: 5767 4d61 7420 3d20 5767 2e6d 756c 7469  WgMat = Wg.multi
+000151b0: 706c 7928 6e5f 6469 6d2c 2031 2920 2320  ply(n_dim, 1) # 
+000151c0: 285b 6e5f 6261 7463 685d 2c20 6e5f 6469  ([n_batch], n_di
+000151d0: 6d2c 207b 6e5f 6469 6d7d 2c20 6e5f 6461  m, {n_dim}, n_da
+000151e0: 7461 290a 2020 2020 2020 2020 2020 2020  ta).            
+000151f0: 7465 6d70 5767 4d61 745b 3a2c 2062 742e  tempWgMat[:, bt.
+00015200: 6172 616e 6765 286e 5f64 696d 292c 2062  arange(n_dim), b
+00015210: 742e 6172 616e 6765 286e 5f64 696d 295d  t.arange(n_dim)]
+00015220: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
+00015230: 2064 5767 203d 2074 656d 7057 674d 6174   dWg = tempWgMat
+00015240: 2e70 726f 6428 3129 202a 2028 4720 2a20  .prod(1) * (G * 
+00015250: 3220 2d20 3129 2e66 6c6f 6174 2829 0a20  2 - 1).float(). 
+00015260: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+00015270: 7420 2b3d 2028 6457 6720 2a20 4956 2e75  t += (dWg * IV.u
+00015280: 6e73 7175 6565 7a65 2831 2929 2e76 6965  nsqueeze(1)).vie
+00015290: 775f 6173 286f 7574 7075 7429 0a20 2020  w_as(output).   
+000152a0: 2062 742e 746f 7263 682e 6375 6461 2e65   bt.torch.cuda.e
+000152b0: 6d70 7479 5f63 6163 6865 2829 0a20 2020  mpty_cache().   
+000152c0: 2065 7073 203d 2031 652d 360a 2020 2020   eps = 1e-6.    
+000152d0: 6d20 3d20 3020 6966 2069 6d61 6765 2e6d  m = 0 if image.m
+000152e0: 696e 2829 203e 202d 6570 7320 656c 7365  in() > -eps else
+000152f0: 2069 6d61 6765 2e6d 696e 2829 2e69 7465   image.min().ite
+00015300: 6d28 290a 2020 2020 4d20 3d20 3120 6966  m().    M = 1 if
+00015310: 2069 6d61 6765 2e6d 6178 2829 203c 2031   image.max() < 1
+00015320: 202b 2065 7073 2065 6c73 6520 696d 6167   + eps else imag
+00015330: 652e 6d61 7828 292e 6974 656d 2829 0a20  e.max().item(). 
+00015340: 2020 2072 6574 7572 6e20 6f75 7470 7574     return output
+00015350: 2e63 6c61 6d70 286d 2c20 4d29 0a0a 4061  .clamp(m, M)..@a
+00015360: 6c69 6173 2822 7265 7361 6d70 6c65 5f66  lias("resample_f
+00015370: 6f72 7761 7264 2229 0a64 6566 2069 6e74  orward").def int
+00015380: 6572 706f 6c61 7469 6f6e 5f66 6f72 7761  erpolation_forwa
+00015390: 7264 280a 2020 2020 2020 2020 696d 6167  rd(.        imag
+000153a0: 652c 200a 2020 2020 2020 2020 7472 616e  e, .        tran
+000153b0: 7320 3d20 4e6f 6e65 2c20 0a20 2020 2020  s = None, .     
+000153c0: 2020 206d 6574 686f 6420 3d20 274c 696e     method = 'Lin
+000153d0: 6561 7227 2c20 0a20 2020 2020 2020 2074  ear', .        t
+000153e0: 6172 6765 745f 7370 6163 6520 3d20 4e6f  arget_space = No
+000153f0: 6e65 2c0a 2020 2020 2020 2020 6669 6c6c  ne,.        fill
+00015400: 203d 2027 7a65 726f 272c 0a20 2020 2020   = 'zero',.     
+00015410: 2020 2064 6572 6976 6174 6976 6520 3d20     derivative = 
+00015420: 4661 6c73 650a 2020 2020 293a 0a20 2020  False.    ):.   
+00015430: 2027 2727 0a20 2020 2049 6e74 6572 706f   '''.    Interpo
+00015440: 6c61 7465 2075 7369 6e67 2066 6f72 7761  late using forwa
+00015450: 7264 2074 7261 6e73 666f 726d 6174 696f  rd transformatio
+00015460: 6e2e 2049 7420 6973 206e 6f74 2079 6574  n. It is not yet
+00015470: 2069 6d70 6c65 6d65 6e74 6564 2e20 0a20   implemented. . 
+00015480: 2020 2069 2e65 2e20 436f 6d70 7574 6520     i.e. Compute 
+00015490: 7468 6520 696d 6167 6520 4920 732e 742e  the image I s.t.
+000154a0: 2074 7261 6e73 2878 2920 3d20 7920 666f   trans(x) = y fo
+000154b0: 7220 7820 696e 2069 6e70 7574 2069 6d61  r x in input ima
+000154c0: 6765 2061 6e64 2079 2069 6e20 7468 6520  ge and y in the 
+000154d0: 6f75 7470 7574 2049 2075 7369 6e67 2069  output I using i
+000154e0: 6e74 6572 706f 6c61 7469 6f6e 206d 6574  nterpolation met
+000154f0: 686f 643a 0a20 2020 2020 2020 206d 6574  hod:.        met
+00015500: 686f 6420 3d20 4c69 6e65 6172 205b 4e4f  hod = Linear [NO
+00015510: 2047 5241 4449 454e 5421 2121 5d3a 2042   GRADIENT!!!]: B
+00015520: 696c 696e 6561 7220 696e 7465 7270 6f6c  ilinear interpol
+00015530: 6174 696f 6e0a 2020 2020 2020 2020 6d65  ation.        me
+00015540: 7468 6f64 203d 204e 6561 7265 7374 205b  thod = Nearest [
+00015550: 4e4f 2047 5241 4449 454e 5421 2121 5d3a  NO GRADIENT!!!]:
+00015560: 204e 6561 7265 7374 2069 6e74 6572 706f   Nearest interpo
+00015570: 6c61 7469 6f6e 0a0a 2020 2020 5061 7261  lation..    Para
+00015580: 6d73 3a0a 2020 2020 2020 2020 696d 6167  ms:.        imag
+00015590: 6520 5b62 742e 5465 6e73 6f72 5d3a 2054  e [bt.Tensor]: T
+000155a0: 6865 2074 6172 6765 7420 696d 6167 652e  he target image.
+000155b0: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+000155c0: 653a 2028 5b6e 5f62 6174 6368 3a6f 7074  e: ([n_batch:opt
+000155d0: 696f 6e61 6c5d 2c20 7b6e 5f63 6861 6e6e  ional], {n_chann
+000155e0: 656c 3a6f 7074 696f 6e61 6c7d 2c20 6d40  el:optional}, m@
+000155f0: 312c 206d 4032 2c20 2e2e 2e2c 206d 406e  1, m@2, ..., m@n
+00015600: 5f64 696d 290a 2020 2020 2020 2020 7472  _dim).        tr
+00015610: 616e 7320 5b46 756e 6374 696f 6e20 6f72  ans [Function or
+00015620: 206d 6963 6f6d 7075 7469 6e67 2e53 7061   micomputing.Spa
+00015630: 7469 616c 5472 616e 7366 6f72 6d61 7469  tialTransformati
+00015640: 6f6e 5d3a 2054 7261 6e73 666f 726d 6174  on]: Transformat
+00015650: 696f 6e20 6675 6e63 7469 6f6e 2c20 6d61  ion function, ma
+00015660: 7070 696e 670a 2020 2020 2020 2020 2020  pping.          
+00015670: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
+00015680: 683a 6f70 7469 6f6e 616c 5d2c 207b 6e5f  h:optional], {n_
+00015690: 6469 6d7d 2c20 6e40 312c 206e 4032 2c20  dim}, n@1, n@2, 
+000156a0: 2e2e 2e2c 206e 406e 5f64 696d 2920 746f  ..., n@n_dim) to
+000156b0: 2028 5b6e 5f62 6174 6368 5d2c 207b 6e5f   ([n_batch], {n_
+000156c0: 6469 6d7d 2c20 6e40 312c 206e 4032 2c20  dim}, n@1, n@2, 
+000156d0: 2e2e 2e2c 206e 406e 5f64 696d 290a 2020  ..., n@n_dim).  
+000156e0: 2020 2020 2020 6d65 7468 6f64 205b 7374        method [st
+000156f0: 723a 206c 696e 6561 727c 6e65 6172 6573  r: linear|neares
+00015700: 745d 3a20 5468 6520 696e 7465 7270 6f6c  t]: The interpol
+00015710: 6174 696f 6e20 6d65 7468 6f64 2e20 0a20  ation method. . 
+00015720: 2020 2020 2020 2074 6172 6765 745f 7370         target_sp
+00015730: 6163 6520 5b74 7570 6c65 206f 7220 6274  ace [tuple or bt
+00015740: 2e54 656e 736f 725d 3a0a 2020 2020 2020  .Tensor]:.      
+00015750: 2020 2020 2020 5369 7a65 2028 7475 706c        Size (tupl
+00015760: 6529 206f 6620 6120 7461 7267 6574 2052  e) of a target R
+00015770: 4f49 2061 7420 7468 6520 6365 6e74 6572  OI at the center
+00015780: 206f 6620 696d 6167 652e 200a 2020 2020   of image. .    
+00015790: 2020 2020 2020 2020 4f52 2054 7261 6e73          OR Trans
+000157a0: 666f 726d 6564 2063 6f6f 7264 696e 6174  formed coordinat
+000157b0: 6520 7370 6163 6520 2862 742e 5465 6e73  e space (bt.Tens
+000157c0: 6f72 2920 6f66 2074 6865 206f 7574 7075  or) of the outpu
+000157d0: 7420 696d 6167 652e 200a 2020 2020 2020  t image. .      
+000157e0: 2020 2020 2020 7369 7a65 3a20 6c65 6e67        size: leng
+000157f0: 7468 286e 5f64 696d 2920 6f72 2028 5b6e  th(n_dim) or ([n
+00015800: 5f62 6174 6368 3a6f 7074 696f 6e61 6c5d  _batch:optional]
+00015810: 2c20 7b6e 5f64 696d 3a6f 7074 696f 6e61  , {n_dim:optiona
+00015820: 6c7d 2c20 7369 7a65 4031 2c20 7369 7a65  l}, size@1, size
+00015830: 4032 2c20 2e2e 2e2c 2073 697a 6540 6e5f  @2, ..., size@n_
+00015840: 6469 6d29 0a20 2020 2020 2020 2066 696c  dim).        fil
+00015850: 6c20 5b73 7472 3a20 6e65 6172 6573 747c  l [str: nearest|
+00015860: 6261 636b 6772 6f75 6e64 206f 7220 696e  background or in
+00015870: 7420 6f72 2066 6c6f 6174 286e 756d 6265  t or float(numbe
+00015880: 7229 5d3a 2049 6e64 6963 6174 6520 7468  r)]: Indicate th
+00015890: 6520 7761 7920 746f 2066 696c 6c20 6261  e way to fill ba
+000158a0: 636b 6772 6f75 6e64 206f 7574 7369 6465  ckground outside
+000158b0: 2060 5375 7272 6f75 6e64 696e 6760 2e20   `Surrounding`. 
+000158c0: 0a20 2020 2020 2020 2064 6572 6976 6174  .        derivat
+000158d0: 6976 6520 5b62 6f6f 6c5d 3a20 5768 6574  ive [bool]: Whet
+000158e0: 6865 7220 746f 2072 6574 7572 6e20 7468  her to return th
+000158f0: 6520 6772 6164 6965 6e74 2e20 4f6e 6520  e gradient. One 
+00015900: 6361 6e20 6f6d 6974 2069 7420 7768 656e  can omit it when
+00015910: 2075 7369 6e67 2074 6f72 6368 2e61 7574   using torch.aut
+00015920: 6f67 7261 642e 0a0a 2020 2020 2020 2020  ograd...        
+00015930: 6f75 7470 7574 205b 6274 2e54 656e 736f  output [bt.Tenso
+00015940: 725d 3a20 5468 6520 7472 616e 7366 6f72  r]: The transfor
+00015950: 6d65 6420 696d 6167 652e 0a20 2020 2020  med image..     
+00015960: 2020 2020 2020 2073 697a 653a 2028 5b6e         size: ([n
+00015970: 5f62 6174 6368 5d2c 207b 6e5f 6368 616e  _batch], {n_chan
+00015980: 6e65 6c3a 6f70 7469 6f6e 616c 7d2c 206d  nel:optional}, m
+00015990: 4031 2c20 6d40 322c 202e 2e2e 2c20 6d40  @1, m@2, ..., m@
+000159a0: 6e5f 6469 6d29 0a20 2020 2020 2020 2020  n_dim).         
+000159b0: 2020 206f 7220 7768 656e 2060 7461 7267     or when `targ
+000159c0: 6574 5f73 7061 6365 6020 6973 2064 6566  et_space` is def
+000159d0: 696e 6564 2062 7920 7465 6e73 6f72 2e20  ined by tensor. 
+000159e0: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+000159f0: 653a 2028 5b6e 5f62 6174 6368 5d2c 2073  e: ([n_batch], s
+00015a00: 697a 6540 312c 2073 697a 6540 322c 202e  ize@1, size@2, .
+00015a10: 2e2e 2c20 7369 7a65 406e 5f64 696d 290a  .., size@n_dim).
+00015a20: 2020 2020 2020 2020 2020 2020 6f72 2074              or t
+00015a30: 6865 2064 6572 6976 6174 6976 6520 666f  he derivative fo
+00015a40: 7220 7468 6520 696e 7465 7270 6f6c 6174  r the interpolat
+00015a50: 696f 6e2e 2028 6966 2060 6465 7269 7661  ion. (if `deriva
+00015a60: 7469 7665 203d 2054 7275 6560 290a 2020  tive = True`).  
+00015a70: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
+00015a80: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f64  ([n_batch], {n_d
+00015a90: 696d 7d2c 2073 697a 6540 312c 2073 697a  im}, size@1, siz
+00015aa0: 6540 322c 202e 2e2e 2c20 7369 7a65 406e  e@2, ..., size@n
+00015ab0: 5f64 696d 290a 0a20 2020 2045 7861 6d70  _dim)..    Examp
+00015ac0: 6c65 733a 0a20 2020 202d 2d2d 2d2d 2d2d  les:.    -------
+00015ad0: 2d2d 2d0a 2020 2020 3e3e 3e20 496d 6167  ---.    >>> Imag
+00015ae0: 6520 3d20 6274 2e72 616e 6428 332c 2031  e = bt.rand(3, 1
+00015af0: 3030 2c20 3132 302c 2038 3029 0a20 2020  00, 120, 80).   
+00015b00: 203e 3e3e 2041 4d20 3d20 6274 2e72 616e   >>> AM = bt.ran
+00015b10: 6428 342c 2034 290a 2020 2020 3e3e 3e20  d(4, 4).    >>> 
+00015b20: 414d 5b33 2c20 3a5d 203d 2062 742e 6f6e  AM[3, :] = bt.on
+00015b30: 655f 686f 7428 2d31 2c20 3429 0a20 2020  e_hot(-1, 4).   
+00015b40: 203e 3e3e 2069 6e74 6572 706f 6c61 7469   >>> interpolati
+00015b50: 6f6e 2849 6d61 6765 2c20 4166 6669 6e65  on(Image, Affine
+00015b60: 2841 4d29 2c20 6d65 7468 6f64 3d27 4c69  (AM), method='Li
+00015b70: 6e65 6172 2729 0a20 2020 2027 2727 0a20  near').    '''. 
+00015b80: 2020 2069 6620 7472 616e 7320 6973 206e     if trans is n
+00015b90: 6f74 204e 6f6e 6520 616e 6420 7472 616e  ot None and tran
+00015ba0: 732e 6261 636b 7761 7264 3a0a 2020 2020  s.backward:.    
+00015bb0: 2020 2020 6966 2068 6173 6174 7472 2874      if hasattr(t
+00015bc0: 7261 6e73 2c20 2769 6e76 2729 3a20 7472  rans, 'inv'): tr
+00015bd0: 616e 7320 3d20 7472 616e 732e 696e 7628  ans = trans.inv(
+00015be0: 292e 6661 6b65 5f69 6e76 2829 0a20 2020  ).fake_inv().   
+00015bf0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00015c00: 2020 2020 2020 2070 7269 6e74 2822 5761         print("Wa
+00015c10: 726e 696e 673a 2042 6163 6b77 6172 6420  rning: Backward 
+00015c20: 7472 616e 7366 6f72 6d61 7469 6f6e 2066  transformation f
+00015c30: 6f75 6e64 2069 6e20 6d65 7468 6f64 2060  ound in method `
+00015c40: 696e 7465 7270 6f6c 6174 696f 6e5f 666f  interpolation_fo
+00015c50: 7277 6172 6460 2e20 5573 696e 6720 6069  rward`. Using `i
+00015c60: 6e74 6572 706f 6c61 7469 6f6e 6020 696e  nterpolation` in
+00015c70: 7374 6561 642e 2022 290a 2020 2020 2020  stead. ").      
+00015c80: 2020 2020 2020 7265 7475 726e 2069 6e74        return int
+00015c90: 6572 706f 6c61 7469 6f6e 2869 6d61 6765  erpolation(image
+00015ca0: 2c20 7472 616e 732c 206d 6574 686f 6420  , trans, method 
+00015cb0: 3d20 6d65 7468 6f64 2c20 7461 7267 6574  = method, target
+00015cc0: 5f73 7061 6365 203d 2074 6172 6765 745f  _space = target_
+00015cd0: 7370 6163 652c 2066 696c 6c20 3d20 6669  space, fill = fi
+00015ce0: 6c6c 290a 2020 2020 7265 7475 726e 204e  ll).    return N
+00015cf0: 6f74 496d 706c 656d 656e 7465 640a 0a23  otImplemented..#
+00015d00: 2323 2323 2323 2323 2323 2320 496d 6167  ########### Imag
+00015d10: 6520 5472 616e 7366 6f72 6d61 7469 6f6e  e Transformation
+00015d20: 7320 2323 2323 2323 2323 2323 2323 0a0a  s ############..
+00015d30: 636c 6173 7320 496d 6167 6554 7261 6e73  class ImageTrans
+00015d40: 666f 726d 6174 696f 6e28 5472 616e 7366  formation(Transf
+00015d50: 6f72 6d61 7469 6f6e 293a 0a20 2020 2020  ormation):.     
+00015d60: 2020 200a 2020 2020 6465 6620 5f5f 6361     .    def __ca
+00015d70: 6c6c 5f5f 2873 656c 662c 2058 293a 0a20  ll__(self, X):. 
+00015d80: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00015d90: 2020 2058 205b 6274 2e54 656e 736f 725d     X [bt.Tensor]
+00015da0: 3a20 496d 6167 6520 746f 2062 6520 7472  : Image to be tr
+00015db0: 616e 7366 6f72 6d65 642e 0a20 2020 2020  ansformed..     
+00015dc0: 2020 2020 2020 2073 697a 653a 2028 5b6e         size: ([n
+00015dd0: 5f62 6174 6368 3a6f 7074 696f 6e61 6c5d  _batch:optional]
+00015de0: 2c20 7b6e 5f63 6861 6e6e 656c 3a6f 7074  , {n_channel:opt
+00015df0: 696f 6e61 6c7d 2c20 6e40 312c 206e 4032  ional}, n@1, n@2
+00015e00: 2c20 2e2e 2e2c 206e 406e 5f64 696d 290a  , ..., n@n_dim).
+00015e10: 2020 2020 2020 2020 6f75 7470 7574 205b          output [
+00015e20: 6274 2e54 656e 736f 725d 3a20 5468 6520  bt.Tensor]: The 
+00015e30: 7472 616e 7366 6f72 6d65 6420 696d 6167  transformed imag
+00015e40: 652e 0a20 2020 2020 2020 2020 2020 2073  e..            s
+00015e50: 697a 653a 2028 5b6e 5f62 6174 6368 5d2c  ize: ([n_batch],
+00015e60: 207b 6e5f 6368 616e 6e65 6c7d 2c20 6e40   {n_channel}, n@
+00015e70: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
+00015e80: 5f64 696d 290a 2020 2020 2020 2020 2727  _dim).        ''
+00015e90: 270a 2020 2020 2020 2020 5820 3d20 6261  '.        X = ba
+00015ea0: 746f 7263 685f 7465 6e73 6f72 2858 290a  torch_tensor(X).
+00015eb0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00015ec0: 6e5f 6469 6d20 6973 204e 6f6e 653a 0a20  n_dim is None:. 
+00015ed0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00015ee0: 7420 582e 6861 735f 6261 7463 683a 2058  t X.has_batch: X
+00015ef0: 203d 2058 2e75 6e73 7175 6565 7a65 285b   = X.unsqueeze([
+00015f00: 5d29 0a20 2020 2020 2020 2020 2020 2069  ]).            i
+00015f10: 6620 6e6f 7420 582e 6861 735f 6368 616e  f not X.has_chan
+00015f20: 6e65 6c3a 2058 203d 2058 2e73 7461 6e64  nel: X = X.stand
+00015f30: 6172 6428 292e 756e 7371 7565 657a 6528  ard().unsqueeze(
+00015f40: 7b31 7d29 0a20 2020 2020 2020 2065 6c73  {1}).        els
+00015f50: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+00015f60: 6620 582e 6e5f 6469 6d20 3d3d 2073 656c  f X.n_dim == sel
+00015f70: 662e 6e5f 6469 6d3a 2058 203d 2058 2e72  f.n_dim: X = X.r
+00015f80: 656d 6f76 655f 7370 6563 6961 6c5f 2829  emove_special_()
+00015f90: 2e75 6e73 7175 6565 7a65 285b 5d29 2e75  .unsqueeze([]).u
+00015fa0: 6e73 7175 6565 7a65 287b 317d 290a 2020  nsqueeze({1}).  
+00015fb0: 2020 2020 2020 2020 2020 656c 6966 2058            elif X
+00015fc0: 2e6e 5f64 696d 203d 3d20 7365 6c66 2e6e  .n_dim == self.n
+00015fd0: 5f64 696d 202b 2031 3a0a 2020 2020 2020  _dim + 1:.      
+00015fe0: 2020 2020 2020 2020 2020 6966 2058 2e68            if X.h
+00015ff0: 6173 5f62 6174 6368 3a20 582e 6368 616e  as_batch: X.chan
+00016000: 6e65 6c5f 6469 6d65 6e73 696f 6e20 3d20  nel_dimension = 
+00016010: 4e6f 6e65 3b20 5820 3d20 582e 756e 7371  None; X = X.unsq
+00016020: 7565 657a 6528 7b30 2069 6620 582e 6261  ueeze({0 if X.ba
+00016030: 7463 685f 6469 6d65 6e73 696f 6e20 3e20  tch_dimension > 
+00016040: 3020 656c 7365 2031 7d29 0a20 2020 2020  0 else 1}).     
+00016050: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00016060: 582e 6861 735f 6368 616e 6e65 6c3a 2058  X.has_channel: X
+00016070: 203d 2058 2e75 6e73 7175 6565 7a65 285b   = X.unsqueeze([
+00016080: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00016090: 2020 2065 6c73 653a 2058 203d 2058 2e62     else: X = X.b
+000160a0: 6174 6368 5f64 696d 656e 7369 6f6e 5f28  atch_dimension_(
+000160b0: 3029 2e75 6e73 7175 6565 7a65 287b 317d  0).unsqueeze({1}
+000160c0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+000160d0: 6966 2058 2e6e 5f64 696d 203d 3d20 7365  if X.n_dim == se
+000160e0: 6c66 2e6e 5f64 696d 202b 2032 3a0a 2020  lf.n_dim + 2:.  
+000160f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00016100: 5f63 6861 6e6e 616c 2f62 6174 6368 2064  _channal/batch d
+00016110: 696d 656e 7369 6f6e 7320 7573 6564 2068  imensions used h
+00016120: 6572 6520 6173 2074 6865 7920 6172 6520  ere as they are 
+00016130: 6e5f 6469 6d20 7768 656e 206e 6f74 2065  n_dim when not e
+00016140: 7869 7374 6564 2e20 0a20 2020 2020 2020  xisted. .       
+00016150: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00016160: 582e 6861 735f 6261 7463 683a 2058 2e62  X.has_batch: X.b
+00016170: 6174 6368 5f64 696d 656e 7369 6f6e 203d  atch_dimension =
+00016180: 2030 2069 6620 582e 5f63 6861 6e6e 656c   0 if X._channel
+00016190: 5f64 696d 656e 7369 6f6e 203e 2030 2065  _dimension > 0 e
+000161a0: 6c73 6520 310a 2020 2020 2020 2020 2020  lse 1.          
+000161b0: 2020 2020 2020 6966 206e 6f74 2058 2e68        if not X.h
+000161c0: 6173 5f63 6861 6e6e 656c 3a20 582e 6368  as_channel: X.ch
+000161d0: 616e 6e65 6c5f 6469 6d65 6e73 696f 6e20  annel_dimension 
+000161e0: 3d20 3020 6966 2058 2e5f 6261 7463 685f  = 0 if X._batch_
+000161f0: 6469 6d65 6e73 696f 6e20 3e20 3020 656c  dimension > 0 el
+00016200: 7365 2031 0a20 2020 2020 2020 2061 766f  se 1.        avo
+00016210: 7563 6828 582e 6861 735f 6261 7463 6820  uch(X.has_batch 
+00016220: 616e 6420 582e 6861 735f 6368 616e 6e65  and X.has_channe
+00016230: 6c2c 2066 2250 6c65 6173 6520 7573 6520  l, f"Please use 
+00016240: 6261 746f 7263 6820 7465 6e73 6f72 206f  batorch tensor o
+00016250: 6620 7369 7a65 205c 0a20 2020 2020 2020  f size \.       
+00016260: 2020 2020 2028 5b6e 5f62 6174 6368 5d2c       ([n_batch],
+00016270: 207b 7b6e 5f63 6861 6e6e 656c 2f6e 5f66   {{n_channel/n_f
+00016280: 6561 7475 7265 3a6f 7074 696f 6e61 6c7d  eature:optional}
+00016290: 7d2c 206d 5f31 2c20 6d5f 322c 202e 2e2e  }, m_1, m_2, ...
+000162a0: 2c20 6d5f 7229 205b 723d 6e5f 6469 6d5d  , m_r) [r=n_dim]
+000162b0: 2066 6f72 205c 0a20 2020 2020 2020 2020   for \.         
+000162c0: 2020 2020 2020 207b 7365 6c66 2e5f 5f63         {self.__c
+000162d0: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f2e  lass__.__name__.
+000162e0: 7370 6c69 7428 272e 2729 5b2d 315d 7d20  split('.')[-1]} 
+000162f0: 5472 616e 7366 6f72 6d61 7469 6f6e 2c20  Transformation, 
+00016300: 696e 7374 6561 6420 6f66 207b 582e 7368  instead of {X.sh
+00016310: 6170 657d 2e20 2229 0a20 2020 2020 2020  ape}. ").       
+00016320: 2072 6574 7572 6e20 582e 636c 6f6e 6528   return X.clone(
+00016330: 290a 0a63 6c61 7373 204e 6f72 6d61 6c69  )..class Normali
+00016340: 7a65 2849 6d61 6765 5472 616e 7366 6f72  ze(ImageTransfor
+00016350: 6d61 7469 6f6e 293a 0a20 2020 2064 6566  mation):.    def
+00016360: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00016370: 2a5f 7261 6e67 6529 3a0a 2020 2020 2020  *_range):.      
+00016380: 2020 2727 270a 2020 2020 2020 2020 4e6f    '''.        No
+00016390: 726d 616c 697a 6520 7468 6520 696e 7465  rmalize the inte
+000163a0: 6e73 6974 7920 6f66 2061 6e20 696d 6167  nsity of an imag
+000163b0: 652e 0a20 2020 2020 2020 200a 2020 2020  e..        .    
+000163c0: 2020 2020 5061 7261 6d73 3a0a 2020 2020      Params:.    
+000163d0: 2020 2020 2020 2020 5f72 616e 6765 203d          _range =
+000163e0: 2028 6c6f 772c 2068 6967 6829 205b 696e   (low, high) [in
+000163f0: 7420 6f72 2066 6c6f 6174 206f 7220 6274  t or float or bt
+00016400: 2e54 656e 736f 725d 3a20 5468 6520 6c6f  .Tensor]: The lo
+00016410: 7765 7374 2028 616e 6420 6869 6768 6573  west (and highes
+00016420: 7429 2069 6e74 656e 7369 7479 2e20 0a20  t) intensity. . 
+00016430: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016440: 697a 653a 206c 656e 6774 6828 3229 206f  ize: length(2) o
+00016450: 7220 285b 6e5f 6261 7463 685d 2c20 7b32  r ([n_batch], {2
+00016460: 7d29 0a20 2020 2020 2020 2020 2020 200a  }).            .
+00016470: 2020 2020 2020 2020 5768 656e 2069 7420          When it 
+00016480: 6973 2063 616c 6c65 643a 0a20 2020 2020  is called:.     
+00016490: 2020 2020 2020 2058 205b 6274 2e54 656e         X [bt.Ten
+000164a0: 736f 725d 3a20 496d 6167 6520 746f 2062  sor]: Image to b
+000164b0: 6520 7472 616e 7366 6f72 6d65 642e 0a20  e transformed.. 
+000164c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000164d0: 697a 653a 2028 5b6e 5f62 6174 6368 3a6f  ize: ([n_batch:o
+000164e0: 7074 696f 6e61 6c5d 2c20 7b6e 5f63 6861  ptional], {n_cha
+000164f0: 6e6e 656c 3a6f 7074 696f 6e61 6c7d 2c20  nnel:optional}, 
+00016500: 6e40 312c 206e 4032 2c20 2e2e 2e2c 206e  n@1, n@2, ..., n
+00016510: 406e 5f64 696d 290a 2020 2020 2020 2020  @n_dim).        
+00016520: 2020 2020 6f75 7470 7574 205b 6274 2e54      output [bt.T
+00016530: 656e 736f 725d 3a20 5468 6520 7472 616e  ensor]: The tran
+00016540: 7366 6f72 6d65 6420 696d 6167 652e 0a20  sformed image.. 
+00016550: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016560: 697a 653a 2028 5b6e 5f62 6174 6368 5d2c  ize: ([n_batch],
+00016570: 207b 6e5f 6368 616e 6e65 6c7d 2c20 6e40   {n_channel}, n@
+00016580: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
+00016590: 5f64 696d 290a 2020 2020 2020 2020 2727  _dim).        ''
+000165a0: 270a 2020 2020 2020 2020 6966 206c 656e  '.        if len
+000165b0: 285f 7261 6e67 6529 203d 3d20 303a 205f  (_range) == 0: _
+000165c0: 7261 6e67 6520 3d20 4e6f 6e65 0a20 2020  range = None.   
+000165d0: 2020 2020 2065 6c69 6620 6c65 6e28 5f72       elif len(_r
+000165e0: 616e 6765 2920 3d3d 2031 2061 6e64 2069  ange) == 1 and i
+000165f0: 7369 6e73 7461 6e63 6528 5f72 616e 6765  sinstance(_range
+00016600: 5b30 5d2c 2028 6c69 7374 2c20 7475 706c  [0], (list, tupl
+00016610: 6529 293a 205f 7261 6e67 6520 3d20 6261  e)): _range = ba
+00016620: 746f 7263 685f 7465 6e73 6f72 286c 6973  torch_tensor(lis
+00016630: 7428 5f72 616e 6765 5b30 5d29 290a 2020  t(_range[0])).  
+00016640: 2020 2020 2020 656c 6966 206c 656e 285f        elif len(_
+00016650: 7261 6e67 6529 203d 3d20 3120 616e 6420  range) == 1 and 
+00016660: 6973 696e 7374 616e 6365 285f 7261 6e67  isinstance(_rang
+00016670: 655b 305d 2c20 6274 2e54 656e 736f 7229  e[0], bt.Tensor)
+00016680: 3a20 5f72 616e 6765 203d 205f 7261 6e67  : _range = _rang
+00016690: 655b 305d 0a20 2020 2020 2020 2065 6c69  e[0].        eli
+000166a0: 6620 6c65 6e28 5f72 616e 6765 2920 3d3d  f len(_range) ==
+000166b0: 2031 3a20 5f72 616e 6765 203d 2062 742e   1: _range = bt.
+000166c0: 6368 616e 6e65 6c5f 7465 6e73 6f72 2828  channel_tensor((
+000166d0: 302c 205f 7261 6e67 6529 290a 2020 2020  0, _range)).    
+000166e0: 2020 2020 656c 6966 206c 656e 285f 7261      elif len(_ra
+000166f0: 6e67 6529 203d 3d20 323a 205f 7261 6e67  nge) == 2: _rang
+00016700: 6520 3d20 6274 2e63 6861 6e6e 656c 5f74  e = bt.channel_t
+00016710: 656e 736f 7228 5f72 616e 6765 290a 2020  ensor(_range).  
+00016720: 2020 2020 2020 656c 7365 3a20 7261 6973        else: rais
+00016730: 6520 5479 7065 4572 726f 7228 6622 496e  e TypeError(f"In
+00016740: 7661 6c69 6420 7261 6e67 6520 666f 7220  valid range for 
+00016750: 4e6f 726d 616c 697a 653a 207b 5f72 616e  Normalize: {_ran
+00016760: 6765 7d2e 2022 290a 2020 2020 2020 2020  ge}. ").        
+00016770: 6966 205f 7261 6e67 6520 6973 204e 6f6e  if _range is Non
+00016780: 653a 2070 6173 730a 2020 2020 2020 2020  e: pass.        
+00016790: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000167a0: 2020 6966 205f 7261 6e67 652e 6e5f 6469    if _range.n_di
+000167b0: 6d20 3c20 323a 205f 7261 6e67 6520 3d20  m < 2: _range = 
+000167c0: 5f72 616e 6765 2e75 6e73 7175 6565 7a65  _range.unsqueeze
+000167d0: 285b 5d29 0a20 2020 2020 2020 2020 2020  ([]).           
+000167e0: 2069 6620 6e6f 7420 5f72 616e 6765 2e68   if not _range.h
+000167f0: 6173 5f62 6174 6368 3a20 5f72 616e 6765  as_batch: _range
+00016800: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
+00016810: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
+00016820: 2069 6620 6e6f 7420 5f72 616e 6765 2e68   if not _range.h
+00016830: 6173 5f63 6861 6e6e 656c 3a20 5f72 616e  as_channel: _ran
+00016840: 6765 2e63 6861 6e6e 656c 5f64 696d 656e  ge.channel_dimen
+00016850: 7369 6f6e 203d 2031 0a20 2020 2020 2020  sion = 1.       
+00016860: 2020 2020 2061 766f 7563 6828 5f72 616e       avouch(_ran
+00016870: 6765 2e68 6173 5f62 6174 6368 2061 6e64  ge.has_batch and
+00016880: 205f 7261 6e67 652e 6861 735f 6368 616e   _range.has_chan
+00016890: 6e65 6c2c 2066 2250 6c65 6173 6520 7573  nel, f"Please us
+000168a0: 6520 6261 746f 7263 6820 7465 6e73 6f72  e batorch tensor
+000168b0: 206f 6620 7369 7a65 205c 0a20 2020 2020   of size \.     
+000168c0: 2020 2020 2020 2020 2020 2028 5b6e 5f62             ([n_b
+000168d0: 6174 6368 3a6f 7074 696f 6e61 6c5d 2c20  atch:optional], 
+000168e0: 7b7b 327d 7d29 2066 6f72 204e 6f72 6d61  {{2}}) for Norma
+000168f0: 6c69 7a69 6e67 2070 6172 616d 6574 6572  lizing parameter
+00016900: 732c 2069 6e73 7465 6164 206f 6620 7b5f  s, instead of {_
+00016910: 7261 6e67 652e 7368 6170 657d 2e20 2229  range.shape}. ")
+00016920: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+00016930: 2e5f 5f69 6e69 745f 5f28 5f72 616e 6765  .__init__(_range
+00016940: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+00016950: 616e 6765 203d 205f 7261 6e67 650a 2020  ange = _range.  
+00016960: 2020 2020 2020 7365 6c66 2e5f 7261 6e67        self._rang
+00016970: 6520 3d20 4e6f 6e65 0a0a 2020 2020 6465  e = None..    de
+00016980: 6620 5f5f 6361 6c6c 5f5f 2873 656c 662c  f __call__(self,
+00016990: 2058 293a 0a20 2020 2020 2020 2058 203d   X):.        X =
+000169a0: 2073 7570 6572 2829 2e5f 5f63 616c 6c5f   super().__call_
+000169b0: 5f28 5829 0a20 2020 2020 2020 205f 7261  _(X).        _ra
+000169c0: 6e67 6520 3d20 7365 6c66 2e72 616e 6765  nge = self.range
+000169d0: 0a20 2020 2020 2020 2069 6620 5f72 616e  .        if _ran
+000169e0: 6765 2069 7320 4e6f 6e65 3a0a 2020 2020  ge is None:.    
+000169f0: 2020 2020 2020 2020 5f72 616e 6765 203d          _range =
+00016a00: 2062 742e 7175 616e 7469 6c65 2858 2e66   bt.quantile(X.f
+00016a10: 6c61 7474 656e 2829 2e66 6c6f 6174 2829  latten().float()
+00016a20: 2c20 6261 746f 7263 685f 7465 6e73 6f72  , batorch_tensor
+00016a30: 285b 302e 3032 352c 2030 2e39 3735 5d29  ([0.025, 0.975])
+00016a40: 2c20 6178 6973 3d2d 3129 2e6d 6f76 6564  , axis=-1).moved
+00016a50: 696d 2830 2c20 2d31 292e 7370 6563 6961  im(0, -1).specia
+00016a60: 6c5f 6672 6f6d 5f28 5829 0a20 2020 2020  l_from_(X).     
+00016a70: 2020 2020 2020 2073 656c 662e 5f72 616e         self._ran
+00016a80: 6765 203d 205f 7261 6e67 650a 2020 2020  ge = _range.    
+00016a90: 2020 2020 7265 7475 726e 2028 2858 202d      return ((X -
+00016aa0: 205f 7261 6e67 655b 2e2e 2e2c 2030 5d29   _range[..., 0])
+00016ab0: 202f 2028 5f72 616e 6765 5b2e 2e2e 2c20   / (_range[..., 
+00016ac0: 315d 202d 205f 7261 6e67 655b 2e2e 2e2c  1] - _range[...,
+00016ad0: 2030 5d29 292e 636c 616d 7028 302e 2c20   0])).clamp(0., 
+00016ae0: 312e 290a 2020 2020 0a20 2020 2064 6566  1.).    .    def
+00016af0: 2069 6e76 2873 656c 6629 3a0a 2020 2020   inv(self):.    
+00016b00: 2020 2020 6966 2073 656c 662e 7261 6e67      if self.rang
+00016b10: 6520 6973 206e 6f74 204e 6f6e 653a 205f  e is not None: _
+00016b20: 7261 6e67 6520 3d20 7365 6c66 2e72 616e  range = self.ran
+00016b30: 6765 0a20 2020 2020 2020 2065 6c69 6620  ge.        elif 
+00016b40: 7365 6c66 2e5f 7261 6e67 6520 6973 206e  self._range is n
+00016b50: 6f74 204e 6f6e 653a 205f 7261 6e67 6520  ot None: _range 
+00016b60: 3d20 7365 6c66 2e5f 7261 6e67 650a 2020  = self._range.  
+00016b70: 2020 2020 2020 656c 7365 3a20 7265 7475        else: retu
+00016b80: 726e 204e 6f72 6d61 6c69 7a65 284e 6f6e  rn Normalize(Non
+00016b90: 6529 0a20 2020 2020 2020 2064 656e 203d  e).        den =
+00016ba0: 205f 7261 6e67 655b 2e2e 2e2c 2031 5d20   _range[..., 1] 
+00016bb0: 2d20 5f72 616e 6765 5b2e 2e2e 2c20 305d  - _range[..., 0]
+00016bc0: 0a20 2020 2020 2020 205f 7261 6e67 6520  .        _range 
+00016bd0: 3d20 6274 2e73 7461 636b 282d 5f72 616e  = bt.stack(-_ran
+00016be0: 6765 5b2e 2e2e 2c20 305d 2c20 312d 5f72  ge[..., 0], 1-_r
+00016bf0: 616e 6765 5b2e 2e2e 2c20 305d 2c20 2d31  ange[..., 0], -1
+00016c00: 2920 2f20 6465 6e0a 2020 2020 2020 2020  ) / den.        
+00016c10: 7265 7475 726e 204e 6f72 6d61 6c69 7a65  return Normalize
+00016c20: 285f 7261 6e67 6529 0a0a 2323 2323 2323  (_range)..######
+00016c30: 2323 2323 2323 2320 5375 7070 6f72 7469  ####### Supporti
+00016c40: 6e67 2046 756e 6374 696f 6e73 2023 2323  ng Functions ###
+00016c50: 2323 2323 2323 2323 230a 0a64 6566 2042  #########..def B
+00016c60: 7370 6c69 6e65 2869 2c20 5529 3a0a 2020  spline(i, U):.  
+00016c70: 2020 2222 220a 2020 2020 4375 6269 6320    """.    Cubic 
+00016c80: 422d 7370 6c69 6e65 2066 756e 6374 696f  B-spline functio
+00016c90: 6e2e 200a 2020 2020 4e6f 7465 3a20 4173  n. .    Note: As
+00016ca0: 206c 6f6e 6720 6173 2069 2061 6e64 2055   long as i and U
+00016cb0: 2068 6176 6520 7468 6520 7361 6d65 2073   have the same s
+00016cc0: 697a 652c 2061 6e79 2073 6861 7065 206f  ize, any shape o
+00016cd0: 6620 7465 6e73 6f72 7320 776f 756c 6420  f tensors would 
+00016ce0: 646f 2e0a 2020 2020 0a20 2020 2050 6172  do..    .    Par
+00016cf0: 616d 733a 0a20 2020 2020 2020 2069 205b  ams:.        i [
+00016d00: 6274 2e54 656e 736f 725d 3a20 7468 6520  bt.Tensor]: the 
+00016d10: 696e 6465 7820 6f66 2073 6567 6d65 6e74  index of segment
+00016d20: 2066 756e 6374 696f 6e20 6f66 2042 2d73   function of B-s
+00016d30: 706c 696e 652e 0a20 2020 2020 2020 2020  pline..         
+00016d40: 2020 2054 6865 2076 616c 7565 206f 6620     The value of 
+00016d50: 6561 6368 2065 6c65 6d65 6e74 2063 616e  each element can
+00016d60: 2062 6520 6368 6f73 656e 2069 6e20 282d   be chosen in (-
+00016d70: 312c 2030 2c20 312c 2032 292e 200a 2020  1, 0, 1, 2). .  
+00016d80: 2020 2020 2020 5520 5b62 742e 5465 6e73        U [bt.Tens
+00016d90: 6f72 5d3a 2074 6865 2064 6563 696d 616c  or]: the decimal
+00016da0: 2061 7267 756d 656e 7420 6f66 2042 2d73   argument of B-s
+00016db0: 706c 696e 6520 6675 6e63 7469 6f6e 2e20  pline function. 
+00016dc0: 4974 2073 686f 756c 6420 6265 2077 6974  It should be wit
+00016dd0: 6869 6e20 7261 6e67 6520 5b30 2c20 3129  hin range [0, 1)
+00016de0: 2e0a 2020 2020 2222 220a 2020 2020 6920  ..    """.    i 
+00016df0: 3d20 6261 746f 7263 685f 7465 6e73 6f72  = batorch_tensor
+00016e00: 2869 293b 2055 203d 2062 6174 6f72 6368  (i); U = batorch
+00016e10: 5f74 656e 736f 7228 5529 0a20 2020 2072  _tensor(U).    r
+00016e20: 6574 7572 6e20 280a 2020 2020 2020 2020  eturn (.        
+00016e30: 6274 2e77 6865 7265 2869 203d 3d20 2d31  bt.where(i == -1
+00016e40: 2c20 2831 202d 2055 2920 2a2a 2033 202f  , (1 - U) ** 3 /
+00016e50: 2036 2c0a 2020 2020 2020 2020 6274 2e77   6,.        bt.w
+00016e60: 6865 7265 2869 203d 3d20 302c 2055 202a  here(i == 0, U *
+00016e70: 2a20 3320 2f20 3220 2d20 5520 2a20 5520  * 3 / 2 - U * U 
+00016e80: 2b20 3220 2f20 332c 0a20 2020 2020 2020  + 2 / 3,.       
+00016e90: 2062 742e 7768 6572 6528 6920 3d3d 2031   bt.where(i == 1
+00016ea0: 2c20 282d 2033 202a 2055 202a 2a20 3320  , (- 3 * U ** 3 
+00016eb0: 2b20 3320 2a20 5520 2a20 5520 2b20 3320  + 3 * U * U + 3 
+00016ec0: 2a20 5520 2b20 3129 202f 2036 2c0a 2020  * U + 1) / 6,.  
+00016ed0: 2020 2020 2020 6274 2e77 6865 7265 2869        bt.where(i
+00016ee0: 203d 3d20 322c 2055 202a 2a20 3320 2f20   == 2, U ** 3 / 
+00016ef0: 362c 0a20 2020 2020 2020 2062 742e 7a65  6,.        bt.ze
+00016f00: 726f 735f 6c69 6b65 2855 2929 2929 290a  ros_like(U))))).
+00016f10: 2020 2020 290a 0a64 6566 2064 4273 706c      )..def dBspl
+00016f20: 696e 6528 692c 2055 293a 0a20 2020 2022  ine(i, U):.    "
+00016f30: 2222 0a20 2020 2054 6865 2064 6572 6976  "".    The deriv
+00016f40: 6174 6976 6520 6f66 2042 2d73 706c 696e  ative of B-splin
+00016f50: 6520 6675 6e63 7469 6f6e 2c20 7769 7468  e function, with
+00016f60: 2072 6573 7065 6374 2074 6f20 552e 200a   respect to U. .
+00016f70: 2020 2020 4e6f 7465 3a20 4173 206c 6f6e      Note: As lon
+00016f80: 6720 6173 2069 2061 6e64 2055 2068 6176  g as i and U hav
+00016f90: 6520 7468 6520 7361 6d65 2073 697a 652c  e the same size,
+00016fa0: 2061 6e79 2073 6861 7065 206f 6620 7465   any shape of te
+00016fb0: 6e73 6f72 7320 776f 756c 6420 646f 2e0a  nsors would do..
+00016fc0: 2020 2020 0a20 2020 2050 6172 616d 733a      .    Params:
+00016fd0: 0a20 2020 2020 2020 2069 205b 6274 2e54  .        i [bt.T
+00016fe0: 656e 736f 725d 3a20 7468 6520 696e 6465  ensor]: the inde
+00016ff0: 7820 6f66 2073 6567 6d65 6e74 2066 756e  x of segment fun
+00017000: 6374 696f 6e20 6f66 2042 2d73 706c 696e  ction of B-splin
+00017010: 652e 0a20 2020 2020 2020 2020 2020 2054  e..            T
+00017020: 6865 2076 616c 7565 206f 6620 6561 6368  he value of each
+00017030: 2065 6c65 6d65 6e74 2063 616e 2062 6520   element can be 
+00017040: 6368 6f73 656e 2069 6e20 282d 312c 2030  chosen in (-1, 0
+00017050: 2c20 312c 2032 292e 200a 2020 2020 2020  , 1, 2). .      
+00017060: 2020 5520 5b62 742e 5465 6e73 6f72 5d3a    U [bt.Tensor]:
+00017070: 2074 6865 2064 6563 696d 616c 2061 7267   the decimal arg
+00017080: 756d 656e 7420 6f66 2042 2d73 706c 696e  ument of B-splin
+00017090: 6520 6675 6e63 7469 6f6e 2e20 4974 2073  e function. It s
+000170a0: 686f 756c 6420 6265 2077 6974 6869 6e20  hould be within 
+000170b0: 7261 6e67 6520 5b30 2c20 3129 2e0a 2020  range [0, 1)..  
+000170c0: 2020 2222 220a 2020 2020 6920 3d20 6261    """.    i = ba
+000170d0: 746f 7263 685f 7465 6e73 6f72 2869 293b  torch_tensor(i);
+000170e0: 2055 203d 2062 6174 6f72 6368 5f74 656e   U = batorch_ten
+000170f0: 736f 7228 5529 0a20 2020 2072 6574 7572  sor(U).    retur
+00017100: 6e20 280a 2020 2020 2020 2020 6274 2e77  n (.        bt.w
+00017110: 6865 7265 2869 203d 3d20 2d31 2c20 2d20  here(i == -1, - 
+00017120: 3320 2a20 2831 202d 2055 2920 2a2a 2032  3 * (1 - U) ** 2
+00017130: 202f 2036 2c0a 2020 2020 2020 2020 6274   / 6,.        bt
+00017140: 2e77 6865 7265 2869 203d 3d20 302c 2033  .where(i == 0, 3
+00017150: 202a 2055 202a 2a20 3220 2f20 3220 2d20   * U ** 2 / 2 - 
+00017160: 3220 2a20 552c 0a20 2020 2020 2020 2062  2 * U,.        b
+00017170: 742e 7768 6572 6528 6920 3d3d 2031 2c20  t.where(i == 1, 
+00017180: 282d 2033 202a 2055 202a 2a20 3220 2b20  (- 3 * U ** 2 + 
+00017190: 3220 2a20 5520 2b20 3129 202f 2032 2c0a  2 * U + 1) / 2,.
+000171a0: 2020 2020 2020 2020 6274 2e77 6865 7265          bt.where
+000171b0: 2869 203d 3d20 322c 2033 202a 2055 202a  (i == 2, 3 * U *
+000171c0: 2a20 3220 2f20 362c 0a20 2020 2020 2020  * 2 / 6,.       
+000171d0: 2062 742e 7a65 726f 735f 6c69 6b65 2855   bt.zeros_like(U
+000171e0: 2929 2929 290a 2020 2020 290a 0a64 6566  ))))).    )..def
+000171f0: 2066 4273 706c 696e 6528 632c 2078 293a   fBspline(c, x):
+00017200: 0a20 2020 2063 203d 2062 6174 6f72 6368  .    c = batorch
+00017210: 5f74 656e 736f 7228 6329 3b20 7820 3d20  _tensor(c); x = 
+00017220: 6261 746f 7263 685f 7465 6e73 6f72 2878  batorch_tensor(x
+00017230: 290a 2020 2020 6420 3d20 7820 2d20 630a  ).    d = x - c.
+00017240: 2020 2020 7265 7475 726e 2028 0a20 2020      return (.   
+00017250: 2020 2020 2062 742e 7768 6572 6528 282d       bt.where((-
+00017260: 3220 3c3d 2064 2920 2a20 2864 203c 202d  2 <= d) * (d < -
+00017270: 3129 2c20 6420 2a2a 2033 202b 2036 202a  1), d ** 3 + 6 *
+00017280: 2064 202a 2a20 3220 2b20 3132 202a 2064   d ** 2 + 12 * d
+00017290: 202b 2038 2c0a 2020 2020 2020 2020 6274   + 8,.        bt
+000172a0: 2e77 6865 7265 2828 2d31 203c 3d20 6429  .where((-1 <= d)
+000172b0: 202a 2028 6420 3c20 3029 2c20 2d20 3320   * (d < 0), - 3 
+000172c0: 2a20 6420 2a2a 2033 202d 2036 202a 2064  * d ** 3 - 6 * d
+000172d0: 202a 2a20 3220 2b20 342c 0a20 2020 2020   ** 2 + 4,.     
+000172e0: 2020 2062 742e 7768 6572 6528 2830 203c     bt.where((0 <
+000172f0: 3d20 6429 202a 2028 6420 3c20 3129 2c20  = d) * (d < 1), 
+00017300: 3320 2a20 6420 2a2a 2033 202d 2036 202a  3 * d ** 3 - 6 *
+00017310: 2064 202a 2a20 3220 2b20 342c 0a20 2020   d ** 2 + 4,.   
+00017320: 2020 2020 2062 742e 7768 6572 6528 2831       bt.where((1
+00017330: 203c 3d20 6429 202a 2028 6420 3c20 3229   <= d) * (d < 2)
+00017340: 2c20 2d20 6420 2a2a 2033 202b 2036 202a  , - d ** 3 + 6 *
+00017350: 2064 202a 2a20 3220 2d20 3132 202a 2064   d ** 2 - 12 * d
+00017360: 202b 2038 2c0a 2020 2020 2020 2020 6274   + 8,.        bt
+00017370: 2e7a 6572 6f73 5f6c 696b 6528 6429 2929  .zeros_like(d)))
+00017380: 2929 202f 2036 0a20 2020 2029 0a0a 6465  )) / 6.    )..de
+00017390: 6620 4166 6669 6e65 3244 324d 6174 7269  f Affine2D2Matri
+000173a0: 7828 7061 7261 6d73 293a 0a20 2020 2022  x(params):.    "
+000173b0: 2222 0a20 2020 2074 312c 2074 322c 20ce  "".    t1, t2, .
+000173c0: b82c 2073 312c 2073 322c 20cf 8131 2c20  ., s1, s2, ..1, 
+000173d0: cf81 3220 696e 2073 697a 653a 2028 5b6e  ..2 in size: ([n
+000173e0: 5f62 6174 6368 5d2c 207b 377d 290a 2020  _batch], {7}).  
+000173f0: 2020 7431 2c20 7432 2c20 6331 2c20 6332    t1, t2, c1, c2
+00017400: 2c20 ceb8 2c20 7331 2c20 7332 2c20 cf81  , .., s1, s2, ..
+00017410: 312c 20cf 8132 2069 6e20 7369 7a65 3a20  1, ..2 in size: 
+00017420: 285b 6e5f 6261 7463 685d 2c20 7b39 7d29  ([n_batch], {9})
+00017430: 0a20 2020 206f 7574 7075 7420 696e 2073  .    output in s
+00017440: 697a 653a 2028 5b6e 5f62 6174 6368 5d2c  ize: ([n_batch],
+00017450: 2033 2c20 3329 0a20 2020 2022 2222 0a20   3, 3).    """. 
+00017460: 2020 2070 6172 616d 7320 3d20 6261 746f     params = bato
+00017470: 7263 685f 7465 6e73 6f72 2870 6172 616d  rch_tensor(param
+00017480: 7329 0a20 2020 2069 6620 7061 7261 6d73  s).    if params
+00017490: 2e6e 5f64 696d 203c 3d20 3120 616e 6420  .n_dim <= 1 and 
+000174a0: 6e6f 7420 7061 7261 6d73 2e68 6173 5f62  not params.has_b
+000174b0: 6174 6368 3a20 7061 7261 6d73 203d 2070  atch: params = p
+000174c0: 6172 616d 732e 756e 7371 7565 657a 6528  arams.unsqueeze(
+000174d0: 5b5d 290a 2020 2020 6966 2070 6172 616d  []).    if param
+000174e0: 732e 6e5f 6469 6d20 3c3d 2031 2061 6e64  s.n_dim <= 1 and
+000174f0: 206e 6f74 2070 6172 616d 732e 6861 735f   not params.has_
+00017500: 6368 616e 6e65 6c3a 2070 6172 616d 7320  channel: params 
+00017510: 3d20 7061 7261 6d73 2e75 6e73 7175 6565  = params.unsquee
+00017520: 7a65 287b 317d 290a 2020 2020 6966 2070  ze({1}).    if p
+00017530: 6172 616d 732e 6e5f 6469 6d20 3d3d 2032  arams.n_dim == 2
+00017540: 2061 6e64 206e 6f74 2070 6172 616d 732e   and not params.
+00017550: 6861 735f 6261 7463 683a 2070 6172 616d  has_batch: param
+00017560: 732e 6261 7463 685f 6469 6d65 6e73 696f  s.batch_dimensio
+00017570: 6e20 3d20 300a 2020 2020 6966 2070 6172  n = 0.    if par
+00017580: 616d 732e 6e5f 6469 6d20 3d3d 2032 2061  ams.n_dim == 2 a
+00017590: 6e64 206e 6f74 2070 6172 616d 732e 6861  nd not params.ha
+000175a0: 735f 6368 616e 6e65 6c3a 2070 6172 616d  s_channel: param
+000175b0: 732e 6368 616e 6e65 6c5f 6469 6d65 6e73  s.channel_dimens
+000175c0: 696f 6e20 3d20 310a 2020 2020 6176 6f75  ion = 1.    avou
+000175d0: 6368 2870 6172 616d 732e 6861 735f 6261  ch(params.has_ba
+000175e0: 7463 682c 2066 2250 6c65 6173 6520 7573  tch, f"Please us
+000175f0: 6520 6261 746f 7263 6820 7465 6e73 6f72  e batorch tensor
+00017600: 206f 6620 7369 7a65 2028 5b6e 5f62 6174   of size ([n_bat
+00017610: 6368 5d2c 207b 3720 6f72 2039 7d29 205c  ch], {7 or 9}) \
+00017620: 0a20 2020 2020 2020 2066 6f72 2041 6666  .        for Aff
+00017630: 696e 6520 7061 7261 6d65 7465 7273 2c20  ine parameters, 
+00017640: 696e 7374 6561 6420 6f66 207b 7061 7261  instead of {para
+00017650: 6d73 2e73 6861 7065 7d2e 2022 290a 2020  ms.shape}. ").  
+00017660: 2020 6e5f 6261 7463 6820 3d20 7061 7261    n_batch = para
+00017670: 6d73 2e6e 5f62 6174 6368 0a20 2020 2069  ms.n_batch.    i
+00017680: 6620 7061 7261 6d73 2e73 697a 6528 3129  f params.size(1)
+00017690: 203d 3d20 373a 0a20 2020 2020 2020 2074   == 7:.        t
+000176a0: 312c 2074 322c 20ce b82c 2073 312c 2073  1, t2, .., s1, s
+000176b0: 322c 20cf 8131 2c20 cf81 3220 3d20 7061  2, ..1, ..2 = pa
+000176c0: 7261 6d73 2e73 706c 6974 2829 0a20 2020  rams.split().   
+000176d0: 2020 2020 2063 3120 3d20 6274 2e7a 6572       c1 = bt.zer
+000176e0: 6f73 285b 6e5f 6261 7463 685d 2c20 3129  os([n_batch], 1)
+000176f0: 3b20 6332 203d 2062 742e 7a65 726f 7328  ; c2 = bt.zeros(
+00017700: 5b6e 5f62 6174 6368 5d2c 2031 290a 2020  [n_batch], 1).  
+00017710: 2020 6966 2070 6172 616d 732e 7369 7a65    if params.size
+00017720: 2831 2920 3d3d 2039 3a0a 2020 2020 2020  (1) == 9:.      
+00017730: 2020 7431 2c20 7432 2c20 6331 2c20 6332    t1, t2, c1, c2
+00017740: 2c20 ceb8 2c20 7331 2c20 7332 2c20 cf81  , .., s1, s2, ..
+00017750: 312c 20cf 8132 203d 2070 6172 616d 732e  1, ..2 = params.
+00017760: 7370 6c69 7428 290a 2020 2020 6120 3d20  split().    a = 
+00017770: 28cf 8131 202a 20cf 8132 202b 2031 2920  (..1 * ..2 + 1) 
+00017780: 2a20 7331 202a 2062 742e 636f 7328 ceb8  * s1 * bt.cos(..
+00017790: 2920 2b20 cf81 3120 2a20 7332 202a 2062  ) + ..1 * s2 * b
+000177a0: 742e 7369 6e28 ceb8 290a 2020 2020 6220  t.sin(..).    b 
+000177b0: 3d20 2d20 28cf 8131 202a 20cf 8132 202b  = - (..1 * ..2 +
+000177c0: 2031 2920 2a20 7331 202a 2062 742e 7369   1) * s1 * bt.si
+000177d0: 6e28 ceb8 2920 2b20 cf81 3120 2a20 7332  n(..) + ..1 * s2
+000177e0: 202a 2062 742e 636f 7328 ceb8 290a 2020   * bt.cos(..).  
+000177f0: 2020 6320 3d20 cf81 3220 2a20 7331 202a    c = ..2 * s1 *
+00017800: 2062 742e 636f 7328 ceb8 2920 2b20 7332   bt.cos(..) + s2
+00017810: 202a 2062 742e 7369 6e28 ceb8 290a 2020   * bt.sin(..).  
+00017820: 2020 6420 3d20 2d20 cf81 3220 2a20 7331    d = - ..2 * s1
+00017830: 202a 2062 742e 7369 6e28 ceb8 2920 2b20   * bt.sin(..) + 
+00017840: 7332 202a 2062 742e 636f 7328 ceb8 290a  s2 * bt.cos(..).
+00017850: 2020 2020 7265 7475 726e 2062 742e 6361      return bt.ca
+00017860: 7428 0a20 2020 2020 2020 2062 742e 6361  t(.        bt.ca
+00017870: 7428 2861 2c20 622c 2074 3120 2d20 6120  t((a, b, t1 - a 
+00017880: 2a20 6331 202d 2062 202a 2063 3220 2b20  * c1 - b * c2 + 
+00017890: 6331 2c20 632c 2064 2c20 7432 202d 2063  c1, c, d, t2 - c
+000178a0: 202a 2063 3120 2d20 6420 2a20 6332 202b   * c1 - d * c2 +
+000178b0: 2063 3229 2c20 7b7d 292e 7669 6577 285b   c2), {}).view([
+000178c0: 6e5f 6261 7463 685d 2c20 322c 2033 292c  n_batch], 2, 3),
+000178d0: 200a 2020 2020 2020 2020 6274 2e6f 6e65   .        bt.one
+000178e0: 5f68 6f74 282d 312c 2033 292e 6d75 6c74  _hot(-1, 3).mult
+000178f0: 6970 6c79 286e 5f62 6174 6368 2c20 5b5d  iply(n_batch, []
+00017900: 292e 7669 6577 285b 6e5f 6261 7463 685d  ).view([n_batch]
+00017910: 2c20 312c 2033 292c 2031 0a20 2020 2029  , 1, 3), 1.    )
+00017920: 0a0a 6465 6620 5175 6174 6572 6e73 324d  ..def Quaterns2M
+00017930: 6174 7269 7828 7061 7261 6d73 293a 0a20  atrix(params):. 
+00017940: 2020 2022 2222 0a20 2020 2020 2020 2051     """.        Q
+00017950: 7561 7465 726e 3a20 7162 2c20 7163 2c20  uatern: qb, qc, 
+00017960: 7164 2c20 7078 2c20 7079 2c20 707a 2069  qd, px, py, pz i
+00017970: 6e20 7369 7a65 3a20 285b 6e5f 6261 7463  n size: ([n_batc
+00017980: 685d 2c20 7b36 7d29 0a20 2020 2020 2020  h], {6}).       
+00017990: 204d 6174 7269 783a 2028 5b6e 5f62 6174   Matrix: ([n_bat
+000179a0: 6368 5d2c 2034 2c20 3429 0a20 2020 2022  ch], 4, 4).    "
+000179b0: 2222 0a20 2020 2070 6172 616d 7320 3d20  "".    params = 
+000179c0: 6261 746f 7263 685f 7465 6e73 6f72 2870  batorch_tensor(p
+000179d0: 6172 616d 7329 0a20 2020 2069 6620 7061  arams).    if pa
+000179e0: 7261 6d73 2e6e 5f64 696d 203c 3d20 3120  rams.n_dim <= 1 
+000179f0: 616e 6420 6e6f 7420 7061 7261 6d73 2e68  and not params.h
+00017a00: 6173 5f62 6174 6368 3a20 7061 7261 6d73  as_batch: params
+00017a10: 203d 2070 6172 616d 732e 756e 7371 7565   = params.unsque
+00017a20: 657a 6528 5b5d 290a 2020 2020 6966 2070  eze([]).    if p
+00017a30: 6172 616d 732e 6e5f 6469 6d20 3c3d 2031  arams.n_dim <= 1
+00017a40: 2061 6e64 206e 6f74 2070 6172 616d 732e   and not params.
+00017a50: 6861 735f 6368 616e 6e65 6c3a 2070 6172  has_channel: par
+00017a60: 616d 7320 3d20 7061 7261 6d73 2e75 6e73  ams = params.uns
+00017a70: 7175 6565 7a65 287b 317d 290a 2020 2020  queeze({1}).    
+00017a80: 6966 2070 6172 616d 732e 6e5f 6469 6d20  if params.n_dim 
+00017a90: 3d3d 2032 2061 6e64 206e 6f74 2070 6172  == 2 and not par
+00017aa0: 616d 732e 6861 735f 6261 7463 683a 2070  ams.has_batch: p
+00017ab0: 6172 616d 732e 6261 7463 685f 6469 6d65  arams.batch_dime
+00017ac0: 6e73 696f 6e20 3d20 300a 2020 2020 6966  nsion = 0.    if
+00017ad0: 2070 6172 616d 732e 6e5f 6469 6d20 3d3d   params.n_dim ==
+00017ae0: 2032 2061 6e64 206e 6f74 2070 6172 616d   2 and not param
+00017af0: 732e 6861 735f 6368 616e 6e65 6c3a 2070  s.has_channel: p
+00017b00: 6172 616d 732e 6368 616e 6e65 6c5f 6469  arams.channel_di
+00017b10: 6d65 6e73 696f 6e20 3d20 310a 2020 2020  mension = 1.    
+00017b20: 6176 6f75 6368 2870 6172 616d 732e 6e5f  avouch(params.n_
+00017b30: 6469 6d20 3d3d 2032 2061 6e64 2070 6172  dim == 2 and par
+00017b40: 616d 732e 6861 735f 6261 7463 6820 616e  ams.has_batch an
+00017b50: 6420 7061 7261 6d73 2e68 6173 5f63 6861  d params.has_cha
+00017b60: 6e6e 656c 2c20 0a20 2020 2020 2020 2020  nnel, .         
+00017b70: 2020 6622 506c 6561 7365 2075 7365 2062    f"Please use b
+00017b80: 6174 6f72 6368 2074 656e 736f 7220 6f66  atorch tensor of
+00017b90: 2073 697a 6520 285b 6e5f 6261 7463 685d   size ([n_batch]
+00017ba0: 2c20 7b7b 367d 7d29 2066 6f72 2041 6666  , {{6}}) for Aff
+00017bb0: 696e 6520 7061 7261 6d65 7465 7273 2c20  ine parameters, 
+00017bc0: 696e 7374 6561 6420 6f66 207b 7061 7261  instead of {para
+00017bd0: 6d73 2e73 6861 7065 7d2e 2022 290a 2020  ms.shape}. ").  
+00017be0: 2020 6e5f 6261 7463 6820 3d20 7061 7261    n_batch = para
+00017bf0: 6d73 2e6e 5f62 6174 6368 0a20 2020 2062  ms.n_batch.    b
+00017c00: 2c20 632c 2064 2c20 782c 2079 2c20 7a20  , c, d, x, y, z 
+00017c10: 3d20 7061 7261 6d73 2e73 706c 6974 2829  = params.split()
+00017c20: 0a20 2020 2061 203d 2062 742e 7371 7274  .    a = bt.sqrt
+00017c30: 2828 312d 622a 622d 632a 632d 642a 6429  ((1-b*b-c*c-d*d)
+00017c40: 2e63 6c61 6d70 2830 2929 0a20 2020 2052  .clamp(0)).    R
+00017c50: 3131 203d 2061 2a61 2b62 2a62 2d63 2a63  11 = a*a+b*b-c*c
+00017c60: 2d64 2a64 0a20 2020 2052 3132 203d 2032  -d*d.    R12 = 2
+00017c70: 2a62 2a63 2d32 2a61 2a64 0a20 2020 2052  *b*c-2*a*d.    R
+00017c80: 3133 203d 2032 2a62 2a64 2b32 2a61 2a63  13 = 2*b*d+2*a*c
+00017c90: 0a20 2020 2052 3231 203d 2032 2a62 2a63  .    R21 = 2*b*c
+00017ca0: 2b32 2a61 2a64 0a20 2020 2052 3232 203d  +2*a*d.    R22 =
+00017cb0: 2061 2a61 2b63 2a63 2d62 2a62 2d64 2a64   a*a+c*c-b*b-d*d
+00017cc0: 0a20 2020 2052 3233 203d 2032 2a63 2a64  .    R23 = 2*c*d
+00017cd0: 2d32 2a61 2a62 0a20 2020 2052 3331 203d  -2*a*b.    R31 =
+00017ce0: 2032 2a62 2a64 2d32 2a61 2a63 0a20 2020   2*b*d-2*a*c.   
+00017cf0: 2052 3332 203d 2032 2a63 2a64 2b32 2a61   R32 = 2*c*d+2*a
+00017d00: 2a62 0a20 2020 2052 3333 203d 2061 2a61  *b.    R33 = a*a
+00017d10: 2b64 2a64 2d63 2a63 2d62 2a62 0a20 2020  +d*d-c*c-b*b.   
+00017d20: 2072 6574 7572 6e20 6274 2e63 6174 280a   return bt.cat(.
+00017d30: 2020 2020 2020 2020 6274 2e63 6174 2828          bt.cat((
+00017d40: 5231 312c 2052 3132 2c20 5231 332c 2078  R11, R12, R13, x
+00017d50: 2c20 5232 312c 2052 3232 2c20 5232 332c  , R21, R22, R23,
+00017d60: 2079 2c20 5233 312c 2052 3332 2c20 5233   y, R31, R32, R3
+00017d70: 332c 207a 292c 2031 292e 7669 6577 285b  3, z), 1).view([
+00017d80: 6e5f 6261 7463 685d 2c20 332c 2034 292c  n_batch], 3, 4),
+00017d90: 0a20 2020 2020 2020 2062 742e 6f6e 655f  .        bt.one_
+00017da0: 686f 7428 2d31 2c20 3429 2e6d 756c 7469  hot(-1, 4).multi
+00017db0: 706c 7928 6e5f 6261 7463 682c 205b 5d29  ply(n_batch, [])
+00017dc0: 2e76 6965 7728 5b6e 5f62 6174 6368 5d2c  .view([n_batch],
+00017dd0: 2031 2c20 3429 2c20 310a 2020 2020 290a   1, 4), 1.    ).
+00017de0: 0a64 6566 204d 6174 7269 7832 5175 6174  .def Matrix2Quat
+00017df0: 6572 6e73 2870 6172 616d 7329 3a0a 2020  erns(params):.  
+00017e00: 2020 2222 220a 2020 2020 2020 2020 4d61    """.        Ma
+00017e10: 7472 6978 3a20 285b 6e5f 6261 7463 685d  trix: ([n_batch]
+00017e20: 2c20 342c 2034 290a 2020 2020 2020 2020  , 4, 4).        
+00017e30: 5175 6174 6572 6e3a 2071 622c 2071 632c  Quatern: qb, qc,
+00017e40: 2071 642c 2070 782c 2070 792c 2070 7a20   qd, px, py, pz 
+00017e50: 696e 2073 697a 653a 2028 5b6e 5f62 6174  in size: ([n_bat
+00017e60: 6368 5d2c 207b 367d 290a 2020 2020 2222  ch], {6}).    ""
+00017e70: 220a 2020 2020 7061 7261 6d73 203d 2062  ".    params = b
+00017e80: 6174 6f72 6368 5f74 656e 736f 7228 7061  atorch_tensor(pa
+00017e90: 7261 6d73 290a 2020 2020 6966 2070 6172  rams).    if par
+00017ea0: 616d 732e 6e5f 6469 6d20 3c3d 2032 2061  ams.n_dim <= 2 a
+00017eb0: 6e64 206e 6f74 2070 6172 616d 732e 6861  nd not params.ha
+00017ec0: 735f 6261 7463 683a 2070 6172 616d 7320  s_batch: params 
+00017ed0: 3d20 7061 7261 6d73 2e75 6e73 7175 6565  = params.unsquee
+00017ee0: 7a65 285b 5d29 0a20 2020 2069 6620 7061  ze([]).    if pa
+00017ef0: 7261 6d73 2e6e 5f64 696d 203d 3d20 3320  rams.n_dim == 3 
+00017f00: 616e 6420 6e6f 7420 7061 7261 6d73 2e68  and not params.h
+00017f10: 6173 5f62 6174 6368 3a20 7061 7261 6d73  as_batch: params
+00017f20: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
+00017f30: 203d 2030 0a20 2020 2069 6620 7061 7261   = 0.    if para
+00017f40: 6d73 2e6e 5f64 696d 203d 3d20 3320 616e  ms.n_dim == 3 an
+00017f50: 6420 7061 7261 6d73 2e68 6173 5f63 6861  d params.has_cha
+00017f60: 6e6e 656c 3a20 7061 7261 6d73 2e63 6861  nnel: params.cha
+00017f70: 6e6e 656c 5f64 696d 656e 7369 6f6e 203d  nnel_dimension =
+00017f80: 204e 6f6e 650a 2020 2020 6176 6f75 6368   None.    avouch
+00017f90: 2870 6172 616d 732e 6e5f 6469 6d20 3d3d  (params.n_dim ==
+00017fa0: 2033 2061 6e64 2070 6172 616d 732e 6861   3 and params.ha
+00017fb0: 735f 6261 7463 6820 616e 6420 6e6f 7420  s_batch and not 
+00017fc0: 7061 7261 6d73 2e68 6173 5f63 6861 6e6e  params.has_chann
+00017fd0: 656c 2c20 0a20 2020 2020 2020 2020 2020  el, .           
+00017fe0: 6622 506c 6561 7365 2075 7365 2062 6174  f"Please use bat
+00017ff0: 6f72 6368 2074 656e 736f 7220 6f66 2073  orch tensor of s
+00018000: 697a 6520 285b 6e5f 6261 7463 685d 2c20  ize ([n_batch], 
+00018010: 342c 2034 2920 666f 7220 4166 6669 6e65  4, 4) for Affine
+00018020: 206d 6174 7269 782c 2069 6e73 7465 6164   matrix, instead
+00018030: 206f 6620 7b70 6172 616d 732e 7368 6170   of {params.shap
+00018040: 657d 2e20 2229 0a20 2020 206e 5f62 6174  e}. ").    n_bat
+00018050: 6368 203d 2070 6172 616d 732e 6e5f 6261  ch = params.n_ba
+00018060: 7463 680a 2020 2020 782c 2079 2c20 7a20  tch.    x, y, z 
+00018070: 3d20 7061 7261 6d73 5b2e 2e2e 2c20 3a33  = params[..., :3
+00018080: 2c20 2d31 5d2e 6368 616e 6e65 6c5f 6469  , -1].channel_di
+00018090: 6d5f 2831 292e 7370 6c69 7428 312c 2031  m_(1).split(1, 1
+000180a0: 290a 2020 2020 6132 203d 2028 6274 2e64  ).    a2 = (bt.d
+000180b0: 6961 6728 7061 7261 6d73 292e 7375 6d28  iag(params).sum(
+000180c0: 292e 756e 7371 7565 657a 6528 7b7d 2920  ).unsqueeze({}) 
+000180d0: 2b20 3129 202f 2034 0a20 2020 2061 203d  + 1) / 4.    a =
+000180e0: 2062 742e 7371 7274 2861 3229 0a20 2020   bt.sqrt(a2).   
+000180f0: 2062 3220 3d20 6132 202d 2028 7061 7261   b2 = a2 - (para
+00018100: 6d73 5b2e 2e2e 2c20 312c 2031 5d20 2b20  ms[..., 1, 1] + 
+00018110: 7061 7261 6d73 5b2e 2e2e 2c20 322c 2032  params[..., 2, 2
+00018120: 5d29 202f 2032 0a20 2020 2063 3220 3d20  ]) / 2.    c2 = 
+00018130: 6132 202d 2028 7061 7261 6d73 5b2e 2e2e  a2 - (params[...
+00018140: 2c20 322c 2032 5d20 2b20 7061 7261 6d73  , 2, 2] + params
+00018150: 5b2e 2e2e 2c20 302c 2030 5d29 202f 2032  [..., 0, 0]) / 2
+00018160: 0a20 2020 2064 3220 3d20 6132 202d 2028  .    d2 = a2 - (
+00018170: 7061 7261 6d73 5b2e 2e2e 2c20 302c 2030  params[..., 0, 0
+00018180: 5d20 2b20 7061 7261 6d73 5b2e 2e2e 2c20  ] + params[..., 
+00018190: 312c 2031 5d29 202f 2032 0a20 2020 2044  1, 1]) / 2.    D
+000181a0: 203d 2070 6172 616d 7320 2d20 7061 7261   = params - para
+000181b0: 6d73 2e54 0a20 2020 2062 203d 2062 742e  ms.T.    b = bt.
+000181c0: 7369 676e 2844 5b2e 2e2e 2c20 322c 2031  sign(D[..., 2, 1
+000181d0: 5d29 202a 2062 742e 7371 7274 2862 3229  ]) * bt.sqrt(b2)
+000181e0: 0a20 2020 2063 203d 202d 2062 742e 7369  .    c = - bt.si
+000181f0: 676e 2844 5b2e 2e2e 2c20 322c 2030 5d29  gn(D[..., 2, 0])
+00018200: 202a 2062 742e 7371 7274 2863 3229 0a20   * bt.sqrt(c2). 
+00018210: 2020 2064 203d 2062 742e 7369 676e 2844     d = bt.sign(D
+00018220: 5b2e 2e2e 2c20 312c 2030 5d29 202a 2062  [..., 1, 0]) * b
+00018230: 742e 7371 7274 2864 3229 0a20 2020 2072  t.sqrt(d2).    r
+00018240: 6574 7572 6e20 6274 2e63 6174 2862 2c20  eturn bt.cat(b, 
+00018250: 632c 2064 2c20 782c 2079 2c20 7a2c 207b  c, d, x, y, z, {
+00018260: 7d29 0a                                  }).
```

### Comparing `micomputing-1.1.38/micomputing/zxhtools/TRS.py` & `micomputing-1.1.39/micomputing/zxhtools/TRS.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc` & `micomputing-1.1.39/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc` & `micomputing-1.1.39/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc` & `micomputing-1.1.39/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc` & `micomputing-1.1.39/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/micomputing/zxhtools/exec.py` & `micomputing-1.1.39/micomputing/zxhtools/exec.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/micomputing/zxhtools/image2.FFD` & `micomputing-1.1.39/micomputing/zxhtools/image2.FFD`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/micomputing.egg-info/PKG-INFO` & `micomputing-1.1.39/micomputing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micomputing
-Version: 1.1.38
+Version: 1.1.39
 Summary: 'micomputing' is a package for medical image computing. 
 Home-page: https://github.com/Bertie97/PyZMyc/micomputing
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # MIComputing
```

### Comparing `micomputing-1.1.38/micomputing.egg-info/SOURCES.txt` & `micomputing-1.1.39/micomputing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.38/setup_micomputing.py` & `micomputing-1.1.39/setup_micomputing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'micomputing',
-	version = '1.1.38',
+	version = '1.1.39',
 	keywords = ['pip', 'pymyc', 'micomputing', 'medical image', 'image registration', 'image similarities'],
 	description = "'micomputing' is a package for medical image computing. ",
 	long_description = '# MIComputing\n\n## Introduction\n\nPackage [`micomputing`](https://github.com/Bertie97/pycamia/tree/main/micomputing) is the medical image processing package under project [`PyCAMIA`](https://github.com/Bertie97/pycamia). It handles medical image read write, image interpolation, transformation, registration and so on. This package works under `PyCAMIA` and use `batorch.Tensor` as its basic data format. \n\n## Installation\n\nThis package can be installed by `pip install micomputing` or moving the source code to the directory of python libraries (the source code can be downloaded on [github](https://github.com/Bertie97/pycamia) or [PyPI](https://pypi.org/project/micomputing/)). \n\n```shell\npip install micomputing\n```\n\n\n\n## Acknowledgment\n\n@Yuncheng Zhou: Developer\n',
 	long_description_content_type = 'text/markdown',
 	license = 'MIT Licence',
 	url = 'https://github.com/Bertie97/PyZMyc/micomputing',
 	author = 'Yuncheng Zhou',
```

