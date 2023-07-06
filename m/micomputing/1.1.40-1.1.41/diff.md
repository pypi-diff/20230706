# Comparing `tmp/micomputing-1.1.40.tar.gz` & `tmp/micomputing-1.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micomputing-1.1.40.tar", last modified: Thu Jul  6 15:31:20 2023, max compression
+gzip compressed data, was "micomputing-1.1.41.tar", last modified: Thu Jul  6 15:33:19 2023, max compression
```

## Comparing `micomputing-1.1.40.tar` & `micomputing-1.1.41.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 15:31:20.569189 micomputing-1.1.40/
--rw-r--r--   0 admin      (501) staff       (20)       99 2023-07-06 15:31:20.000000 micomputing-1.1.40/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-06 15:31:20.568995 micomputing-1.1.40/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-06 15:31:20.000000 micomputing-1.1.40/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 15:31:20.566341 micomputing-1.1.40/micomputing/
--rw-r--r--   0 admin      (501) staff       (20)     2360 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/data.py
--rw-r--r--   0 admin      (501) staff       (20)    38286 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/funcs.py
--rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/metrics.py
--rwxr-xr-x   0 admin      (501) staff       (20)    33404 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/micfunctions.so
--rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/network.py
--rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/plot.py
--rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/stdio.py
--rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/test.py
--rw-r--r--   0 admin      (501) staff       (20)    98915 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/trans.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 15:31:20.568098 micomputing-1.1.40/micomputing/zxhtools/
--rw-r--r--   0 admin      (501) staff       (20)     7454 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/zxhtools/TRS.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 15:31:20.568708 micomputing-1.1.40/micomputing/zxhtools/__pycache__/
--rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     9153 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc
--rw-r--r--   0 admin      (501) staff       (20)     8988 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     8071 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/zxhtools/exec.py
--rw-r--r--   0 admin      (501) staff       (20)      507 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/zxhtools/image2.AFF
--rw-r--r--   0 admin      (501) staff       (20)    21032 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing/zxhtools/image2.FFD
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 15:31:20.567452 micomputing-1.1.40/micomputing.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       72 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       12 2023-07-06 15:31:20.000000 micomputing-1.1.40/micomputing.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-06 15:31:20.569253 micomputing-1.1.40/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1482 2023-07-06 15:31:20.000000 micomputing-1.1.40/setup_micomputing.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 15:33:19.855929 micomputing-1.1.41/
+-rw-r--r--   0 admin      (501) staff       (20)       99 2023-07-06 15:33:19.000000 micomputing-1.1.41/MANIFEST.in
+-rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-06 15:33:19.855786 micomputing-1.1.41/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-06 15:33:19.000000 micomputing-1.1.41/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 15:33:19.853455 micomputing-1.1.41/micomputing/
+-rw-r--r--   0 admin      (501) staff       (20)     2360 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/data.py
+-rw-r--r--   0 admin      (501) staff       (20)    38286 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/funcs.py
+-rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/metrics.py
+-rwxr-xr-x   0 admin      (501) staff       (20)    33404 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/micfunctions.so
+-rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/network.py
+-rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/plot.py
+-rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/stdio.py
+-rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/test.py
+-rw-r--r--   0 admin      (501) staff       (20)    98918 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/trans.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 15:33:19.854912 micomputing-1.1.41/micomputing/zxhtools/
+-rw-r--r--   0 admin      (501) staff       (20)     7454 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/zxhtools/TRS.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 15:33:19.855548 micomputing-1.1.41/micomputing/zxhtools/__pycache__/
+-rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     9153 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     8988 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     8071 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/zxhtools/exec.py
+-rw-r--r--   0 admin      (501) staff       (20)      507 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/zxhtools/image2.AFF
+-rw-r--r--   0 admin      (501) staff       (20)    21032 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing/zxhtools/image2.FFD
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 15:33:19.854229 micomputing-1.1.41/micomputing.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       72 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       12 2023-07-06 15:33:19.000000 micomputing-1.1.41/micomputing.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-06 15:33:19.855983 micomputing-1.1.41/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1482 2023-07-06 15:33:19.000000 micomputing-1.1.41/setup_micomputing.py
```

### Comparing `micomputing-1.1.40/PKG-INFO` & `micomputing-1.1.41/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micomputing
-Version: 1.1.40
+Version: 1.1.41
 Summary: 'micomputing' is a package for medical image computing. 
 Home-page: https://github.com/Bertie97/PyZMyc/micomputing
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # MIComputing
```

### Comparing `micomputing-1.1.40/README.md` & `micomputing-1.1.41/README.md`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/micomputing/__init__.py` & `micomputing-1.1.41/micomputing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = 'micomputing',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.1.39',
+    version = '1.1.40',
     contact = 'bertiezhou@163.com',
     keywords = ['medical image', 'image registration', 'image similarities'],
     description = "'micomputing' is a package for medical image computing. ",
     requires = ['numpy', 'torch>=1.5.1', 'batorch', 'pycamia', 'pyoverload', 'nibabel', 'pydicom', 'SimpleITK'],
-    update = '2023-07-06 23:29:03',
+    update = '2023-07-06 23:31:20',
     package_data = True
 ).check()
 
 from . import plot as plt
 from .stdio import IMG, dcm2nii, nii2dcm #*
 from .data import Info, Subject, ImageObject, Dataset, MedicalDataset #*
 from .network import U_Net, CNN, FCN
```

### Comparing `micomputing-1.1.40/micomputing/data.py` & `micomputing-1.1.41/micomputing/data.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/micomputing/funcs.py` & `micomputing-1.1.41/micomputing/funcs.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/micomputing/metrics.py` & `micomputing-1.1.41/micomputing/metrics.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/micomputing/micfunctions.so` & `micomputing-1.1.41/micomputing/micfunctions.so`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/micomputing/network.py` & `micomputing-1.1.41/micomputing/network.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/micomputing/plot.py` & `micomputing-1.1.41/micomputing/plot.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/micomputing/stdio.py` & `micomputing-1.1.41/micomputing/stdio.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/micomputing/test.py` & `micomputing-1.1.41/micomputing/test.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/micomputing/trans.py` & `micomputing-1.1.41/micomputing/trans.py`

 * *Files 0% similar despite different names*

