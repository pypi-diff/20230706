# Comparing `tmp/batorch-1.0.40.tar.gz` & `tmp/batorch-1.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batorch-1.0.40.tar", last modified: Thu Jul  6 14:27:06 2023, max compression
+gzip compressed data, was "batorch-1.0.41.tar", last modified: Thu Jul  6 14:31:56 2023, max compression
```

## Comparing `batorch-1.0.40.tar` & `batorch-1.0.41.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:27:06.801712 batorch-1.0.40/
--rw-r--r--   0 admin      (501) staff       (20)     4301 2023-07-06 14:27:06.801570 batorch-1.0.40/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     3509 2023-07-06 14:27:06.000000 batorch-1.0.40/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:27:06.793624 batorch-1.0.40/batorch/
--rw-r--r--   0 admin      (501) staff       (20)    20337 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     7702 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/device.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:27:06.795589 batorch-1.0.40/batorch/nn/
--rw-r--r--   0 admin      (501) staff       (20)      343 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1599 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/_reduction.py
--rw-r--r--   0 admin      (501) staff       (20)     1766 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/common_types.py
--rw-r--r--   0 admin      (501) staff       (20)   186195 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/functional.py
--rw-r--r--   0 admin      (501) staff       (20)    14006 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/grad.py
--rw-r--r--   0 admin      (501) staff       (20)    18207 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/init.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:27:06.800041 batorch-1.0.40/batorch/nn/modules/
--rw-r--r--   0 admin      (501) staff       (20)     4618 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     7250 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/_functions.py
--rw-r--r--   0 admin      (501) staff       (20)    48520 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/activation.py
--rw-r--r--   0 admin      (501) staff       (20)    10997 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/adaptive.py
--rw-r--r--   0 admin      (501) staff       (20)    25981 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/batchnorm.py
--rw-r--r--   0 admin      (501) staff       (20)    23822 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/container.py
--rw-r--r--   0 admin      (501) staff       (20)    51560 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/conv.py
--rw-r--r--   0 admin      (501) staff       (20)     2662 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/distance.py
--rw-r--r--   0 admin      (501) staff       (20)     8997 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/dropout.py
--rw-r--r--   0 admin      (501) staff       (20)     4861 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/flatten.py
--rw-r--r--   0 admin      (501) staff       (20)    12545 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/fold.py
--rw-r--r--   0 admin      (501) staff       (20)    13332 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/instancenorm.py
--rw-r--r--   0 admin      (501) staff       (20)     6191 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/linear.py
--rw-r--r--   0 admin      (501) staff       (20)    77226 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/loss.py
--rw-r--r--   0 admin      (501) staff       (20)     7100 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/module.py
--rw-r--r--   0 admin      (501) staff       (20)     9717 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/normalization.py
--rw-r--r--   0 admin      (501) staff       (20)    16584 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/padding.py
--rw-r--r--   0 admin      (501) staff       (20)     1728 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/pixelshuffle.py
--rw-r--r--   0 admin      (501) staff       (20)    48072 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/pooling.py
--rw-r--r--   0 admin      (501) staff       (20)    48452 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/rnn.py
--rw-r--r--   0 admin      (501) staff       (20)    17824 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/sparse.py
--rw-r--r--   0 admin      (501) staff       (20)    17745 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/transformer.py
--rw-r--r--   0 admin      (501) staff       (20)    10086 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/upsampling.py
--rw-r--r--   0 admin      (501) staff       (20)      957 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/modules/utils.py
--rw-r--r--   0 admin      (501) staff       (20)     2734 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/parameter.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:27:06.801321 batorch-1.0.40/batorch/nn/utils/
--rw-r--r--   0 admin      (501) staff       (20)      409 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/utils/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     2914 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/utils/clip_grad.py
--rw-r--r--   0 admin      (501) staff       (20)     3027 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/utils/convert_parameters.py
--rw-r--r--   0 admin      (501) staff       (20)      813 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/utils/fusion.py
--rw-r--r--   0 admin      (501) staff       (20)     3801 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/utils/memory_format.py
--rw-r--r--   0 admin      (501) staff       (20)    52652 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/utils/prune.py
--rw-r--r--   0 admin      (501) staff       (20)    17955 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/utils/rnn.py
--rw-r--r--   0 admin      (501) staff       (20)    13674 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/utils/spectral_norm.py
--rw-r--r--   0 admin      (501) staff       (20)     4287 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/nn/utils/weight_norm.py
--rw-r--r--   0 admin      (501) staff       (20)    20603 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/optimizer.py
--rwxr-xr-x   0 admin      (501) staff       (20)   106144 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/tensor.py
--rw-r--r--   0 admin      (501) staff       (20)    45557 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/tensor2.py
--rw-r--r--   0 admin      (501) staff       (20)    24015 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/tensorfunc.py
--rw-r--r--   0 admin      (501) staff       (20)     9875 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/torch_namespace.py
--rw-r--r--   0 admin      (501) staff       (20)    13174 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch/torchext.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:27:06.794447 batorch-1.0.40/batorch.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     4301 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     1520 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       21 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        8 2023-07-06 14:27:06.000000 batorch-1.0.40/batorch.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-06 14:27:06.801761 batorch-1.0.40/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     4176 2023-07-06 14:27:06.000000 batorch-1.0.40/setup_batorch.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:31:56.633850 batorch-1.0.41/
+-rw-r--r--   0 admin      (501) staff       (20)     4301 2023-07-06 14:31:56.633690 batorch-1.0.41/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     3509 2023-07-06 14:31:56.000000 batorch-1.0.41/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:31:56.625560 batorch-1.0.41/batorch/
+-rw-r--r--   0 admin      (501) staff       (20)    20337 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     7704 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/device.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:31:56.628110 batorch-1.0.41/batorch/nn/
+-rw-r--r--   0 admin      (501) staff       (20)      343 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1599 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/_reduction.py
+-rw-r--r--   0 admin      (501) staff       (20)     1766 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/common_types.py
+-rw-r--r--   0 admin      (501) staff       (20)   186195 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/functional.py
+-rw-r--r--   0 admin      (501) staff       (20)    14006 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/grad.py
+-rw-r--r--   0 admin      (501) staff       (20)    18207 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/init.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:31:56.632081 batorch-1.0.41/batorch/nn/modules/
+-rw-r--r--   0 admin      (501) staff       (20)     4618 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     7250 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/_functions.py
+-rw-r--r--   0 admin      (501) staff       (20)    48520 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/activation.py
+-rw-r--r--   0 admin      (501) staff       (20)    10997 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/adaptive.py
+-rw-r--r--   0 admin      (501) staff       (20)    25981 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/batchnorm.py
+-rw-r--r--   0 admin      (501) staff       (20)    23822 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/container.py
+-rw-r--r--   0 admin      (501) staff       (20)    51560 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/conv.py
+-rw-r--r--   0 admin      (501) staff       (20)     2662 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/distance.py
+-rw-r--r--   0 admin      (501) staff       (20)     8997 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/dropout.py
+-rw-r--r--   0 admin      (501) staff       (20)     4861 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/flatten.py
+-rw-r--r--   0 admin      (501) staff       (20)    12545 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/fold.py
+-rw-r--r--   0 admin      (501) staff       (20)    13332 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/instancenorm.py
+-rw-r--r--   0 admin      (501) staff       (20)     6191 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/linear.py
+-rw-r--r--   0 admin      (501) staff       (20)    77226 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/loss.py
+-rw-r--r--   0 admin      (501) staff       (20)     7100 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/module.py
+-rw-r--r--   0 admin      (501) staff       (20)     9717 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/normalization.py
+-rw-r--r--   0 admin      (501) staff       (20)    16584 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/padding.py
+-rw-r--r--   0 admin      (501) staff       (20)     1728 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/pixelshuffle.py
+-rw-r--r--   0 admin      (501) staff       (20)    48072 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/pooling.py
+-rw-r--r--   0 admin      (501) staff       (20)    48452 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/rnn.py
+-rw-r--r--   0 admin      (501) staff       (20)    17824 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/sparse.py
+-rw-r--r--   0 admin      (501) staff       (20)    17745 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/transformer.py
+-rw-r--r--   0 admin      (501) staff       (20)    10086 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/upsampling.py
+-rw-r--r--   0 admin      (501) staff       (20)      957 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/modules/utils.py
+-rw-r--r--   0 admin      (501) staff       (20)     2734 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/parameter.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:31:56.633406 batorch-1.0.41/batorch/nn/utils/
+-rw-r--r--   0 admin      (501) staff       (20)      409 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/utils/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2914 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/utils/clip_grad.py
+-rw-r--r--   0 admin      (501) staff       (20)     3027 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/utils/convert_parameters.py
+-rw-r--r--   0 admin      (501) staff       (20)      813 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/utils/fusion.py
+-rw-r--r--   0 admin      (501) staff       (20)     3801 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/utils/memory_format.py
+-rw-r--r--   0 admin      (501) staff       (20)    52652 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/utils/prune.py
+-rw-r--r--   0 admin      (501) staff       (20)    17955 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/utils/rnn.py
+-rw-r--r--   0 admin      (501) staff       (20)    13674 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/utils/spectral_norm.py
+-rw-r--r--   0 admin      (501) staff       (20)     4287 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/nn/utils/weight_norm.py
+-rw-r--r--   0 admin      (501) staff       (20)    20603 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/optimizer.py
+-rwxr-xr-x   0 admin      (501) staff       (20)   106144 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/tensor.py
+-rw-r--r--   0 admin      (501) staff       (20)    45557 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/tensor2.py
+-rw-r--r--   0 admin      (501) staff       (20)    24015 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/tensorfunc.py
+-rw-r--r--   0 admin      (501) staff       (20)     9875 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/torch_namespace.py
+-rw-r--r--   0 admin      (501) staff       (20)    13174 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch/torchext.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:31:56.626222 batorch-1.0.41/batorch.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     4301 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     1520 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       21 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)        8 2023-07-06 14:31:56.000000 batorch-1.0.41/batorch.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-06 14:31:56.633903 batorch-1.0.41/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     4176 2023-07-06 14:31:56.000000 batorch-1.0.41/setup_batorch.py
```

### Comparing `batorch-1.0.40/PKG-INFO` & `batorch-1.0.41/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batorch
-Version: 1.0.40
+Version: 1.0.41
 Summary: 'batorch' is an extension of package torch, for tensors with batch dimensions. 
 Home-page: https://github.com/Bertie97/PyZMyc/batorch
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # batorch
```

### Comparing `batorch-1.0.40/README.md` & `batorch-1.0.41/README.md`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/__init__.py` & `batorch-1.0.41/batorch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = 'batorch',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.0.39',
+    version = '1.0.40',
     contact = 'bertiezhou@163.com',
     keywords = ['torch', 'batch', 'batched data'],
     description = "'batorch' is an extension of package torch, for tensors with batch dimensions. ",
     requires = ['pycamia', 'torch', 'pynvml'],
-    update = '2023-07-06 22:00:03'
+    update = '2023-07-06 22:27:05'
 ).check()
 
 import torch
 distributed = torch.distributed
 autograd = torch.autograd
 random = torch.random
 optim = torch.optim
```

