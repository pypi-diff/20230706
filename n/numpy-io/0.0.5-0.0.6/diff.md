# Comparing `tmp/numpy_io-0.0.5-py3-none-any.whl.zip` & `tmp/numpy_io-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 27385 bytes, number of entries: 30
+Zip file size: 27383 bytes, number of entries: 30
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Apr-27 06:30 numpy_io/__init__.py
--rw-rw-rw-  2.0 fat      629 b- defN 23-Jul-04 02:07 numpy_io/setup.py
+-rw-rw-rw-  2.0 fat      628 b- defN 23-Jul-06 09:11 numpy_io/setup.py
 -rw-rw-rw-  2.0 fat       80 b- defN 23-Apr-27 06:30 numpy_io/core/__init__.py
 -rw-rw-rw-  2.0 fat    19443 b- defN 23-Jul-04 03:27 numpy_io/core/numpyadapter.py
 -rw-rw-rw-  2.0 fat     5457 b- defN 23-Apr-27 06:30 numpy_io/core/parallel.py
 -rw-rw-rw-  2.0 fat     1894 b- defN 23-Apr-27 06:30 numpy_io/core/reader.py
 -rw-rw-rw-  2.0 fat     2244 b- defN 23-Jul-04 02:33 numpy_io/core/writer.py
 -rw-rw-rw-  2.0 fat       54 b- defN 23-Apr-27 06:30 numpy_io/examples/__init__.py
 -rw-rw-rw-  2.0 fat     3236 b- defN 23-Jul-03 23:35 numpy_io/examples/auto_parallel_writer.py
@@ -21,12 +21,12 @@
 -rw-rw-rw-  2.0 fat     2658 b- defN 23-Apr-27 06:30 numpy_io/examples/testing/lmdb_test.py
 -rw-rw-rw-  2.0 fat      613 b- defN 23-Apr-27 06:30 numpy_io/examples/testing/test_mem.py
 -rw-rw-rw-  2.0 fat     2907 b- defN 23-Apr-27 07:08 numpy_io/examples/testing/test_mutiprocess.py
 -rw-rw-rw-  2.0 fat       73 b- defN 23-Apr-28 00:25 numpy_io/pytorch_loader/__init__.py
 -rw-rw-rw-  2.0 fat    10309 b- defN 23-Jul-04 03:24 numpy_io/pytorch_loader/data_helper.py
 -rw-rw-rw-  2.0 fat     8940 b- defN 23-Jul-04 01:02 numpy_io/pytorch_loader/dataloaders.py
 -rw-rw-rw-  2.0 fat     3780 b- defN 23-May-25 05:42 numpy_io/pytorch_loader/tokenizer_config_helper.py
--rw-rw-rw-  2.0 fat      390 b- defN 23-Jul-04 06:35 numpy_io-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 06:35 numpy_io-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-04 06:35 numpy_io-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2715 b- defN 23-Jul-04 06:35 numpy_io-0.0.5.dist-info/RECORD
-30 files, 82769 bytes uncompressed, 22933 bytes compressed:  72.3%
+-rw-rw-rw-  2.0 fat      389 b- defN 23-Jul-06 09:12 numpy_io-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-06 09:12 numpy_io-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-06 09:12 numpy_io-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2715 b- defN 23-Jul-06 09:12 numpy_io-0.0.6.dist-info/RECORD
+30 files, 82767 bytes uncompressed, 22931 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -72,20 +72,20 @@
 
 Filename: numpy_io/pytorch_loader/dataloaders.py
 Comment: 
 
 Filename: numpy_io/pytorch_loader/tokenizer_config_helper.py
 Comment: 
 
-Filename: numpy_io-0.0.5.dist-info/METADATA
+Filename: numpy_io-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: numpy_io-0.0.5.dist-info/WHEEL
+Filename: numpy_io-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: numpy_io-0.0.5.dist-info/top_level.txt
+Filename: numpy_io-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: numpy_io-0.0.5.dist-info/RECORD
+Filename: numpy_io-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## numpy_io/setup.py