```diff
@@ -4901,1283 +4901,1283 @@
 00013240: 2020 2072 6574 7572 6e20 696e 7465 7270     return interp
 00013250: 6f6c 6174 696f 6e5f 666f 7277 6172 6428  olation_forward(
 00013260: 696d 6167 652c 2074 7261 6e73 2c20 6d65  image, trans, me
 00013270: 7468 6f64 203d 206d 6574 686f 642c 2074  thod = method, t
 00013280: 6172 6765 745f 7370 6163 6520 3d20 7461  arget_space = ta
 00013290: 7267 6574 5f73 7061 6365 2c20 6669 6c6c  rget_space, fill
 000132a0: 203d 2066 696c 6c29 0a20 2020 2069 6d61   = fill).    ima
-000132b0: 6765 203d 2074 6f5f 6465 7669 6365 2862  ge = to_device(b
-000132c0: 6174 6f72 6368 5f74 656e 736f 7228 696d  atorch_tensor(im
-000132d0: 6167 6529 290a 2020 2020 7368 6170 655f  age)).    shape_
-000132e0: 6f75 7420 3d20 696d 6167 652e 7368 6170  out = image.shap
-000132f0: 650a 2020 2020 6966 2074 7261 6e73 2069  e.    if trans i
-00013300: 7320 4e6f 6e65 206f 7220 7472 616e 732e  s None or trans.
-00013310: 6e5f 6469 6d20 6973 204e 6f6e 653a 0a20  n_dim is None:. 
-00013320: 2020 2020 2020 2069 6620 6e6f 7420 696d         if not im
-00013330: 6167 652e 6861 735f 6261 7463 683a 2069  age.has_batch: i
-00013340: 6d61 6765 2e75 6e73 7175 6565 7a65 5f28  mage.unsqueeze_(
-00013350: 5b5d 290a 2020 2020 2020 2020 6966 206e  []).        if n
-00013360: 6f74 2069 6d61 6765 2e68 6173 5f63 6861  ot image.has_cha
-00013370: 6e6e 656c 3a20 696d 6167 652e 7374 616e  nnel: image.stan
-00013380: 6461 7264 5f28 292e 756e 7371 7565 657a  dard_().unsqueez
-00013390: 655f 287b 317d 290a 2020 2020 2020 2020  e_({1}).        
-000133a0: 6e5f 6469 6d20 3d20 696d 6167 652e 6e5f  n_dim = image.n_
-000133b0: 7370 6163 6520 2320 4765 7420 7468 6520  space # Get the 
-000133c0: 7370 6174 6961 6c20 7261 6e6b 2e0a 2020  spatial rank..  
-000133d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000133e0: 6e5f 6469 6d20 3d20 7472 616e 732e 6e5f  n_dim = trans.n_
-000133f0: 6469 6d0a 2020 2020 2020 2020 6966 2069  dim.        if i
-00013400: 6d61 6765 2e6e 5f64 696d 203d 3d20 6e5f  mage.n_dim == n_
-00013410: 6469 6d3a 0a20 2020 2020 2020 2020 2020  dim:.           
-00013420: 2069 6620 696d 6167 652e 6861 735f 7370   if image.has_sp
-00013430: 6563 6961 6c3a 0a20 2020 2020 2020 2020  ecial:.         
-00013440: 2020 2020 2020 2070 7269 6e74 2866 2257         print(f"W
-00013450: 6172 6e69 6e67 3a20 2769 6e74 6572 706f  arning: 'interpo
-00013460: 6c61 7469 6f6e 2720 7472 7969 6e67 2074  lation' trying t
-00013470: 6f20 7472 616e 7366 6f72 6d20 7b69 6d61  o transform {ima
-00013480: 6765 2e6e 5f73 7061 6365 7d2b 7b69 6d61  ge.n_space}+{ima
-00013490: 6765 2e6e 5f73 7065 6369 616c 7d44 2069  ge.n_special}D i
-000134a0: 6d61 6765 2028 7769 7468 2062 6174 6368  mage (with batch
-000134b0: 206f 7220 6368 616e 6e65 6c29 2062 7920   or channel) by 
-000134c0: 7b6e 5f64 696d 7d44 2074 7261 6e73 666f  {n_dim}D transfo
-000134d0: 726d 6174 696f 6e2c 2061 7574 6f2d 7265  rmation, auto-re
-000134e0: 6d6f 7669 6e67 2073 7065 6369 616c 2064  moving special d
-000134f0: 696d 656e 7369 6f6e 732e 2229 0a20 2020  imensions.").   
-00013500: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
-00013510: 6765 2e72 656d 6f76 655f 7370 6563 6961  ge.remove_specia
-00013520: 6c5f 2829 0a20 2020 2020 2020 2020 2020  l_().           
-00013530: 2069 6d61 6765 2e75 6e73 7175 6565 7a65   image.unsqueeze
-00013540: 5f28 5b5d 292e 756e 7371 7565 657a 655f  _([]).unsqueeze_
-00013550: 287b 7d29 0a20 2020 2020 2020 2065 6c69  ({}).        eli
-00013560: 6620 696d 6167 652e 6e5f 6469 6d20 3d3d  f image.n_dim ==
-00013570: 206e 5f64 696d 202b 2031 3a0a 2020 2020   n_dim + 1:.    
-00013580: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00013590: 6d61 6765 2e68 6173 5f62 6174 6368 3a0a  mage.has_batch:.
-000135a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135b0: 6966 2069 6d61 6765 2e68 6173 5f63 6861  if image.has_cha
-000135c0: 6e6e 656c 3a20 696d 6167 652e 756e 7371  nnel: image.unsq
-000135d0: 7565 657a 655f 285b 5d29 0a20 2020 2020  ueeze_([]).     
-000135e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000135f0: 2069 6d61 6765 2e77 6974 685f 6261 7463   image.with_batc
-00013600: 6864 696d 2830 292e 756e 7371 7565 657a  hdim(0).unsqueez
-00013610: 655f 287b 317d 290a 2020 2020 2020 2020  e_({1}).        
-00013620: 2020 2020 656c 6966 206e 6f74 2069 6d61      elif not ima
-00013630: 6765 2e68 6173 5f63 6861 6e6e 656c 3a20  ge.has_channel: 
-00013640: 696d 6167 652e 756e 7371 7565 657a 655f  image.unsqueeze_
-00013650: 287b 7d29 0a20 2020 2020 2020 2020 2020  ({}).           
-00013660: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00013670: 2020 2020 2020 2070 7269 6e74 2866 2257         print(f"W
-00013680: 6172 6e69 6e67 3a20 2769 6e74 6572 706f  arning: 'interpo
-00013690: 6c61 7469 6f6e 2720 7472 7969 6e67 2074  lation' trying t
-000136a0: 6f20 7472 616e 7366 6f72 6d20 7b69 6d61  o transform {ima
-000136b0: 6765 2e6e 5f73 7061 6365 7d2b 7b69 6d61  ge.n_space}+{ima
-000136c0: 6765 2e6e 5f73 7065 6369 616c 7d44 2069  ge.n_special}D i
-000136d0: 6d61 6765 2028 7769 7468 2062 6174 6368  mage (with batch
-000136e0: 206f 7220 6368 616e 6e65 6c29 2062 7920   or channel) by 
-000136f0: 7b6e 5f64 696d 7d44 2074 7261 6e73 666f  {n_dim}D transfo
-00013700: 726d 6174 696f 6e2c 2061 7574 6f2d 7265  rmation, auto-re
-00013710: 6d6f 7669 6e67 2074 6865 2063 6861 6e6e  moving the chann
-00013720: 656c 2064 696d 656e 7369 6f6e 732e 2229  el dimensions.")
-00013730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013740: 2069 6d61 6765 2e77 6974 685f 6368 616e   image.with_chan
-00013750: 6e65 6c64 696d 284e 6f6e 6529 2e75 6e73  neldim(None).uns
-00013760: 7175 6565 7a65 5f28 7b7d 290a 2020 2020  queeze_({}).    
-00013770: 2020 2020 656c 6966 2069 6d61 6765 2e6e      elif image.n
-00013780: 5f64 696d 203d 3d20 6e5f 6469 6d20 2b20  _dim == n_dim + 
-00013790: 323a 0a20 2020 2020 2020 2020 2020 2023  2:.            #
-000137a0: 205f 6368 616e 6e61 6c2f 6261 7463 6820   _channal/batch 
-000137b0: 6469 6d65 6e73 696f 6e73 2075 7365 6420  dimensions used 
-000137c0: 6865 7265 2061 7320 7468 6579 2061 7265  here as they are
-000137d0: 206e 5f64 696d 2077 6865 6e20 6e6f 7420   n_dim when not 
-000137e0: 6578 6973 7465 642e 200a 2020 2020 2020  existed. .      
-000137f0: 2020 2020 2020 6966 2069 6d61 6765 2e6e        if image.n
-00013800: 5f73 7065 6369 616c 203d 3d20 313a 0a20  _special == 1:. 
-00013810: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00013820: 7269 6e74 2866 2257 6172 6e69 6e67 3a20  rint(f"Warning: 
-00013830: 2769 6e74 6572 706f 6c61 7469 6f6e 2720  'interpolation' 
-00013840: 7472 7969 6e67 2074 6f20 7472 616e 7366  trying to transf
-00013850: 6f72 6d20 7b69 6d61 6765 2e6e 5f73 7061  orm {image.n_spa
-00013860: 6365 7d2b 3144 2069 6d61 6765 2028 7769  ce}+1D image (wi
-00013870: 7468 2062 6174 6368 206f 7220 6368 616e  th batch or chan
-00013880: 6e65 6c29 2062 7920 7b6e 5f64 696d 7d44  nel) by {n_dim}D
-00013890: 2074 7261 6e73 666f 726d 6174 696f 6e2c   transformation,
-000138a0: 2061 7574 6f2d 696e 7365 7274 696e 6720   auto-inserting 
-000138b0: 6e65 7720 7370 6563 6961 6c20 6469 6d65  new special dime
-000138c0: 6e73 696f 6e2e 2229 0a20 2020 2020 2020  nsion.").       
-000138d0: 2020 2020 2069 6620 6e6f 7420 696d 6167       if not imag
-000138e0: 652e 6861 735f 6261 7463 683a 2069 6d61  e.has_batch: ima
-000138f0: 6765 2e62 6174 6368 5f64 696d 656e 7369  ge.batch_dimensi
-00013900: 6f6e 203d 2030 2069 6620 696d 6167 652e  on = 0 if image.
-00013910: 5f63 6861 6e6e 656c 5f64 696d 656e 7369  _channel_dimensi
-00013920: 6f6e 203e 2030 2065 6c73 6520 310a 2020  on > 0 else 1.  
-00013930: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00013940: 2069 6d61 6765 2e68 6173 5f63 6861 6e6e   image.has_chann
-00013950: 656c 3a20 696d 6167 652e 6368 616e 6e65  el: image.channe
-00013960: 6c5f 6469 6d65 6e73 696f 6e20 3d20 3020  l_dimension = 0 
-00013970: 6966 2069 6d61 6765 2e5f 6261 7463 685f  if image._batch_
-00013980: 6469 6d65 6e73 696f 6e20 3e20 3020 656c  dimension > 0 el
-00013990: 7365 2031 0a20 2020 2061 766f 7563 6828  se 1.    avouch(
-000139a0: 696d 6167 652e 6861 735f 6261 7463 6820  image.has_batch 
-000139b0: 616e 6420 696d 6167 652e 6861 735f 6368  and image.has_ch
-000139c0: 616e 6e65 6c2c 2022 506c 6561 7365 2075  annel, "Please u
-000139d0: 7365 2062 6174 6f72 6368 2074 656e 736f  se batorch tenso
-000139e0: 7220 6f66 2073 697a 6520 2220 2b0a 2020  r of size " +.  
-000139f0: 2020 2020 2020 2020 2020 2228 5b6e 5f62            "([n_b
-00013a00: 6174 6368 5d2c 207b 6e5f 6368 616e 6e65  atch], {n_channe
-00013a10: 6c2f 6e5f 6665 6174 7572 653a 6f70 7469  l/n_feature:opti
-00013a20: 6f6e 616c 7d2c 206d 5f31 2c20 6d5f 322c  onal}, m_1, m_2,
-00013a30: 202e 2e2e 2c20 6d5f 7229 205b 723d 6e5f   ..., m_r) [r=n_
-00013a40: 6469 6d5d 2066 6f72 2022 202b 200a 2020  dim] for " + .  
-00013a50: 2020 2020 2020 2020 2020 6622 6461 7461            f"data
-00013a60: 2074 6f20 6265 2073 7061 7469 616c 6c79   to be spatially
-00013a70: 2069 6e74 6572 706f 6c61 7465 642c 2069   interpolated, i
-00013a80: 6e73 7465 6164 206f 6620 7b69 6d61 6765  nstead of {image
-00013a90: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
-00013aa0: 6966 2074 7261 6e73 2069 7320 6e6f 7420  if trans is not 
-00013ab0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6176  None:.        av
-00013ac0: 6f75 6368 2869 6d61 6765 2e6e 5f62 6174  ouch(image.n_bat
-00013ad0: 6368 203d 3d20 3120 6f72 2074 7261 6e73  ch == 1 or trans
-00013ae0: 2e6e 5f62 6174 6368 2069 6e20 284e 6f6e  .n_batch in (Non
-00013af0: 652c 2069 6d61 6765 2e6e 5f62 6174 6368  e, image.n_batch
-00013b00: 2c20 3129 2c20 2250 6c65 6173 6520 7573  , 1), "Please us
-00013b10: 6520 7472 616e 7366 6f72 6d61 7469 6f6e  e transformation
-00013b20: 206f 6620 6120 2220 2b0a 2020 2020 2020   of a " +.      
-00013b30: 2020 2020 2020 6622 7375 6974 6162 6c65        f"suitable
-00013b40: 206e 5f62 6174 6368 2074 6f20 7472 616e   n_batch to tran
-00013b50: 7366 6f72 6d20 696d 6167 6520 7769 7468  sform image with
-00013b60: 2062 6174 6368 7369 7a65 207b 696d 6167   batchsize {imag
-00013b70: 652e 6e5f 6261 7463 687d 2c20 6375 7272  e.n_batch}, curr
-00013b80: 656e 746c 7920 7b74 7261 6e73 2e6e 5f62  ently {trans.n_b
-00013b90: 6174 6368 7d2e 2229 0a0a 2020 2020 6e5f  atch}.")..    n_
-00013ba0: 6261 7463 6820 3d20 696d 6167 652e 6e5f  batch = image.n_
-00013bb0: 6261 7463 680a 2020 2020 6966 206e 5f62  batch.    if n_b
-00013bc0: 6174 6368 203d 3d20 3120 616e 6420 7472  atch == 1 and tr
-00013bd0: 616e 7320 6973 206e 6f74 204e 6f6e 6520  ans is not None 
-00013be0: 616e 6420 7472 616e 732e 6e5f 6261 7463  and trans.n_batc
-00013bf0: 6820 6973 206e 6f74 204e 6f6e 6520 616e  h is not None an
-00013c00: 6420 7472 616e 732e 6e5f 6261 7463 6820  d trans.n_batch 
-00013c10: 3e20 313a 206e 5f62 6174 6368 203d 2074  > 1: n_batch = t
-00013c20: 7261 6e73 2e6e 5f62 6174 6368 0a20 2020  rans.n_batch.   
-00013c30: 2069 6620 6e5f 6261 7463 6820 3d3d 2031   if n_batch == 1
-00013c40: 2061 6e64 2069 7369 6e73 7461 6e63 6528   and isinstance(
-00013c50: 7461 7267 6574 5f73 7061 6365 2c20 6274  target_space, bt
-00013c60: 2e54 656e 736f 7229 2061 6e64 2074 6172  .Tensor) and tar
-00013c70: 6765 745f 7370 6163 652e 6861 735f 6261  get_space.has_ba
-00013c80: 7463 6820 616e 6420 7461 7267 6574 5f73  tch and target_s
-00013c90: 7061 6365 2e6e 5f62 6174 6368 203e 2031  pace.n_batch > 1
-00013ca0: 3a20 6e5f 6261 7463 6820 3d20 7461 7267  : n_batch = targ
-00013cb0: 6574 5f73 7061 6365 2e6e 5f62 6174 6368  et_space.n_batch
-00013cc0: 0a20 2020 2069 6620 696d 6167 652e 6e5f  .    if image.n_
-00013cd0: 6261 7463 6820 3d3d 2031 3a20 696d 6167  batch == 1: imag
-00013ce0: 6520 3d20 696d 6167 652e 7265 7065 6174  e = image.repeat
-00013cf0: 6564 286e 5f62 6174 6368 2c20 5b5d 290a  ed(n_batch, []).
-00013d00: 2020 2020 6e5f 6665 6174 7572 6520 3d20      n_feature = 
-00013d10: 696d 6167 652e 6e5f 6368 616e 6e65 6c0a  image.n_channel.
-00013d20: 2020 2020 7369 7a65 203d 2062 742e 6368      size = bt.ch
-00013d30: 616e 6e65 6c5f 7465 6e73 6f72 2869 6d61  annel_tensor(ima
-00013d40: 6765 2e73 7061 6365 292e 696e 7428 290a  ge.space).int().
-00013d50: 2020 2020 6966 206e 5f62 6174 6368 203e      if n_batch >
-00013d60: 2031 2061 6e64 206e 6f74 2073 6861 7065   1 and not shape
-00013d70: 5f6f 7574 2e68 6173 5f62 6174 6368 3a20  _out.has_batch: 
-00013d80: 7368 6170 655f 6f75 7420 3d20 6274 2e53  shape_out = bt.S
-00013d90: 697a 6528 5b6e 5f62 6174 6368 5d29 202b  ize([n_batch]) +
-00013da0: 2073 6861 7065 5f6f 7574 0a20 2020 2069   shape_out.    i
-00013db0: 6620 7461 7267 6574 5f73 7061 6365 2069  f target_space i
-00013dc0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00013dd0: 7363 616c 652c 202a 7061 6972 7320 3d20  scale, *pairs = 
-00013de0: 7472 616e 732e 7265 7368 6170 650a 2020  trans.reshape.  
-00013df0: 2020 2020 2020 6966 206c 656e 2873 6361        if len(sca
-00013e00: 6c65 2920 3d3d 2031 3a20 7363 616c 6520  le) == 1: scale 
-00013e10: 2a3d 206e 5f64 696d 0a20 2020 2020 2020  *= n_dim.       
-00013e20: 2074 6172 6765 745f 7370 6163 6520 3d20   target_space = 
-00013e30: 5b69 6e74 2878 202a 2079 2920 666f 7220  [int(x * y) for 
-00013e40: 782c 2079 2069 6e20 7a69 7028 696d 6167  x, y in zip(imag
-00013e50: 652e 7370 6163 652c 2073 6361 6c65 295d  e.space, scale)]
-00013e60: 0a20 2020 2020 2020 2066 6f72 2070 2c20  .        for p, 
-00013e70: 7120 696e 2070 6169 7273 3a20 7461 7267  q in pairs: targ
-00013e80: 6574 5f73 7061 6365 5b70 5d2c 2074 6172  et_space[p], tar
-00013e90: 6765 745f 7370 6163 655b 715d 203d 2074  get_space[q] = t
-00013ea0: 6172 6765 745f 7370 6163 655b 715d 2c20  arget_space[q], 
-00013eb0: 7461 7267 6574 5f73 7061 6365 5b70 5d0a  target_space[p].
-00013ec0: 2020 2020 2020 2020 7461 7267 6574 5f73          target_s
-00013ed0: 7061 6365 203d 2074 7570 6c65 2874 6172  pace = tuple(tar
-00013ee0: 6765 745f 7370 6163 6529 0a20 2020 2020  get_space).     
-00013ef0: 2020 2073 6861 7065 5f6f 7574 203d 2073     shape_out = s
-00013f00: 6861 7065 5f6f 7574 2e72 6573 6574 5f73  hape_out.reset_s
-00013f10: 7061 6365 2874 6172 6765 745f 7370 6163  pace(target_spac
-00013f20: 6529 0a20 2020 2069 6620 6973 696e 7374  e).    if isinst
-00013f30: 616e 6365 2874 6172 6765 745f 7370 6163  ance(target_spac
-00013f40: 652c 2074 7570 6c65 2920 616e 6420 6c65  e, tuple) and le
-00013f50: 6e28 7461 7267 6574 5f73 7061 6365 2920  n(target_space) 
-00013f60: 3d3d 206e 5f64 696d 3a20 7061 7373 0a20  == n_dim: pass. 
-00013f70: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-00013f80: 6365 2874 6172 6765 745f 7370 6163 652c  ce(target_space,
-00013f90: 2062 742e 746f 7263 682e 5465 6e73 6f72   bt.torch.Tensor
-00013fa0: 293a 2070 6173 730a 2020 2020 656c 7365  ): pass.    else
-00013fb0: 3a20 7261 6973 6520 5479 7065 4572 726f  : raise TypeErro
-00013fc0: 7228 6622 5772 6f6e 6720 7461 7267 6574  r(f"Wrong target
-00013fd0: 2073 7061 6365 2066 6f72 2069 6e74 6572   space for inter
-00013fe0: 706f 6c61 7469 6f6e 3a20 7b74 6172 6765  polation: {targe
-00013ff0: 745f 7370 6163 657d 2e20 2229 0a20 2020  t_space}. ").   
-00014000: 2069 6620 6973 696e 7374 616e 6365 2874   if isinstance(t
-00014010: 6172 6765 745f 7370 6163 652c 2074 7570  arget_space, tup
-00014020: 6c65 293a 200a 2020 2020 2020 2020 2320  le): .        # 
-00014030: 4372 6561 7465 2061 2067 7269 6420 5820  Create a grid X 
-00014040: 7769 7468 2073 697a 6520 287b 6e5f 6469  with size ({n_di
-00014050: 6d7d 2c20 7369 7a65 5f31 2c20 7369 7a65  m}, size_1, size
-00014060: 5f32 2c20 2e2e 2e2c 2073 697a 655f 7229  _2, ..., size_r)
-00014070: 205b 723d 6e5f 6469 6d5d 2e0a 2020 2020   [r=n_dim]..    
-00014080: 2020 2020 5820 3d20 6274 2e69 6d61 6765      X = bt.image
-00014090: 5f67 7269 6428 7461 7267 6574 5f73 7061  _grid(target_spa
-000140a0: 6365 292e 666c 6f61 7428 2920 2320 2b20  ce).float() # + 
-000140b0: 6274 2e63 6861 6e6e 656c 5f74 656e 736f  bt.channel_tenso
-000140c0: 7228 5b66 6c6f 6174 2861 2d62 292f 3220  r([float(a-b)/2 
-000140d0: 666f 7220 612c 2062 2069 6e20 7a69 7028  for a, b in zip(
-000140e0: 696d 6167 652e 7370 6163 652c 2074 6172  image.space, tar
-000140f0: 6765 745f 7370 6163 6529 5d29 0a20 2020  get_space)]).   
-00014100: 2020 2020 2023 2043 6f6d 7075 7465 2074       # Compute t
-00014110: 6865 2074 7261 6e73 666f 726d 6564 2063  he transformed c
-00014120: 6f6f 7264 696e 6174 6573 2e20 593a 2028  oordinates. Y: (
-00014130: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 6469  [n_batch], {n_di
-00014140: 6d7d 2c20 7369 7a65 5f31 2c20 7369 7a65  m}, size_1, size
-00014150: 5f32 2c20 2e2e 2e2c 2073 697a 655f 7229  _2, ..., size_r)
-00014160: 205b 723d 6e5f 6469 6d5d 2e0a 2020 2020   [r=n_dim]..    
-00014170: 2020 2020 6966 2074 7261 6e73 2069 7320      if trans is 
-00014180: 4e6f 6e65 3a20 7472 616e 7320 3d20 4964  None: trans = Id
-00014190: 656e 7469 7479 2829 0a20 2020 2020 2020  entity().       
-000141a0: 2059 203d 2074 7261 6e73 2858 290a 2020   Y = trans(X).  
-000141b0: 2020 2020 2020 6966 206e 6f74 2059 2e68        if not Y.h
-000141c0: 6173 5f62 6174 6368 3a20 5920 3d20 592e  as_batch: Y = Y.
-000141d0: 6d75 6c74 6970 6c79 286e 5f62 6174 6368  multiply(n_batch
-000141e0: 2c20 5b5d 290a 2020 2020 2020 2020 6966  , []).        if
-000141f0: 2059 2e6e 5f62 6174 6368 203d 3d20 313a   Y.n_batch == 1:
-00014200: 2059 203d 2059 2e72 6570 6561 7465 6428   Y = Y.repeated(
-00014210: 6e5f 6261 7463 682c 205b 5d29 0a20 2020  n_batch, []).   
-00014220: 2020 2020 2059 203d 2059 2e61 6d70 6c69       Y = Y.ampli
-00014230: 6679 286e 5f66 6561 7475 7265 2c20 5b5d  fy(n_feature, []
-00014240: 290a 2020 2020 2020 2020 7368 6170 655f  ).        shape_
-00014250: 6f75 7420 3d20 7368 6170 655f 6f75 742e  out = shape_out.
-00014260: 7265 7365 745f 7370 6163 6528 7461 7267  reset_space(targ
-00014270: 6574 5f73 7061 6365 290a 2020 2020 656c  et_space).    el
-00014280: 7365 3a0a 2020 2020 2020 2020 7461 7267  se:.        targ
-00014290: 6574 5f73 7061 6365 203d 2062 6174 6f72  et_space = bator
-000142a0: 6368 5f74 656e 736f 7228 7461 7267 6574  ch_tensor(target
-000142b0: 5f73 7061 6365 290a 2020 2020 2020 2020  _space).        
-000142c0: 6966 206e 6f74 2074 6172 6765 745f 7370  if not target_sp
-000142d0: 6163 652e 6861 735f 6261 7463 683a 0a20  ace.has_batch:. 
-000142e0: 2020 2020 2020 2020 2020 2069 6620 7461             if ta
-000142f0: 7267 6574 5f73 7061 6365 2e73 697a 6528  rget_space.size(
-00014300: 3029 203d 3d20 6e5f 6261 7463 6820 616e  0) == n_batch an
-00014310: 6420 6e5f 6261 7463 6820 213d 206e 5f64  d n_batch != n_d
-00014320: 696d 206f 7220 6c65 6e28 5b78 2066 6f72  im or len([x for
-00014330: 2078 2069 6e20 7461 7267 6574 5f73 7061   x in target_spa
-00014340: 6365 2e73 6861 7065 2069 6620 7820 3d3d  ce.shape if x ==
-00014350: 206e 5f64 696d 5d29 203e 3d20 323a 0a20   n_dim]) >= 2:. 
-00014360: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00014370: 6172 6765 745f 7370 6163 652e 7769 7468  arget_space.with
-00014380: 5f62 6174 6368 6469 6d28 3029 0a20 2020  _batchdim(0).   
-00014390: 2020 2020 2020 2020 2065 6c73 653a 2074           else: t
-000143a0: 6172 6765 745f 7370 6163 652e 756e 7371  arget_space.unsq
-000143b0: 7565 657a 655f 285b 5d29 0a20 2020 2020  ueeze_([]).     
-000143c0: 2020 2069 6620 6e6f 7420 7461 7267 6574     if not target
-000143d0: 5f73 7061 6365 2e68 6173 5f63 6861 6e6e  _space.has_chann
-000143e0: 656c 3a0a 2020 2020 2020 2020 2020 2020  el:.            
-000143f0: 6966 2074 6172 6765 745f 7370 6163 652e  if target_space.
-00014400: 6261 7463 685f 6469 6d65 6e73 696f 6e20  batch_dimension 
-00014410: 213d 2030 2061 6e64 2074 6172 6765 745f  != 0 and target_
-00014420: 7370 6163 652e 7369 7a65 2830 2920 3d3d  space.size(0) ==
-00014430: 206e 5f64 696d 3a20 7461 7267 6574 5f73   n_dim: target_s
-00014440: 7061 6365 2e77 6974 685f 6368 616e 6e65  pace.with_channe
-00014450: 6c64 696d 2830 290a 2020 2020 2020 2020  ldim(0).        
-00014460: 2020 2020 656c 6966 2074 6172 6765 745f      elif target_
-00014470: 7370 6163 652e 6261 7463 685f 6469 6d65  space.batch_dime
-00014480: 6e73 696f 6e20 213d 2031 2061 6e64 2074  nsion != 1 and t
-00014490: 6172 6765 745f 7370 6163 652e 7369 7a65  arget_space.size
-000144a0: 2831 2920 3d3d 206e 5f64 696d 3a20 7461  (1) == n_dim: ta
-000144b0: 7267 6574 5f73 7061 6365 2e77 6974 685f  rget_space.with_
-000144c0: 6368 616e 6e65 6c64 696d 2831 290a 2020  channeldim(1).  
-000144d0: 2020 2020 2020 2020 2020 656c 6966 2074            elif t
-000144e0: 6172 6765 745f 7370 6163 652e 6261 7463  arget_space.batc
-000144f0: 685f 6469 6d65 6e73 696f 6e20 213d 2074  h_dimension != t
-00014500: 6172 6765 745f 7370 6163 652e 6e5f 6469  arget_space.n_di
-00014510: 6d20 2d20 3120 616e 6420 7461 7267 6574  m - 1 and target
-00014520: 5f73 7061 6365 2e73 697a 6528 2d31 2920  _space.size(-1) 
-00014530: 3d3d 206e 5f64 696d 3a20 7461 7267 6574  == n_dim: target
-00014540: 5f73 7061 6365 2e77 6974 685f 6368 616e  _space.with_chan
-00014550: 6e65 6c64 696d 282d 3129 0a20 2020 2020  neldim(-1).     
-00014560: 2020 2061 766f 7563 6828 7461 7267 6574     avouch(target
-00014570: 5f73 7061 6365 2e68 6173 5f63 6861 6e6e  _space.has_chann
-00014580: 656c 2061 6e64 2074 6172 6765 745f 7370  el and target_sp
-00014590: 6163 652e 6e5f 6368 616e 6e65 6c20 3d3d  ace.n_channel ==
-000145a0: 206e 5f64 696d 2c20 2227 7461 7267 6574   n_dim, "'target
-000145b0: 5f73 7061 6365 2720 666f 7220 696e 7465  _space' for inte
-000145c0: 7270 6f6c 6174 696f 6e20 7368 6f75 6c64  rpolation should
-000145d0: 2068 6176 6520 6120 6368 616e 6e65 6c20   have a channel 
-000145e0: 6469 6d65 6e73 696f 6e20 666f 7220 636f  dimension for co
-000145f0: 6f72 6469 6e61 7465 732e 2022 290a 2020  ordinates. ").  
-00014600: 2020 2020 2020 5920 3d20 7461 7267 6574        Y = target
-00014610: 5f73 7061 6365 2e72 6570 6561 7465 6428  _space.repeated(
-00014620: 6e5f 6261 7463 6820 2f2f 2074 6172 6765  n_batch // targe
-00014630: 745f 7370 6163 652e 6e5f 6261 7463 682c  t_space.n_batch,
-00014640: 205b 5d29 2e61 6d70 6c69 6679 286e 5f66   []).amplify(n_f
-00014650: 6561 7475 7265 2c20 5b5d 290a 2020 2020  eature, []).    
-00014660: 2020 2020 7368 6170 655f 6f75 7420 3d20      shape_out = 
-00014670: 7368 6170 655f 6f75 742e 7265 7365 745f  shape_out.reset_
-00014680: 7370 6163 6528 7461 7267 6574 5f73 7061  space(target_spa
-00014690: 6365 2e73 7061 6365 290a 2020 2020 2020  ce.space).      
-000146a0: 2020 0a20 2020 2069 6d61 6765 203d 2069    .    image = i
-000146b0: 6d61 6765 2e6d 6572 6765 6469 6d73 287b  mage.mergedims({
-000146c0: 7d2c 205b 5d29 0a20 2020 206e 5f62 6174  }, []).    n_bat
-000146d0: 6368 203d 2069 6d61 6765 2e6e 5f62 6174  ch = image.n_bat
-000146e0: 6368 0a0a 2020 2020 6966 206d 6574 686f  ch..    if metho
-000146f0: 642e 6c6f 7765 7228 2920 3d3d 2027 6273  d.lower() == 'bs
-00014700: 706c 696e 6527 3a0a 2020 2020 2020 2020  pline':.        
-00014710: 6966 2064 6572 6976 6174 6976 653a 2072  if derivative: r
-00014720: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
-00014730: 4e6f 2064 6572 6976 6174 6976 6573 2066  No derivatives f
-00014740: 6f72 2062 7370 6c69 6e65 2069 6e74 6572  or bspline inter
-00014750: 706f 6c61 7469 6f6e 7320 6172 6520 6176  polations are av
-00014760: 6169 6c61 626c 6520 736f 2066 6172 2e20  ailable so far. 
-00014770: 506c 6561 7365 2077 7269 7465 2069 7420  Please write it 
-00014780: 6279 2079 6f75 7273 656c 662e 2022 290a  by yourself. ").
-00014790: 2020 2020 2020 2020 2320 544f 444f 3a20          # TODO: 
-000147a0: 4646 440a 2020 2020 2020 2020 7261 6973  FFD.        rais
-000147b0: 6520 5479 7065 4572 726f 7228 2242 7370  e TypeError("Bsp
-000147c0: 6c69 6e65 2069 6e74 6572 706f 6c61 7469  line interpolati
-000147d0: 6f6e 2069 7320 6e6f 7420 6176 6169 6c61  on is not availa
-000147e0: 626c 6520 736f 2066 6172 2e20 506c 6561  ble so far. Plea
-000147f0: 7365 2077 7269 7465 2069 7420 6279 2079  se write it by y
-00014800: 6f75 7273 656c 662e 2022 290a 0a20 2020  ourself. ")..   
-00014810: 2069 5920 3d20 6274 2e66 6c6f 6f72 2859   iY = bt.floor(Y
-00014820: 292e 6c6f 6e67 2829 2023 2047 656e 6572  ).long() # Gener
-00014830: 6174 6520 7468 6520 696e 7465 6765 7220  ate the integer 
-00014840: 7061 7274 206f 6620 590a 2020 2020 6a59  part of Y.    jY
-00014850: 203d 2069 5920 2b20 3120 2320 616e 6420   = iY + 1 # and 
-00014860: 7468 6520 696e 7465 6765 7220 7061 7274  the integer part
-00014870: 2070 6c75 7320 6f6e 652e 0a20 2020 2069   plus one..    i
-00014880: 6620 6d65 7468 6f64 2e6c 6f77 6572 2829  f method.lower()
-00014890: 203d 3d20 276c 696e 6561 7227 3a20 6659   == 'linear': fY
-000148a0: 203d 2059 202d 2069 592e 666c 6f61 7428   = Y - iY.float(
-000148b0: 2920 2320 5468 6520 6465 6369 6d61 6c20  ) # The decimal 
-000148c0: 7061 7274 206f 6620 592e 0a20 2020 2065  part of Y..    e
-000148d0: 6c69 6620 6d65 7468 6f64 2e6c 6f77 6572  lif method.lower
-000148e0: 2829 203d 3d20 276e 6561 7265 7374 273a  () == 'nearest':
-000148f0: 2066 5920 3d20 6274 2e66 6c6f 6f72 2859   fY = bt.floor(Y
-00014900: 202d 2069 592e 666c 6f61 7428 2920 2b20   - iY.float() + 
-00014910: 302e 3529 2023 2054 6865 2064 6563 696d  0.5) # The decim
-00014920: 616c 2070 6172 7420 6f66 2059 2e0a 2020  al part of Y..  
-00014930: 2020 656c 7365 3a20 7261 6973 6520 5479    else: raise Ty
-00014940: 7065 4572 726f 7228 2255 6e72 6563 6f67  peError("Unrecog
-00014950: 6e69 7a65 6420 6172 6775 6d65 6e74 2027  nized argument '
-00014960: 6d65 7468 6f64 272e 2022 290a 2020 2020  method'. ").    
-00014970: 6259 203d 2062 742e 7374 6163 6b28 2869  bY = bt.stack((i
-00014980: 592c 206a 5929 2c20 3129 2e76 6965 7728  Y, jY), 1).view(
-00014990: 5b6e 5f62 6174 6368 5d2c 2032 2c20 7b6e  [n_batch], 2, {n
-000149a0: 5f64 696d 7d2c 202d 3129 2023 2028 5b6e  _dim}, -1) # ([n
-000149b0: 5f62 6174 6368 5d2c 2032 2c20 7b6e 5f64  _batch], 2, {n_d
-000149c0: 696d 7d2c 206e 5f64 6174 6129 2e0a 2020  im}, n_data)..  
-000149d0: 2020 5720 3d20 6274 2e73 7461 636b 2828    W = bt.stack((
-000149e0: 3120 2d20 6659 2c20 6659 292c 2031 292e  1 - fY, fY), 1).
-000149f0: 7669 6577 285b 6e5f 6261 7463 685d 2c20  view([n_batch], 
-00014a00: 322c 207b 6e5f 6469 6d7d 2c20 2d31 2920  2, {n_dim}, -1) 
-00014a10: 2320 285b 6e5f 6261 7463 685d 2c20 322c  # ([n_batch], 2,
-00014a20: 207b 6e5f 6469 6d7d 2c20 6e5f 6461 7461   {n_dim}, n_data
-00014a30: 292e 0a20 2020 206e 5f64 6174 6120 3d20  )..    n_data = 
-00014a40: 6259 2e73 697a 6528 2d31 290a 0a20 2020  bY.size(-1)..   
-00014a50: 2023 2050 7265 7061 7265 2066 6f72 2074   # Prepare for t
-00014a60: 6865 206f 7574 7075 7420 7370 6163 653a  he output space:
-00014a70: 206e 5f62 6174 6368 2c20 6d5f 312c 202e   n_batch, m_1, .
-00014a80: 2e2e 2c20 6d5f 730a 2020 2020 6966 2064  .., m_s.    if d
-00014a90: 6572 6976 6174 6976 653a 206f 7574 7075  erivative: outpu
-00014aa0: 7420 3d20 6274 2e7a 6572 6f73 285b 6e5f  t = bt.zeros([n_
-00014ab0: 6261 7463 685d 2c20 7b6e 5f64 696d 7d2c  batch], {n_dim},
-00014ac0: 202a 7368 6170 655f 6f75 742e 7370 6163   *shape_out.spac
-00014ad0: 6529 0a20 2020 2065 6c73 653a 206f 7574  e).    else: out
-00014ae0: 7075 7420 3d20 6274 2e7a 6572 6f73 2873  put = bt.zeros(s
-00014af0: 6861 7065 5f6f 7574 290a 2020 2020 666f  hape_out).    fo
-00014b00: 7220 4720 696e 2062 742e 696d 6167 655f  r G in bt.image_
-00014b10: 6772 6964 285b 325d 2a6e 5f64 696d 292e  grid([2]*n_dim).
-00014b20: 666c 6174 7465 6e28 292e 7472 616e 7370  flatten().transp
-00014b30: 6f73 6528 302c 2031 293a 0a20 2020 2020  ose(0, 1):.     
-00014b40: 2020 2023 2047 6574 2074 6865 2069 6e64     # Get the ind
-00014b50: 6963 6573 2066 6f72 2074 6865 2074 6572  ices for the ter
-00014b60: 6d3a 2062 595b 3a2c 2047 5b44 5d2c 2044  m: bY[:, G[D], D
-00014b70: 2c20 3a5d 2c20 7369 7a65 3d28 5b6e 5f62  , :], size=([n_b
-00014b80: 6174 6368 5d2c 207b 6e5f 6469 6d7d 2c20  atch], {n_dim}, 
-00014b90: 6e5f 6461 7461 290a 2020 2020 2020 2020  n_data).        
-00014ba0: 496e 6420 3d20 6259 2e67 6174 6865 7228  Ind = bY.gather(
-00014bb0: 312c 2047 2e65 7870 616e 645f 746f 285b  1, G.expand_to([
-00014bc0: 6e5f 6261 7463 685d 2c20 312c 207b 6e5f  n_batch], 1, {n_
-00014bd0: 6469 6d7d 2c20 6e5f 6461 7461 2929 2e73  dim}, n_data)).s
-00014be0: 7175 6565 7a65 2831 290a 2020 2020 2020  queeze(1).      
-00014bf0: 2020 2320 436c 616d 7020 7468 6520 696e    # Clamp the in
-00014c00: 6469 6365 7320 696e 2074 6865 2063 6f72  dices in the cor
-00014c10: 7265 6374 2072 616e 6765 2026 2043 6f6d  rect range & Com
-00014c20: 7075 7465 2074 6865 2062 6f72 6465 7220  pute the border 
-00014c30: 636f 6e64 6974 696f 6e0a 2020 2020 2020  condition.      
-00014c40: 2020 636f 6e64 6974 696f 6e20 3d20 6274    condition = bt
-00014c50: 2e73 756d 2828 496e 6420 3c20 3029 202b  .sum((Ind < 0) +
-00014c60: 2028 496e 6420 3e20 7369 7a65 202d 2031   (Ind > size - 1
-00014c70: 292c 2031 290a 2020 2020 2020 2020 496e  ), 1).        In
-00014c80: 6420 3d20 6274 2e6d 696e 2862 742e 636c  d = bt.min(bt.cl
-00014c90: 616d 7028 496e 642c 206d 696e 3d30 292c  amp(Ind, min=0),
-00014ca0: 2028 7369 7a65 202d 2031 292e 6578 7061   (size - 1).expa
-00014cb0: 6e64 5f74 6f28 496e 6429 290a 2020 2020  nd_to(Ind)).    
-00014cc0: 2020 2020 2320 436f 6e76 6572 7420 7468      # Convert th
-00014cd0: 6520 696e 6469 6365 7320 746f 2031 2064  e indices to 1 d
-00014ce0: 696d 656e 7369 6f6e 616c 2e20 446f 743a  imensional. Dot:
-00014cf0: 2028 5b6e 5f62 6174 6368 5d2c 206e 5f64   ([n_batch], n_d
-00014d00: 6174 6129 0a20 2020 2020 2020 2044 6f74  ata).        Dot
-00014d10: 203d 2049 6e64 5b3a 2c20 305d 0a20 2020   = Ind[:, 0].   
-00014d20: 2020 2020 2066 6f72 2072 2069 6e20 7261       for r in ra
-00014d30: 6e67 6528 312c 206e 5f64 696d 293a 2044  nge(1, n_dim): D
-00014d40: 6f74 202a 3d20 7369 7a65 5b72 5d3b 2044  ot *= size[r]; D
-00014d50: 6f74 202b 3d20 496e 645b 3a2c 2072 5d0a  ot += Ind[:, r].
-00014d60: 2020 2020 2020 2020 2320 4765 7420 7468          # Get th
-00014d70: 6520 696d 6167 6520 7661 6c75 6573 2049  e image values I
-00014d80: 563a 2028 5b6e 5f62 6174 6368 5d2c 206e  V: ([n_batch], n
-00014d90: 5f64 6174 6129 0a20 2020 2020 2020 2049  _data).        I
-00014da0: 5620 3d20 4e6f 6e65 0a20 2020 2020 2020  V = None.       
-00014db0: 2069 6620 6973 696e 7374 616e 6365 2866   if isinstance(f
-00014dc0: 696c 6c2c 2073 7472 293a 0a20 2020 2020  ill, str):.     
-00014dd0: 2020 2020 2020 2069 6620 6669 6c6c 2e6c         if fill.l
-00014de0: 6f77 6572 2829 203d 3d20 276e 6561 7265  ower() == 'neare
-00014df0: 7374 273a 0a20 2020 2020 2020 2020 2020  st':.           
-00014e00: 2020 2020 2049 5620 3d20 696d 6167 652e       IV = image.
-00014e10: 666c 6174 7465 6e28 292e 6761 7468 6572  flatten().gather
-00014e20: 2831 2c20 446f 7429 0a20 2020 2020 2020  (1, Dot).       
-00014e30: 2020 2020 2065 6c69 6620 6669 6c6c 2e6c       elif fill.l
-00014e40: 6f77 6572 2829 203d 3d20 2762 6163 6b67  ower() == 'backg
-00014e50: 726f 756e 6427 3a0a 2020 2020 2020 2020  round':.        
-00014e60: 2020 2020 2020 2020 626b 5f76 616c 7565          bk_value
-00014e70: 203d 2062 742e 7374 6163 6b28 5b69 6d61   = bt.stack([ima
-00014e80: 6765 5b28 736c 6963 6528 4e6f 6e65 292c  ge[(slice(None),
-00014e90: 2920 2b20 7475 706c 6528 6729 5d20 666f  ) + tuple(g)] fo
-00014ea0: 7220 6720 696e 2028 6274 2e69 6d61 6765  r g in (bt.image
-00014eb0: 5f67 7269 6428 5b32 5d2a 6e5f 6469 6d29  _grid([2]*n_dim)
-00014ec0: 202a 2062 742e 6368 616e 6e65 6c5f 7465   * bt.channel_te
-00014ed0: 6e73 6f72 2873 697a 652d 3129 292e 666c  nsor(size-1)).fl
-00014ee0: 6174 7465 6e28 292e 7472 616e 7370 6f73  atten().transpos
-00014ef0: 6528 302c 3129 5d2c 2031 292e 6d65 6469  e(0,1)], 1).medi
-00014f00: 616e 2831 292e 7661 6c75 6573 0a20 2020  an(1).values.   
-00014f10: 2020 2020 2020 2020 2020 2020 2062 6163               bac
-00014f20: 6b67 726f 756e 6420 3d20 626b 5f76 616c  kground = bk_val
-00014f30: 7565 202a 2062 742e 6f6e 6573 5f6c 696b  ue * bt.ones_lik
-00014f40: 6528 446f 7429 0a20 2020 2020 2020 2020  e(Dot).         
-00014f50: 2020 2065 6c69 6620 6669 6c6c 2e6c 6f77     elif fill.low
-00014f60: 6572 2829 203d 3d20 277a 6572 6f27 3a0a  er() == 'zero':.
-00014f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f80: 6261 636b 6772 6f75 6e64 203d 2062 742e  background = bt.
-00014f90: 7a65 726f 735f 6c69 6b65 2844 6f74 290a  zeros_like(Dot).
-00014fa0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00014fb0: 2020 2020 2020 2020 2020 6261 636b 6772            backgr
-00014fc0: 6f75 6e64 203d 2066 696c 6c20 2a20 6274  ound = fill * bt
-00014fd0: 2e6f 6e65 735f 6c69 6b65 2844 6f74 290a  .ones_like(Dot).
-00014fe0: 2020 2020 2020 2020 6966 2049 5620 6973          if IV is
-00014ff0: 204e 6f6e 653a 2049 5620 3d20 6274 2e77   None: IV = bt.w
-00015000: 6865 7265 2863 6f6e 6469 7469 6f6e 203e  here(condition >
-00015010: 3d20 312c 2062 6163 6b67 726f 756e 642e  = 1, background.
-00015020: 666c 6f61 7428 292c 2069 6d61 6765 2e66  float(), image.f
-00015030: 6c61 7474 656e 2829 2e67 6174 6865 7228  latten().gather(
-00015040: 312c 2044 6f74 292e 666c 6f61 7428 2929  1, Dot).float())
-00015050: 0a20 2020 2020 2020 2023 2057 6569 6768  .        # Weigh
-00015060: 7473 2066 6f72 2065 6163 6820 706f 696e  ts for each poin
-00015070: 743a 205b 7072 6f64 7563 7420 6f66 2057  t: [product of W
-00015080: 5b3a 2c20 475b 445d 2c20 442c 2078 5d20  [:, G[D], D, x] 
-00015090: 666f 7220 4420 696e 2072 616e 6765 286e  for D in range(n
-000150a0: 5f64 696d 295d 2066 6f72 2070 6f69 6e74  _dim)] for point
-000150b0: 2078 2e0a 2020 2020 2020 2020 2320 5767   x..        # Wg
-000150c0: 3a20 285b 6e5f 6261 7463 685d 2c20 7b6e  : ([n_batch], {n
-000150d0: 5f64 696d 7d2c 206e 5f64 6174 6129 0a20  _dim}, n_data). 
-000150e0: 2020 2020 2020 2057 6720 3d20 572e 6761         Wg = W.ga
-000150f0: 7468 6572 2831 2c20 472e 6578 7061 6e64  ther(1, G.expand
-00015100: 5f74 6f28 5b6e 5f62 6174 6368 5d2c 2031  _to([n_batch], 1
-00015110: 2c20 7b6e 5f64 696d 7d2c 206e 5f64 6174  , {n_dim}, n_dat
-00015120: 6129 292e 7371 7565 657a 6528 3129 0a20  a)).squeeze(1). 
-00015130: 2020 2020 2020 2069 6620 6e6f 7420 6465         if not de
-00015140: 7269 7661 7469 7665 3a0a 2020 2020 2020  rivative:.      
-00015150: 2020 2020 2020 6f75 7470 7574 202b 3d20        output += 
-00015160: 2857 672e 7072 6f64 2831 2920 2a20 4956  (Wg.prod(1) * IV
-00015170: 292e 7669 6577 5f61 7328 6f75 7470 7574  ).view_as(output
-00015180: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00015190: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-000151a0: 5767 4d61 7420 3d20 5767 2e6d 756c 7469  WgMat = Wg.multi
-000151b0: 706c 7928 6e5f 6469 6d2c 2031 2920 2320  ply(n_dim, 1) # 
-000151c0: 285b 6e5f 6261 7463 685d 2c20 6e5f 6469  ([n_batch], n_di
-000151d0: 6d2c 207b 6e5f 6469 6d7d 2c20 6e5f 6461  m, {n_dim}, n_da
-000151e0: 7461 290a 2020 2020 2020 2020 2020 2020  ta).            
-000151f0: 7465 6d70 5767 4d61 745b 3a2c 2062 742e  tempWgMat[:, bt.
-00015200: 6172 616e 6765 286e 5f64 696d 292c 2062  arange(n_dim), b
-00015210: 742e 6172 616e 6765 286e 5f64 696d 295d  t.arange(n_dim)]
-00015220: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
-00015230: 2064 5767 203d 2074 656d 7057 674d 6174   dWg = tempWgMat
-00015240: 2e70 726f 6428 3129 202a 2028 4720 2a20  .prod(1) * (G * 
-00015250: 3220 2d20 3129 2e66 6c6f 6174 2829 0a20  2 - 1).float(). 
-00015260: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-00015270: 7420 2b3d 2028 6457 6720 2a20 4956 2e75  t += (dWg * IV.u
-00015280: 6e73 7175 6565 7a65 2831 2929 2e76 6965  nsqueeze(1)).vie
-00015290: 775f 6173 286f 7574 7075 7429 0a20 2020  w_as(output).   
-000152a0: 2062 742e 746f 7263 682e 6375 6461 2e65   bt.torch.cuda.e
-000152b0: 6d70 7479 5f63 6163 6865 2829 0a20 2020  mpty_cache().   
-000152c0: 2065 7073 203d 2031 652d 360a 2020 2020   eps = 1e-6.    
-000152d0: 6d20 3d20 3020 6966 2069 6d61 6765 2e6d  m = 0 if image.m
-000152e0: 696e 2829 203e 202d 6570 7320 656c 7365  in() > -eps else
-000152f0: 2069 6d61 6765 2e6d 696e 2829 2e69 7465   image.min().ite
-00015300: 6d28 290a 2020 2020 4d20 3d20 3120 6966  m().    M = 1 if
-00015310: 2069 6d61 6765 2e6d 6178 2829 203c 2031   image.max() < 1
-00015320: 202b 2065 7073 2065 6c73 6520 696d 6167   + eps else imag
-00015330: 652e 6d61 7828 292e 6974 656d 2829 0a20  e.max().item(). 
-00015340: 2020 2072 6574 7572 6e20 6f75 7470 7574     return output
-00015350: 2e63 6c61 6d70 286d 2c20 4d29 0a0a 4061  .clamp(m, M)..@a
-00015360: 6c69 6173 2822 7265 7361 6d70 6c65 5f66  lias("resample_f
-00015370: 6f72 7761 7264 2229 0a64 6566 2069 6e74  orward").def int
-00015380: 6572 706f 6c61 7469 6f6e 5f66 6f72 7761  erpolation_forwa
-00015390: 7264 280a 2020 2020 2020 2020 696d 6167  rd(.        imag
-000153a0: 652c 200a 2020 2020 2020 2020 7472 616e  e, .        tran
-000153b0: 7320 3d20 4e6f 6e65 2c20 0a20 2020 2020  s = None, .     
-000153c0: 2020 206d 6574 686f 6420 3d20 274c 696e     method = 'Lin
-000153d0: 6561 7227 2c20 0a20 2020 2020 2020 2074  ear', .        t
-000153e0: 6172 6765 745f 7370 6163 6520 3d20 4e6f  arget_space = No
-000153f0: 6e65 2c0a 2020 2020 2020 2020 6669 6c6c  ne,.        fill
-00015400: 203d 2027 7a65 726f 272c 0a20 2020 2020   = 'zero',.     
-00015410: 2020 2064 6572 6976 6174 6976 6520 3d20     derivative = 
-00015420: 4661 6c73 650a 2020 2020 293a 0a20 2020  False.    ):.   
-00015430: 2027 2727 0a20 2020 2049 6e74 6572 706f   '''.    Interpo
-00015440: 6c61 7465 2075 7369 6e67 2066 6f72 7761  late using forwa
-00015450: 7264 2074 7261 6e73 666f 726d 6174 696f  rd transformatio
-00015460: 6e2e 2049 7420 6973 206e 6f74 2079 6574  n. It is not yet
-00015470: 2069 6d70 6c65 6d65 6e74 6564 2e20 0a20   implemented. . 
-00015480: 2020 2069 2e65 2e20 436f 6d70 7574 6520     i.e. Compute 
-00015490: 7468 6520 696d 6167 6520 4920 732e 742e  the image I s.t.
-000154a0: 2074 7261 6e73 2878 2920 3d20 7920 666f   trans(x) = y fo
-000154b0: 7220 7820 696e 2069 6e70 7574 2069 6d61  r x in input ima
-000154c0: 6765 2061 6e64 2079 2069 6e20 7468 6520  ge and y in the 
-000154d0: 6f75 7470 7574 2049 2075 7369 6e67 2069  output I using i
-000154e0: 6e74 6572 706f 6c61 7469 6f6e 206d 6574  nterpolation met
-000154f0: 686f 643a 0a20 2020 2020 2020 206d 6574  hod:.        met
-00015500: 686f 6420 3d20 4c69 6e65 6172 205b 4e4f  hod = Linear [NO
-00015510: 2047 5241 4449 454e 5421 2121 5d3a 2042   GRADIENT!!!]: B
-00015520: 696c 696e 6561 7220 696e 7465 7270 6f6c  ilinear interpol
-00015530: 6174 696f 6e0a 2020 2020 2020 2020 6d65  ation.        me
-00015540: 7468 6f64 203d 204e 6561 7265 7374 205b  thod = Nearest [
-00015550: 4e4f 2047 5241 4449 454e 5421 2121 5d3a  NO GRADIENT!!!]:
-00015560: 204e 6561 7265 7374 2069 6e74 6572 706f   Nearest interpo
-00015570: 6c61 7469 6f6e 0a0a 2020 2020 5061 7261  lation..    Para
-00015580: 6d73 3a0a 2020 2020 2020 2020 696d 6167  ms:.        imag
-00015590: 6520 5b62 742e 5465 6e73 6f72 5d3a 2054  e [bt.Tensor]: T
-000155a0: 6865 2074 6172 6765 7420 696d 6167 652e  he target image.
-000155b0: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
-000155c0: 653a 2028 5b6e 5f62 6174 6368 3a6f 7074  e: ([n_batch:opt
-000155d0: 696f 6e61 6c5d 2c20 7b6e 5f63 6861 6e6e  ional], {n_chann
-000155e0: 656c 3a6f 7074 696f 6e61 6c7d 2c20 6d40  el:optional}, m@
-000155f0: 312c 206d 4032 2c20 2e2e 2e2c 206d 406e  1, m@2, ..., m@n
-00015600: 5f64 696d 290a 2020 2020 2020 2020 7472  _dim).        tr
-00015610: 616e 7320 5b46 756e 6374 696f 6e20 6f72  ans [Function or
-00015620: 206d 6963 6f6d 7075 7469 6e67 2e53 7061   micomputing.Spa
-00015630: 7469 616c 5472 616e 7366 6f72 6d61 7469  tialTransformati
-00015640: 6f6e 5d3a 2054 7261 6e73 666f 726d 6174  on]: Transformat
-00015650: 696f 6e20 6675 6e63 7469 6f6e 2c20 6d61  ion function, ma
-00015660: 7070 696e 670a 2020 2020 2020 2020 2020  pping.          
-00015670: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
-00015680: 683a 6f70 7469 6f6e 616c 5d2c 207b 6e5f  h:optional], {n_
-00015690: 6469 6d7d 2c20 6e40 312c 206e 4032 2c20  dim}, n@1, n@2, 
-000156a0: 2e2e 2e2c 206e 406e 5f64 696d 2920 746f  ..., n@n_dim) to
-000156b0: 2028 5b6e 5f62 6174 6368 5d2c 207b 6e5f   ([n_batch], {n_
-000156c0: 6469 6d7d 2c20 6e40 312c 206e 4032 2c20  dim}, n@1, n@2, 
-000156d0: 2e2e 2e2c 206e 406e 5f64 696d 290a 2020  ..., n@n_dim).  
-000156e0: 2020 2020 2020 6d65 7468 6f64 205b 7374        method [st
-000156f0: 723a 206c 696e 6561 727c 6e65 6172 6573  r: linear|neares
-00015700: 745d 3a20 5468 6520 696e 7465 7270 6f6c  t]: The interpol
-00015710: 6174 696f 6e20 6d65 7468 6f64 2e20 0a20  ation method. . 
-00015720: 2020 2020 2020 2074 6172 6765 745f 7370         target_sp
-00015730: 6163 6520 5b74 7570 6c65 206f 7220 6274  ace [tuple or bt
-00015740: 2e54 656e 736f 725d 3a0a 2020 2020 2020  .Tensor]:.      
-00015750: 2020 2020 2020 5369 7a65 2028 7475 706c        Size (tupl
-00015760: 6529 206f 6620 6120 7461 7267 6574 2052  e) of a target R
-00015770: 4f49 2061 7420 7468 6520 6365 6e74 6572  OI at the center
-00015780: 206f 6620 696d 6167 652e 200a 2020 2020   of image. .    
-00015790: 2020 2020 2020 2020 4f52 2054 7261 6e73          OR Trans
-000157a0: 666f 726d 6564 2063 6f6f 7264 696e 6174  formed coordinat
-000157b0: 6520 7370 6163 6520 2862 742e 5465 6e73  e space (bt.Tens
-000157c0: 6f72 2920 6f66 2074 6865 206f 7574 7075  or) of the outpu
-000157d0: 7420 696d 6167 652e 200a 2020 2020 2020  t image. .      
-000157e0: 2020 2020 2020 7369 7a65 3a20 6c65 6e67        size: leng
-000157f0: 7468 286e 5f64 696d 2920 6f72 2028 5b6e  th(n_dim) or ([n
-00015800: 5f62 6174 6368 3a6f 7074 696f 6e61 6c5d  _batch:optional]
-00015810: 2c20 7b6e 5f64 696d 3a6f 7074 696f 6e61  , {n_dim:optiona
-00015820: 6c7d 2c20 7369 7a65 4031 2c20 7369 7a65  l}, size@1, size
-00015830: 4032 2c20 2e2e 2e2c 2073 697a 6540 6e5f  @2, ..., size@n_
-00015840: 6469 6d29 0a20 2020 2020 2020 2066 696c  dim).        fil
-00015850: 6c20 5b73 7472 3a20 6e65 6172 6573 747c  l [str: nearest|
-00015860: 6261 636b 6772 6f75 6e64 206f 7220 696e  background or in
-00015870: 7420 6f72 2066 6c6f 6174 286e 756d 6265  t or float(numbe
-00015880: 7229 5d3a 2049 6e64 6963 6174 6520 7468  r)]: Indicate th
-00015890: 6520 7761 7920 746f 2066 696c 6c20 6261  e way to fill ba
-000158a0: 636b 6772 6f75 6e64 206f 7574 7369 6465  ckground outside
-000158b0: 2060 5375 7272 6f75 6e64 696e 6760 2e20   `Surrounding`. 
-000158c0: 0a20 2020 2020 2020 2064 6572 6976 6174  .        derivat
-000158d0: 6976 6520 5b62 6f6f 6c5d 3a20 5768 6574  ive [bool]: Whet
-000158e0: 6865 7220 746f 2072 6574 7572 6e20 7468  her to return th
-000158f0: 6520 6772 6164 6965 6e74 2e20 4f6e 6520  e gradient. One 
-00015900: 6361 6e20 6f6d 6974 2069 7420 7768 656e  can omit it when
-00015910: 2075 7369 6e67 2074 6f72 6368 2e61 7574   using torch.aut
-00015920: 6f67 7261 642e 0a0a 2020 2020 2020 2020  ograd...        
-00015930: 6f75 7470 7574 205b 6274 2e54 656e 736f  output [bt.Tenso
-00015940: 725d 3a20 5468 6520 7472 616e 7366 6f72  r]: The transfor
-00015950: 6d65 6420 696d 6167 652e 0a20 2020 2020  med image..     
-00015960: 2020 2020 2020 2073 697a 653a 2028 5b6e         size: ([n
-00015970: 5f62 6174 6368 5d2c 207b 6e5f 6368 616e  _batch], {n_chan
-00015980: 6e65 6c3a 6f70 7469 6f6e 616c 7d2c 206d  nel:optional}, m
-00015990: 4031 2c20 6d40 322c 202e 2e2e 2c20 6d40  @1, m@2, ..., m@
-000159a0: 6e5f 6469 6d29 0a20 2020 2020 2020 2020  n_dim).         
-000159b0: 2020 206f 7220 7768 656e 2060 7461 7267     or when `targ
-000159c0: 6574 5f73 7061 6365 6020 6973 2064 6566  et_space` is def
-000159d0: 696e 6564 2062 7920 7465 6e73 6f72 2e20  ined by tensor. 
-000159e0: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
-000159f0: 653a 2028 5b6e 5f62 6174 6368 5d2c 2073  e: ([n_batch], s
-00015a00: 697a 6540 312c 2073 697a 6540 322c 202e  ize@1, size@2, .
-00015a10: 2e2e 2c20 7369 7a65 406e 5f64 696d 290a  .., size@n_dim).
-00015a20: 2020 2020 2020 2020 2020 2020 6f72 2074              or t
-00015a30: 6865 2064 6572 6976 6174 6976 6520 666f  he derivative fo
-00015a40: 7220 7468 6520 696e 7465 7270 6f6c 6174  r the interpolat
-00015a50: 696f 6e2e 2028 6966 2060 6465 7269 7661  ion. (if `deriva
-00015a60: 7469 7665 203d 2054 7275 6560 290a 2020  tive = True`).  
-00015a70: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
-00015a80: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f64  ([n_batch], {n_d
-00015a90: 696d 7d2c 2073 697a 6540 312c 2073 697a  im}, size@1, siz
-00015aa0: 6540 322c 202e 2e2e 2c20 7369 7a65 406e  e@2, ..., size@n
-00015ab0: 5f64 696d 290a 0a20 2020 2045 7861 6d70  _dim)..    Examp
-00015ac0: 6c65 733a 0a20 2020 202d 2d2d 2d2d 2d2d  les:.    -------
-00015ad0: 2d2d 2d0a 2020 2020 3e3e 3e20 496d 6167  ---.    >>> Imag
-00015ae0: 6520 3d20 6274 2e72 616e 6428 332c 2031  e = bt.rand(3, 1
-00015af0: 3030 2c20 3132 302c 2038 3029 0a20 2020  00, 120, 80).   
-00015b00: 203e 3e3e 2041 4d20 3d20 6274 2e72 616e   >>> AM = bt.ran
-00015b10: 6428 342c 2034 290a 2020 2020 3e3e 3e20  d(4, 4).    >>> 
-00015b20: 414d 5b33 2c20 3a5d 203d 2062 742e 6f6e  AM[3, :] = bt.on
-00015b30: 655f 686f 7428 2d31 2c20 3429 0a20 2020  e_hot(-1, 4).   
-00015b40: 203e 3e3e 2069 6e74 6572 706f 6c61 7469   >>> interpolati
-00015b50: 6f6e 2849 6d61 6765 2c20 4166 6669 6e65  on(Image, Affine
-00015b60: 2841 4d29 2c20 6d65 7468 6f64 3d27 4c69  (AM), method='Li
-00015b70: 6e65 6172 2729 0a20 2020 2027 2727 0a20  near').    '''. 
-00015b80: 2020 2069 6620 7472 616e 7320 6973 206e     if trans is n
-00015b90: 6f74 204e 6f6e 6520 616e 6420 7472 616e  ot None and tran
-00015ba0: 732e 6261 636b 7761 7264 3a0a 2020 2020  s.backward:.    
-00015bb0: 2020 2020 6966 2068 6173 6174 7472 2874      if hasattr(t
-00015bc0: 7261 6e73 2c20 2769 6e76 2729 3a20 7472  rans, 'inv'): tr
-00015bd0: 616e 7320 3d20 7472 616e 732e 696e 7628  ans = trans.inv(
-00015be0: 292e 6661 6b65 5f69 6e76 2829 0a20 2020  ).fake_inv().   
-00015bf0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00015c00: 2020 2020 2020 2070 7269 6e74 2822 5761         print("Wa
-00015c10: 726e 696e 673a 2042 6163 6b77 6172 6420  rning: Backward 
-00015c20: 7472 616e 7366 6f72 6d61 7469 6f6e 2066  transformation f
-00015c30: 6f75 6e64 2069 6e20 6d65 7468 6f64 2060  ound in method `
-00015c40: 696e 7465 7270 6f6c 6174 696f 6e5f 666f  interpolation_fo
-00015c50: 7277 6172 6460 2e20 5573 696e 6720 6069  rward`. Using `i
-00015c60: 6e74 6572 706f 6c61 7469 6f6e 6020 696e  nterpolation` in
-00015c70: 7374 6561 642e 2022 290a 2020 2020 2020  stead. ").      
-00015c80: 2020 2020 2020 7265 7475 726e 2069 6e74        return int
-00015c90: 6572 706f 6c61 7469 6f6e 2869 6d61 6765  erpolation(image
-00015ca0: 2c20 7472 616e 732c 206d 6574 686f 6420  , trans, method 
-00015cb0: 3d20 6d65 7468 6f64 2c20 7461 7267 6574  = method, target
-00015cc0: 5f73 7061 6365 203d 2074 6172 6765 745f  _space = target_
-00015cd0: 7370 6163 652c 2066 696c 6c20 3d20 6669  space, fill = fi
-00015ce0: 6c6c 290a 2020 2020 7265 7475 726e 204e  ll).    return N
-00015cf0: 6f74 496d 706c 656d 656e 7465 640a 0a23  otImplemented..#
-00015d00: 2323 2323 2323 2323 2323 2320 496d 6167  ########### Imag
-00015d10: 6520 5472 616e 7366 6f72 6d61 7469 6f6e  e Transformation
-00015d20: 7320 2323 2323 2323 2323 2323 2323 0a0a  s ############..
-00015d30: 636c 6173 7320 496d 6167 6554 7261 6e73  class ImageTrans
-00015d40: 666f 726d 6174 696f 6e28 5472 616e 7366  formation(Transf
-00015d50: 6f72 6d61 7469 6f6e 293a 0a20 2020 2020  ormation):.     
-00015d60: 2020 200a 2020 2020 6465 6620 5f5f 6361     .    def __ca
-00015d70: 6c6c 5f5f 2873 656c 662c 2058 293a 0a20  ll__(self, X):. 
-00015d80: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00015d90: 2020 2058 205b 6274 2e54 656e 736f 725d     X [bt.Tensor]
-00015da0: 3a20 496d 6167 6520 746f 2062 6520 7472  : Image to be tr
-00015db0: 616e 7366 6f72 6d65 642e 0a20 2020 2020  ansformed..     
-00015dc0: 2020 2020 2020 2073 697a 653a 2028 5b6e         size: ([n
-00015dd0: 5f62 6174 6368 3a6f 7074 696f 6e61 6c5d  _batch:optional]
-00015de0: 2c20 7b6e 5f63 6861 6e6e 656c 3a6f 7074  , {n_channel:opt
-00015df0: 696f 6e61 6c7d 2c20 6e40 312c 206e 4032  ional}, n@1, n@2
-00015e00: 2c20 2e2e 2e2c 206e 406e 5f64 696d 290a  , ..., n@n_dim).
-00015e10: 2020 2020 2020 2020 6f75 7470 7574 205b          output [
-00015e20: 6274 2e54 656e 736f 725d 3a20 5468 6520  bt.Tensor]: The 
-00015e30: 7472 616e 7366 6f72 6d65 6420 696d 6167  transformed imag
-00015e40: 652e 0a20 2020 2020 2020 2020 2020 2073  e..            s
-00015e50: 697a 653a 2028 5b6e 5f62 6174 6368 5d2c  ize: ([n_batch],
-00015e60: 207b 6e5f 6368 616e 6e65 6c7d 2c20 6e40   {n_channel}, n@
-00015e70: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
-00015e80: 5f64 696d 290a 2020 2020 2020 2020 2727  _dim).        ''
-00015e90: 270a 2020 2020 2020 2020 5820 3d20 6261  '.        X = ba
-00015ea0: 746f 7263 685f 7465 6e73 6f72 2858 290a  torch_tensor(X).
-00015eb0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00015ec0: 6e5f 6469 6d20 6973 204e 6f6e 653a 0a20  n_dim is None:. 
-00015ed0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00015ee0: 7420 582e 6861 735f 6261 7463 683a 2058  t X.has_batch: X
-00015ef0: 203d 2058 2e75 6e73 7175 6565 7a65 285b   = X.unsqueeze([
-00015f00: 5d29 0a20 2020 2020 2020 2020 2020 2069  ]).            i
-00015f10: 6620 6e6f 7420 582e 6861 735f 6368 616e  f not X.has_chan
-00015f20: 6e65 6c3a 2058 203d 2058 2e73 7461 6e64  nel: X = X.stand
-00015f30: 6172 6428 292e 756e 7371 7565 657a 6528  ard().unsqueeze(
-00015f40: 7b31 7d29 0a20 2020 2020 2020 2065 6c73  {1}).        els
-00015f50: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00015f60: 6620 582e 6e5f 6469 6d20 3d3d 2073 656c  f X.n_dim == sel
-00015f70: 662e 6e5f 6469 6d3a 2058 203d 2058 2e72  f.n_dim: X = X.r
-00015f80: 656d 6f76 655f 7370 6563 6961 6c5f 2829  emove_special_()
-00015f90: 2e75 6e73 7175 6565 7a65 285b 5d29 2e75  .unsqueeze([]).u
-00015fa0: 6e73 7175 6565 7a65 287b 317d 290a 2020  nsqueeze({1}).  
-00015fb0: 2020 2020 2020 2020 2020 656c 6966 2058            elif X
-00015fc0: 2e6e 5f64 696d 203d 3d20 7365 6c66 2e6e  .n_dim == self.n
-00015fd0: 5f64 696d 202b 2031 3a0a 2020 2020 2020  _dim + 1:.      
-00015fe0: 2020 2020 2020 2020 2020 6966 2058 2e68            if X.h
-00015ff0: 6173 5f62 6174 6368 3a20 582e 6368 616e  as_batch: X.chan
-00016000: 6e65 6c5f 6469 6d65 6e73 696f 6e20 3d20  nel_dimension = 
-00016010: 4e6f 6e65 3b20 5820 3d20 582e 756e 7371  None; X = X.unsq
-00016020: 7565 657a 6528 7b30 2069 6620 582e 6261  ueeze({0 if X.ba
-00016030: 7463 685f 6469 6d65 6e73 696f 6e20 3e20  tch_dimension > 
-00016040: 3020 656c 7365 2031 7d29 0a20 2020 2020  0 else 1}).     
-00016050: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00016060: 582e 6861 735f 6368 616e 6e65 6c3a 2058  X.has_channel: X
-00016070: 203d 2058 2e75 6e73 7175 6565 7a65 285b   = X.unsqueeze([
-00016080: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00016090: 2020 2065 6c73 653a 2058 203d 2058 2e62     else: X = X.b
-000160a0: 6174 6368 5f64 696d 656e 7369 6f6e 5f28  atch_dimension_(
-000160b0: 3029 2e75 6e73 7175 6565 7a65 287b 317d  0).unsqueeze({1}
-000160c0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-000160d0: 6966 2058 2e6e 5f64 696d 203d 3d20 7365  if X.n_dim == se
-000160e0: 6c66 2e6e 5f64 696d 202b 2032 3a0a 2020  lf.n_dim + 2:.  
-000160f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00016100: 5f63 6861 6e6e 616c 2f62 6174 6368 2064  _channal/batch d
-00016110: 696d 656e 7369 6f6e 7320 7573 6564 2068  imensions used h
-00016120: 6572 6520 6173 2074 6865 7920 6172 6520  ere as they are 
-00016130: 6e5f 6469 6d20 7768 656e 206e 6f74 2065  n_dim when not e
-00016140: 7869 7374 6564 2e20 0a20 2020 2020 2020  xisted. .       
-00016150: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00016160: 582e 6861 735f 6261 7463 683a 2058 2e62  X.has_batch: X.b
-00016170: 6174 6368 5f64 696d 656e 7369 6f6e 203d  atch_dimension =
-00016180: 2030 2069 6620 582e 5f63 6861 6e6e 656c   0 if X._channel
-00016190: 5f64 696d 656e 7369 6f6e 203e 2030 2065  _dimension > 0 e
-000161a0: 6c73 6520 310a 2020 2020 2020 2020 2020  lse 1.          
-000161b0: 2020 2020 2020 6966 206e 6f74 2058 2e68        if not X.h
-000161c0: 6173 5f63 6861 6e6e 656c 3a20 582e 6368  as_channel: X.ch
-000161d0: 616e 6e65 6c5f 6469 6d65 6e73 696f 6e20  annel_dimension 
-000161e0: 3d20 3020 6966 2058 2e5f 6261 7463 685f  = 0 if X._batch_
-000161f0: 6469 6d65 6e73 696f 6e20 3e20 3020 656c  dimension > 0 el
-00016200: 7365 2031 0a20 2020 2020 2020 2061 766f  se 1.        avo
-00016210: 7563 6828 582e 6861 735f 6261 7463 6820  uch(X.has_batch 
-00016220: 616e 6420 582e 6861 735f 6368 616e 6e65  and X.has_channe
-00016230: 6c2c 2066 2250 6c65 6173 6520 7573 6520  l, f"Please use 
-00016240: 6261 746f 7263 6820 7465 6e73 6f72 206f  batorch tensor o
-00016250: 6620 7369 7a65 205c 0a20 2020 2020 2020  f size \.       
-00016260: 2020 2020 2028 5b6e 5f62 6174 6368 5d2c       ([n_batch],
-00016270: 207b 7b6e 5f63 6861 6e6e 656c 2f6e 5f66   {{n_channel/n_f
-00016280: 6561 7475 7265 3a6f 7074 696f 6e61 6c7d  eature:optional}
-00016290: 7d2c 206d 5f31 2c20 6d5f 322c 202e 2e2e  }, m_1, m_2, ...
-000162a0: 2c20 6d5f 7229 205b 723d 6e5f 6469 6d5d  , m_r) [r=n_dim]
-000162b0: 2066 6f72 205c 0a20 2020 2020 2020 2020   for \.         
-000162c0: 2020 2020 2020 207b 7365 6c66 2e5f 5f63         {self.__c
-000162d0: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f2e  lass__.__name__.
-000162e0: 7370 6c69 7428 272e 2729 5b2d 315d 7d20  split('.')[-1]} 
-000162f0: 5472 616e 7366 6f72 6d61 7469 6f6e 2c20  Transformation, 
-00016300: 696e 7374 6561 6420 6f66 207b 582e 7368  instead of {X.sh
-00016310: 6170 657d 2e20 2229 0a20 2020 2020 2020  ape}. ").       
-00016320: 2072 6574 7572 6e20 582e 636c 6f6e 6528   return X.clone(
-00016330: 290a 0a63 6c61 7373 204e 6f72 6d61 6c69  )..class Normali
-00016340: 7a65 2849 6d61 6765 5472 616e 7366 6f72  ze(ImageTransfor
-00016350: 6d61 7469 6f6e 293a 0a20 2020 2064 6566  mation):.    def
-00016360: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00016370: 2a5f 7261 6e67 6529 3a0a 2020 2020 2020  *_range):.      
-00016380: 2020 2727 270a 2020 2020 2020 2020 4e6f    '''.        No
-00016390: 726d 616c 697a 6520 7468 6520 696e 7465  rmalize the inte
-000163a0: 6e73 6974 7920 6f66 2061 6e20 696d 6167  nsity of an imag
-000163b0: 652e 0a20 2020 2020 2020 200a 2020 2020  e..        .    
-000163c0: 2020 2020 5061 7261 6d73 3a0a 2020 2020      Params:.    
-000163d0: 2020 2020 2020 2020 5f72 616e 6765 203d          _range =
-000163e0: 2028 6c6f 772c 2068 6967 6829 205b 696e   (low, high) [in
-000163f0: 7420 6f72 2066 6c6f 6174 206f 7220 6274  t or float or bt
-00016400: 2e54 656e 736f 725d 3a20 5468 6520 6c6f  .Tensor]: The lo
-00016410: 7765 7374 2028 616e 6420 6869 6768 6573  west (and highes
-00016420: 7429 2069 6e74 656e 7369 7479 2e20 0a20  t) intensity. . 
-00016430: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016440: 697a 653a 206c 656e 6774 6828 3229 206f  ize: length(2) o
-00016450: 7220 285b 6e5f 6261 7463 685d 2c20 7b32  r ([n_batch], {2
-00016460: 7d29 0a20 2020 2020 2020 2020 2020 200a  }).            .
-00016470: 2020 2020 2020 2020 5768 656e 2069 7420          When it 
-00016480: 6973 2063 616c 6c65 643a 0a20 2020 2020  is called:.     
-00016490: 2020 2020 2020 2058 205b 6274 2e54 656e         X [bt.Ten
-000164a0: 736f 725d 3a20 496d 6167 6520 746f 2062  sor]: Image to b
-000164b0: 6520 7472 616e 7366 6f72 6d65 642e 0a20  e transformed.. 
-000164c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000164d0: 697a 653a 2028 5b6e 5f62 6174 6368 3a6f  ize: ([n_batch:o
-000164e0: 7074 696f 6e61 6c5d 2c20 7b6e 5f63 6861  ptional], {n_cha
-000164f0: 6e6e 656c 3a6f 7074 696f 6e61 6c7d 2c20  nnel:optional}, 
-00016500: 6e40 312c 206e 4032 2c20 2e2e 2e2c 206e  n@1, n@2, ..., n
-00016510: 406e 5f64 696d 290a 2020 2020 2020 2020  @n_dim).        
-00016520: 2020 2020 6f75 7470 7574 205b 6274 2e54      output [bt.T
-00016530: 656e 736f 725d 3a20 5468 6520 7472 616e  ensor]: The tran
-00016540: 7366 6f72 6d65 6420 696d 6167 652e 0a20  sformed image.. 
-00016550: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016560: 697a 653a 2028 5b6e 5f62 6174 6368 5d2c  ize: ([n_batch],
-00016570: 207b 6e5f 6368 616e 6e65 6c7d 2c20 6e40   {n_channel}, n@
-00016580: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
-00016590: 5f64 696d 290a 2020 2020 2020 2020 2727  _dim).        ''
-000165a0: 270a 2020 2020 2020 2020 6966 206c 656e  '.        if len
-000165b0: 285f 7261 6e67 6529 203d 3d20 303a 205f  (_range) == 0: _
-000165c0: 7261 6e67 6520 3d20 4e6f 6e65 0a20 2020  range = None.   
-000165d0: 2020 2020 2065 6c69 6620 6c65 6e28 5f72       elif len(_r
-000165e0: 616e 6765 2920 3d3d 2031 2061 6e64 2069  ange) == 1 and i
-000165f0: 7369 6e73 7461 6e63 6528 5f72 616e 6765  sinstance(_range
-00016600: 5b30 5d2c 2028 6c69 7374 2c20 7475 706c  [0], (list, tupl
-00016610: 6529 293a 205f 7261 6e67 6520 3d20 6261  e)): _range = ba
-00016620: 746f 7263 685f 7465 6e73 6f72 286c 6973  torch_tensor(lis
-00016630: 7428 5f72 616e 6765 5b30 5d29 290a 2020  t(_range[0])).  
-00016640: 2020 2020 2020 656c 6966 206c 656e 285f        elif len(_
-00016650: 7261 6e67 6529 203d 3d20 3120 616e 6420  range) == 1 and 
-00016660: 6973 696e 7374 616e 6365 285f 7261 6e67  isinstance(_rang
-00016670: 655b 305d 2c20 6274 2e54 656e 736f 7229  e[0], bt.Tensor)
-00016680: 3a20 5f72 616e 6765 203d 205f 7261 6e67  : _range = _rang
-00016690: 655b 305d 0a20 2020 2020 2020 2065 6c69  e[0].        eli
-000166a0: 6620 6c65 6e28 5f72 616e 6765 2920 3d3d  f len(_range) ==
-000166b0: 2031 3a20 5f72 616e 6765 203d 2062 742e   1: _range = bt.
-000166c0: 6368 616e 6e65 6c5f 7465 6e73 6f72 2828  channel_tensor((
-000166d0: 302c 205f 7261 6e67 6529 290a 2020 2020  0, _range)).    
-000166e0: 2020 2020 656c 6966 206c 656e 285f 7261      elif len(_ra
-000166f0: 6e67 6529 203d 3d20 323a 205f 7261 6e67  nge) == 2: _rang
-00016700: 6520 3d20 6274 2e63 6861 6e6e 656c 5f74  e = bt.channel_t
-00016710: 656e 736f 7228 5f72 616e 6765 290a 2020  ensor(_range).  
-00016720: 2020 2020 2020 656c 7365 3a20 7261 6973        else: rais
-00016730: 6520 5479 7065 4572 726f 7228 6622 496e  e TypeError(f"In
-00016740: 7661 6c69 6420 7261 6e67 6520 666f 7220  valid range for 
-00016750: 4e6f 726d 616c 697a 653a 207b 5f72 616e  Normalize: {_ran
-00016760: 6765 7d2e 2022 290a 2020 2020 2020 2020  ge}. ").        
-00016770: 6966 205f 7261 6e67 6520 6973 204e 6f6e  if _range is Non
-00016780: 653a 2070 6173 730a 2020 2020 2020 2020  e: pass.        
-00016790: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000167a0: 2020 6966 205f 7261 6e67 652e 6e5f 6469    if _range.n_di
-000167b0: 6d20 3c20 323a 205f 7261 6e67 6520 3d20  m < 2: _range = 
-000167c0: 5f72 616e 6765 2e75 6e73 7175 6565 7a65  _range.unsqueeze
-000167d0: 285b 5d29 0a20 2020 2020 2020 2020 2020  ([]).           
-000167e0: 2069 6620 6e6f 7420 5f72 616e 6765 2e68   if not _range.h
-000167f0: 6173 5f62 6174 6368 3a20 5f72 616e 6765  as_batch: _range
-00016800: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
-00016810: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
-00016820: 2069 6620 6e6f 7420 5f72 616e 6765 2e68   if not _range.h
-00016830: 6173 5f63 6861 6e6e 656c 3a20 5f72 616e  as_channel: _ran
-00016840: 6765 2e63 6861 6e6e 656c 5f64 696d 656e  ge.channel_dimen
-00016850: 7369 6f6e 203d 2031 0a20 2020 2020 2020  sion = 1.       
-00016860: 2020 2020 2061 766f 7563 6828 5f72 616e       avouch(_ran
-00016870: 6765 2e68 6173 5f62 6174 6368 2061 6e64  ge.has_batch and
-00016880: 205f 7261 6e67 652e 6861 735f 6368 616e   _range.has_chan
-00016890: 6e65 6c2c 2066 2250 6c65 6173 6520 7573  nel, f"Please us
-000168a0: 6520 6261 746f 7263 6820 7465 6e73 6f72  e batorch tensor
-000168b0: 206f 6620 7369 7a65 205c 0a20 2020 2020   of size \.     
-000168c0: 2020 2020 2020 2020 2020 2028 5b6e 5f62             ([n_b
-000168d0: 6174 6368 3a6f 7074 696f 6e61 6c5d 2c20  atch:optional], 
-000168e0: 7b7b 327d 7d29 2066 6f72 204e 6f72 6d61  {{2}}) for Norma
-000168f0: 6c69 7a69 6e67 2070 6172 616d 6574 6572  lizing parameter
-00016900: 732c 2069 6e73 7465 6164 206f 6620 7b5f  s, instead of {_
-00016910: 7261 6e67 652e 7368 6170 657d 2e20 2229  range.shape}. ")
-00016920: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-00016930: 2e5f 5f69 6e69 745f 5f28 5f72 616e 6765  .__init__(_range
-00016940: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
-00016950: 616e 6765 203d 205f 7261 6e67 650a 2020  ange = _range.  
-00016960: 2020 2020 2020 7365 6c66 2e5f 7261 6e67        self._rang
-00016970: 6520 3d20 4e6f 6e65 0a0a 2020 2020 6465  e = None..    de
-00016980: 6620 5f5f 6361 6c6c 5f5f 2873 656c 662c  f __call__(self,
-00016990: 2058 293a 0a20 2020 2020 2020 2058 203d   X):.        X =
-000169a0: 2073 7570 6572 2829 2e5f 5f63 616c 6c5f   super().__call_
-000169b0: 5f28 5829 0a20 2020 2020 2020 205f 7261  _(X).        _ra
-000169c0: 6e67 6520 3d20 7365 6c66 2e72 616e 6765  nge = self.range
-000169d0: 0a20 2020 2020 2020 2069 6620 5f72 616e  .        if _ran
-000169e0: 6765 2069 7320 4e6f 6e65 3a0a 2020 2020  ge is None:.    
-000169f0: 2020 2020 2020 2020 5f72 616e 6765 203d          _range =
-00016a00: 2062 742e 7175 616e 7469 6c65 2858 2e66   bt.quantile(X.f
-00016a10: 6c61 7474 656e 2829 2e66 6c6f 6174 2829  latten().float()
-00016a20: 2c20 6261 746f 7263 685f 7465 6e73 6f72  , batorch_tensor
-00016a30: 285b 302e 3032 352c 2030 2e39 3735 5d29  ([0.025, 0.975])
-00016a40: 2c20 6178 6973 3d2d 3129 2e6d 6f76 6564  , axis=-1).moved
-00016a50: 696d 2830 2c20 2d31 292e 7370 6563 6961  im(0, -1).specia
-00016a60: 6c5f 6672 6f6d 5f28 5829 0a20 2020 2020  l_from_(X).     
-00016a70: 2020 2020 2020 2073 656c 662e 5f72 616e         self._ran
-00016a80: 6765 203d 205f 7261 6e67 650a 2020 2020  ge = _range.    
-00016a90: 2020 2020 7265 7475 726e 2028 2858 202d      return ((X -
-00016aa0: 205f 7261 6e67 655b 2e2e 2e2c 2030 5d29   _range[..., 0])
-00016ab0: 202f 2028 5f72 616e 6765 5b2e 2e2e 2c20   / (_range[..., 
-00016ac0: 315d 202d 205f 7261 6e67 655b 2e2e 2e2c  1] - _range[...,
-00016ad0: 2030 5d29 292e 636c 616d 7028 302e 2c20   0])).clamp(0., 
-00016ae0: 312e 290a 2020 2020 0a20 2020 2064 6566  1.).    .    def
-00016af0: 2069 6e76 2873 656c 6629 3a0a 2020 2020   inv(self):.    
-00016b00: 2020 2020 6966 2073 656c 662e 7261 6e67      if self.rang
-00016b10: 6520 6973 206e 6f74 204e 6f6e 653a 205f  e is not None: _
-00016b20: 7261 6e67 6520 3d20 7365 6c66 2e72 616e  range = self.ran
-00016b30: 6765 0a20 2020 2020 2020 2065 6c69 6620  ge.        elif 
-00016b40: 7365 6c66 2e5f 7261 6e67 6520 6973 206e  self._range is n
-00016b50: 6f74 204e 6f6e 653a 205f 7261 6e67 6520  ot None: _range 
-00016b60: 3d20 7365 6c66 2e5f 7261 6e67 650a 2020  = self._range.  
-00016b70: 2020 2020 2020 656c 7365 3a20 7265 7475        else: retu
-00016b80: 726e 204e 6f72 6d61 6c69 7a65 284e 6f6e  rn Normalize(Non
-00016b90: 6529 0a20 2020 2020 2020 2064 656e 203d  e).        den =
-00016ba0: 205f 7261 6e67 655b 2e2e 2e2c 2031 5d20   _range[..., 1] 
-00016bb0: 2d20 5f72 616e 6765 5b2e 2e2e 2c20 305d  - _range[..., 0]
-00016bc0: 0a20 2020 2020 2020 205f 7261 6e67 6520  .        _range 
-00016bd0: 3d20 6274 2e73 7461 636b 282d 5f72 616e  = bt.stack(-_ran
-00016be0: 6765 5b2e 2e2e 2c20 305d 2c20 312d 5f72  ge[..., 0], 1-_r
-00016bf0: 616e 6765 5b2e 2e2e 2c20 305d 2c20 2d31  ange[..., 0], -1
-00016c00: 2920 2f20 6465 6e0a 2020 2020 2020 2020  ) / den.        
-00016c10: 7265 7475 726e 204e 6f72 6d61 6c69 7a65  return Normalize
-00016c20: 285f 7261 6e67 6529 0a0a 2323 2323 2323  (_range)..######
-00016c30: 2323 2323 2323 2320 5375 7070 6f72 7469  ####### Supporti
-00016c40: 6e67 2046 756e 6374 696f 6e73 2023 2323  ng Functions ###
-00016c50: 2323 2323 2323 2323 230a 0a64 6566 2042  #########..def B
-00016c60: 7370 6c69 6e65 2869 2c20 5529 3a0a 2020  spline(i, U):.  
-00016c70: 2020 2222 220a 2020 2020 4375 6269 6320    """.    Cubic 
-00016c80: 422d 7370 6c69 6e65 2066 756e 6374 696f  B-spline functio
-00016c90: 6e2e 200a 2020 2020 4e6f 7465 3a20 4173  n. .    Note: As
-00016ca0: 206c 6f6e 6720 6173 2069 2061 6e64 2055   long as i and U
-00016cb0: 2068 6176 6520 7468 6520 7361 6d65 2073   have the same s
-00016cc0: 697a 652c 2061 6e79 2073 6861 7065 206f  ize, any shape o
-00016cd0: 6620 7465 6e73 6f72 7320 776f 756c 6420  f tensors would 
-00016ce0: 646f 2e0a 2020 2020 0a20 2020 2050 6172  do..    .    Par
-00016cf0: 616d 733a 0a20 2020 2020 2020 2069 205b  ams:.        i [
-00016d00: 6274 2e54 656e 736f 725d 3a20 7468 6520  bt.Tensor]: the 
-00016d10: 696e 6465 7820 6f66 2073 6567 6d65 6e74  index of segment
-00016d20: 2066 756e 6374 696f 6e20 6f66 2042 2d73   function of B-s
-00016d30: 706c 696e 652e 0a20 2020 2020 2020 2020  pline..         
-00016d40: 2020 2054 6865 2076 616c 7565 206f 6620     The value of 
-00016d50: 6561 6368 2065 6c65 6d65 6e74 2063 616e  each element can
-00016d60: 2062 6520 6368 6f73 656e 2069 6e20 282d   be chosen in (-
-00016d70: 312c 2030 2c20 312c 2032 292e 200a 2020  1, 0, 1, 2). .  
-00016d80: 2020 2020 2020 5520 5b62 742e 5465 6e73        U [bt.Tens
-00016d90: 6f72 5d3a 2074 6865 2064 6563 696d 616c  or]: the decimal
-00016da0: 2061 7267 756d 656e 7420 6f66 2042 2d73   argument of B-s
-00016db0: 706c 696e 6520 6675 6e63 7469 6f6e 2e20  pline function. 
-00016dc0: 4974 2073 686f 756c 6420 6265 2077 6974  It should be wit
-00016dd0: 6869 6e20 7261 6e67 6520 5b30 2c20 3129  hin range [0, 1)
-00016de0: 2e0a 2020 2020 2222 220a 2020 2020 6920  ..    """.    i 
-00016df0: 3d20 6261 746f 7263 685f 7465 6e73 6f72  = batorch_tensor
-00016e00: 2869 293b 2055 203d 2062 6174 6f72 6368  (i); U = batorch
-00016e10: 5f74 656e 736f 7228 5529 0a20 2020 2072  _tensor(U).    r
-00016e20: 6574 7572 6e20 280a 2020 2020 2020 2020  eturn (.        
-00016e30: 6274 2e77 6865 7265 2869 203d 3d20 2d31  bt.where(i == -1
-00016e40: 2c20 2831 202d 2055 2920 2a2a 2033 202f  , (1 - U) ** 3 /
-00016e50: 2036 2c0a 2020 2020 2020 2020 6274 2e77   6,.        bt.w
-00016e60: 6865 7265 2869 203d 3d20 302c 2055 202a  here(i == 0, U *
-00016e70: 2a20 3320 2f20 3220 2d20 5520 2a20 5520  * 3 / 2 - U * U 
-00016e80: 2b20 3220 2f20 332c 0a20 2020 2020 2020  + 2 / 3,.       
-00016e90: 2062 742e 7768 6572 6528 6920 3d3d 2031   bt.where(i == 1
-00016ea0: 2c20 282d 2033 202a 2055 202a 2a20 3320  , (- 3 * U ** 3 
-00016eb0: 2b20 3320 2a20 5520 2a20 5520 2b20 3320  + 3 * U * U + 3 
-00016ec0: 2a20 5520 2b20 3129 202f 2036 2c0a 2020  * U + 1) / 6,.  
-00016ed0: 2020 2020 2020 6274 2e77 6865 7265 2869        bt.where(i
-00016ee0: 203d 3d20 322c 2055 202a 2a20 3320 2f20   == 2, U ** 3 / 
-00016ef0: 362c 0a20 2020 2020 2020 2062 742e 7a65  6,.        bt.ze
-00016f00: 726f 735f 6c69 6b65 2855 2929 2929 290a  ros_like(U))))).
-00016f10: 2020 2020 290a 0a64 6566 2064 4273 706c      )..def dBspl
-00016f20: 696e 6528 692c 2055 293a 0a20 2020 2022  ine(i, U):.    "
-00016f30: 2222 0a20 2020 2054 6865 2064 6572 6976  "".    The deriv
-00016f40: 6174 6976 6520 6f66 2042 2d73 706c 696e  ative of B-splin
-00016f50: 6520 6675 6e63 7469 6f6e 2c20 7769 7468  e function, with
-00016f60: 2072 6573 7065 6374 2074 6f20 552e 200a   respect to U. .
-00016f70: 2020 2020 4e6f 7465 3a20 4173 206c 6f6e      Note: As lon
-00016f80: 6720 6173 2069 2061 6e64 2055 2068 6176  g as i and U hav
-00016f90: 6520 7468 6520 7361 6d65 2073 697a 652c  e the same size,
-00016fa0: 2061 6e79 2073 6861 7065 206f 6620 7465   any shape of te
-00016fb0: 6e73 6f72 7320 776f 756c 6420 646f 2e0a  nsors would do..
-00016fc0: 2020 2020 0a20 2020 2050 6172 616d 733a      .    Params:
-00016fd0: 0a20 2020 2020 2020 2069 205b 6274 2e54  .        i [bt.T
-00016fe0: 656e 736f 725d 3a20 7468 6520 696e 6465  ensor]: the inde
-00016ff0: 7820 6f66 2073 6567 6d65 6e74 2066 756e  x of segment fun
-00017000: 6374 696f 6e20 6f66 2042 2d73 706c 696e  ction of B-splin
-00017010: 652e 0a20 2020 2020 2020 2020 2020 2054  e..            T
-00017020: 6865 2076 616c 7565 206f 6620 6561 6368  he value of each
-00017030: 2065 6c65 6d65 6e74 2063 616e 2062 6520   element can be 
-00017040: 6368 6f73 656e 2069 6e20 282d 312c 2030  chosen in (-1, 0
-00017050: 2c20 312c 2032 292e 200a 2020 2020 2020  , 1, 2). .      
-00017060: 2020 5520 5b62 742e 5465 6e73 6f72 5d3a    U [bt.Tensor]:
-00017070: 2074 6865 2064 6563 696d 616c 2061 7267   the decimal arg
-00017080: 756d 656e 7420 6f66 2042 2d73 706c 696e  ument of B-splin
-00017090: 6520 6675 6e63 7469 6f6e 2e20 4974 2073  e function. It s
-000170a0: 686f 756c 6420 6265 2077 6974 6869 6e20  hould be within 
-000170b0: 7261 6e67 6520 5b30 2c20 3129 2e0a 2020  range [0, 1)..  
-000170c0: 2020 2222 220a 2020 2020 6920 3d20 6261    """.    i = ba
-000170d0: 746f 7263 685f 7465 6e73 6f72 2869 293b  torch_tensor(i);
-000170e0: 2055 203d 2062 6174 6f72 6368 5f74 656e   U = batorch_ten
-000170f0: 736f 7228 5529 0a20 2020 2072 6574 7572  sor(U).    retur
-00017100: 6e20 280a 2020 2020 2020 2020 6274 2e77  n (.        bt.w
-00017110: 6865 7265 2869 203d 3d20 2d31 2c20 2d20  here(i == -1, - 
-00017120: 3320 2a20 2831 202d 2055 2920 2a2a 2032  3 * (1 - U) ** 2
-00017130: 202f 2036 2c0a 2020 2020 2020 2020 6274   / 6,.        bt
-00017140: 2e77 6865 7265 2869 203d 3d20 302c 2033  .where(i == 0, 3
-00017150: 202a 2055 202a 2a20 3220 2f20 3220 2d20   * U ** 2 / 2 - 
-00017160: 3220 2a20 552c 0a20 2020 2020 2020 2062  2 * U,.        b
-00017170: 742e 7768 6572 6528 6920 3d3d 2031 2c20  t.where(i == 1, 
-00017180: 282d 2033 202a 2055 202a 2a20 3220 2b20  (- 3 * U ** 2 + 
-00017190: 3220 2a20 5520 2b20 3129 202f 2032 2c0a  2 * U + 1) / 2,.
-000171a0: 2020 2020 2020 2020 6274 2e77 6865 7265          bt.where
-000171b0: 2869 203d 3d20 322c 2033 202a 2055 202a  (i == 2, 3 * U *
-000171c0: 2a20 3220 2f20 362c 0a20 2020 2020 2020  * 2 / 6,.       
-000171d0: 2062 742e 7a65 726f 735f 6c69 6b65 2855   bt.zeros_like(U
-000171e0: 2929 2929 290a 2020 2020 290a 0a64 6566  ))))).    )..def
-000171f0: 2066 4273 706c 696e 6528 632c 2078 293a   fBspline(c, x):
-00017200: 0a20 2020 2063 203d 2062 6174 6f72 6368  .    c = batorch
-00017210: 5f74 656e 736f 7228 6329 3b20 7820 3d20  _tensor(c); x = 
-00017220: 6261 746f 7263 685f 7465 6e73 6f72 2878  batorch_tensor(x
-00017230: 290a 2020 2020 6420 3d20 7820 2d20 630a  ).    d = x - c.
-00017240: 2020 2020 7265 7475 726e 2028 0a20 2020      return (.   
-00017250: 2020 2020 2062 742e 7768 6572 6528 282d       bt.where((-
-00017260: 3220 3c3d 2064 2920 2a20 2864 203c 202d  2 <= d) * (d < -
-00017270: 3129 2c20 6420 2a2a 2033 202b 2036 202a  1), d ** 3 + 6 *
-00017280: 2064 202a 2a20 3220 2b20 3132 202a 2064   d ** 2 + 12 * d
-00017290: 202b 2038 2c0a 2020 2020 2020 2020 6274   + 8,.        bt
-000172a0: 2e77 6865 7265 2828 2d31 203c 3d20 6429  .where((-1 <= d)
-000172b0: 202a 2028 6420 3c20 3029 2c20 2d20 3320   * (d < 0), - 3 
-000172c0: 2a20 6420 2a2a 2033 202d 2036 202a 2064  * d ** 3 - 6 * d
-000172d0: 202a 2a20 3220 2b20 342c 0a20 2020 2020   ** 2 + 4,.     
-000172e0: 2020 2062 742e 7768 6572 6528 2830 203c     bt.where((0 <
-000172f0: 3d20 6429 202a 2028 6420 3c20 3129 2c20  = d) * (d < 1), 
-00017300: 3320 2a20 6420 2a2a 2033 202d 2036 202a  3 * d ** 3 - 6 *
-00017310: 2064 202a 2a20 3220 2b20 342c 0a20 2020   d ** 2 + 4,.   
-00017320: 2020 2020 2062 742e 7768 6572 6528 2831       bt.where((1
-00017330: 203c 3d20 6429 202a 2028 6420 3c20 3229   <= d) * (d < 2)
-00017340: 2c20 2d20 6420 2a2a 2033 202b 2036 202a  , - d ** 3 + 6 *
-00017350: 2064 202a 2a20 3220 2d20 3132 202a 2064   d ** 2 - 12 * d
-00017360: 202b 2038 2c0a 2020 2020 2020 2020 6274   + 8,.        bt
-00017370: 2e7a 6572 6f73 5f6c 696b 6528 6429 2929  .zeros_like(d)))
-00017380: 2929 202f 2036 0a20 2020 2029 0a0a 6465  )) / 6.    )..de
-00017390: 6620 4166 6669 6e65 3244 324d 6174 7269  f Affine2D2Matri
-000173a0: 7828 7061 7261 6d73 293a 0a20 2020 2022  x(params):.    "
-000173b0: 2222 0a20 2020 2074 312c 2074 322c 20ce  "".    t1, t2, .
-000173c0: b82c 2073 312c 2073 322c 20cf 8131 2c20  ., s1, s2, ..1, 
-000173d0: cf81 3220 696e 2073 697a 653a 2028 5b6e  ..2 in size: ([n
-000173e0: 5f62 6174 6368 5d2c 207b 377d 290a 2020  _batch], {7}).  
-000173f0: 2020 7431 2c20 7432 2c20 6331 2c20 6332    t1, t2, c1, c2
-00017400: 2c20 ceb8 2c20 7331 2c20 7332 2c20 cf81  , .., s1, s2, ..
-00017410: 312c 20cf 8132 2069 6e20 7369 7a65 3a20  1, ..2 in size: 
-00017420: 285b 6e5f 6261 7463 685d 2c20 7b39 7d29  ([n_batch], {9})
-00017430: 0a20 2020 206f 7574 7075 7420 696e 2073  .    output in s
-00017440: 697a 653a 2028 5b6e 5f62 6174 6368 5d2c  ize: ([n_batch],
-00017450: 2033 2c20 3329 0a20 2020 2022 2222 0a20   3, 3).    """. 
-00017460: 2020 2070 6172 616d 7320 3d20 6261 746f     params = bato
-00017470: 7263 685f 7465 6e73 6f72 2870 6172 616d  rch_tensor(param
-00017480: 7329 0a20 2020 2069 6620 7061 7261 6d73  s).    if params
-00017490: 2e6e 5f64 696d 203c 3d20 3120 616e 6420  .n_dim <= 1 and 
-000174a0: 6e6f 7420 7061 7261 6d73 2e68 6173 5f62  not params.has_b
-000174b0: 6174 6368 3a20 7061 7261 6d73 203d 2070  atch: params = p
-000174c0: 6172 616d 732e 756e 7371 7565 657a 6528  arams.unsqueeze(
-000174d0: 5b5d 290a 2020 2020 6966 2070 6172 616d  []).    if param
-000174e0: 732e 6e5f 6469 6d20 3c3d 2031 2061 6e64  s.n_dim <= 1 and
-000174f0: 206e 6f74 2070 6172 616d 732e 6861 735f   not params.has_
-00017500: 6368 616e 6e65 6c3a 2070 6172 616d 7320  channel: params 
-00017510: 3d20 7061 7261 6d73 2e75 6e73 7175 6565  = params.unsquee
-00017520: 7a65 287b 317d 290a 2020 2020 6966 2070  ze({1}).    if p
-00017530: 6172 616d 732e 6e5f 6469 6d20 3d3d 2032  arams.n_dim == 2
-00017540: 2061 6e64 206e 6f74 2070 6172 616d 732e   and not params.
-00017550: 6861 735f 6261 7463 683a 2070 6172 616d  has_batch: param
-00017560: 732e 6261 7463 685f 6469 6d65 6e73 696f  s.batch_dimensio
-00017570: 6e20 3d20 300a 2020 2020 6966 2070 6172  n = 0.    if par
-00017580: 616d 732e 6e5f 6469 6d20 3d3d 2032 2061  ams.n_dim == 2 a
-00017590: 6e64 206e 6f74 2070 6172 616d 732e 6861  nd not params.ha
-000175a0: 735f 6368 616e 6e65 6c3a 2070 6172 616d  s_channel: param
-000175b0: 732e 6368 616e 6e65 6c5f 6469 6d65 6e73  s.channel_dimens
-000175c0: 696f 6e20 3d20 310a 2020 2020 6176 6f75  ion = 1.    avou
-000175d0: 6368 2870 6172 616d 732e 6861 735f 6261  ch(params.has_ba
-000175e0: 7463 682c 2066 2250 6c65 6173 6520 7573  tch, f"Please us
-000175f0: 6520 6261 746f 7263 6820 7465 6e73 6f72  e batorch tensor
-00017600: 206f 6620 7369 7a65 2028 5b6e 5f62 6174   of size ([n_bat
-00017610: 6368 5d2c 207b 3720 6f72 2039 7d29 205c  ch], {7 or 9}) \
-00017620: 0a20 2020 2020 2020 2066 6f72 2041 6666  .        for Aff
-00017630: 696e 6520 7061 7261 6d65 7465 7273 2c20  ine parameters, 
-00017640: 696e 7374 6561 6420 6f66 207b 7061 7261  instead of {para
-00017650: 6d73 2e73 6861 7065 7d2e 2022 290a 2020  ms.shape}. ").  
-00017660: 2020 6e5f 6261 7463 6820 3d20 7061 7261    n_batch = para
-00017670: 6d73 2e6e 5f62 6174 6368 0a20 2020 2069  ms.n_batch.    i
-00017680: 6620 7061 7261 6d73 2e73 697a 6528 3129  f params.size(1)
-00017690: 203d 3d20 373a 0a20 2020 2020 2020 2074   == 7:.        t
-000176a0: 312c 2074 322c 20ce b82c 2073 312c 2073  1, t2, .., s1, s
-000176b0: 322c 20cf 8131 2c20 cf81 3220 3d20 7061  2, ..1, ..2 = pa
-000176c0: 7261 6d73 2e73 706c 6974 2829 0a20 2020  rams.split().   
-000176d0: 2020 2020 2063 3120 3d20 6274 2e7a 6572       c1 = bt.zer
-000176e0: 6f73 285b 6e5f 6261 7463 685d 2c20 3129  os([n_batch], 1)
-000176f0: 3b20 6332 203d 2062 742e 7a65 726f 7328  ; c2 = bt.zeros(
-00017700: 5b6e 5f62 6174 6368 5d2c 2031 290a 2020  [n_batch], 1).  
-00017710: 2020 6966 2070 6172 616d 732e 7369 7a65    if params.size
-00017720: 2831 2920 3d3d 2039 3a0a 2020 2020 2020  (1) == 9:.      
-00017730: 2020 7431 2c20 7432 2c20 6331 2c20 6332    t1, t2, c1, c2
-00017740: 2c20 ceb8 2c20 7331 2c20 7332 2c20 cf81  , .., s1, s2, ..
-00017750: 312c 20cf 8132 203d 2070 6172 616d 732e  1, ..2 = params.
-00017760: 7370 6c69 7428 290a 2020 2020 6120 3d20  split().    a = 
-00017770: 28cf 8131 202a 20cf 8132 202b 2031 2920  (..1 * ..2 + 1) 
-00017780: 2a20 7331 202a 2062 742e 636f 7328 ceb8  * s1 * bt.cos(..
-00017790: 2920 2b20 cf81 3120 2a20 7332 202a 2062  ) + ..1 * s2 * b
-000177a0: 742e 7369 6e28 ceb8 290a 2020 2020 6220  t.sin(..).    b 
-000177b0: 3d20 2d20 28cf 8131 202a 20cf 8132 202b  = - (..1 * ..2 +
-000177c0: 2031 2920 2a20 7331 202a 2062 742e 7369   1) * s1 * bt.si
-000177d0: 6e28 ceb8 2920 2b20 cf81 3120 2a20 7332  n(..) + ..1 * s2
-000177e0: 202a 2062 742e 636f 7328 ceb8 290a 2020   * bt.cos(..).  
-000177f0: 2020 6320 3d20 cf81 3220 2a20 7331 202a    c = ..2 * s1 *
-00017800: 2062 742e 636f 7328 ceb8 2920 2b20 7332   bt.cos(..) + s2
-00017810: 202a 2062 742e 7369 6e28 ceb8 290a 2020   * bt.sin(..).  
-00017820: 2020 6420 3d20 2d20 cf81 3220 2a20 7331    d = - ..2 * s1
-00017830: 202a 2062 742e 7369 6e28 ceb8 2920 2b20   * bt.sin(..) + 
-00017840: 7332 202a 2062 742e 636f 7328 ceb8 290a  s2 * bt.cos(..).
-00017850: 2020 2020 7265 7475 726e 2062 742e 6361      return bt.ca
-00017860: 7428 0a20 2020 2020 2020 2062 742e 6361  t(.        bt.ca
-00017870: 7428 2861 2c20 622c 2074 3120 2d20 6120  t((a, b, t1 - a 
-00017880: 2a20 6331 202d 2062 202a 2063 3220 2b20  * c1 - b * c2 + 
-00017890: 6331 2c20 632c 2064 2c20 7432 202d 2063  c1, c, d, t2 - c
-000178a0: 202a 2063 3120 2d20 6420 2a20 6332 202b   * c1 - d * c2 +
-000178b0: 2063 3229 2c20 7b7d 292e 7669 6577 285b   c2), {}).view([
-000178c0: 6e5f 6261 7463 685d 2c20 322c 2033 292c  n_batch], 2, 3),
-000178d0: 200a 2020 2020 2020 2020 6274 2e6f 6e65   .        bt.one
-000178e0: 5f68 6f74 282d 312c 2033 292e 6d75 6c74  _hot(-1, 3).mult
-000178f0: 6970 6c79 286e 5f62 6174 6368 2c20 5b5d  iply(n_batch, []
-00017900: 292e 7669 6577 285b 6e5f 6261 7463 685d  ).view([n_batch]
-00017910: 2c20 312c 2033 292c 2031 0a20 2020 2029  , 1, 3), 1.    )
-00017920: 0a0a 6465 6620 5175 6174 6572 6e73 324d  ..def Quaterns2M
-00017930: 6174 7269 7828 7061 7261 6d73 293a 0a20  atrix(params):. 
-00017940: 2020 2022 2222 0a20 2020 2020 2020 2051     """.        Q
-00017950: 7561 7465 726e 3a20 7162 2c20 7163 2c20  uatern: qb, qc, 
-00017960: 7164 2c20 7078 2c20 7079 2c20 707a 2069  qd, px, py, pz i
-00017970: 6e20 7369 7a65 3a20 285b 6e5f 6261 7463  n size: ([n_batc
-00017980: 685d 2c20 7b36 7d29 0a20 2020 2020 2020  h], {6}).       
-00017990: 204d 6174 7269 783a 2028 5b6e 5f62 6174   Matrix: ([n_bat
-000179a0: 6368 5d2c 2034 2c20 3429 0a20 2020 2022  ch], 4, 4).    "
-000179b0: 2222 0a20 2020 2070 6172 616d 7320 3d20  "".    params = 
-000179c0: 6261 746f 7263 685f 7465 6e73 6f72 2870  batorch_tensor(p
-000179d0: 6172 616d 7329 0a20 2020 2069 6620 7061  arams).    if pa
-000179e0: 7261 6d73 2e6e 5f64 696d 203c 3d20 3120  rams.n_dim <= 1 
-000179f0: 616e 6420 6e6f 7420 7061 7261 6d73 2e68  and not params.h
-00017a00: 6173 5f62 6174 6368 3a20 7061 7261 6d73  as_batch: params
-00017a10: 203d 2070 6172 616d 732e 756e 7371 7565   = params.unsque
-00017a20: 657a 6528 5b5d 290a 2020 2020 6966 2070  eze([]).    if p
-00017a30: 6172 616d 732e 6e5f 6469 6d20 3c3d 2031  arams.n_dim <= 1
-00017a40: 2061 6e64 206e 6f74 2070 6172 616d 732e   and not params.
-00017a50: 6861 735f 6368 616e 6e65 6c3a 2070 6172  has_channel: par
-00017a60: 616d 7320 3d20 7061 7261 6d73 2e75 6e73  ams = params.uns
-00017a70: 7175 6565 7a65 287b 317d 290a 2020 2020  queeze({1}).    
-00017a80: 6966 2070 6172 616d 732e 6e5f 6469 6d20  if params.n_dim 
-00017a90: 3d3d 2032 2061 6e64 206e 6f74 2070 6172  == 2 and not par
-00017aa0: 616d 732e 6861 735f 6261 7463 683a 2070  ams.has_batch: p
-00017ab0: 6172 616d 732e 6261 7463 685f 6469 6d65  arams.batch_dime
-00017ac0: 6e73 696f 6e20 3d20 300a 2020 2020 6966  nsion = 0.    if
-00017ad0: 2070 6172 616d 732e 6e5f 6469 6d20 3d3d   params.n_dim ==
-00017ae0: 2032 2061 6e64 206e 6f74 2070 6172 616d   2 and not param
-00017af0: 732e 6861 735f 6368 616e 6e65 6c3a 2070  s.has_channel: p
-00017b00: 6172 616d 732e 6368 616e 6e65 6c5f 6469  arams.channel_di
-00017b10: 6d65 6e73 696f 6e20 3d20 310a 2020 2020  mension = 1.    
-00017b20: 6176 6f75 6368 2870 6172 616d 732e 6e5f  avouch(params.n_
-00017b30: 6469 6d20 3d3d 2032 2061 6e64 2070 6172  dim == 2 and par
-00017b40: 616d 732e 6861 735f 6261 7463 6820 616e  ams.has_batch an
-00017b50: 6420 7061 7261 6d73 2e68 6173 5f63 6861  d params.has_cha
-00017b60: 6e6e 656c 2c20 0a20 2020 2020 2020 2020  nnel, .         
-00017b70: 2020 6622 506c 6561 7365 2075 7365 2062    f"Please use b
-00017b80: 6174 6f72 6368 2074 656e 736f 7220 6f66  atorch tensor of
-00017b90: 2073 697a 6520 285b 6e5f 6261 7463 685d   size ([n_batch]
-00017ba0: 2c20 7b7b 367d 7d29 2066 6f72 2041 6666  , {{6}}) for Aff
-00017bb0: 696e 6520 7061 7261 6d65 7465 7273 2c20  ine parameters, 
-00017bc0: 696e 7374 6561 6420 6f66 207b 7061 7261  instead of {para
-00017bd0: 6d73 2e73 6861 7065 7d2e 2022 290a 2020  ms.shape}. ").  
-00017be0: 2020 6e5f 6261 7463 6820 3d20 7061 7261    n_batch = para
-00017bf0: 6d73 2e6e 5f62 6174 6368 0a20 2020 2062  ms.n_batch.    b
-00017c00: 2c20 632c 2064 2c20 782c 2079 2c20 7a20  , c, d, x, y, z 
-00017c10: 3d20 7061 7261 6d73 2e73 706c 6974 2829  = params.split()
-00017c20: 0a20 2020 2061 203d 2062 742e 7371 7274  .    a = bt.sqrt
-00017c30: 2828 312d 622a 622d 632a 632d 642a 6429  ((1-b*b-c*c-d*d)
-00017c40: 2e63 6c61 6d70 2830 2929 0a20 2020 2052  .clamp(0)).    R
-00017c50: 3131 203d 2061 2a61 2b62 2a62 2d63 2a63  11 = a*a+b*b-c*c
-00017c60: 2d64 2a64 0a20 2020 2052 3132 203d 2032  -d*d.    R12 = 2
-00017c70: 2a62 2a63 2d32 2a61 2a64 0a20 2020 2052  *b*c-2*a*d.    R
-00017c80: 3133 203d 2032 2a62 2a64 2b32 2a61 2a63  13 = 2*b*d+2*a*c
-00017c90: 0a20 2020 2052 3231 203d 2032 2a62 2a63  .    R21 = 2*b*c
-00017ca0: 2b32 2a61 2a64 0a20 2020 2052 3232 203d  +2*a*d.    R22 =
-00017cb0: 2061 2a61 2b63 2a63 2d62 2a62 2d64 2a64   a*a+c*c-b*b-d*d
-00017cc0: 0a20 2020 2052 3233 203d 2032 2a63 2a64  .    R23 = 2*c*d
-00017cd0: 2d32 2a61 2a62 0a20 2020 2052 3331 203d  -2*a*b.    R31 =
-00017ce0: 2032 2a62 2a64 2d32 2a61 2a63 0a20 2020   2*b*d-2*a*c.   
-00017cf0: 2052 3332 203d 2032 2a63 2a64 2b32 2a61   R32 = 2*c*d+2*a
-00017d00: 2a62 0a20 2020 2052 3333 203d 2061 2a61  *b.    R33 = a*a
-00017d10: 2b64 2a64 2d63 2a63 2d62 2a62 0a20 2020  +d*d-c*c-b*b.   
-00017d20: 2072 6574 7572 6e20 6274 2e63 6174 280a   return bt.cat(.
-00017d30: 2020 2020 2020 2020 6274 2e63 6174 2828          bt.cat((
-00017d40: 5231 312c 2052 3132 2c20 5231 332c 2078  R11, R12, R13, x
-00017d50: 2c20 5232 312c 2052 3232 2c20 5232 332c  , R21, R22, R23,
-00017d60: 2079 2c20 5233 312c 2052 3332 2c20 5233   y, R31, R32, R3
-00017d70: 332c 207a 292c 2031 292e 7669 6577 285b  3, z), 1).view([
-00017d80: 6e5f 6261 7463 685d 2c20 332c 2034 292c  n_batch], 3, 4),
-00017d90: 0a20 2020 2020 2020 2062 742e 6f6e 655f  .        bt.one_
-00017da0: 686f 7428 2d31 2c20 3429 2e6d 756c 7469  hot(-1, 4).multi
-00017db0: 706c 7928 6e5f 6261 7463 682c 205b 5d29  ply(n_batch, [])
-00017dc0: 2e76 6965 7728 5b6e 5f62 6174 6368 5d2c  .view([n_batch],
-00017dd0: 2031 2c20 3429 2c20 310a 2020 2020 290a   1, 4), 1.    ).
-00017de0: 0a64 6566 204d 6174 7269 7832 5175 6174  .def Matrix2Quat
-00017df0: 6572 6e73 2870 6172 616d 7329 3a0a 2020  erns(params):.  
-00017e00: 2020 2222 220a 2020 2020 2020 2020 4d61    """.        Ma
-00017e10: 7472 6978 3a20 285b 6e5f 6261 7463 685d  trix: ([n_batch]
-00017e20: 2c20 342c 2034 290a 2020 2020 2020 2020  , 4, 4).        
-00017e30: 5175 6174 6572 6e3a 2071 622c 2071 632c  Quatern: qb, qc,
-00017e40: 2071 642c 2070 782c 2070 792c 2070 7a20   qd, px, py, pz 
-00017e50: 696e 2073 697a 653a 2028 5b6e 5f62 6174  in size: ([n_bat
-00017e60: 6368 5d2c 207b 367d 290a 2020 2020 2222  ch], {6}).    ""
-00017e70: 220a 2020 2020 7061 7261 6d73 203d 2062  ".    params = b
-00017e80: 6174 6f72 6368 5f74 656e 736f 7228 7061  atorch_tensor(pa
-00017e90: 7261 6d73 290a 2020 2020 6966 2070 6172  rams).    if par
-00017ea0: 616d 732e 6e5f 6469 6d20 3c3d 2032 2061  ams.n_dim <= 2 a
-00017eb0: 6e64 206e 6f74 2070 6172 616d 732e 6861  nd not params.ha
-00017ec0: 735f 6261 7463 683a 2070 6172 616d 7320  s_batch: params 
-00017ed0: 3d20 7061 7261 6d73 2e75 6e73 7175 6565  = params.unsquee
-00017ee0: 7a65 285b 5d29 0a20 2020 2069 6620 7061  ze([]).    if pa
-00017ef0: 7261 6d73 2e6e 5f64 696d 203d 3d20 3320  rams.n_dim == 3 
-00017f00: 616e 6420 6e6f 7420 7061 7261 6d73 2e68  and not params.h
-00017f10: 6173 5f62 6174 6368 3a20 7061 7261 6d73  as_batch: params
-00017f20: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
-00017f30: 203d 2030 0a20 2020 2069 6620 7061 7261   = 0.    if para
-00017f40: 6d73 2e6e 5f64 696d 203d 3d20 3320 616e  ms.n_dim == 3 an
-00017f50: 6420 7061 7261 6d73 2e68 6173 5f63 6861  d params.has_cha
-00017f60: 6e6e 656c 3a20 7061 7261 6d73 2e63 6861  nnel: params.cha
-00017f70: 6e6e 656c 5f64 696d 656e 7369 6f6e 203d  nnel_dimension =
-00017f80: 204e 6f6e 650a 2020 2020 6176 6f75 6368   None.    avouch
-00017f90: 2870 6172 616d 732e 6e5f 6469 6d20 3d3d  (params.n_dim ==
-00017fa0: 2033 2061 6e64 2070 6172 616d 732e 6861   3 and params.ha
-00017fb0: 735f 6261 7463 6820 616e 6420 6e6f 7420  s_batch and not 
-00017fc0: 7061 7261 6d73 2e68 6173 5f63 6861 6e6e  params.has_chann
-00017fd0: 656c 2c20 0a20 2020 2020 2020 2020 2020  el, .           
-00017fe0: 6622 506c 6561 7365 2075 7365 2062 6174  f"Please use bat
-00017ff0: 6f72 6368 2074 656e 736f 7220 6f66 2073  orch tensor of s
-00018000: 697a 6520 285b 6e5f 6261 7463 685d 2c20  ize ([n_batch], 
-00018010: 342c 2034 2920 666f 7220 4166 6669 6e65  4, 4) for Affine
-00018020: 206d 6174 7269 782c 2069 6e73 7465 6164   matrix, instead
-00018030: 206f 6620 7b70 6172 616d 732e 7368 6170   of {params.shap
-00018040: 657d 2e20 2229 0a20 2020 206e 5f62 6174  e}. ").    n_bat
-00018050: 6368 203d 2070 6172 616d 732e 6e5f 6261  ch = params.n_ba
-00018060: 7463 680a 2020 2020 782c 2079 2c20 7a20  tch.    x, y, z 
-00018070: 3d20 7061 7261 6d73 5b2e 2e2e 2c20 3a33  = params[..., :3
-00018080: 2c20 2d31 5d2e 6368 616e 6e65 6c5f 6469  , -1].channel_di
-00018090: 6d5f 2831 292e 7370 6c69 7428 312c 2031  m_(1).split(1, 1
-000180a0: 290a 2020 2020 6132 203d 2028 6274 2e64  ).    a2 = (bt.d
-000180b0: 6961 6728 7061 7261 6d73 292e 7375 6d28  iag(params).sum(
-000180c0: 292e 756e 7371 7565 657a 6528 7b7d 2920  ).unsqueeze({}) 
-000180d0: 2b20 3129 202f 2034 0a20 2020 2061 203d  + 1) / 4.    a =
-000180e0: 2062 742e 7371 7274 2861 3229 0a20 2020   bt.sqrt(a2).   
-000180f0: 2062 3220 3d20 6132 202d 2028 7061 7261   b2 = a2 - (para
-00018100: 6d73 5b2e 2e2e 2c20 312c 2031 5d20 2b20  ms[..., 1, 1] + 
-00018110: 7061 7261 6d73 5b2e 2e2e 2c20 322c 2032  params[..., 2, 2
-00018120: 5d29 202f 2032 0a20 2020 2063 3220 3d20  ]) / 2.    c2 = 
-00018130: 6132 202d 2028 7061 7261 6d73 5b2e 2e2e  a2 - (params[...
-00018140: 2c20 322c 2032 5d20 2b20 7061 7261 6d73  , 2, 2] + params
-00018150: 5b2e 2e2e 2c20 302c 2030 5d29 202f 2032  [..., 0, 0]) / 2
-00018160: 0a20 2020 2064 3220 3d20 6132 202d 2028  .    d2 = a2 - (
-00018170: 7061 7261 6d73 5b2e 2e2e 2c20 302c 2030  params[..., 0, 0
-00018180: 5d20 2b20 7061 7261 6d73 5b2e 2e2e 2c20  ] + params[..., 
-00018190: 312c 2031 5d29 202f 2032 0a20 2020 2044  1, 1]) / 2.    D
-000181a0: 203d 2070 6172 616d 7320 2d20 7061 7261   = params - para
-000181b0: 6d73 2e54 0a20 2020 2062 203d 2062 742e  ms.T.    b = bt.
-000181c0: 7369 676e 2844 5b2e 2e2e 2c20 322c 2031  sign(D[..., 2, 1
-000181d0: 5d29 202a 2062 742e 7371 7274 2862 3229  ]) * bt.sqrt(b2)
-000181e0: 0a20 2020 2063 203d 202d 2062 742e 7369  .    c = - bt.si
-000181f0: 676e 2844 5b2e 2e2e 2c20 322c 2030 5d29  gn(D[..., 2, 0])
-00018200: 202a 2062 742e 7371 7274 2863 3229 0a20   * bt.sqrt(c2). 
-00018210: 2020 2064 203d 2062 742e 7369 676e 2844     d = bt.sign(D
-00018220: 5b2e 2e2e 2c20 312c 2030 5d29 202a 2062  [..., 1, 0]) * b
-00018230: 742e 7371 7274 2864 3229 0a20 2020 2072  t.sqrt(d2).    r
-00018240: 6574 7572 6e20 6274 2e63 6174 2862 2c20  eturn bt.cat(b, 
-00018250: 632c 2064 2c20 782c 2079 2c20 7a2c 207b  c, d, x, y, z, {
-00018260: 7d29 0a                                  }).
+000132b0: 6765 203d 2062 742e 746f 5f64 6576 6963  ge = bt.to_devic
+000132c0: 6528 6261 746f 7263 685f 7465 6e73 6f72  e(batorch_tensor
+000132d0: 2869 6d61 6765 2929 0a20 2020 2073 6861  (image)).    sha
+000132e0: 7065 5f6f 7574 203d 2069 6d61 6765 2e73  pe_out = image.s
+000132f0: 6861 7065 0a20 2020 2069 6620 7472 616e  hape.    if tran
+00013300: 7320 6973 204e 6f6e 6520 6f72 2074 7261  s is None or tra
+00013310: 6e73 2e6e 5f64 696d 2069 7320 4e6f 6e65  ns.n_dim is None
+00013320: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
+00013330: 2069 6d61 6765 2e68 6173 5f62 6174 6368   image.has_batch
+00013340: 3a20 696d 6167 652e 756e 7371 7565 657a  : image.unsqueez
+00013350: 655f 285b 5d29 0a20 2020 2020 2020 2069  e_([]).        i
+00013360: 6620 6e6f 7420 696d 6167 652e 6861 735f  f not image.has_
+00013370: 6368 616e 6e65 6c3a 2069 6d61 6765 2e73  channel: image.s
+00013380: 7461 6e64 6172 645f 2829 2e75 6e73 7175  tandard_().unsqu
+00013390: 6565 7a65 5f28 7b31 7d29 0a20 2020 2020  eeze_({1}).     
+000133a0: 2020 206e 5f64 696d 203d 2069 6d61 6765     n_dim = image
+000133b0: 2e6e 5f73 7061 6365 2023 2047 6574 2074  .n_space # Get t
+000133c0: 6865 2073 7061 7469 616c 2072 616e 6b2e  he spatial rank.
+000133d0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+000133e0: 2020 206e 5f64 696d 203d 2074 7261 6e73     n_dim = trans
+000133f0: 2e6e 5f64 696d 0a20 2020 2020 2020 2069  .n_dim.        i
+00013400: 6620 696d 6167 652e 6e5f 6469 6d20 3d3d  f image.n_dim ==
+00013410: 206e 5f64 696d 3a0a 2020 2020 2020 2020   n_dim:.        
+00013420: 2020 2020 6966 2069 6d61 6765 2e68 6173      if image.has
+00013430: 5f73 7065 6369 616c 3a0a 2020 2020 2020  _special:.      
+00013440: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00013450: 6622 5761 726e 696e 673a 2027 696e 7465  f"Warning: 'inte
+00013460: 7270 6f6c 6174 696f 6e27 2074 7279 696e  rpolation' tryin
+00013470: 6720 746f 2074 7261 6e73 666f 726d 207b  g to transform {
+00013480: 696d 6167 652e 6e5f 7370 6163 657d 2b7b  image.n_space}+{
+00013490: 696d 6167 652e 6e5f 7370 6563 6961 6c7d  image.n_special}
+000134a0: 4420 696d 6167 6520 2877 6974 6820 6261  D image (with ba
+000134b0: 7463 6820 6f72 2063 6861 6e6e 656c 2920  tch or channel) 
+000134c0: 6279 207b 6e5f 6469 6d7d 4420 7472 616e  by {n_dim}D tran
+000134d0: 7366 6f72 6d61 7469 6f6e 2c20 6175 746f  sformation, auto
+000134e0: 2d72 656d 6f76 696e 6720 7370 6563 6961  -removing specia
+000134f0: 6c20 6469 6d65 6e73 696f 6e73 2e22 290a  l dimensions.").
+00013500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013510: 696d 6167 652e 7265 6d6f 7665 5f73 7065  image.remove_spe
+00013520: 6369 616c 5f28 290a 2020 2020 2020 2020  cial_().        
+00013530: 2020 2020 696d 6167 652e 756e 7371 7565      image.unsque
+00013540: 657a 655f 285b 5d29 2e75 6e73 7175 6565  eze_([]).unsquee
+00013550: 7a65 5f28 7b7d 290a 2020 2020 2020 2020  ze_({}).        
+00013560: 656c 6966 2069 6d61 6765 2e6e 5f64 696d  elif image.n_dim
+00013570: 203d 3d20 6e5f 6469 6d20 2b20 313a 0a20   == n_dim + 1:. 
+00013580: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00013590: 7420 696d 6167 652e 6861 735f 6261 7463  t image.has_batc
+000135a0: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
+000135b0: 2020 2069 6620 696d 6167 652e 6861 735f     if image.has_
+000135c0: 6368 616e 6e65 6c3a 2069 6d61 6765 2e75  channel: image.u
+000135d0: 6e73 7175 6565 7a65 5f28 5b5d 290a 2020  nsqueeze_([]).  
+000135e0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+000135f0: 7365 3a20 696d 6167 652e 7769 7468 5f62  se: image.with_b
+00013600: 6174 6368 6469 6d28 3029 2e75 6e73 7175  atchdim(0).unsqu
+00013610: 6565 7a65 5f28 7b31 7d29 0a20 2020 2020  eeze_({1}).     
+00013620: 2020 2020 2020 2065 6c69 6620 6e6f 7420         elif not 
+00013630: 696d 6167 652e 6861 735f 6368 616e 6e65  image.has_channe
+00013640: 6c3a 2069 6d61 6765 2e75 6e73 7175 6565  l: image.unsquee
+00013650: 7a65 5f28 7b7d 290a 2020 2020 2020 2020  ze_({}).        
+00013660: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00013670: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00013680: 6622 5761 726e 696e 673a 2027 696e 7465  f"Warning: 'inte
+00013690: 7270 6f6c 6174 696f 6e27 2074 7279 696e  rpolation' tryin
+000136a0: 6720 746f 2074 7261 6e73 666f 726d 207b  g to transform {
+000136b0: 696d 6167 652e 6e5f 7370 6163 657d 2b7b  image.n_space}+{
+000136c0: 696d 6167 652e 6e5f 7370 6563 6961 6c7d  image.n_special}
+000136d0: 4420 696d 6167 6520 2877 6974 6820 6261  D image (with ba
+000136e0: 7463 6820 6f72 2063 6861 6e6e 656c 2920  tch or channel) 
+000136f0: 6279 207b 6e5f 6469 6d7d 4420 7472 616e  by {n_dim}D tran
+00013700: 7366 6f72 6d61 7469 6f6e 2c20 6175 746f  sformation, auto
+00013710: 2d72 656d 6f76 696e 6720 7468 6520 6368  -removing the ch
+00013720: 616e 6e65 6c20 6469 6d65 6e73 696f 6e73  annel dimensions
+00013730: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
+00013740: 2020 2020 696d 6167 652e 7769 7468 5f63      image.with_c
+00013750: 6861 6e6e 656c 6469 6d28 4e6f 6e65 292e  hanneldim(None).
+00013760: 756e 7371 7565 657a 655f 287b 7d29 0a20  unsqueeze_({}). 
+00013770: 2020 2020 2020 2065 6c69 6620 696d 6167         elif imag
+00013780: 652e 6e5f 6469 6d20 3d3d 206e 5f64 696d  e.n_dim == n_dim
+00013790: 202b 2032 3a0a 2020 2020 2020 2020 2020   + 2:.          
+000137a0: 2020 2320 5f63 6861 6e6e 616c 2f62 6174    # _channal/bat
+000137b0: 6368 2064 696d 656e 7369 6f6e 7320 7573  ch dimensions us
+000137c0: 6564 2068 6572 6520 6173 2074 6865 7920  ed here as they 
+000137d0: 6172 6520 6e5f 6469 6d20 7768 656e 206e  are n_dim when n
+000137e0: 6f74 2065 7869 7374 6564 2e20 0a20 2020  ot existed. .   
+000137f0: 2020 2020 2020 2020 2069 6620 696d 6167           if imag
+00013800: 652e 6e5f 7370 6563 6961 6c20 3d3d 2031  e.n_special == 1
+00013810: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013820: 2020 7072 696e 7428 6622 5761 726e 696e    print(f"Warnin
+00013830: 673a 2027 696e 7465 7270 6f6c 6174 696f  g: 'interpolatio
+00013840: 6e27 2074 7279 696e 6720 746f 2074 7261  n' trying to tra
+00013850: 6e73 666f 726d 207b 696d 6167 652e 6e5f  nsform {image.n_
+00013860: 7370 6163 657d 2b31 4420 696d 6167 6520  space}+1D image 
+00013870: 2877 6974 6820 6261 7463 6820 6f72 2063  (with batch or c
+00013880: 6861 6e6e 656c 2920 6279 207b 6e5f 6469  hannel) by {n_di
+00013890: 6d7d 4420 7472 616e 7366 6f72 6d61 7469  m}D transformati
+000138a0: 6f6e 2c20 6175 746f 2d69 6e73 6572 7469  on, auto-inserti
+000138b0: 6e67 206e 6577 2073 7065 6369 616c 2064  ng new special d
+000138c0: 696d 656e 7369 6f6e 2e22 290a 2020 2020  imension.").    
+000138d0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+000138e0: 6d61 6765 2e68 6173 5f62 6174 6368 3a20  mage.has_batch: 
+000138f0: 696d 6167 652e 6261 7463 685f 6469 6d65  image.batch_dime
+00013900: 6e73 696f 6e20 3d20 3020 6966 2069 6d61  nsion = 0 if ima
+00013910: 6765 2e5f 6368 616e 6e65 6c5f 6469 6d65  ge._channel_dime
+00013920: 6e73 696f 6e20 3e20 3020 656c 7365 2031  nsion > 0 else 1
+00013930: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00013940: 6e6f 7420 696d 6167 652e 6861 735f 6368  not image.has_ch
+00013950: 616e 6e65 6c3a 2069 6d61 6765 2e63 6861  annel: image.cha
+00013960: 6e6e 656c 5f64 696d 656e 7369 6f6e 203d  nnel_dimension =
+00013970: 2030 2069 6620 696d 6167 652e 5f62 6174   0 if image._bat
+00013980: 6368 5f64 696d 656e 7369 6f6e 203e 2030  ch_dimension > 0
+00013990: 2065 6c73 6520 310a 2020 2020 6176 6f75   else 1.    avou
+000139a0: 6368 2869 6d61 6765 2e68 6173 5f62 6174  ch(image.has_bat
+000139b0: 6368 2061 6e64 2069 6d61 6765 2e68 6173  ch and image.has
+000139c0: 5f63 6861 6e6e 656c 2c20 2250 6c65 6173  _channel, "Pleas
+000139d0: 6520 7573 6520 6261 746f 7263 6820 7465  e use batorch te
+000139e0: 6e73 6f72 206f 6620 7369 7a65 2022 202b  nsor of size " +
+000139f0: 0a20 2020 2020 2020 2020 2020 2022 285b  .            "([
+00013a00: 6e5f 6261 7463 685d 2c20 7b6e 5f63 6861  n_batch], {n_cha
+00013a10: 6e6e 656c 2f6e 5f66 6561 7475 7265 3a6f  nnel/n_feature:o
+00013a20: 7074 696f 6e61 6c7d 2c20 6d5f 312c 206d  ptional}, m_1, m
+00013a30: 5f32 2c20 2e2e 2e2c 206d 5f72 2920 5b72  _2, ..., m_r) [r
+00013a40: 3d6e 5f64 696d 5d20 666f 7220 2220 2b20  =n_dim] for " + 
+00013a50: 0a20 2020 2020 2020 2020 2020 2066 2264  .            f"d
+00013a60: 6174 6120 746f 2062 6520 7370 6174 6961  ata to be spatia
+00013a70: 6c6c 7920 696e 7465 7270 6f6c 6174 6564  lly interpolated
+00013a80: 2c20 696e 7374 6561 6420 6f66 207b 696d  , instead of {im
+00013a90: 6167 652e 7368 6170 657d 2e20 2229 0a20  age.shape}. "). 
+00013aa0: 2020 2069 6620 7472 616e 7320 6973 206e     if trans is n
+00013ab0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00013ac0: 2061 766f 7563 6828 696d 6167 652e 6e5f   avouch(image.n_
+00013ad0: 6261 7463 6820 3d3d 2031 206f 7220 7472  batch == 1 or tr
+00013ae0: 616e 732e 6e5f 6261 7463 6820 696e 2028  ans.n_batch in (
+00013af0: 4e6f 6e65 2c20 696d 6167 652e 6e5f 6261  None, image.n_ba
+00013b00: 7463 682c 2031 292c 2022 506c 6561 7365  tch, 1), "Please
+00013b10: 2075 7365 2074 7261 6e73 666f 726d 6174   use transformat
+00013b20: 696f 6e20 6f66 2061 2022 202b 0a20 2020  ion of a " +.   
+00013b30: 2020 2020 2020 2020 2066 2273 7569 7461           f"suita
+00013b40: 626c 6520 6e5f 6261 7463 6820 746f 2074  ble n_batch to t
+00013b50: 7261 6e73 666f 726d 2069 6d61 6765 2077  ransform image w
+00013b60: 6974 6820 6261 7463 6873 697a 6520 7b69  ith batchsize {i
+00013b70: 6d61 6765 2e6e 5f62 6174 6368 7d2c 2063  mage.n_batch}, c
+00013b80: 7572 7265 6e74 6c79 207b 7472 616e 732e  urrently {trans.
+00013b90: 6e5f 6261 7463 687d 2e22 290a 0a20 2020  n_batch}.")..   
+00013ba0: 206e 5f62 6174 6368 203d 2069 6d61 6765   n_batch = image
+00013bb0: 2e6e 5f62 6174 6368 0a20 2020 2069 6620  .n_batch.    if 
+00013bc0: 6e5f 6261 7463 6820 3d3d 2031 2061 6e64  n_batch == 1 and
+00013bd0: 2074 7261 6e73 2069 7320 6e6f 7420 4e6f   trans is not No
+00013be0: 6e65 2061 6e64 2074 7261 6e73 2e6e 5f62  ne and trans.n_b
+00013bf0: 6174 6368 2069 7320 6e6f 7420 4e6f 6e65  atch is not None
+00013c00: 2061 6e64 2074 7261 6e73 2e6e 5f62 6174   and trans.n_bat
+00013c10: 6368 203e 2031 3a20 6e5f 6261 7463 6820  ch > 1: n_batch 
+00013c20: 3d20 7472 616e 732e 6e5f 6261 7463 680a  = trans.n_batch.
+00013c30: 2020 2020 6966 206e 5f62 6174 6368 203d      if n_batch =
+00013c40: 3d20 3120 616e 6420 6973 696e 7374 616e  = 1 and isinstan
+00013c50: 6365 2874 6172 6765 745f 7370 6163 652c  ce(target_space,
+00013c60: 2062 742e 5465 6e73 6f72 2920 616e 6420   bt.Tensor) and 
+00013c70: 7461 7267 6574 5f73 7061 6365 2e68 6173  target_space.has
+00013c80: 5f62 6174 6368 2061 6e64 2074 6172 6765  _batch and targe
+00013c90: 745f 7370 6163 652e 6e5f 6261 7463 6820  t_space.n_batch 
+00013ca0: 3e20 313a 206e 5f62 6174 6368 203d 2074  > 1: n_batch = t
+00013cb0: 6172 6765 745f 7370 6163 652e 6e5f 6261  arget_space.n_ba
+00013cc0: 7463 680a 2020 2020 6966 2069 6d61 6765  tch.    if image
+00013cd0: 2e6e 5f62 6174 6368 203d 3d20 313a 2069  .n_batch == 1: i
+00013ce0: 6d61 6765 203d 2069 6d61 6765 2e72 6570  mage = image.rep
+00013cf0: 6561 7465 6428 6e5f 6261 7463 682c 205b  eated(n_batch, [
+00013d00: 5d29 0a20 2020 206e 5f66 6561 7475 7265  ]).    n_feature
+00013d10: 203d 2069 6d61 6765 2e6e 5f63 6861 6e6e   = image.n_chann
+00013d20: 656c 0a20 2020 2073 697a 6520 3d20 6274  el.    size = bt
+00013d30: 2e63 6861 6e6e 656c 5f74 656e 736f 7228  .channel_tensor(
+00013d40: 696d 6167 652e 7370 6163 6529 2e69 6e74  image.space).int
+00013d50: 2829 0a20 2020 2069 6620 6e5f 6261 7463  ().    if n_batc
+00013d60: 6820 3e20 3120 616e 6420 6e6f 7420 7368  h > 1 and not sh
+00013d70: 6170 655f 6f75 742e 6861 735f 6261 7463  ape_out.has_batc
+00013d80: 683a 2073 6861 7065 5f6f 7574 203d 2062  h: shape_out = b
+00013d90: 742e 5369 7a65 285b 6e5f 6261 7463 685d  t.Size([n_batch]
+00013da0: 2920 2b20 7368 6170 655f 6f75 740a 2020  ) + shape_out.  
+00013db0: 2020 6966 2074 6172 6765 745f 7370 6163    if target_spac
+00013dc0: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+00013dd0: 2020 2073 6361 6c65 2c20 2a70 6169 7273     scale, *pairs
+00013de0: 203d 2074 7261 6e73 2e72 6573 6861 7065   = trans.reshape
+00013df0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00013e00: 7363 616c 6529 203d 3d20 313a 2073 6361  scale) == 1: sca
+00013e10: 6c65 202a 3d20 6e5f 6469 6d0a 2020 2020  le *= n_dim.    
+00013e20: 2020 2020 7461 7267 6574 5f73 7061 6365      target_space
+00013e30: 203d 205b 696e 7428 7820 2a20 7929 2066   = [int(x * y) f
+00013e40: 6f72 2078 2c20 7920 696e 207a 6970 2869  or x, y in zip(i
+00013e50: 6d61 6765 2e73 7061 6365 2c20 7363 616c  mage.space, scal
+00013e60: 6529 5d0a 2020 2020 2020 2020 666f 7220  e)].        for 
+00013e70: 702c 2071 2069 6e20 7061 6972 733a 2074  p, q in pairs: t
+00013e80: 6172 6765 745f 7370 6163 655b 705d 2c20  arget_space[p], 
+00013e90: 7461 7267 6574 5f73 7061 6365 5b71 5d20  target_space[q] 
+00013ea0: 3d20 7461 7267 6574 5f73 7061 6365 5b71  = target_space[q
+00013eb0: 5d2c 2074 6172 6765 745f 7370 6163 655b  ], target_space[
+00013ec0: 705d 0a20 2020 2020 2020 2074 6172 6765  p].        targe
+00013ed0: 745f 7370 6163 6520 3d20 7475 706c 6528  t_space = tuple(
+00013ee0: 7461 7267 6574 5f73 7061 6365 290a 2020  target_space).  
+00013ef0: 2020 2020 2020 7368 6170 655f 6f75 7420        shape_out 
+00013f00: 3d20 7368 6170 655f 6f75 742e 7265 7365  = shape_out.rese
+00013f10: 745f 7370 6163 6528 7461 7267 6574 5f73  t_space(target_s
+00013f20: 7061 6365 290a 2020 2020 6966 2069 7369  pace).    if isi
+00013f30: 6e73 7461 6e63 6528 7461 7267 6574 5f73  nstance(target_s
+00013f40: 7061 6365 2c20 7475 706c 6529 2061 6e64  pace, tuple) and
+00013f50: 206c 656e 2874 6172 6765 745f 7370 6163   len(target_spac
+00013f60: 6529 203d 3d20 6e5f 6469 6d3a 2070 6173  e) == n_dim: pas
+00013f70: 730a 2020 2020 656c 6966 2069 7369 6e73  s.    elif isins
+00013f80: 7461 6e63 6528 7461 7267 6574 5f73 7061  tance(target_spa
+00013f90: 6365 2c20 6274 2e74 6f72 6368 2e54 656e  ce, bt.torch.Ten
+00013fa0: 736f 7229 3a20 7061 7373 0a20 2020 2065  sor): pass.    e
+00013fb0: 6c73 653a 2072 6169 7365 2054 7970 6545  lse: raise TypeE
+00013fc0: 7272 6f72 2866 2257 726f 6e67 2074 6172  rror(f"Wrong tar
+00013fd0: 6765 7420 7370 6163 6520 666f 7220 696e  get space for in
+00013fe0: 7465 7270 6f6c 6174 696f 6e3a 207b 7461  terpolation: {ta
+00013ff0: 7267 6574 5f73 7061 6365 7d2e 2022 290a  rget_space}. ").
+00014000: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00014010: 6528 7461 7267 6574 5f73 7061 6365 2c20  e(target_space, 
+00014020: 7475 706c 6529 3a20 0a20 2020 2020 2020  tuple): .       
+00014030: 2023 2043 7265 6174 6520 6120 6772 6964   # Create a grid
+00014040: 2058 2077 6974 6820 7369 7a65 2028 7b6e   X with size ({n
+00014050: 5f64 696d 7d2c 2073 697a 655f 312c 2073  _dim}, size_1, s
+00014060: 697a 655f 322c 202e 2e2e 2c20 7369 7a65  ize_2, ..., size
+00014070: 5f72 2920 5b72 3d6e 5f64 696d 5d2e 0a20  _r) [r=n_dim].. 
+00014080: 2020 2020 2020 2058 203d 2062 742e 696d         X = bt.im
+00014090: 6167 655f 6772 6964 2874 6172 6765 745f  age_grid(target_
+000140a0: 7370 6163 6529 2e66 6c6f 6174 2829 2023  space).float() #
+000140b0: 202b 2062 742e 6368 616e 6e65 6c5f 7465   + bt.channel_te
+000140c0: 6e73 6f72 285b 666c 6f61 7428 612d 6229  nsor([float(a-b)
+000140d0: 2f32 2066 6f72 2061 2c20 6220 696e 207a  /2 for a, b in z
+000140e0: 6970 2869 6d61 6765 2e73 7061 6365 2c20  ip(image.space, 
+000140f0: 7461 7267 6574 5f73 7061 6365 295d 290a  target_space)]).
+00014100: 2020 2020 2020 2020 2320 436f 6d70 7574          # Comput
+00014110: 6520 7468 6520 7472 616e 7366 6f72 6d65  e the transforme
+00014120: 6420 636f 6f72 6469 6e61 7465 732e 2059  d coordinates. Y
+00014130: 3a20 285b 6e5f 6261 7463 685d 2c20 7b6e  : ([n_batch], {n
+00014140: 5f64 696d 7d2c 2073 697a 655f 312c 2073  _dim}, size_1, s
+00014150: 697a 655f 322c 202e 2e2e 2c20 7369 7a65  ize_2, ..., size
+00014160: 5f72 2920 5b72 3d6e 5f64 696d 5d2e 0a20  _r) [r=n_dim].. 
+00014170: 2020 2020 2020 2069 6620 7472 616e 7320         if trans 
+00014180: 6973 204e 6f6e 653a 2074 7261 6e73 203d  is None: trans =
+00014190: 2049 6465 6e74 6974 7928 290a 2020 2020   Identity().    
+000141a0: 2020 2020 5920 3d20 7472 616e 7328 5829      Y = trans(X)
+000141b0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000141c0: 592e 6861 735f 6261 7463 683a 2059 203d  Y.has_batch: Y =
+000141d0: 2059 2e6d 756c 7469 706c 7928 6e5f 6261   Y.multiply(n_ba
+000141e0: 7463 682c 205b 5d29 0a20 2020 2020 2020  tch, []).       
+000141f0: 2069 6620 592e 6e5f 6261 7463 6820 3d3d   if Y.n_batch ==
+00014200: 2031 3a20 5920 3d20 592e 7265 7065 6174   1: Y = Y.repeat
+00014210: 6564 286e 5f62 6174 6368 2c20 5b5d 290a  ed(n_batch, []).
+00014220: 2020 2020 2020 2020 5920 3d20 592e 616d          Y = Y.am
+00014230: 706c 6966 7928 6e5f 6665 6174 7572 652c  plify(n_feature,
+00014240: 205b 5d29 0a20 2020 2020 2020 2073 6861   []).        sha
+00014250: 7065 5f6f 7574 203d 2073 6861 7065 5f6f  pe_out = shape_o
+00014260: 7574 2e72 6573 6574 5f73 7061 6365 2874  ut.reset_space(t
+00014270: 6172 6765 745f 7370 6163 6529 0a20 2020  arget_space).   
+00014280: 2065 6c73 653a 0a20 2020 2020 2020 2074   else:.        t
+00014290: 6172 6765 745f 7370 6163 6520 3d20 6261  arget_space = ba
+000142a0: 746f 7263 685f 7465 6e73 6f72 2874 6172  torch_tensor(tar
+000142b0: 6765 745f 7370 6163 6529 0a20 2020 2020  get_space).     
+000142c0: 2020 2069 6620 6e6f 7420 7461 7267 6574     if not target
+000142d0: 5f73 7061 6365 2e68 6173 5f62 6174 6368  _space.has_batch
+000142e0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000142f0: 2074 6172 6765 745f 7370 6163 652e 7369   target_space.si
+00014300: 7a65 2830 2920 3d3d 206e 5f62 6174 6368  ze(0) == n_batch
+00014310: 2061 6e64 206e 5f62 6174 6368 2021 3d20   and n_batch != 
+00014320: 6e5f 6469 6d20 6f72 206c 656e 285b 7820  n_dim or len([x 
+00014330: 666f 7220 7820 696e 2074 6172 6765 745f  for x in target_
+00014340: 7370 6163 652e 7368 6170 6520 6966 2078  space.shape if x
+00014350: 203d 3d20 6e5f 6469 6d5d 2920 3e3d 2032   == n_dim]) >= 2
+00014360: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014370: 2020 7461 7267 6574 5f73 7061 6365 2e77    target_space.w
+00014380: 6974 685f 6261 7463 6864 696d 2830 290a  ith_batchdim(0).
+00014390: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000143a0: 3a20 7461 7267 6574 5f73 7061 6365 2e75  : target_space.u
+000143b0: 6e73 7175 6565 7a65 5f28 5b5d 290a 2020  nsqueeze_([]).  
+000143c0: 2020 2020 2020 6966 206e 6f74 2074 6172        if not tar
+000143d0: 6765 745f 7370 6163 652e 6861 735f 6368  get_space.has_ch
+000143e0: 616e 6e65 6c3a 0a20 2020 2020 2020 2020  annel:.         
+000143f0: 2020 2069 6620 7461 7267 6574 5f73 7061     if target_spa
+00014400: 6365 2e62 6174 6368 5f64 696d 656e 7369  ce.batch_dimensi
+00014410: 6f6e 2021 3d20 3020 616e 6420 7461 7267  on != 0 and targ
+00014420: 6574 5f73 7061 6365 2e73 697a 6528 3029  et_space.size(0)
+00014430: 203d 3d20 6e5f 6469 6d3a 2074 6172 6765   == n_dim: targe
+00014440: 745f 7370 6163 652e 7769 7468 5f63 6861  t_space.with_cha
+00014450: 6e6e 656c 6469 6d28 3029 0a20 2020 2020  nneldim(0).     
+00014460: 2020 2020 2020 2065 6c69 6620 7461 7267         elif targ
+00014470: 6574 5f73 7061 6365 2e62 6174 6368 5f64  et_space.batch_d
+00014480: 696d 656e 7369 6f6e 2021 3d20 3120 616e  imension != 1 an
+00014490: 6420 7461 7267 6574 5f73 7061 6365 2e73  d target_space.s
+000144a0: 697a 6528 3129 203d 3d20 6e5f 6469 6d3a  ize(1) == n_dim:
+000144b0: 2074 6172 6765 745f 7370 6163 652e 7769   target_space.wi
+000144c0: 7468 5f63 6861 6e6e 656c 6469 6d28 3129  th_channeldim(1)
+000144d0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+000144e0: 6620 7461 7267 6574 5f73 7061 6365 2e62  f target_space.b
+000144f0: 6174 6368 5f64 696d 656e 7369 6f6e 2021  atch_dimension !
+00014500: 3d20 7461 7267 6574 5f73 7061 6365 2e6e  = target_space.n
+00014510: 5f64 696d 202d 2031 2061 6e64 2074 6172  _dim - 1 and tar
+00014520: 6765 745f 7370 6163 652e 7369 7a65 282d  get_space.size(-
+00014530: 3129 203d 3d20 6e5f 6469 6d3a 2074 6172  1) == n_dim: tar
+00014540: 6765 745f 7370 6163 652e 7769 7468 5f63  get_space.with_c
+00014550: 6861 6e6e 656c 6469 6d28 2d31 290a 2020  hanneldim(-1).  
+00014560: 2020 2020 2020 6176 6f75 6368 2874 6172        avouch(tar
+00014570: 6765 745f 7370 6163 652e 6861 735f 6368  get_space.has_ch
+00014580: 616e 6e65 6c20 616e 6420 7461 7267 6574  annel and target
+00014590: 5f73 7061 6365 2e6e 5f63 6861 6e6e 656c  _space.n_channel
+000145a0: 203d 3d20 6e5f 6469 6d2c 2022 2774 6172   == n_dim, "'tar
+000145b0: 6765 745f 7370 6163 6527 2066 6f72 2069  get_space' for i
+000145c0: 6e74 6572 706f 6c61 7469 6f6e 2073 686f  nterpolation sho
+000145d0: 756c 6420 6861 7665 2061 2063 6861 6e6e  uld have a chann
+000145e0: 656c 2064 696d 656e 7369 6f6e 2066 6f72  el dimension for
+000145f0: 2063 6f6f 7264 696e 6174 6573 2e20 2229   coordinates. ")
+00014600: 0a20 2020 2020 2020 2059 203d 2074 6172  .        Y = tar
+00014610: 6765 745f 7370 6163 652e 7265 7065 6174  get_space.repeat
+00014620: 6564 286e 5f62 6174 6368 202f 2f20 7461  ed(n_batch // ta
+00014630: 7267 6574 5f73 7061 6365 2e6e 5f62 6174  rget_space.n_bat
+00014640: 6368 2c20 5b5d 292e 616d 706c 6966 7928  ch, []).amplify(
+00014650: 6e5f 6665 6174 7572 652c 205b 5d29 0a20  n_feature, []). 
+00014660: 2020 2020 2020 2073 6861 7065 5f6f 7574         shape_out
+00014670: 203d 2073 6861 7065 5f6f 7574 2e72 6573   = shape_out.res
+00014680: 6574 5f73 7061 6365 2874 6172 6765 745f  et_space(target_
+00014690: 7370 6163 652e 7370 6163 6529 0a20 2020  space.space).   
+000146a0: 2020 2020 200a 2020 2020 696d 6167 6520       .    image 
+000146b0: 3d20 696d 6167 652e 6d65 7267 6564 696d  = image.mergedim
+000146c0: 7328 7b7d 2c20 5b5d 290a 2020 2020 6e5f  s({}, []).    n_
+000146d0: 6261 7463 6820 3d20 696d 6167 652e 6e5f  batch = image.n_
+000146e0: 6261 7463 680a 0a20 2020 2069 6620 6d65  batch..    if me
+000146f0: 7468 6f64 2e6c 6f77 6572 2829 203d 3d20  thod.lower() == 
+00014700: 2762 7370 6c69 6e65 273a 0a20 2020 2020  'bspline':.     
+00014710: 2020 2069 6620 6465 7269 7661 7469 7665     if derivative
+00014720: 3a20 7261 6973 6520 5479 7065 4572 726f  : raise TypeErro
+00014730: 7228 224e 6f20 6465 7269 7661 7469 7665  r("No derivative
+00014740: 7320 666f 7220 6273 706c 696e 6520 696e  s for bspline in
+00014750: 7465 7270 6f6c 6174 696f 6e73 2061 7265  terpolations are
+00014760: 2061 7661 696c 6162 6c65 2073 6f20 6661   available so fa
+00014770: 722e 2050 6c65 6173 6520 7772 6974 6520  r. Please write 
+00014780: 6974 2062 7920 796f 7572 7365 6c66 2e20  it by yourself. 
+00014790: 2229 0a20 2020 2020 2020 2023 2054 4f44  ").        # TOD
+000147a0: 4f3a 2046 4644 0a20 2020 2020 2020 2072  O: FFD.        r
+000147b0: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
+000147c0: 4273 706c 696e 6520 696e 7465 7270 6f6c  Bspline interpol
+000147d0: 6174 696f 6e20 6973 206e 6f74 2061 7661  ation is not ava
+000147e0: 696c 6162 6c65 2073 6f20 6661 722e 2050  ilable so far. P
+000147f0: 6c65 6173 6520 7772 6974 6520 6974 2062  lease write it b
+00014800: 7920 796f 7572 7365 6c66 2e20 2229 0a0a  y yourself. ")..
+00014810: 2020 2020 6959 203d 2062 742e 666c 6f6f      iY = bt.floo
+00014820: 7228 5929 2e6c 6f6e 6728 2920 2320 4765  r(Y).long() # Ge
+00014830: 6e65 7261 7465 2074 6865 2069 6e74 6567  nerate the integ
+00014840: 6572 2070 6172 7420 6f66 2059 0a20 2020  er part of Y.   
+00014850: 206a 5920 3d20 6959 202b 2031 2023 2061   jY = iY + 1 # a
+00014860: 6e64 2074 6865 2069 6e74 6567 6572 2070  nd the integer p
+00014870: 6172 7420 706c 7573 206f 6e65 2e0a 2020  art plus one..  
+00014880: 2020 6966 206d 6574 686f 642e 6c6f 7765    if method.lowe
+00014890: 7228 2920 3d3d 2027 6c69 6e65 6172 273a  r() == 'linear':
+000148a0: 2066 5920 3d20 5920 2d20 6959 2e66 6c6f   fY = Y - iY.flo
+000148b0: 6174 2829 2023 2054 6865 2064 6563 696d  at() # The decim
+000148c0: 616c 2070 6172 7420 6f66 2059 2e0a 2020  al part of Y..  
+000148d0: 2020 656c 6966 206d 6574 686f 642e 6c6f    elif method.lo
+000148e0: 7765 7228 2920 3d3d 2027 6e65 6172 6573  wer() == 'neares
+000148f0: 7427 3a20 6659 203d 2062 742e 666c 6f6f  t': fY = bt.floo
+00014900: 7228 5920 2d20 6959 2e66 6c6f 6174 2829  r(Y - iY.float()
+00014910: 202b 2030 2e35 2920 2320 5468 6520 6465   + 0.5) # The de
+00014920: 6369 6d61 6c20 7061 7274 206f 6620 592e  cimal part of Y.
+00014930: 0a20 2020 2065 6c73 653a 2072 6169 7365  .    else: raise
+00014940: 2054 7970 6545 7272 6f72 2822 556e 7265   TypeError("Unre
+00014950: 636f 676e 697a 6564 2061 7267 756d 656e  cognized argumen
+00014960: 7420 276d 6574 686f 6427 2e20 2229 0a20  t 'method'. "). 
+00014970: 2020 2062 5920 3d20 6274 2e73 7461 636b     bY = bt.stack
+00014980: 2828 6959 2c20 6a59 292c 2031 292e 7669  ((iY, jY), 1).vi
+00014990: 6577 285b 6e5f 6261 7463 685d 2c20 322c  ew([n_batch], 2,
+000149a0: 207b 6e5f 6469 6d7d 2c20 2d31 2920 2320   {n_dim}, -1) # 
+000149b0: 285b 6e5f 6261 7463 685d 2c20 322c 207b  ([n_batch], 2, {
+000149c0: 6e5f 6469 6d7d 2c20 6e5f 6461 7461 292e  n_dim}, n_data).
+000149d0: 0a20 2020 2057 203d 2062 742e 7374 6163  .    W = bt.stac
+000149e0: 6b28 2831 202d 2066 592c 2066 5929 2c20  k((1 - fY, fY), 
+000149f0: 3129 2e76 6965 7728 5b6e 5f62 6174 6368  1).view([n_batch
+00014a00: 5d2c 2032 2c20 7b6e 5f64 696d 7d2c 202d  ], 2, {n_dim}, -
+00014a10: 3129 2023 2028 5b6e 5f62 6174 6368 5d2c  1) # ([n_batch],
+00014a20: 2032 2c20 7b6e 5f64 696d 7d2c 206e 5f64   2, {n_dim}, n_d
+00014a30: 6174 6129 2e0a 2020 2020 6e5f 6461 7461  ata)..    n_data
+00014a40: 203d 2062 592e 7369 7a65 282d 3129 0a0a   = bY.size(-1)..
+00014a50: 2020 2020 2320 5072 6570 6172 6520 666f      # Prepare fo
+00014a60: 7220 7468 6520 6f75 7470 7574 2073 7061  r the output spa
+00014a70: 6365 3a20 6e5f 6261 7463 682c 206d 5f31  ce: n_batch, m_1
+00014a80: 2c20 2e2e 2e2c 206d 5f73 0a20 2020 2069  , ..., m_s.    i
+00014a90: 6620 6465 7269 7661 7469 7665 3a20 6f75  f derivative: ou
+00014aa0: 7470 7574 203d 2062 742e 7a65 726f 7328  tput = bt.zeros(
+00014ab0: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 6469  [n_batch], {n_di
+00014ac0: 6d7d 2c20 2a73 6861 7065 5f6f 7574 2e73  m}, *shape_out.s
+00014ad0: 7061 6365 290a 2020 2020 656c 7365 3a20  pace).    else: 
+00014ae0: 6f75 7470 7574 203d 2062 742e 7a65 726f  output = bt.zero
+00014af0: 7328 7368 6170 655f 6f75 7429 0a20 2020  s(shape_out).   
+00014b00: 2066 6f72 2047 2069 6e20 6274 2e69 6d61   for G in bt.ima
+00014b10: 6765 5f67 7269 6428 5b32 5d2a 6e5f 6469  ge_grid([2]*n_di
+00014b20: 6d29 2e66 6c61 7474 656e 2829 2e74 7261  m).flatten().tra
+00014b30: 6e73 706f 7365 2830 2c20 3129 3a0a 2020  nspose(0, 1):.  
+00014b40: 2020 2020 2020 2320 4765 7420 7468 6520        # Get the 
+00014b50: 696e 6469 6365 7320 666f 7220 7468 6520  indices for the 
+00014b60: 7465 726d 3a20 6259 5b3a 2c20 475b 445d  term: bY[:, G[D]
+00014b70: 2c20 442c 203a 5d2c 2073 697a 653d 285b  , D, :], size=([
+00014b80: 6e5f 6261 7463 685d 2c20 7b6e 5f64 696d  n_batch], {n_dim
+00014b90: 7d2c 206e 5f64 6174 6129 0a20 2020 2020  }, n_data).     
+00014ba0: 2020 2049 6e64 203d 2062 592e 6761 7468     Ind = bY.gath
+00014bb0: 6572 2831 2c20 472e 6578 7061 6e64 5f74  er(1, G.expand_t
+00014bc0: 6f28 5b6e 5f62 6174 6368 5d2c 2031 2c20  o([n_batch], 1, 
+00014bd0: 7b6e 5f64 696d 7d2c 206e 5f64 6174 6129  {n_dim}, n_data)
+00014be0: 292e 7371 7565 657a 6528 3129 0a20 2020  ).squeeze(1).   
+00014bf0: 2020 2020 2023 2043 6c61 6d70 2074 6865       # Clamp the
+00014c00: 2069 6e64 6963 6573 2069 6e20 7468 6520   indices in the 
+00014c10: 636f 7272 6563 7420 7261 6e67 6520 2620  correct range & 
+00014c20: 436f 6d70 7574 6520 7468 6520 626f 7264  Compute the bord
+00014c30: 6572 2063 6f6e 6469 7469 6f6e 0a20 2020  er condition.   
+00014c40: 2020 2020 2063 6f6e 6469 7469 6f6e 203d       condition =
+00014c50: 2062 742e 7375 6d28 2849 6e64 203c 2030   bt.sum((Ind < 0
+00014c60: 2920 2b20 2849 6e64 203e 2073 697a 6520  ) + (Ind > size 
+00014c70: 2d20 3129 2c20 3129 0a20 2020 2020 2020  - 1), 1).       
+00014c80: 2049 6e64 203d 2062 742e 6d69 6e28 6274   Ind = bt.min(bt
+00014c90: 2e63 6c61 6d70 2849 6e64 2c20 6d69 6e3d  .clamp(Ind, min=
+00014ca0: 3029 2c20 2873 697a 6520 2d20 3129 2e65  0), (size - 1).e
+00014cb0: 7870 616e 645f 746f 2849 6e64 2929 0a20  xpand_to(Ind)). 
+00014cc0: 2020 2020 2020 2023 2043 6f6e 7665 7274         # Convert
+00014cd0: 2074 6865 2069 6e64 6963 6573 2074 6f20   the indices to 
+00014ce0: 3120 6469 6d65 6e73 696f 6e61 6c2e 2044  1 dimensional. D
+00014cf0: 6f74 3a20 285b 6e5f 6261 7463 685d 2c20  ot: ([n_batch], 
+00014d00: 6e5f 6461 7461 290a 2020 2020 2020 2020  n_data).        
+00014d10: 446f 7420 3d20 496e 645b 3a2c 2030 5d0a  Dot = Ind[:, 0].
+00014d20: 2020 2020 2020 2020 666f 7220 7220 696e          for r in
+00014d30: 2072 616e 6765 2831 2c20 6e5f 6469 6d29   range(1, n_dim)
+00014d40: 3a20 446f 7420 2a3d 2073 697a 655b 725d  : Dot *= size[r]
+00014d50: 3b20 446f 7420 2b3d 2049 6e64 5b3a 2c20  ; Dot += Ind[:, 
+00014d60: 725d 0a20 2020 2020 2020 2023 2047 6574  r].        # Get
+00014d70: 2074 6865 2069 6d61 6765 2076 616c 7565   the image value
+00014d80: 7320 4956 3a20 285b 6e5f 6261 7463 685d  s IV: ([n_batch]
+00014d90: 2c20 6e5f 6461 7461 290a 2020 2020 2020  , n_data).      
+00014da0: 2020 4956 203d 204e 6f6e 650a 2020 2020    IV = None.    
+00014db0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00014dc0: 6528 6669 6c6c 2c20 7374 7229 3a0a 2020  e(fill, str):.  
+00014dd0: 2020 2020 2020 2020 2020 6966 2066 696c            if fil
+00014de0: 6c2e 6c6f 7765 7228 2920 3d3d 2027 6e65  l.lower() == 'ne
+00014df0: 6172 6573 7427 3a0a 2020 2020 2020 2020  arest':.        
+00014e00: 2020 2020 2020 2020 4956 203d 2069 6d61          IV = ima
+00014e10: 6765 2e66 6c61 7474 656e 2829 2e67 6174  ge.flatten().gat
+00014e20: 6865 7228 312c 2044 6f74 290a 2020 2020  her(1, Dot).    
+00014e30: 2020 2020 2020 2020 656c 6966 2066 696c          elif fil
+00014e40: 6c2e 6c6f 7765 7228 2920 3d3d 2027 6261  l.lower() == 'ba
+00014e50: 636b 6772 6f75 6e64 273a 0a20 2020 2020  ckground':.     
+00014e60: 2020 2020 2020 2020 2020 2062 6b5f 7661             bk_va
+00014e70: 6c75 6520 3d20 6274 2e73 7461 636b 285b  lue = bt.stack([
+00014e80: 696d 6167 655b 2873 6c69 6365 284e 6f6e  image[(slice(Non
+00014e90: 6529 2c29 202b 2074 7570 6c65 2867 295d  e),) + tuple(g)]
+00014ea0: 2066 6f72 2067 2069 6e20 2862 742e 696d   for g in (bt.im
+00014eb0: 6167 655f 6772 6964 285b 325d 2a6e 5f64  age_grid([2]*n_d
+00014ec0: 696d 2920 2a20 6274 2e63 6861 6e6e 656c  im) * bt.channel
+00014ed0: 5f74 656e 736f 7228 7369 7a65 2d31 2929  _tensor(size-1))
+00014ee0: 2e66 6c61 7474 656e 2829 2e74 7261 6e73  .flatten().trans
+00014ef0: 706f 7365 2830 2c31 295d 2c20 3129 2e6d  pose(0,1)], 1).m
+00014f00: 6564 6961 6e28 3129 2e76 616c 7565 730a  edian(1).values.
+00014f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f20: 6261 636b 6772 6f75 6e64 203d 2062 6b5f  background = bk_
+00014f30: 7661 6c75 6520 2a20 6274 2e6f 6e65 735f  value * bt.ones_
+00014f40: 6c69 6b65 2844 6f74 290a 2020 2020 2020  like(Dot).      
+00014f50: 2020 2020 2020 656c 6966 2066 696c 6c2e        elif fill.
+00014f60: 6c6f 7765 7228 2920 3d3d 2027 7a65 726f  lower() == 'zero
+00014f70: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
+00014f80: 2020 2062 6163 6b67 726f 756e 6420 3d20     background = 
+00014f90: 6274 2e7a 6572 6f73 5f6c 696b 6528 446f  bt.zeros_like(Do
+00014fa0: 7429 0a20 2020 2020 2020 2065 6c73 653a  t).        else:
+00014fb0: 0a20 2020 2020 2020 2020 2020 2062 6163  .            bac
+00014fc0: 6b67 726f 756e 6420 3d20 6669 6c6c 202a  kground = fill *
+00014fd0: 2062 742e 6f6e 6573 5f6c 696b 6528 446f   bt.ones_like(Do
+00014fe0: 7429 0a20 2020 2020 2020 2069 6620 4956  t).        if IV
+00014ff0: 2069 7320 4e6f 6e65 3a20 4956 203d 2062   is None: IV = b
+00015000: 742e 7768 6572 6528 636f 6e64 6974 696f  t.where(conditio
+00015010: 6e20 3e3d 2031 2c20 6261 636b 6772 6f75  n >= 1, backgrou
+00015020: 6e64 2e66 6c6f 6174 2829 2c20 696d 6167  nd.float(), imag
+00015030: 652e 666c 6174 7465 6e28 292e 6761 7468  e.flatten().gath
+00015040: 6572 2831 2c20 446f 7429 2e66 6c6f 6174  er(1, Dot).float
+00015050: 2829 290a 2020 2020 2020 2020 2320 5765  ()).        # We
+00015060: 6967 6874 7320 666f 7220 6561 6368 2070  ights for each p
+00015070: 6f69 6e74 3a20 5b70 726f 6475 6374 206f  oint: [product o
+00015080: 6620 575b 3a2c 2047 5b44 5d2c 2044 2c20  f W[:, G[D], D, 
+00015090: 785d 2066 6f72 2044 2069 6e20 7261 6e67  x] for D in rang
+000150a0: 6528 6e5f 6469 6d29 5d20 666f 7220 706f  e(n_dim)] for po
+000150b0: 696e 7420 782e 0a20 2020 2020 2020 2023  int x..        #
+000150c0: 2057 673a 2028 5b6e 5f62 6174 6368 5d2c   Wg: ([n_batch],
+000150d0: 207b 6e5f 6469 6d7d 2c20 6e5f 6461 7461   {n_dim}, n_data
+000150e0: 290a 2020 2020 2020 2020 5767 203d 2057  ).        Wg = W
+000150f0: 2e67 6174 6865 7228 312c 2047 2e65 7870  .gather(1, G.exp
+00015100: 616e 645f 746f 285b 6e5f 6261 7463 685d  and_to([n_batch]
+00015110: 2c20 312c 207b 6e5f 6469 6d7d 2c20 6e5f  , 1, {n_dim}, n_
+00015120: 6461 7461 2929 2e73 7175 6565 7a65 2831  data)).squeeze(1
+00015130: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00015140: 2064 6572 6976 6174 6976 653a 0a20 2020   derivative:.   
+00015150: 2020 2020 2020 2020 206f 7574 7075 7420           output 
+00015160: 2b3d 2028 5767 2e70 726f 6428 3129 202a  += (Wg.prod(1) *
+00015170: 2049 5629 2e76 6965 775f 6173 286f 7574   IV).view_as(out
+00015180: 7075 7429 0a20 2020 2020 2020 2065 6c73  put).        els
+00015190: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+000151a0: 656d 7057 674d 6174 203d 2057 672e 6d75  empWgMat = Wg.mu
+000151b0: 6c74 6970 6c79 286e 5f64 696d 2c20 3129  ltiply(n_dim, 1)
+000151c0: 2023 2028 5b6e 5f62 6174 6368 5d2c 206e   # ([n_batch], n
+000151d0: 5f64 696d 2c20 7b6e 5f64 696d 7d2c 206e  _dim, {n_dim}, n
+000151e0: 5f64 6174 6129 0a20 2020 2020 2020 2020  _data).         
+000151f0: 2020 2074 656d 7057 674d 6174 5b3a 2c20     tempWgMat[:, 
+00015200: 6274 2e61 7261 6e67 6528 6e5f 6469 6d29  bt.arange(n_dim)
+00015210: 2c20 6274 2e61 7261 6e67 6528 6e5f 6469  , bt.arange(n_di
+00015220: 6d29 5d20 3d20 310a 2020 2020 2020 2020  m)] = 1.        
+00015230: 2020 2020 6457 6720 3d20 7465 6d70 5767      dWg = tempWg
+00015240: 4d61 742e 7072 6f64 2831 2920 2a20 2847  Mat.prod(1) * (G
+00015250: 202a 2032 202d 2031 292e 666c 6f61 7428   * 2 - 1).float(
+00015260: 290a 2020 2020 2020 2020 2020 2020 6f75  ).            ou
+00015270: 7470 7574 202b 3d20 2864 5767 202a 2049  tput += (dWg * I
+00015280: 562e 756e 7371 7565 657a 6528 3129 292e  V.unsqueeze(1)).
+00015290: 7669 6577 5f61 7328 6f75 7470 7574 290a  view_as(output).
+000152a0: 2020 2020 6274 2e74 6f72 6368 2e63 7564      bt.torch.cud
+000152b0: 612e 656d 7074 795f 6361 6368 6528 290a  a.empty_cache().
+000152c0: 2020 2020 6570 7320 3d20 3165 2d36 0a20      eps = 1e-6. 
+000152d0: 2020 206d 203d 2030 2069 6620 696d 6167     m = 0 if imag
+000152e0: 652e 6d69 6e28 2920 3e20 2d65 7073 2065  e.min() > -eps e
+000152f0: 6c73 6520 696d 6167 652e 6d69 6e28 292e  lse image.min().
+00015300: 6974 656d 2829 0a20 2020 204d 203d 2031  item().    M = 1
+00015310: 2069 6620 696d 6167 652e 6d61 7828 2920   if image.max() 
+00015320: 3c20 3120 2b20 6570 7320 656c 7365 2069  < 1 + eps else i
+00015330: 6d61 6765 2e6d 6178 2829 2e69 7465 6d28  mage.max().item(
+00015340: 290a 2020 2020 7265 7475 726e 206f 7574  ).    return out
+00015350: 7075 742e 636c 616d 7028 6d2c 204d 290a  put.clamp(m, M).
+00015360: 0a40 616c 6961 7328 2272 6573 616d 706c  .@alias("resampl
+00015370: 655f 666f 7277 6172 6422 290a 6465 6620  e_forward").def 
+00015380: 696e 7465 7270 6f6c 6174 696f 6e5f 666f  interpolation_fo
+00015390: 7277 6172 6428 0a20 2020 2020 2020 2069  rward(.        i
+000153a0: 6d61 6765 2c20 0a20 2020 2020 2020 2074  mage, .        t
+000153b0: 7261 6e73 203d 204e 6f6e 652c 200a 2020  rans = None, .  
+000153c0: 2020 2020 2020 6d65 7468 6f64 203d 2027        method = '
+000153d0: 4c69 6e65 6172 272c 200a 2020 2020 2020  Linear', .      
+000153e0: 2020 7461 7267 6574 5f73 7061 6365 203d    target_space =
+000153f0: 204e 6f6e 652c 0a20 2020 2020 2020 2066   None,.        f
+00015400: 696c 6c20 3d20 277a 6572 6f27 2c0a 2020  ill = 'zero',.  
+00015410: 2020 2020 2020 6465 7269 7661 7469 7665        derivative
+00015420: 203d 2046 616c 7365 0a20 2020 2029 3a0a   = False.    ):.
+00015430: 2020 2020 2727 270a 2020 2020 496e 7465      '''.    Inte
+00015440: 7270 6f6c 6174 6520 7573 696e 6720 666f  rpolate using fo
+00015450: 7277 6172 6420 7472 616e 7366 6f72 6d61  rward transforma
+00015460: 7469 6f6e 2e20 4974 2069 7320 6e6f 7420  tion. It is not 
+00015470: 7965 7420 696d 706c 656d 656e 7465 642e  yet implemented.
+00015480: 200a 2020 2020 692e 652e 2043 6f6d 7075   .    i.e. Compu
+00015490: 7465 2074 6865 2069 6d61 6765 2049 2073  te the image I s
+000154a0: 2e74 2e20 7472 616e 7328 7829 203d 2079  .t. trans(x) = y
+000154b0: 2066 6f72 2078 2069 6e20 696e 7075 7420   for x in input 
+000154c0: 696d 6167 6520 616e 6420 7920 696e 2074  image and y in t
+000154d0: 6865 206f 7574 7075 7420 4920 7573 696e  he output I usin
+000154e0: 6720 696e 7465 7270 6f6c 6174 696f 6e20  g interpolation 
+000154f0: 6d65 7468 6f64 3a0a 2020 2020 2020 2020  method:.        
+00015500: 6d65 7468 6f64 203d 204c 696e 6561 7220  method = Linear 
+00015510: 5b4e 4f20 4752 4144 4945 4e54 2121 215d  [NO GRADIENT!!!]
+00015520: 3a20 4269 6c69 6e65 6172 2069 6e74 6572  : Bilinear inter
+00015530: 706f 6c61 7469 6f6e 0a20 2020 2020 2020  polation.       
+00015540: 206d 6574 686f 6420 3d20 4e65 6172 6573   method = Neares
+00015550: 7420 5b4e 4f20 4752 4144 4945 4e54 2121  t [NO GRADIENT!!
+00015560: 215d 3a20 4e65 6172 6573 7420 696e 7465  !]: Nearest inte
+00015570: 7270 6f6c 6174 696f 6e0a 0a20 2020 2050  rpolation..    P
+00015580: 6172 616d 733a 0a20 2020 2020 2020 2069  arams:.        i
+00015590: 6d61 6765 205b 6274 2e54 656e 736f 725d  mage [bt.Tensor]
+000155a0: 3a20 5468 6520 7461 7267 6574 2069 6d61  : The target ima
+000155b0: 6765 2e0a 2020 2020 2020 2020 2020 2020  ge..            
+000155c0: 7369 7a65 3a20 285b 6e5f 6261 7463 683a  size: ([n_batch:
+000155d0: 6f70 7469 6f6e 616c 5d2c 207b 6e5f 6368  optional], {n_ch
+000155e0: 616e 6e65 6c3a 6f70 7469 6f6e 616c 7d2c  annel:optional},
+000155f0: 206d 4031 2c20 6d40 322c 202e 2e2e 2c20   m@1, m@2, ..., 
+00015600: 6d40 6e5f 6469 6d29 0a20 2020 2020 2020  m@n_dim).       
+00015610: 2074 7261 6e73 205b 4675 6e63 7469 6f6e   trans [Function
+00015620: 206f 7220 6d69 636f 6d70 7574 696e 672e   or micomputing.
+00015630: 5370 6174 6961 6c54 7261 6e73 666f 726d  SpatialTransform
+00015640: 6174 696f 6e5d 3a20 5472 616e 7366 6f72  ation]: Transfor
+00015650: 6d61 7469 6f6e 2066 756e 6374 696f 6e2c  mation function,
+00015660: 206d 6170 7069 6e67 0a20 2020 2020 2020   mapping.       
+00015670: 2020 2020 2073 697a 653a 2028 5b6e 5f62       size: ([n_b
+00015680: 6174 6368 3a6f 7074 696f 6e61 6c5d 2c20  atch:optional], 
+00015690: 7b6e 5f64 696d 7d2c 206e 4031 2c20 6e40  {n_dim}, n@1, n@
+000156a0: 322c 202e 2e2e 2c20 6e40 6e5f 6469 6d29  2, ..., n@n_dim)
+000156b0: 2074 6f20 285b 6e5f 6261 7463 685d 2c20   to ([n_batch], 
+000156c0: 7b6e 5f64 696d 7d2c 206e 4031 2c20 6e40  {n_dim}, n@1, n@
+000156d0: 322c 202e 2e2e 2c20 6e40 6e5f 6469 6d29  2, ..., n@n_dim)
+000156e0: 0a20 2020 2020 2020 206d 6574 686f 6420  .        method 
+000156f0: 5b73 7472 3a20 6c69 6e65 6172 7c6e 6561  [str: linear|nea
+00015700: 7265 7374 5d3a 2054 6865 2069 6e74 6572  rest]: The inter
+00015710: 706f 6c61 7469 6f6e 206d 6574 686f 642e  polation method.
+00015720: 200a 2020 2020 2020 2020 7461 7267 6574   .        target
+00015730: 5f73 7061 6365 205b 7475 706c 6520 6f72  _space [tuple or
+00015740: 2062 742e 5465 6e73 6f72 5d3a 0a20 2020   bt.Tensor]:.   
+00015750: 2020 2020 2020 2020 2053 697a 6520 2874           Size (t
+00015760: 7570 6c65 2920 6f66 2061 2074 6172 6765  uple) of a targe
+00015770: 7420 524f 4920 6174 2074 6865 2063 656e  t ROI at the cen
+00015780: 7465 7220 6f66 2069 6d61 6765 2e20 0a20  ter of image. . 
+00015790: 2020 2020 2020 2020 2020 204f 5220 5472             OR Tr
+000157a0: 616e 7366 6f72 6d65 6420 636f 6f72 6469  ansformed coordi
+000157b0: 6e61 7465 2073 7061 6365 2028 6274 2e54  nate space (bt.T
+000157c0: 656e 736f 7229 206f 6620 7468 6520 6f75  ensor) of the ou
+000157d0: 7470 7574 2069 6d61 6765 2e20 0a20 2020  tput image. .   
+000157e0: 2020 2020 2020 2020 2073 697a 653a 206c           size: l
+000157f0: 656e 6774 6828 6e5f 6469 6d29 206f 7220  ength(n_dim) or 
+00015800: 285b 6e5f 6261 7463 683a 6f70 7469 6f6e  ([n_batch:option
+00015810: 616c 5d2c 207b 6e5f 6469 6d3a 6f70 7469  al], {n_dim:opti
+00015820: 6f6e 616c 7d2c 2073 697a 6540 312c 2073  onal}, size@1, s
+00015830: 697a 6540 322c 202e 2e2e 2c20 7369 7a65  ize@2, ..., size
+00015840: 406e 5f64 696d 290a 2020 2020 2020 2020  @n_dim).        
+00015850: 6669 6c6c 205b 7374 723a 206e 6561 7265  fill [str: neare
+00015860: 7374 7c62 6163 6b67 726f 756e 6420 6f72  st|background or
+00015870: 2069 6e74 206f 7220 666c 6f61 7428 6e75   int or float(nu
+00015880: 6d62 6572 295d 3a20 496e 6469 6361 7465  mber)]: Indicate
+00015890: 2074 6865 2077 6179 2074 6f20 6669 6c6c   the way to fill
+000158a0: 2062 6163 6b67 726f 756e 6420 6f75 7473   background outs
+000158b0: 6964 6520 6053 7572 726f 756e 6469 6e67  ide `Surrounding
+000158c0: 602e 200a 2020 2020 2020 2020 6465 7269  `. .        deri
+000158d0: 7661 7469 7665 205b 626f 6f6c 5d3a 2057  vative [bool]: W
+000158e0: 6865 7468 6572 2074 6f20 7265 7475 726e  hether to return
+000158f0: 2074 6865 2067 7261 6469 656e 742e 204f   the gradient. O
+00015900: 6e65 2063 616e 206f 6d69 7420 6974 2077  ne can omit it w
+00015910: 6865 6e20 7573 696e 6720 746f 7263 682e  hen using torch.
+00015920: 6175 746f 6772 6164 2e0a 0a20 2020 2020  autograd...     
+00015930: 2020 206f 7574 7075 7420 5b62 742e 5465     output [bt.Te
+00015940: 6e73 6f72 5d3a 2054 6865 2074 7261 6e73  nsor]: The trans
+00015950: 666f 726d 6564 2069 6d61 6765 2e0a 2020  formed image..  
+00015960: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
+00015970: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f63  ([n_batch], {n_c
+00015980: 6861 6e6e 656c 3a6f 7074 696f 6e61 6c7d  hannel:optional}
+00015990: 2c20 6d40 312c 206d 4032 2c20 2e2e 2e2c  , m@1, m@2, ...,
+000159a0: 206d 406e 5f64 696d 290a 2020 2020 2020   m@n_dim).      
+000159b0: 2020 2020 2020 6f72 2077 6865 6e20 6074        or when `t
+000159c0: 6172 6765 745f 7370 6163 6560 2069 7320  arget_space` is 
+000159d0: 6465 6669 6e65 6420 6279 2074 656e 736f  defined by tenso
+000159e0: 722e 200a 2020 2020 2020 2020 2020 2020  r. .            
+000159f0: 7369 7a65 3a20 285b 6e5f 6261 7463 685d  size: ([n_batch]
+00015a00: 2c20 7369 7a65 4031 2c20 7369 7a65 4032  , size@1, size@2
+00015a10: 2c20 2e2e 2e2c 2073 697a 6540 6e5f 6469  , ..., size@n_di
+00015a20: 6d29 0a20 2020 2020 2020 2020 2020 206f  m).            o
+00015a30: 7220 7468 6520 6465 7269 7661 7469 7665  r the derivative
+00015a40: 2066 6f72 2074 6865 2069 6e74 6572 706f   for the interpo
+00015a50: 6c61 7469 6f6e 2e20 2869 6620 6064 6572  lation. (if `der
+00015a60: 6976 6174 6976 6520 3d20 5472 7565 6029  ivative = True`)
+00015a70: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+00015a80: 653a 2028 5b6e 5f62 6174 6368 5d2c 207b  e: ([n_batch], {
+00015a90: 6e5f 6469 6d7d 2c20 7369 7a65 4031 2c20  n_dim}, size@1, 
+00015aa0: 7369 7a65 4032 2c20 2e2e 2e2c 2073 697a  size@2, ..., siz
+00015ab0: 6540 6e5f 6469 6d29 0a0a 2020 2020 4578  e@n_dim)..    Ex
+00015ac0: 616d 706c 6573 3a0a 2020 2020 2d2d 2d2d  amples:.    ----
+00015ad0: 2d2d 2d2d 2d2d 0a20 2020 203e 3e3e 2049  ------.    >>> I
+00015ae0: 6d61 6765 203d 2062 742e 7261 6e64 2833  mage = bt.rand(3
+00015af0: 2c20 3130 302c 2031 3230 2c20 3830 290a  , 100, 120, 80).
+00015b00: 2020 2020 3e3e 3e20 414d 203d 2062 742e      >>> AM = bt.
+00015b10: 7261 6e64 2834 2c20 3429 0a20 2020 203e  rand(4, 4).    >
+00015b20: 3e3e 2041 4d5b 332c 203a 5d20 3d20 6274  >> AM[3, :] = bt
+00015b30: 2e6f 6e65 5f68 6f74 282d 312c 2034 290a  .one_hot(-1, 4).
+00015b40: 2020 2020 3e3e 3e20 696e 7465 7270 6f6c      >>> interpol
+00015b50: 6174 696f 6e28 496d 6167 652c 2041 6666  ation(Image, Aff
+00015b60: 696e 6528 414d 292c 206d 6574 686f 643d  ine(AM), method=
+00015b70: 274c 696e 6561 7227 290a 2020 2020 2727  'Linear').    ''
+00015b80: 270a 2020 2020 6966 2074 7261 6e73 2069  '.    if trans i
+00015b90: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2074  s not None and t
+00015ba0: 7261 6e73 2e62 6163 6b77 6172 643a 0a20  rans.backward:. 
+00015bb0: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
+00015bc0: 7228 7472 616e 732c 2027 696e 7627 293a  r(trans, 'inv'):
+00015bd0: 2074 7261 6e73 203d 2074 7261 6e73 2e69   trans = trans.i
+00015be0: 6e76 2829 2e66 616b 655f 696e 7628 290a  nv().fake_inv().
+00015bf0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00015c00: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00015c10: 2257 6172 6e69 6e67 3a20 4261 636b 7761  "Warning: Backwa
+00015c20: 7264 2074 7261 6e73 666f 726d 6174 696f  rd transformatio
+00015c30: 6e20 666f 756e 6420 696e 206d 6574 686f  n found in metho
+00015c40: 6420 6069 6e74 6572 706f 6c61 7469 6f6e  d `interpolation
+00015c50: 5f66 6f72 7761 7264 602e 2055 7369 6e67  _forward`. Using
+00015c60: 2060 696e 7465 7270 6f6c 6174 696f 6e60   `interpolation`
+00015c70: 2069 6e73 7465 6164 2e20 2229 0a20 2020   instead. ").   
+00015c80: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00015c90: 696e 7465 7270 6f6c 6174 696f 6e28 696d  interpolation(im
+00015ca0: 6167 652c 2074 7261 6e73 2c20 6d65 7468  age, trans, meth
+00015cb0: 6f64 203d 206d 6574 686f 642c 2074 6172  od = method, tar
+00015cc0: 6765 745f 7370 6163 6520 3d20 7461 7267  get_space = targ
+00015cd0: 6574 5f73 7061 6365 2c20 6669 6c6c 203d  et_space, fill =
+00015ce0: 2066 696c 6c29 0a20 2020 2072 6574 7572   fill).    retur
+00015cf0: 6e20 4e6f 7449 6d70 6c65 6d65 6e74 6564  n NotImplemented
+00015d00: 0a0a 2323 2323 2323 2323 2323 2323 2049  ..############ I
+00015d10: 6d61 6765 2054 7261 6e73 666f 726d 6174  mage Transformat
+00015d20: 696f 6e73 2023 2323 2323 2323 2323 2323  ions ###########
+00015d30: 230a 0a63 6c61 7373 2049 6d61 6765 5472  #..class ImageTr
+00015d40: 616e 7366 6f72 6d61 7469 6f6e 2854 7261  ansformation(Tra
+00015d50: 6e73 666f 726d 6174 696f 6e29 3a0a 2020  nsformation):.  
+00015d60: 2020 2020 2020 0a20 2020 2064 6566 205f        .    def _
+00015d70: 5f63 616c 6c5f 5f28 7365 6c66 2c20 5829  _call__(self, X)
+00015d80: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
+00015d90: 2020 2020 2020 5820 5b62 742e 5465 6e73        X [bt.Tens
+00015da0: 6f72 5d3a 2049 6d61 6765 2074 6f20 6265  or]: Image to be
+00015db0: 2074 7261 6e73 666f 726d 6564 2e0a 2020   transformed..  
+00015dc0: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
+00015dd0: 285b 6e5f 6261 7463 683a 6f70 7469 6f6e  ([n_batch:option
+00015de0: 616c 5d2c 207b 6e5f 6368 616e 6e65 6c3a  al], {n_channel:
+00015df0: 6f70 7469 6f6e 616c 7d2c 206e 4031 2c20  optional}, n@1, 
+00015e00: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
+00015e10: 6d29 0a20 2020 2020 2020 206f 7574 7075  m).        outpu
+00015e20: 7420 5b62 742e 5465 6e73 6f72 5d3a 2054  t [bt.Tensor]: T
+00015e30: 6865 2074 7261 6e73 666f 726d 6564 2069  he transformed i
+00015e40: 6d61 6765 2e0a 2020 2020 2020 2020 2020  mage..          
+00015e50: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
+00015e60: 685d 2c20 7b6e 5f63 6861 6e6e 656c 7d2c  h], {n_channel},
+00015e70: 206e 4031 2c20 6e40 322c 202e 2e2e 2c20   n@1, n@2, ..., 
+00015e80: 6e40 6e5f 6469 6d29 0a20 2020 2020 2020  n@n_dim).       
+00015e90: 2027 2727 0a20 2020 2020 2020 2058 203d   '''.        X =
+00015ea0: 2062 6174 6f72 6368 5f74 656e 736f 7228   batorch_tensor(
+00015eb0: 5829 0a20 2020 2020 2020 2069 6620 7365  X).        if se
+00015ec0: 6c66 2e6e 5f64 696d 2069 7320 4e6f 6e65  lf.n_dim is None
+00015ed0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00015ee0: 206e 6f74 2058 2e68 6173 5f62 6174 6368   not X.has_batch
+00015ef0: 3a20 5820 3d20 582e 756e 7371 7565 657a  : X = X.unsqueez
+00015f00: 6528 5b5d 290a 2020 2020 2020 2020 2020  e([]).          
+00015f10: 2020 6966 206e 6f74 2058 2e68 6173 5f63    if not X.has_c
+00015f20: 6861 6e6e 656c 3a20 5820 3d20 582e 7374  hannel: X = X.st
+00015f30: 616e 6461 7264 2829 2e75 6e73 7175 6565  andard().unsquee
+00015f40: 7a65 287b 317d 290a 2020 2020 2020 2020  ze({1}).        
+00015f50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00015f60: 2020 6966 2058 2e6e 5f64 696d 203d 3d20    if X.n_dim == 
+00015f70: 7365 6c66 2e6e 5f64 696d 3a20 5820 3d20  self.n_dim: X = 
+00015f80: 582e 7265 6d6f 7665 5f73 7065 6369 616c  X.remove_special
+00015f90: 5f28 292e 756e 7371 7565 657a 6528 5b5d  _().unsqueeze([]
+00015fa0: 292e 756e 7371 7565 657a 6528 7b31 7d29  ).unsqueeze({1})
+00015fb0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00015fc0: 6620 582e 6e5f 6469 6d20 3d3d 2073 656c  f X.n_dim == sel
+00015fd0: 662e 6e5f 6469 6d20 2b20 313a 0a20 2020  f.n_dim + 1:.   
+00015fe0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00015ff0: 582e 6861 735f 6261 7463 683a 2058 2e63  X.has_batch: X.c
+00016000: 6861 6e6e 656c 5f64 696d 656e 7369 6f6e  hannel_dimension
+00016010: 203d 204e 6f6e 653b 2058 203d 2058 2e75   = None; X = X.u
+00016020: 6e73 7175 6565 7a65 287b 3020 6966 2058  nsqueeze({0 if X
+00016030: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
+00016040: 203e 2030 2065 6c73 6520 317d 290a 2020   > 0 else 1}).  
+00016050: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00016060: 6966 2058 2e68 6173 5f63 6861 6e6e 656c  if X.has_channel
+00016070: 3a20 5820 3d20 582e 756e 7371 7565 657a  : X = X.unsqueez
+00016080: 6528 5b5d 290a 2020 2020 2020 2020 2020  e([]).          
+00016090: 2020 2020 2020 656c 7365 3a20 5820 3d20        else: X = 
+000160a0: 582e 6261 7463 685f 6469 6d65 6e73 696f  X.batch_dimensio
+000160b0: 6e5f 2830 292e 756e 7371 7565 657a 6528  n_(0).unsqueeze(
+000160c0: 7b31 7d29 0a20 2020 2020 2020 2020 2020  {1}).           
+000160d0: 2065 6c69 6620 582e 6e5f 6469 6d20 3d3d   elif X.n_dim ==
+000160e0: 2073 656c 662e 6e5f 6469 6d20 2b20 323a   self.n_dim + 2:
+000160f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016100: 2023 205f 6368 616e 6e61 6c2f 6261 7463   # _channal/batc
+00016110: 6820 6469 6d65 6e73 696f 6e73 2075 7365  h dimensions use
+00016120: 6420 6865 7265 2061 7320 7468 6579 2061  d here as they a
+00016130: 7265 206e 5f64 696d 2077 6865 6e20 6e6f  re n_dim when no
+00016140: 7420 6578 6973 7465 642e 200a 2020 2020  t existed. .    
+00016150: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00016160: 6f74 2058 2e68 6173 5f62 6174 6368 3a20  ot X.has_batch: 
+00016170: 582e 6261 7463 685f 6469 6d65 6e73 696f  X.batch_dimensio
+00016180: 6e20 3d20 3020 6966 2058 2e5f 6368 616e  n = 0 if X._chan
+00016190: 6e65 6c5f 6469 6d65 6e73 696f 6e20 3e20  nel_dimension > 
+000161a0: 3020 656c 7365 2031 0a20 2020 2020 2020  0 else 1.       
+000161b0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+000161c0: 582e 6861 735f 6368 616e 6e65 6c3a 2058  X.has_channel: X
+000161d0: 2e63 6861 6e6e 656c 5f64 696d 656e 7369  .channel_dimensi
+000161e0: 6f6e 203d 2030 2069 6620 582e 5f62 6174  on = 0 if X._bat
+000161f0: 6368 5f64 696d 656e 7369 6f6e 203e 2030  ch_dimension > 0
+00016200: 2065 6c73 6520 310a 2020 2020 2020 2020   else 1.        
+00016210: 6176 6f75 6368 2858 2e68 6173 5f62 6174  avouch(X.has_bat
+00016220: 6368 2061 6e64 2058 2e68 6173 5f63 6861  ch and X.has_cha
+00016230: 6e6e 656c 2c20 6622 506c 6561 7365 2075  nnel, f"Please u
+00016240: 7365 2062 6174 6f72 6368 2074 656e 736f  se batorch tenso
+00016250: 7220 6f66 2073 697a 6520 5c0a 2020 2020  r of size \.    
+00016260: 2020 2020 2020 2020 285b 6e5f 6261 7463          ([n_batc
+00016270: 685d 2c20 7b7b 6e5f 6368 616e 6e65 6c2f  h], {{n_channel/
+00016280: 6e5f 6665 6174 7572 653a 6f70 7469 6f6e  n_feature:option
+00016290: 616c 7d7d 2c20 6d5f 312c 206d 5f32 2c20  al}}, m_1, m_2, 
+000162a0: 2e2e 2e2c 206d 5f72 2920 5b72 3d6e 5f64  ..., m_r) [r=n_d
+000162b0: 696d 5d20 666f 7220 5c0a 2020 2020 2020  im] for \.      
+000162c0: 2020 2020 2020 2020 2020 7b73 656c 662e            {self.
+000162d0: 5f5f 636c 6173 735f 5f2e 5f5f 6e61 6d65  __class__.__name
+000162e0: 5f5f 2e73 706c 6974 2827 2e27 295b 2d31  __.split('.')[-1
+000162f0: 5d7d 2054 7261 6e73 666f 726d 6174 696f  ]} Transformatio
+00016300: 6e2c 2069 6e73 7465 6164 206f 6620 7b58  n, instead of {X
+00016310: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
+00016320: 2020 2020 7265 7475 726e 2058 2e63 6c6f      return X.clo
+00016330: 6e65 2829 0a0a 636c 6173 7320 4e6f 726d  ne()..class Norm
+00016340: 616c 697a 6528 496d 6167 6554 7261 6e73  alize(ImageTrans
+00016350: 666f 726d 6174 696f 6e29 3a0a 2020 2020  formation):.    
+00016360: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00016370: 662c 202a 5f72 616e 6765 293a 0a20 2020  f, *_range):.   
+00016380: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00016390: 204e 6f72 6d61 6c69 7a65 2074 6865 2069   Normalize the i
+000163a0: 6e74 656e 7369 7479 206f 6620 616e 2069  ntensity of an i
+000163b0: 6d61 6765 2e0a 2020 2020 2020 2020 0a20  mage..        . 
+000163c0: 2020 2020 2020 2050 6172 616d 733a 0a20         Params:. 
+000163d0: 2020 2020 2020 2020 2020 205f 7261 6e67             _rang
+000163e0: 6520 3d20 286c 6f77 2c20 6869 6768 2920  e = (low, high) 
+000163f0: 5b69 6e74 206f 7220 666c 6f61 7420 6f72  [int or float or
+00016400: 2062 742e 5465 6e73 6f72 5d3a 2054 6865   bt.Tensor]: The
+00016410: 206c 6f77 6573 7420 2861 6e64 2068 6967   lowest (and hig
+00016420: 6865 7374 2920 696e 7465 6e73 6974 792e  hest) intensity.
+00016430: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+00016440: 2020 7369 7a65 3a20 6c65 6e67 7468 2832    size: length(2
+00016450: 2920 6f72 2028 5b6e 5f62 6174 6368 5d2c  ) or ([n_batch],
+00016460: 207b 327d 290a 2020 2020 2020 2020 2020   {2}).          
+00016470: 2020 0a20 2020 2020 2020 2057 6865 6e20    .        When 
+00016480: 6974 2069 7320 6361 6c6c 6564 3a0a 2020  it is called:.  
+00016490: 2020 2020 2020 2020 2020 5820 5b62 742e            X [bt.
+000164a0: 5465 6e73 6f72 5d3a 2049 6d61 6765 2074  Tensor]: Image t
+000164b0: 6f20 6265 2074 7261 6e73 666f 726d 6564  o be transformed
+000164c0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000164d0: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
+000164e0: 683a 6f70 7469 6f6e 616c 5d2c 207b 6e5f  h:optional], {n_
+000164f0: 6368 616e 6e65 6c3a 6f70 7469 6f6e 616c  channel:optional
+00016500: 7d2c 206e 4031 2c20 6e40 322c 202e 2e2e  }, n@1, n@2, ...
+00016510: 2c20 6e40 6e5f 6469 6d29 0a20 2020 2020  , n@n_dim).     
+00016520: 2020 2020 2020 206f 7574 7075 7420 5b62         output [b
+00016530: 742e 5465 6e73 6f72 5d3a 2054 6865 2074  t.Tensor]: The t
+00016540: 7261 6e73 666f 726d 6564 2069 6d61 6765  ransformed image
+00016550: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016560: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
+00016570: 685d 2c20 7b6e 5f63 6861 6e6e 656c 7d2c  h], {n_channel},
+00016580: 206e 4031 2c20 6e40 322c 202e 2e2e 2c20   n@1, n@2, ..., 
+00016590: 6e40 6e5f 6469 6d29 0a20 2020 2020 2020  n@n_dim).       
+000165a0: 2027 2727 0a20 2020 2020 2020 2069 6620   '''.        if 
+000165b0: 6c65 6e28 5f72 616e 6765 2920 3d3d 2030  len(_range) == 0
+000165c0: 3a20 5f72 616e 6765 203d 204e 6f6e 650a  : _range = None.
+000165d0: 2020 2020 2020 2020 656c 6966 206c 656e          elif len
+000165e0: 285f 7261 6e67 6529 203d 3d20 3120 616e  (_range) == 1 an
+000165f0: 6420 6973 696e 7374 616e 6365 285f 7261  d isinstance(_ra
+00016600: 6e67 655b 305d 2c20 286c 6973 742c 2074  nge[0], (list, t
+00016610: 7570 6c65 2929 3a20 5f72 616e 6765 203d  uple)): _range =
+00016620: 2062 6174 6f72 6368 5f74 656e 736f 7228   batorch_tensor(
+00016630: 6c69 7374 285f 7261 6e67 655b 305d 2929  list(_range[0]))
+00016640: 0a20 2020 2020 2020 2065 6c69 6620 6c65  .        elif le
+00016650: 6e28 5f72 616e 6765 2920 3d3d 2031 2061  n(_range) == 1 a
+00016660: 6e64 2069 7369 6e73 7461 6e63 6528 5f72  nd isinstance(_r
+00016670: 616e 6765 5b30 5d2c 2062 742e 5465 6e73  ange[0], bt.Tens
+00016680: 6f72 293a 205f 7261 6e67 6520 3d20 5f72  or): _range = _r
+00016690: 616e 6765 5b30 5d0a 2020 2020 2020 2020  ange[0].        
+000166a0: 656c 6966 206c 656e 285f 7261 6e67 6529  elif len(_range)
+000166b0: 203d 3d20 313a 205f 7261 6e67 6520 3d20   == 1: _range = 
+000166c0: 6274 2e63 6861 6e6e 656c 5f74 656e 736f  bt.channel_tenso
+000166d0: 7228 2830 2c20 5f72 616e 6765 2929 0a20  r((0, _range)). 
+000166e0: 2020 2020 2020 2065 6c69 6620 6c65 6e28         elif len(
+000166f0: 5f72 616e 6765 2920 3d3d 2032 3a20 5f72  _range) == 2: _r
+00016700: 616e 6765 203d 2062 742e 6368 616e 6e65  ange = bt.channe
+00016710: 6c5f 7465 6e73 6f72 285f 7261 6e67 6529  l_tensor(_range)
+00016720: 0a20 2020 2020 2020 2065 6c73 653a 2072  .        else: r
+00016730: 6169 7365 2054 7970 6545 7272 6f72 2866  aise TypeError(f
+00016740: 2249 6e76 616c 6964 2072 616e 6765 2066  "Invalid range f
+00016750: 6f72 204e 6f72 6d61 6c69 7a65 3a20 7b5f  or Normalize: {_
+00016760: 7261 6e67 657d 2e20 2229 0a20 2020 2020  range}. ").     
+00016770: 2020 2069 6620 5f72 616e 6765 2069 7320     if _range is 
+00016780: 4e6f 6e65 3a20 7061 7373 0a20 2020 2020  None: pass.     
+00016790: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000167a0: 2020 2020 2069 6620 5f72 616e 6765 2e6e       if _range.n
+000167b0: 5f64 696d 203c 2032 3a20 5f72 616e 6765  _dim < 2: _range
+000167c0: 203d 205f 7261 6e67 652e 756e 7371 7565   = _range.unsque
+000167d0: 657a 6528 5b5d 290a 2020 2020 2020 2020  eze([]).        
+000167e0: 2020 2020 6966 206e 6f74 205f 7261 6e67      if not _rang
+000167f0: 652e 6861 735f 6261 7463 683a 205f 7261  e.has_batch: _ra
+00016800: 6e67 652e 6261 7463 685f 6469 6d65 6e73  nge.batch_dimens
+00016810: 696f 6e20 3d20 300a 2020 2020 2020 2020  ion = 0.        
+00016820: 2020 2020 6966 206e 6f74 205f 7261 6e67      if not _rang
+00016830: 652e 6861 735f 6368 616e 6e65 6c3a 205f  e.has_channel: _
+00016840: 7261 6e67 652e 6368 616e 6e65 6c5f 6469  range.channel_di
+00016850: 6d65 6e73 696f 6e20 3d20 310a 2020 2020  mension = 1.    
+00016860: 2020 2020 2020 2020 6176 6f75 6368 285f          avouch(_
+00016870: 7261 6e67 652e 6861 735f 6261 7463 6820  range.has_batch 
+00016880: 616e 6420 5f72 616e 6765 2e68 6173 5f63  and _range.has_c
+00016890: 6861 6e6e 656c 2c20 6622 506c 6561 7365  hannel, f"Please
+000168a0: 2075 7365 2062 6174 6f72 6368 2074 656e   use batorch ten
+000168b0: 736f 7220 6f66 2073 697a 6520 5c0a 2020  sor of size \.  
+000168c0: 2020 2020 2020 2020 2020 2020 2020 285b                ([
+000168d0: 6e5f 6261 7463 683a 6f70 7469 6f6e 616c  n_batch:optional
+000168e0: 5d2c 207b 7b32 7d7d 2920 666f 7220 4e6f  ], {{2}}) for No
+000168f0: 726d 616c 697a 696e 6720 7061 7261 6d65  rmalizing parame
+00016900: 7465 7273 2c20 696e 7374 6561 6420 6f66  ters, instead of
+00016910: 207b 5f72 616e 6765 2e73 6861 7065 7d2e   {_range.shape}.
+00016920: 2022 290a 2020 2020 2020 2020 7375 7065   ").        supe
+00016930: 7228 292e 5f5f 696e 6974 5f5f 285f 7261  r().__init__(_ra
+00016940: 6e67 6529 0a20 2020 2020 2020 2073 656c  nge).        sel
+00016950: 662e 7261 6e67 6520 3d20 5f72 616e 6765  f.range = _range
+00016960: 0a20 2020 2020 2020 2073 656c 662e 5f72  .        self._r
+00016970: 616e 6765 203d 204e 6f6e 650a 0a20 2020  ange = None..   
+00016980: 2064 6566 205f 5f63 616c 6c5f 5f28 7365   def __call__(se
+00016990: 6c66 2c20 5829 3a0a 2020 2020 2020 2020  lf, X):.        
+000169a0: 5820 3d20 7375 7065 7228 292e 5f5f 6361  X = super().__ca
+000169b0: 6c6c 5f5f 2858 290a 2020 2020 2020 2020  ll__(X).        
+000169c0: 5f72 616e 6765 203d 2073 656c 662e 7261  _range = self.ra
+000169d0: 6e67 650a 2020 2020 2020 2020 6966 205f  nge.        if _
+000169e0: 7261 6e67 6520 6973 204e 6f6e 653a 0a20  range is None:. 
+000169f0: 2020 2020 2020 2020 2020 205f 7261 6e67             _rang
+00016a00: 6520 3d20 6274 2e71 7561 6e74 696c 6528  e = bt.quantile(
+00016a10: 582e 666c 6174 7465 6e28 292e 666c 6f61  X.flatten().floa
+00016a20: 7428 292c 2062 6174 6f72 6368 5f74 656e  t(), batorch_ten
+00016a30: 736f 7228 5b30 2e30 3235 2c20 302e 3937  sor([0.025, 0.97
+00016a40: 355d 292c 2061 7869 733d 2d31 292e 6d6f  5]), axis=-1).mo
+00016a50: 7665 6469 6d28 302c 202d 3129 2e73 7065  vedim(0, -1).spe
+00016a60: 6369 616c 5f66 726f 6d5f 2858 290a 2020  cial_from_(X).  
+00016a70: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00016a80: 7261 6e67 6520 3d20 5f72 616e 6765 0a20  range = _range. 
+00016a90: 2020 2020 2020 2072 6574 7572 6e20 2828         return ((
+00016aa0: 5820 2d20 5f72 616e 6765 5b2e 2e2e 2c20  X - _range[..., 
+00016ab0: 305d 2920 2f20 285f 7261 6e67 655b 2e2e  0]) / (_range[..
+00016ac0: 2e2c 2031 5d20 2d20 5f72 616e 6765 5b2e  ., 1] - _range[.
+00016ad0: 2e2e 2c20 305d 2929 2e63 6c61 6d70 2830  .., 0])).clamp(0
+00016ae0: 2e2c 2031 2e29 0a20 2020 200a 2020 2020  ., 1.).    .    
+00016af0: 6465 6620 696e 7628 7365 6c66 293a 0a20  def inv(self):. 
+00016b00: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00016b10: 616e 6765 2069 7320 6e6f 7420 4e6f 6e65  ange is not None
+00016b20: 3a20 5f72 616e 6765 203d 2073 656c 662e  : _range = self.
+00016b30: 7261 6e67 650a 2020 2020 2020 2020 656c  range.        el
+00016b40: 6966 2073 656c 662e 5f72 616e 6765 2069  if self._range i
+00016b50: 7320 6e6f 7420 4e6f 6e65 3a20 5f72 616e  s not None: _ran
+00016b60: 6765 203d 2073 656c 662e 5f72 616e 6765  ge = self._range
+00016b70: 0a20 2020 2020 2020 2065 6c73 653a 2072  .        else: r
+00016b80: 6574 7572 6e20 4e6f 726d 616c 697a 6528  eturn Normalize(
+00016b90: 4e6f 6e65 290a 2020 2020 2020 2020 6465  None).        de
+00016ba0: 6e20 3d20 5f72 616e 6765 5b2e 2e2e 2c20  n = _range[..., 
+00016bb0: 315d 202d 205f 7261 6e67 655b 2e2e 2e2c  1] - _range[...,
+00016bc0: 2030 5d0a 2020 2020 2020 2020 5f72 616e   0].        _ran
+00016bd0: 6765 203d 2062 742e 7374 6163 6b28 2d5f  ge = bt.stack(-_
+00016be0: 7261 6e67 655b 2e2e 2e2c 2030 5d2c 2031  range[..., 0], 1
+00016bf0: 2d5f 7261 6e67 655b 2e2e 2e2c 2030 5d2c  -_range[..., 0],
+00016c00: 202d 3129 202f 2064 656e 0a20 2020 2020   -1) / den.     
+00016c10: 2020 2072 6574 7572 6e20 4e6f 726d 616c     return Normal
+00016c20: 697a 6528 5f72 616e 6765 290a 0a23 2323  ize(_range)..###
+00016c30: 2323 2323 2323 2323 2323 2053 7570 706f  ########## Suppo
+00016c40: 7274 696e 6720 4675 6e63 7469 6f6e 7320  rting Functions 
+00016c50: 2323 2323 2323 2323 2323 2323 0a0a 6465  ############..de
+00016c60: 6620 4273 706c 696e 6528 692c 2055 293a  f Bspline(i, U):
+00016c70: 0a20 2020 2022 2222 0a20 2020 2043 7562  .    """.    Cub
+00016c80: 6963 2042 2d73 706c 696e 6520 6675 6e63  ic B-spline func
+00016c90: 7469 6f6e 2e20 0a20 2020 204e 6f74 653a  tion. .    Note:
+00016ca0: 2041 7320 6c6f 6e67 2061 7320 6920 616e   As long as i an
+00016cb0: 6420 5520 6861 7665 2074 6865 2073 616d  d U have the sam
+00016cc0: 6520 7369 7a65 2c20 616e 7920 7368 6170  e size, any shap
+00016cd0: 6520 6f66 2074 656e 736f 7273 2077 6f75  e of tensors wou
+00016ce0: 6c64 2064 6f2e 0a20 2020 200a 2020 2020  ld do..    .    
+00016cf0: 5061 7261 6d73 3a0a 2020 2020 2020 2020  Params:.        
+00016d00: 6920 5b62 742e 5465 6e73 6f72 5d3a 2074  i [bt.Tensor]: t
+00016d10: 6865 2069 6e64 6578 206f 6620 7365 676d  he index of segm
+00016d20: 656e 7420 6675 6e63 7469 6f6e 206f 6620  ent function of 
+00016d30: 422d 7370 6c69 6e65 2e0a 2020 2020 2020  B-spline..      
+00016d40: 2020 2020 2020 5468 6520 7661 6c75 6520        The value 
+00016d50: 6f66 2065 6163 6820 656c 656d 656e 7420  of each element 
+00016d60: 6361 6e20 6265 2063 686f 7365 6e20 696e  can be chosen in
+00016d70: 2028 2d31 2c20 302c 2031 2c20 3229 2e20   (-1, 0, 1, 2). 
+00016d80: 0a20 2020 2020 2020 2055 205b 6274 2e54  .        U [bt.T
+00016d90: 656e 736f 725d 3a20 7468 6520 6465 6369  ensor]: the deci
+00016da0: 6d61 6c20 6172 6775 6d65 6e74 206f 6620  mal argument of 
+00016db0: 422d 7370 6c69 6e65 2066 756e 6374 696f  B-spline functio
+00016dc0: 6e2e 2049 7420 7368 6f75 6c64 2062 6520  n. It should be 
+00016dd0: 7769 7468 696e 2072 616e 6765 205b 302c  within range [0,
+00016de0: 2031 292e 0a20 2020 2022 2222 0a20 2020   1)..    """.   
+00016df0: 2069 203d 2062 6174 6f72 6368 5f74 656e   i = batorch_ten
+00016e00: 736f 7228 6929 3b20 5520 3d20 6261 746f  sor(i); U = bato
+00016e10: 7263 685f 7465 6e73 6f72 2855 290a 2020  rch_tensor(U).  
+00016e20: 2020 7265 7475 726e 2028 0a20 2020 2020    return (.     
+00016e30: 2020 2062 742e 7768 6572 6528 6920 3d3d     bt.where(i ==
+00016e40: 202d 312c 2028 3120 2d20 5529 202a 2a20   -1, (1 - U) ** 
+00016e50: 3320 2f20 362c 0a20 2020 2020 2020 2062  3 / 6,.        b
+00016e60: 742e 7768 6572 6528 6920 3d3d 2030 2c20  t.where(i == 0, 
+00016e70: 5520 2a2a 2033 202f 2032 202d 2055 202a  U ** 3 / 2 - U *
+00016e80: 2055 202b 2032 202f 2033 2c0a 2020 2020   U + 2 / 3,.    
+00016e90: 2020 2020 6274 2e77 6865 7265 2869 203d      bt.where(i =
+00016ea0: 3d20 312c 2028 2d20 3320 2a20 5520 2a2a  = 1, (- 3 * U **
+00016eb0: 2033 202b 2033 202a 2055 202a 2055 202b   3 + 3 * U * U +
+00016ec0: 2033 202a 2055 202b 2031 2920 2f20 362c   3 * U + 1) / 6,
+00016ed0: 0a20 2020 2020 2020 2062 742e 7768 6572  .        bt.wher
+00016ee0: 6528 6920 3d3d 2032 2c20 5520 2a2a 2033  e(i == 2, U ** 3
+00016ef0: 202f 2036 2c0a 2020 2020 2020 2020 6274   / 6,.        bt
+00016f00: 2e7a 6572 6f73 5f6c 696b 6528 5529 2929  .zeros_like(U)))
+00016f10: 2929 0a20 2020 2029 0a0a 6465 6620 6442  )).    )..def dB
+00016f20: 7370 6c69 6e65 2869 2c20 5529 3a0a 2020  spline(i, U):.  
+00016f30: 2020 2222 220a 2020 2020 5468 6520 6465    """.    The de
+00016f40: 7269 7661 7469 7665 206f 6620 422d 7370  rivative of B-sp
+00016f50: 6c69 6e65 2066 756e 6374 696f 6e2c 2077  line function, w
+00016f60: 6974 6820 7265 7370 6563 7420 746f 2055  ith respect to U
+00016f70: 2e20 0a20 2020 204e 6f74 653a 2041 7320  . .    Note: As 
+00016f80: 6c6f 6e67 2061 7320 6920 616e 6420 5520  long as i and U 
+00016f90: 6861 7665 2074 6865 2073 616d 6520 7369  have the same si
+00016fa0: 7a65 2c20 616e 7920 7368 6170 6520 6f66  ze, any shape of
+00016fb0: 2074 656e 736f 7273 2077 6f75 6c64 2064   tensors would d
+00016fc0: 6f2e 0a20 2020 200a 2020 2020 5061 7261  o..    .    Para
+00016fd0: 6d73 3a0a 2020 2020 2020 2020 6920 5b62  ms:.        i [b
+00016fe0: 742e 5465 6e73 6f72 5d3a 2074 6865 2069  t.Tensor]: the i
+00016ff0: 6e64 6578 206f 6620 7365 676d 656e 7420  ndex of segment 
+00017000: 6675 6e63 7469 6f6e 206f 6620 422d 7370  function of B-sp
+00017010: 6c69 6e65 2e0a 2020 2020 2020 2020 2020  line..          
+00017020: 2020 5468 6520 7661 6c75 6520 6f66 2065    The value of e
+00017030: 6163 6820 656c 656d 656e 7420 6361 6e20  ach element can 
+00017040: 6265 2063 686f 7365 6e20 696e 2028 2d31  be chosen in (-1
+00017050: 2c20 302c 2031 2c20 3229 2e20 0a20 2020  , 0, 1, 2). .   
+00017060: 2020 2020 2055 205b 6274 2e54 656e 736f       U [bt.Tenso
+00017070: 725d 3a20 7468 6520 6465 6369 6d61 6c20  r]: the decimal 
+00017080: 6172 6775 6d65 6e74 206f 6620 422d 7370  argument of B-sp
+00017090: 6c69 6e65 2066 756e 6374 696f 6e2e 2049  line function. I
+000170a0: 7420 7368 6f75 6c64 2062 6520 7769 7468  t should be with
+000170b0: 696e 2072 616e 6765 205b 302c 2031 292e  in range [0, 1).
+000170c0: 0a20 2020 2022 2222 0a20 2020 2069 203d  .    """.    i =
+000170d0: 2062 6174 6f72 6368 5f74 656e 736f 7228   batorch_tensor(
+000170e0: 6929 3b20 5520 3d20 6261 746f 7263 685f  i); U = batorch_
+000170f0: 7465 6e73 6f72 2855 290a 2020 2020 7265  tensor(U).    re
+00017100: 7475 726e 2028 0a20 2020 2020 2020 2062  turn (.        b
+00017110: 742e 7768 6572 6528 6920 3d3d 202d 312c  t.where(i == -1,
+00017120: 202d 2033 202a 2028 3120 2d20 5529 202a   - 3 * (1 - U) *
+00017130: 2a20 3220 2f20 362c 0a20 2020 2020 2020  * 2 / 6,.       
+00017140: 2062 742e 7768 6572 6528 6920 3d3d 2030   bt.where(i == 0
+00017150: 2c20 3320 2a20 5520 2a2a 2032 202f 2032  , 3 * U ** 2 / 2
+00017160: 202d 2032 202a 2055 2c0a 2020 2020 2020   - 2 * U,.      
+00017170: 2020 6274 2e77 6865 7265 2869 203d 3d20    bt.where(i == 
+00017180: 312c 2028 2d20 3320 2a20 5520 2a2a 2032  1, (- 3 * U ** 2
+00017190: 202b 2032 202a 2055 202b 2031 2920 2f20   + 2 * U + 1) / 
+000171a0: 322c 0a20 2020 2020 2020 2062 742e 7768  2,.        bt.wh
+000171b0: 6572 6528 6920 3d3d 2032 2c20 3320 2a20  ere(i == 2, 3 * 
+000171c0: 5520 2a2a 2032 202f 2036 2c0a 2020 2020  U ** 2 / 6,.    
+000171d0: 2020 2020 6274 2e7a 6572 6f73 5f6c 696b      bt.zeros_lik
+000171e0: 6528 5529 2929 2929 0a20 2020 2029 0a0a  e(U))))).    )..
+000171f0: 6465 6620 6642 7370 6c69 6e65 2863 2c20  def fBspline(c, 
+00017200: 7829 3a0a 2020 2020 6320 3d20 6261 746f  x):.    c = bato
+00017210: 7263 685f 7465 6e73 6f72 2863 293b 2078  rch_tensor(c); x
+00017220: 203d 2062 6174 6f72 6368 5f74 656e 736f   = batorch_tenso
+00017230: 7228 7829 0a20 2020 2064 203d 2078 202d  r(x).    d = x -
+00017240: 2063 0a20 2020 2072 6574 7572 6e20 280a   c.    return (.
+00017250: 2020 2020 2020 2020 6274 2e77 6865 7265          bt.where
+00017260: 2828 2d32 203c 3d20 6429 202a 2028 6420  ((-2 <= d) * (d 
+00017270: 3c20 2d31 292c 2064 202a 2a20 3320 2b20  < -1), d ** 3 + 
+00017280: 3620 2a20 6420 2a2a 2032 202b 2031 3220  6 * d ** 2 + 12 
+00017290: 2a20 6420 2b20 382c 0a20 2020 2020 2020  * d + 8,.       
+000172a0: 2062 742e 7768 6572 6528 282d 3120 3c3d   bt.where((-1 <=
+000172b0: 2064 2920 2a20 2864 203c 2030 292c 202d   d) * (d < 0), -
+000172c0: 2033 202a 2064 202a 2a20 3320 2d20 3620   3 * d ** 3 - 6 
+000172d0: 2a20 6420 2a2a 2032 202b 2034 2c0a 2020  * d ** 2 + 4,.  
+000172e0: 2020 2020 2020 6274 2e77 6865 7265 2828        bt.where((
+000172f0: 3020 3c3d 2064 2920 2a20 2864 203c 2031  0 <= d) * (d < 1
+00017300: 292c 2033 202a 2064 202a 2a20 3320 2d20  ), 3 * d ** 3 - 
+00017310: 3620 2a20 6420 2a2a 2032 202b 2034 2c0a  6 * d ** 2 + 4,.
+00017320: 2020 2020 2020 2020 6274 2e77 6865 7265          bt.where
+00017330: 2828 3120 3c3d 2064 2920 2a20 2864 203c  ((1 <= d) * (d <
+00017340: 2032 292c 202d 2064 202a 2a20 3320 2b20   2), - d ** 3 + 
+00017350: 3620 2a20 6420 2a2a 2032 202d 2031 3220  6 * d ** 2 - 12 
+00017360: 2a20 6420 2b20 382c 0a20 2020 2020 2020  * d + 8,.       
+00017370: 2062 742e 7a65 726f 735f 6c69 6b65 2864   bt.zeros_like(d
+00017380: 2929 2929 2920 2f20 360a 2020 2020 290a  ))))) / 6.    ).
+00017390: 0a64 6566 2041 6666 696e 6532 4432 4d61  .def Affine2D2Ma
+000173a0: 7472 6978 2870 6172 616d 7329 3a0a 2020  trix(params):.  
+000173b0: 2020 2222 220a 2020 2020 7431 2c20 7432    """.    t1, t2
+000173c0: 2c20 ceb8 2c20 7331 2c20 7332 2c20 cf81  , .., s1, s2, ..
+000173d0: 312c 20cf 8132 2069 6e20 7369 7a65 3a20  1, ..2 in size: 
+000173e0: 285b 6e5f 6261 7463 685d 2c20 7b37 7d29  ([n_batch], {7})
+000173f0: 0a20 2020 2074 312c 2074 322c 2063 312c  .    t1, t2, c1,
+00017400: 2063 322c 20ce b82c 2073 312c 2073 322c   c2, .., s1, s2,
+00017410: 20cf 8131 2c20 cf81 3220 696e 2073 697a   ..1, ..2 in siz
+00017420: 653a 2028 5b6e 5f62 6174 6368 5d2c 207b  e: ([n_batch], {
+00017430: 397d 290a 2020 2020 6f75 7470 7574 2069  9}).    output i
+00017440: 6e20 7369 7a65 3a20 285b 6e5f 6261 7463  n size: ([n_batc
+00017450: 685d 2c20 332c 2033 290a 2020 2020 2222  h], 3, 3).    ""
+00017460: 220a 2020 2020 7061 7261 6d73 203d 2062  ".    params = b
+00017470: 6174 6f72 6368 5f74 656e 736f 7228 7061  atorch_tensor(pa
+00017480: 7261 6d73 290a 2020 2020 6966 2070 6172  rams).    if par
+00017490: 616d 732e 6e5f 6469 6d20 3c3d 2031 2061  ams.n_dim <= 1 a
+000174a0: 6e64 206e 6f74 2070 6172 616d 732e 6861  nd not params.ha
+000174b0: 735f 6261 7463 683a 2070 6172 616d 7320  s_batch: params 
+000174c0: 3d20 7061 7261 6d73 2e75 6e73 7175 6565  = params.unsquee
+000174d0: 7a65 285b 5d29 0a20 2020 2069 6620 7061  ze([]).    if pa
+000174e0: 7261 6d73 2e6e 5f64 696d 203c 3d20 3120  rams.n_dim <= 1 
+000174f0: 616e 6420 6e6f 7420 7061 7261 6d73 2e68  and not params.h
+00017500: 6173 5f63 6861 6e6e 656c 3a20 7061 7261  as_channel: para
+00017510: 6d73 203d 2070 6172 616d 732e 756e 7371  ms = params.unsq
+00017520: 7565 657a 6528 7b31 7d29 0a20 2020 2069  ueeze({1}).    i
+00017530: 6620 7061 7261 6d73 2e6e 5f64 696d 203d  f params.n_dim =
+00017540: 3d20 3220 616e 6420 6e6f 7420 7061 7261  = 2 and not para
+00017550: 6d73 2e68 6173 5f62 6174 6368 3a20 7061  ms.has_batch: pa
+00017560: 7261 6d73 2e62 6174 6368 5f64 696d 656e  rams.batch_dimen
+00017570: 7369 6f6e 203d 2030 0a20 2020 2069 6620  sion = 0.    if 
+00017580: 7061 7261 6d73 2e6e 5f64 696d 203d 3d20  params.n_dim == 
+00017590: 3220 616e 6420 6e6f 7420 7061 7261 6d73  2 and not params
+000175a0: 2e68 6173 5f63 6861 6e6e 656c 3a20 7061  .has_channel: pa
+000175b0: 7261 6d73 2e63 6861 6e6e 656c 5f64 696d  rams.channel_dim
+000175c0: 656e 7369 6f6e 203d 2031 0a20 2020 2061  ension = 1.    a
+000175d0: 766f 7563 6828 7061 7261 6d73 2e68 6173  vouch(params.has
+000175e0: 5f62 6174 6368 2c20 6622 506c 6561 7365  _batch, f"Please
+000175f0: 2075 7365 2062 6174 6f72 6368 2074 656e   use batorch ten
+00017600: 736f 7220 6f66 2073 697a 6520 285b 6e5f  sor of size ([n_
+00017610: 6261 7463 685d 2c20 7b37 206f 7220 397d  batch], {7 or 9}
+00017620: 2920 5c0a 2020 2020 2020 2020 666f 7220  ) \.        for 
+00017630: 4166 6669 6e65 2070 6172 616d 6574 6572  Affine parameter
+00017640: 732c 2069 6e73 7465 6164 206f 6620 7b70  s, instead of {p
+00017650: 6172 616d 732e 7368 6170 657d 2e20 2229  arams.shape}. ")
+00017660: 0a20 2020 206e 5f62 6174 6368 203d 2070  .    n_batch = p
+00017670: 6172 616d 732e 6e5f 6261 7463 680a 2020  arams.n_batch.  
+00017680: 2020 6966 2070 6172 616d 732e 7369 7a65    if params.size
+00017690: 2831 2920 3d3d 2037 3a0a 2020 2020 2020  (1) == 7:.      
+000176a0: 2020 7431 2c20 7432 2c20 ceb8 2c20 7331    t1, t2, .., s1
+000176b0: 2c20 7332 2c20 cf81 312c 20cf 8132 203d  , s2, ..1, ..2 =
+000176c0: 2070 6172 616d 732e 7370 6c69 7428 290a   params.split().
+000176d0: 2020 2020 2020 2020 6331 203d 2062 742e          c1 = bt.
+000176e0: 7a65 726f 7328 5b6e 5f62 6174 6368 5d2c  zeros([n_batch],
+000176f0: 2031 293b 2063 3220 3d20 6274 2e7a 6572   1); c2 = bt.zer
+00017700: 6f73 285b 6e5f 6261 7463 685d 2c20 3129  os([n_batch], 1)
+00017710: 0a20 2020 2069 6620 7061 7261 6d73 2e73  .    if params.s
+00017720: 697a 6528 3129 203d 3d20 393a 0a20 2020  ize(1) == 9:.   
+00017730: 2020 2020 2074 312c 2074 322c 2063 312c       t1, t2, c1,
+00017740: 2063 322c 20ce b82c 2073 312c 2073 322c   c2, .., s1, s2,
+00017750: 20cf 8131 2c20 cf81 3220 3d20 7061 7261   ..1, ..2 = para
+00017760: 6d73 2e73 706c 6974 2829 0a20 2020 2061  ms.split().    a
+00017770: 203d 2028 cf81 3120 2a20 cf81 3220 2b20   = (..1 * ..2 + 
+00017780: 3129 202a 2073 3120 2a20 6274 2e63 6f73  1) * s1 * bt.cos
+00017790: 28ce b829 202b 20cf 8131 202a 2073 3220  (..) + ..1 * s2 
+000177a0: 2a20 6274 2e73 696e 28ce b829 0a20 2020  * bt.sin(..).   
+000177b0: 2062 203d 202d 2028 cf81 3120 2a20 cf81   b = - (..1 * ..
+000177c0: 3220 2b20 3129 202a 2073 3120 2a20 6274  2 + 1) * s1 * bt
+000177d0: 2e73 696e 28ce b829 202b 20cf 8131 202a  .sin(..) + ..1 *
+000177e0: 2073 3220 2a20 6274 2e63 6f73 28ce b829   s2 * bt.cos(..)
+000177f0: 0a20 2020 2063 203d 20cf 8132 202a 2073  .    c = ..2 * s
+00017800: 3120 2a20 6274 2e63 6f73 28ce b829 202b  1 * bt.cos(..) +
+00017810: 2073 3220 2a20 6274 2e73 696e 28ce b829   s2 * bt.sin(..)
+00017820: 0a20 2020 2064 203d 202d 20cf 8132 202a  .    d = - ..2 *
+00017830: 2073 3120 2a20 6274 2e73 696e 28ce b829   s1 * bt.sin(..)
+00017840: 202b 2073 3220 2a20 6274 2e63 6f73 28ce   + s2 * bt.cos(.
+00017850: b829 0a20 2020 2072 6574 7572 6e20 6274  .).    return bt
+00017860: 2e63 6174 280a 2020 2020 2020 2020 6274  .cat(.        bt
+00017870: 2e63 6174 2828 612c 2062 2c20 7431 202d  .cat((a, b, t1 -
+00017880: 2061 202a 2063 3120 2d20 6220 2a20 6332   a * c1 - b * c2
+00017890: 202b 2063 312c 2063 2c20 642c 2074 3220   + c1, c, d, t2 
+000178a0: 2d20 6320 2a20 6331 202d 2064 202a 2063  - c * c1 - d * c
+000178b0: 3220 2b20 6332 292c 207b 7d29 2e76 6965  2 + c2), {}).vie
+000178c0: 7728 5b6e 5f62 6174 6368 5d2c 2032 2c20  w([n_batch], 2, 
+000178d0: 3329 2c20 0a20 2020 2020 2020 2062 742e  3), .        bt.
+000178e0: 6f6e 655f 686f 7428 2d31 2c20 3329 2e6d  one_hot(-1, 3).m
+000178f0: 756c 7469 706c 7928 6e5f 6261 7463 682c  ultiply(n_batch,
+00017900: 205b 5d29 2e76 6965 7728 5b6e 5f62 6174   []).view([n_bat
+00017910: 6368 5d2c 2031 2c20 3329 2c20 310a 2020  ch], 1, 3), 1.  
+00017920: 2020 290a 0a64 6566 2051 7561 7465 726e    )..def Quatern
+00017930: 7332 4d61 7472 6978 2870 6172 616d 7329  s2Matrix(params)
+00017940: 3a0a 2020 2020 2222 220a 2020 2020 2020  :.    """.      
+00017950: 2020 5175 6174 6572 6e3a 2071 622c 2071    Quatern: qb, q
+00017960: 632c 2071 642c 2070 782c 2070 792c 2070  c, qd, px, py, p
+00017970: 7a20 696e 2073 697a 653a 2028 5b6e 5f62  z in size: ([n_b
+00017980: 6174 6368 5d2c 207b 367d 290a 2020 2020  atch], {6}).    
+00017990: 2020 2020 4d61 7472 6978 3a20 285b 6e5f      Matrix: ([n_
+000179a0: 6261 7463 685d 2c20 342c 2034 290a 2020  batch], 4, 4).  
+000179b0: 2020 2222 220a 2020 2020 7061 7261 6d73    """.    params
+000179c0: 203d 2062 6174 6f72 6368 5f74 656e 736f   = batorch_tenso
+000179d0: 7228 7061 7261 6d73 290a 2020 2020 6966  r(params).    if
+000179e0: 2070 6172 616d 732e 6e5f 6469 6d20 3c3d   params.n_dim <=
+000179f0: 2031 2061 6e64 206e 6f74 2070 6172 616d   1 and not param
+00017a00: 732e 6861 735f 6261 7463 683a 2070 6172  s.has_batch: par
+00017a10: 616d 7320 3d20 7061 7261 6d73 2e75 6e73  ams = params.uns
+00017a20: 7175 6565 7a65 285b 5d29 0a20 2020 2069  queeze([]).    i
+00017a30: 6620 7061 7261 6d73 2e6e 5f64 696d 203c  f params.n_dim <
+00017a40: 3d20 3120 616e 6420 6e6f 7420 7061 7261  = 1 and not para
+00017a50: 6d73 2e68 6173 5f63 6861 6e6e 656c 3a20  ms.has_channel: 
+00017a60: 7061 7261 6d73 203d 2070 6172 616d 732e  params = params.
+00017a70: 756e 7371 7565 657a 6528 7b31 7d29 0a20  unsqueeze({1}). 
+00017a80: 2020 2069 6620 7061 7261 6d73 2e6e 5f64     if params.n_d
+00017a90: 696d 203d 3d20 3220 616e 6420 6e6f 7420  im == 2 and not 
+00017aa0: 7061 7261 6d73 2e68 6173 5f62 6174 6368  params.has_batch
+00017ab0: 3a20 7061 7261 6d73 2e62 6174 6368 5f64  : params.batch_d
+00017ac0: 696d 656e 7369 6f6e 203d 2030 0a20 2020  imension = 0.   
+00017ad0: 2069 6620 7061 7261 6d73 2e6e 5f64 696d   if params.n_dim
+00017ae0: 203d 3d20 3220 616e 6420 6e6f 7420 7061   == 2 and not pa
+00017af0: 7261 6d73 2e68 6173 5f63 6861 6e6e 656c  rams.has_channel
+00017b00: 3a20 7061 7261 6d73 2e63 6861 6e6e 656c  : params.channel
+00017b10: 5f64 696d 656e 7369 6f6e 203d 2031 0a20  _dimension = 1. 
+00017b20: 2020 2061 766f 7563 6828 7061 7261 6d73     avouch(params
+00017b30: 2e6e 5f64 696d 203d 3d20 3220 616e 6420  .n_dim == 2 and 
+00017b40: 7061 7261 6d73 2e68 6173 5f62 6174 6368  params.has_batch
+00017b50: 2061 6e64 2070 6172 616d 732e 6861 735f   and params.has_
+00017b60: 6368 616e 6e65 6c2c 200a 2020 2020 2020  channel, .      
+00017b70: 2020 2020 2066 2250 6c65 6173 6520 7573       f"Please us
+00017b80: 6520 6261 746f 7263 6820 7465 6e73 6f72  e batorch tensor
+00017b90: 206f 6620 7369 7a65 2028 5b6e 5f62 6174   of size ([n_bat
+00017ba0: 6368 5d2c 207b 7b36 7d7d 2920 666f 7220  ch], {{6}}) for 
+00017bb0: 4166 6669 6e65 2070 6172 616d 6574 6572  Affine parameter
+00017bc0: 732c 2069 6e73 7465 6164 206f 6620 7b70  s, instead of {p
+00017bd0: 6172 616d 732e 7368 6170 657d 2e20 2229  arams.shape}. ")
+00017be0: 0a20 2020 206e 5f62 6174 6368 203d 2070  .    n_batch = p
+00017bf0: 6172 616d 732e 6e5f 6261 7463 680a 2020  arams.n_batch.  
+00017c00: 2020 622c 2063 2c20 642c 2078 2c20 792c    b, c, d, x, y,
+00017c10: 207a 203d 2070 6172 616d 732e 7370 6c69   z = params.spli
+00017c20: 7428 290a 2020 2020 6120 3d20 6274 2e73  t().    a = bt.s
+00017c30: 7172 7428 2831 2d62 2a62 2d63 2a63 2d64  qrt((1-b*b-c*c-d
+00017c40: 2a64 292e 636c 616d 7028 3029 290a 2020  *d).clamp(0)).  
+00017c50: 2020 5231 3120 3d20 612a 612b 622a 622d    R11 = a*a+b*b-
+00017c60: 632a 632d 642a 640a 2020 2020 5231 3220  c*c-d*d.    R12 
+00017c70: 3d20 322a 622a 632d 322a 612a 640a 2020  = 2*b*c-2*a*d.  
+00017c80: 2020 5231 3320 3d20 322a 622a 642b 322a    R13 = 2*b*d+2*
+00017c90: 612a 630a 2020 2020 5232 3120 3d20 322a  a*c.    R21 = 2*
+00017ca0: 622a 632b 322a 612a 640a 2020 2020 5232  b*c+2*a*d.    R2
+00017cb0: 3220 3d20 612a 612b 632a 632d 622a 622d  2 = a*a+c*c-b*b-
+00017cc0: 642a 640a 2020 2020 5232 3320 3d20 322a  d*d.    R23 = 2*
+00017cd0: 632a 642d 322a 612a 620a 2020 2020 5233  c*d-2*a*b.    R3
+00017ce0: 3120 3d20 322a 622a 642d 322a 612a 630a  1 = 2*b*d-2*a*c.
+00017cf0: 2020 2020 5233 3220 3d20 322a 632a 642b      R32 = 2*c*d+
+00017d00: 322a 612a 620a 2020 2020 5233 3320 3d20  2*a*b.    R33 = 
+00017d10: 612a 612b 642a 642d 632a 632d 622a 620a  a*a+d*d-c*c-b*b.
+00017d20: 2020 2020 7265 7475 726e 2062 742e 6361      return bt.ca
+00017d30: 7428 0a20 2020 2020 2020 2062 742e 6361  t(.        bt.ca
+00017d40: 7428 2852 3131 2c20 5231 322c 2052 3133  t((R11, R12, R13
+00017d50: 2c20 782c 2052 3231 2c20 5232 322c 2052  , x, R21, R22, R
+00017d60: 3233 2c20 792c 2052 3331 2c20 5233 322c  23, y, R31, R32,
+00017d70: 2052 3333 2c20 7a29 2c20 3129 2e76 6965   R33, z), 1).vie
+00017d80: 7728 5b6e 5f62 6174 6368 5d2c 2033 2c20  w([n_batch], 3, 
+00017d90: 3429 2c0a 2020 2020 2020 2020 6274 2e6f  4),.        bt.o
+00017da0: 6e65 5f68 6f74 282d 312c 2034 292e 6d75  ne_hot(-1, 4).mu
+00017db0: 6c74 6970 6c79 286e 5f62 6174 6368 2c20  ltiply(n_batch, 
+00017dc0: 5b5d 292e 7669 6577 285b 6e5f 6261 7463  []).view([n_batc
+00017dd0: 685d 2c20 312c 2034 292c 2031 0a20 2020  h], 1, 4), 1.   
+00017de0: 2029 0a0a 6465 6620 4d61 7472 6978 3251   )..def Matrix2Q
+00017df0: 7561 7465 726e 7328 7061 7261 6d73 293a  uaterns(params):
+00017e00: 0a20 2020 2022 2222 0a20 2020 2020 2020  .    """.       
+00017e10: 204d 6174 7269 783a 2028 5b6e 5f62 6174   Matrix: ([n_bat
+00017e20: 6368 5d2c 2034 2c20 3429 0a20 2020 2020  ch], 4, 4).     
+00017e30: 2020 2051 7561 7465 726e 3a20 7162 2c20     Quatern: qb, 
+00017e40: 7163 2c20 7164 2c20 7078 2c20 7079 2c20  qc, qd, px, py, 
+00017e50: 707a 2069 6e20 7369 7a65 3a20 285b 6e5f  pz in size: ([n_
+00017e60: 6261 7463 685d 2c20 7b36 7d29 0a20 2020  batch], {6}).   
+00017e70: 2022 2222 0a20 2020 2070 6172 616d 7320   """.    params 
+00017e80: 3d20 6261 746f 7263 685f 7465 6e73 6f72  = batorch_tensor
+00017e90: 2870 6172 616d 7329 0a20 2020 2069 6620  (params).    if 
+00017ea0: 7061 7261 6d73 2e6e 5f64 696d 203c 3d20  params.n_dim <= 
+00017eb0: 3220 616e 6420 6e6f 7420 7061 7261 6d73  2 and not params
+00017ec0: 2e68 6173 5f62 6174 6368 3a20 7061 7261  .has_batch: para
+00017ed0: 6d73 203d 2070 6172 616d 732e 756e 7371  ms = params.unsq
+00017ee0: 7565 657a 6528 5b5d 290a 2020 2020 6966  ueeze([]).    if
+00017ef0: 2070 6172 616d 732e 6e5f 6469 6d20 3d3d   params.n_dim ==
+00017f00: 2033 2061 6e64 206e 6f74 2070 6172 616d   3 and not param
+00017f10: 732e 6861 735f 6261 7463 683a 2070 6172  s.has_batch: par
+00017f20: 616d 732e 6261 7463 685f 6469 6d65 6e73  ams.batch_dimens
+00017f30: 696f 6e20 3d20 300a 2020 2020 6966 2070  ion = 0.    if p
+00017f40: 6172 616d 732e 6e5f 6469 6d20 3d3d 2033  arams.n_dim == 3
+00017f50: 2061 6e64 2070 6172 616d 732e 6861 735f   and params.has_
+00017f60: 6368 616e 6e65 6c3a 2070 6172 616d 732e  channel: params.
+00017f70: 6368 616e 6e65 6c5f 6469 6d65 6e73 696f  channel_dimensio
+00017f80: 6e20 3d20 4e6f 6e65 0a20 2020 2061 766f  n = None.    avo
+00017f90: 7563 6828 7061 7261 6d73 2e6e 5f64 696d  uch(params.n_dim
+00017fa0: 203d 3d20 3320 616e 6420 7061 7261 6d73   == 3 and params
+00017fb0: 2e68 6173 5f62 6174 6368 2061 6e64 206e  .has_batch and n
+00017fc0: 6f74 2070 6172 616d 732e 6861 735f 6368  ot params.has_ch
+00017fd0: 616e 6e65 6c2c 200a 2020 2020 2020 2020  annel, .        
+00017fe0: 2020 2066 2250 6c65 6173 6520 7573 6520     f"Please use 
+00017ff0: 6261 746f 7263 6820 7465 6e73 6f72 206f  batorch tensor o
+00018000: 6620 7369 7a65 2028 5b6e 5f62 6174 6368  f size ([n_batch
+00018010: 5d2c 2034 2c20 3429 2066 6f72 2041 6666  ], 4, 4) for Aff
+00018020: 696e 6520 6d61 7472 6978 2c20 696e 7374  ine matrix, inst
+00018030: 6561 6420 6f66 207b 7061 7261 6d73 2e73  ead of {params.s
+00018040: 6861 7065 7d2e 2022 290a 2020 2020 6e5f  hape}. ").    n_
+00018050: 6261 7463 6820 3d20 7061 7261 6d73 2e6e  batch = params.n
+00018060: 5f62 6174 6368 0a20 2020 2078 2c20 792c  _batch.    x, y,
+00018070: 207a 203d 2070 6172 616d 735b 2e2e 2e2c   z = params[...,
+00018080: 203a 332c 202d 315d 2e63 6861 6e6e 656c   :3, -1].channel
+00018090: 5f64 696d 5f28 3129 2e73 706c 6974 2831  _dim_(1).split(1
+000180a0: 2c20 3129 0a20 2020 2061 3220 3d20 2862  , 1).    a2 = (b
+000180b0: 742e 6469 6167 2870 6172 616d 7329 2e73  t.diag(params).s
+000180c0: 756d 2829 2e75 6e73 7175 6565 7a65 287b  um().unsqueeze({
+000180d0: 7d29 202b 2031 2920 2f20 340a 2020 2020  }) + 1) / 4.    
+000180e0: 6120 3d20 6274 2e73 7172 7428 6132 290a  a = bt.sqrt(a2).
+000180f0: 2020 2020 6232 203d 2061 3220 2d20 2870      b2 = a2 - (p
+00018100: 6172 616d 735b 2e2e 2e2c 2031 2c20 315d  arams[..., 1, 1]
+00018110: 202b 2070 6172 616d 735b 2e2e 2e2c 2032   + params[..., 2
+00018120: 2c20 325d 2920 2f20 320a 2020 2020 6332  , 2]) / 2.    c2
+00018130: 203d 2061 3220 2d20 2870 6172 616d 735b   = a2 - (params[
+00018140: 2e2e 2e2c 2032 2c20 325d 202b 2070 6172  ..., 2, 2] + par
+00018150: 616d 735b 2e2e 2e2c 2030 2c20 305d 2920  ams[..., 0, 0]) 
+00018160: 2f20 320a 2020 2020 6432 203d 2061 3220  / 2.    d2 = a2 
+00018170: 2d20 2870 6172 616d 735b 2e2e 2e2c 2030  - (params[..., 0
+00018180: 2c20 305d 202b 2070 6172 616d 735b 2e2e  , 0] + params[..
+00018190: 2e2c 2031 2c20 315d 2920 2f20 320a 2020  ., 1, 1]) / 2.  
+000181a0: 2020 4420 3d20 7061 7261 6d73 202d 2070    D = params - p
+000181b0: 6172 616d 732e 540a 2020 2020 6220 3d20  arams.T.    b = 
+000181c0: 6274 2e73 6967 6e28 445b 2e2e 2e2c 2032  bt.sign(D[..., 2
+000181d0: 2c20 315d 2920 2a20 6274 2e73 7172 7428  , 1]) * bt.sqrt(
+000181e0: 6232 290a 2020 2020 6320 3d20 2d20 6274  b2).    c = - bt
+000181f0: 2e73 6967 6e28 445b 2e2e 2e2c 2032 2c20  .sign(D[..., 2, 
+00018200: 305d 2920 2a20 6274 2e73 7172 7428 6332  0]) * bt.sqrt(c2
+00018210: 290a 2020 2020 6420 3d20 6274 2e73 6967  ).    d = bt.sig
+00018220: 6e28 445b 2e2e 2e2c 2031 2c20 305d 2920  n(D[..., 1, 0]) 
+00018230: 2a20 6274 2e73 7172 7428 6432 290a 2020  * bt.sqrt(d2).  
+00018240: 2020 7265 7475 726e 2062 742e 6361 7428    return bt.cat(
+00018250: 622c 2063 2c20 642c 2078 2c20 792c 207a  b, c, d, x, y, z
+00018260: 2c20 7b7d 290a                           , {}).
```