### Comparing `batorch-1.0.40/batorch/device.py` & `batorch-1.0.41/batorch/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,10 +173,10 @@
         super().__init__(*devices, required_devices=required_devices, auto=auto, required_memory=required_memory, verbose=verbose) 
 
 CPU = FixedDevice(torch.device("cpu"))
 if is_available['mps']:
     __all__.append('MPS')
     MPS = FixedDevice(torch.device("mps"))
 if is_available['cuda']:
-    __all__.append('GPU', 'GPUs')
+    __all__.extend(['GPU', 'GPUs'])
     GPU = FixedDevice(torch.device("cuda:0"))
     GPUs = [FixedDevice(torch.device(f"cuda:{i}")) for i in range(torch.cuda.device_count())]
```

### Comparing `batorch-1.0.40/batorch/nn/_reduction.py` & `batorch-1.0.41/batorch/nn/_reduction.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/common_types.py` & `batorch-1.0.41/batorch/nn/common_types.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/functional.py` & `batorch-1.0.41/batorch/nn/functional.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/grad.py` & `batorch-1.0.41/batorch/nn/grad.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/init.py` & `batorch-1.0.41/batorch/nn/init.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/__init__.py` & `batorch-1.0.41/batorch/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/_functions.py` & `batorch-1.0.41/batorch/nn/modules/_functions.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/activation.py` & `batorch-1.0.41/batorch/nn/modules/activation.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/adaptive.py` & `batorch-1.0.41/batorch/nn/modules/adaptive.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/batchnorm.py` & `batorch-1.0.41/batorch/nn/modules/batchnorm.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/container.py` & `batorch-1.0.41/batorch/nn/modules/container.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/conv.py` & `batorch-1.0.41/batorch/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/distance.py` & `batorch-1.0.41/batorch/nn/modules/distance.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/dropout.py` & `batorch-1.0.41/batorch/nn/modules/dropout.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/flatten.py` & `batorch-1.0.41/batorch/nn/modules/flatten.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/fold.py` & `batorch-1.0.41/batorch/nn/modules/fold.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/instancenorm.py` & `batorch-1.0.41/batorch/nn/modules/instancenorm.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/linear.py` & `batorch-1.0.41/batorch/nn/modules/linear.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/loss.py` & `batorch-1.0.41/batorch/nn/modules/loss.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/module.py` & `batorch-1.0.41/batorch/nn/modules/module.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/normalization.py` & `batorch-1.0.41/batorch/nn/modules/normalization.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/padding.py` & `batorch-1.0.41/batorch/nn/modules/padding.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/pixelshuffle.py` & `batorch-1.0.41/batorch/nn/modules/pixelshuffle.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/pooling.py` & `batorch-1.0.41/batorch/nn/modules/pooling.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/rnn.py` & `batorch-1.0.41/batorch/nn/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/sparse.py` & `batorch-1.0.41/batorch/nn/modules/sparse.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/transformer.py` & `batorch-1.0.41/batorch/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/upsampling.py` & `batorch-1.0.41/batorch/nn/modules/upsampling.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/modules/utils.py` & `batorch-1.0.41/batorch/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/parameter.py` & `batorch-1.0.41/batorch/nn/parameter.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/utils/clip_grad.py` & `batorch-1.0.41/batorch/nn/utils/clip_grad.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/utils/convert_parameters.py` & `batorch-1.0.41/batorch/nn/utils/convert_parameters.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/utils/fusion.py` & `batorch-1.0.41/batorch/nn/utils/fusion.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/utils/memory_format.py` & `batorch-1.0.41/batorch/nn/utils/memory_format.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/utils/prune.py` & `batorch-1.0.41/batorch/nn/utils/prune.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/utils/rnn.py` & `batorch-1.0.41/batorch/nn/utils/rnn.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/utils/spectral_norm.py` & `batorch-1.0.41/batorch/nn/utils/spectral_norm.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/nn/utils/weight_norm.py` & `batorch-1.0.41/batorch/nn/utils/weight_norm.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/optimizer.py` & `batorch-1.0.41/batorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/tensor.py` & `batorch-1.0.41/batorch/tensor.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/tensor2.py` & `batorch-1.0.41/batorch/tensor2.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/tensorfunc.py` & `batorch-1.0.41/batorch/tensorfunc.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/torch_namespace.py` & `batorch-1.0.41/batorch/torch_namespace.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch/torchext.py` & `batorch-1.0.41/batorch/torchext.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/batorch.egg-info/PKG-INFO` & `batorch-1.0.41/batorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batorch
-Version: 1.0.40
+Version: 1.0.41
 Summary: 'batorch' is an extension of package torch, for tensors with batch dimensions. 
 Home-page: https://github.com/Bertie97/PyZMyc/batorch
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # batorch
```

### Comparing `batorch-1.0.40/batorch.egg-info/SOURCES.txt` & `batorch-1.0.41/batorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `batorch-1.0.40/setup_batorch.py` & `batorch-1.0.41/setup_batorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'batorch',
-	version = '1.0.40',
+	version = '1.0.41',
 	keywords = ['pip', 'pymyc', 'batorch', 'torch', 'batch', 'batched data'],
 	description = "'batorch' is an extension of package torch, for tensors with batch dimensions. ",
 	long_description = '# batorch\n\n## Introduction\n\n[batorch](https://github.com/Bertie97/pyctlib/tree/main/batorch) is a package affiliated to project [`PyCAMIA`](https://github.com/Bertie97/pycamia). We encapsulated a new type on top of `torch` tensers, which we call it `batorch.Tensor`. It has the same function as `torch.Tensor`, but it can automatically select the device it was on and provide batch or channel dimensions. Also, we try to provide more useful module for torch users to make deep learning to be implemented more easily. It relies `python v3.6+` with `torch v 1.7.0+`. ***Note that `torch v1.7.0` was released in 2020,*** *and it is necessary for this package as the inheritance behavior for this version is different from previous versions.* Most original `torch` functions should be able to be applied for `batorch` tensors. \n\n> Special features for `batorch` are still under development. If unknown errors pop our, please use traditional `torch` code to bypass it and meanwhile it would be very kind of you to let us know if anything is needed: please contact us by [e-mail](https://github.com/Bertie97/pycamia#Contributors). \n\n```python\n>>> import batorch as bt\n>>> import batorch.nn as nn\n>>> bt.turn_off_autodevice()\n>>> bt.manual_seed(0)\n<torch._C.Generator object at 0x1071b6730>\n>>> t = bt.randn([3000], 400, requires_grad=True)\n>>> LP = nn.Linear(400, 400)\n>>> a = LP(t)\n>>> a.sum().sum().backward()\n>>> print(t.grad)\nTensor([[-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702],\n        [-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702],\n        [-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702],\n        ...,\n        [-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702],\n        [-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702],\n        [-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702]], shape=batorch.Size([3000], 400))\n```\n\n`batorch` has all of following appealing features:\n\n1. **Auto assign** the tensors to available `GPU` **device** by default. \n2. Use `[nbatch]` or `{nchannel}` to specify **the batch and channel dimensions**. i.e. `tp.rand([4], {2}, 20, 30)` returns a 2-channel feature tensor of $20\\times30$ matrices with batch size 4. One may also use `tensor.batch_dimension` to access (or assign) batch dimension, channel dimension can be operated likewise. If you find it hard to remember the symbol, just remember brackets enclose paralleled items in matrices hence it represents the batch dimension for paralleled calculation; braces enclose equation systems which are highly related hence it represents the channel (or feature) dimension. \n3. Batch and channel dimension can help **auto matching the sizes** of two tensors in operations. For example, tensors of sizes `(3, [2], 4)` and `(3, 4)` can be automatically added together with axis of size 3 and 4 matched together. Some methods will also use this information. Sampling, for example, will take the batch dimension as priority.\n4. The tensor object is **compatible with original `torch` functions**. \n\n## Installation\n\nThis package can be installed by `pip install batorch` or moving the source code to the directory of python libraries (the source code can be downloaded on [github](https://github.com/Bertie97/pycamia) or [PyPI](https://pypi.org/project/batorch/)). \n\n```shell\npip install batorch\n```\n\n## Usages\n\nNot available yet, one may check the codes for usages.\n\n## Acknowledgment\n\n@ Yuncheng Zhou: Developer\n@ Yiteng Zhang: Important functions extraction',
 	long_description_content_type = 'text/markdown',
 	license = 'MIT Licence',
 	url = 'https://github.com/Bertie97/PyZMyc/batorch',
 	author = 'Yuncheng Zhou',
```