```diff
@@ -3,22 +3,22 @@
 
 from setuptools import setup, find_packages
 
 ignore = []
 
 setup(
     name='numpy-io',
-    version='0.0.5',
+    version='0.0.6',
     description='an easy training architecture',
     long_description='numpy-io: https://github.com/ssbuild/numpy-io.git',
     license='Apache License 2.0',
     url='https://github.com/ssbuild/numpy-io',
     author='ssbuild',
     author_email='9727464@qq.com',
     install_requires=[
-        'fastdatasets>=0.9.11 , <= 0.9.13',
+        'fastdatasets>=0.9.14 , < 0.9.15',
         'numpy',
         'tqdm',
         'six'
     ],
     packages=[p for p in find_packages() if p not in ignore]
 )
```

## Comparing `numpy_io-0.0.5.dist-info/RECORD` & `numpy_io-0.0.6.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 numpy_io/__init__.py,sha256=aCtpF76c1Jz1-xvsEqeV_ze4a40-KqaqUtIrFy3BTcU,77
-numpy_io/setup.py,sha256=onT5bLye1NON71-1jHsfSUBZI7f2ZNV2qwyCaTmm47w,629
+numpy_io/setup.py,sha256=YhzOCMf8CH_tZ3wBAQ04mm0IW69Z3ONR7Ci-1BOWRtY,628
 numpy_io/core/__init__.py,sha256=gvmkt5S6jF7SlAsFM1e9qGGXV96a5yTB5lBavIVjuKo,80
 numpy_io/core/numpyadapter.py,sha256=snEnLu1oEEcn15fr7-FDaYYktCvhKVQPTAzAZdRFQ0Q,19443
 numpy_io/core/parallel.py,sha256=7pxBQ7w26H5wo1gHEMJwFwrkl57PDUA7rF3y8GD5kjM,5457
 numpy_io/core/reader.py,sha256=-i7NiW3s1gPFwaM03tDWT0NLVG6FEkz6fOuo_nWB3r8,1894
 numpy_io/core/writer.py,sha256=h0aobGbE2_QvM0bNVBg6gWz0uSR8gPrd8At6j56OJOA,2244
 numpy_io/examples/__init__.py,sha256=H6PH5pOOHNUW3_RuUpgWfpv6_Pijqyy_3U1JCTLl6jg,54
 numpy_io/examples/auto_parallel_writer.py,sha256=geSpDCFHxe4skPd3Vk45lhc3azuJEPviGhcYtUlTid4,3236
@@ -20,11 +20,11 @@
 numpy_io/examples/testing/lmdb_test.py,sha256=rQvokJAIDW9esAesab9wHs03OcG2TPImAuybnCO-LBA,2658
 numpy_io/examples/testing/test_mem.py,sha256=gteaDLS79vwwfJETTeL-JCxn3VhRT3So59y5AV4ah9w,613
 numpy_io/examples/testing/test_mutiprocess.py,sha256=rgO758tNAycWGYxyJl2AM2jkffNQs-AjRU9peSotGzQ,2907
 numpy_io/pytorch_loader/__init__.py,sha256=oRU1cnNHyp22vA9HkEYfoPtpdQdU4D9scv9KtgxYVdE,73
 numpy_io/pytorch_loader/data_helper.py,sha256=oVjtyWRobAYx1DMc5FePqQRyiQnoCpS60iidwHxN6k4,10309
 numpy_io/pytorch_loader/dataloaders.py,sha256=ov1DvKCv8GO4QGuoj09-BdUlDFop_4DScXMNv4B-jl0,8940
 numpy_io/pytorch_loader/tokenizer_config_helper.py,sha256=8hoofhL7uMyE8pT-U_3WNKDyy5DBOqQhDwJMZri-InY,3780
-numpy_io-0.0.5.dist-info/METADATA,sha256=ADm7d7mavjUI5NsgUNr0d1Q8kQsdRIzBYlSZr7VrvLY,390
-numpy_io-0.0.5.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-numpy_io-0.0.5.dist-info/top_level.txt,sha256=mV0ZVKt8HA3kBLuj9iZkff1sq-cR9hE36TgSw_7Mr4E,9
-numpy_io-0.0.5.dist-info/RECORD,,
+numpy_io-0.0.6.dist-info/METADATA,sha256=EjlBsnnuFx7h8dywruUxxTWdHEF3S262-lHkyXTUqF8,389
+numpy_io-0.0.6.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+numpy_io-0.0.6.dist-info/top_level.txt,sha256=mV0ZVKt8HA3kBLuj9iZkff1sq-cR9hE36TgSw_7Mr4E,9
+numpy_io-0.0.6.dist-info/RECORD,,
```