### Comparing `micomputing-1.1.40/micomputing/zxhtools/TRS.py` & `micomputing-1.1.41/micomputing/zxhtools/TRS.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc` & `micomputing-1.1.41/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc` & `micomputing-1.1.41/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc` & `micomputing-1.1.41/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc` & `micomputing-1.1.41/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/micomputing/zxhtools/exec.py` & `micomputing-1.1.41/micomputing/zxhtools/exec.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/micomputing/zxhtools/image2.FFD` & `micomputing-1.1.41/micomputing/zxhtools/image2.FFD`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/micomputing.egg-info/PKG-INFO` & `micomputing-1.1.41/micomputing.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micomputing
-Version: 1.1.40
+Version: 1.1.41
 Summary: 'micomputing' is a package for medical image computing. 
 Home-page: https://github.com/Bertie97/PyZMyc/micomputing
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # MIComputing
```

### Comparing `micomputing-1.1.40/micomputing.egg-info/SOURCES.txt` & `micomputing-1.1.41/micomputing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.40/setup_micomputing.py` & `micomputing-1.1.41/setup_micomputing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'micomputing',
-	version = '1.1.40',
+	version = '1.1.41',
 	keywords = ['pip', 'pymyc', 'micomputing', 'medical image', 'image registration', 'image similarities'],
 	description = "'micomputing' is a package for medical image computing. ",
 	long_description = '# MIComputing\n\n## Introduction\n\nPackage [`micomputing`](https://github.com/Bertie97/pycamia/tree/main/micomputing) is the medical image processing package under project [`PyCAMIA`](https://github.com/Bertie97/pycamia). It handles medical image read write, image interpolation, transformation, registration and so on. This package works under `PyCAMIA` and use `batorch.Tensor` as its basic data format. \n\n## Installation\n\nThis package can be installed by `pip install micomputing` or moving the source code to the directory of python libraries (the source code can be downloaded on [github](https://github.com/Bertie97/pycamia) or [PyPI](https://pypi.org/project/micomputing/)). \n\n```shell\npip install micomputing\n```\n\n\n\n## Acknowledgment\n\n@Yuncheng Zhou: Developer\n',
 	long_description_content_type = 'text/markdown',
 	license = 'MIT Licence',
 	url = 'https://github.com/Bertie97/PyZMyc/micomputing',
 	author = 'Yuncheng Zhou',
```

