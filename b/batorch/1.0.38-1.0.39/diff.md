# Comparing `tmp/batorch-1.0.38.tar.gz` & `tmp/batorch-1.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batorch-1.0.38.tar", last modified: Thu Jul  6 12:58:10 2023, max compression
+gzip compressed data, was "batorch-1.0.39.tar", last modified: Thu Jul  6 14:00:04 2023, max compression
```

## Comparing `batorch-1.0.38.tar` & `batorch-1.0.39.tar`

### file list

```diff
@@ -1,85 +1,63 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:10.652979 batorch-1.0.38/
--rw-r--r--   0 admin      (501) staff       (20)       99 2023-07-06 12:58:09.000000 batorch-1.0.38/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)     4301 2023-07-06 12:58:10.652823 batorch-1.0.38/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     3509 2023-07-06 12:58:10.000000 batorch-1.0.38/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:10.642497 batorch-1.0.38/batorch/
--rw-r--r--   0 admin      (501) staff       (20)    20151 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     7450 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/device.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:10.644101 batorch-1.0.38/batorch/nn/
--rw-r--r--   0 admin      (501) staff       (20)      343 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1599 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/_reduction.py
--rw-r--r--   0 admin      (501) staff       (20)     1766 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/common_types.py
--rw-r--r--   0 admin      (501) staff       (20)   186195 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/functional.py
--rw-r--r--   0 admin      (501) staff       (20)    14006 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/grad.py
--rw-r--r--   0 admin      (501) staff       (20)    18207 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/init.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:10.648244 batorch-1.0.38/batorch/nn/modules/
--rw-r--r--   0 admin      (501) staff       (20)     4618 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     7250 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/_functions.py
--rw-r--r--   0 admin      (501) staff       (20)    48520 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/activation.py
--rw-r--r--   0 admin      (501) staff       (20)    10997 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/adaptive.py
--rw-r--r--   0 admin      (501) staff       (20)    25981 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/batchnorm.py
--rw-r--r--   0 admin      (501) staff       (20)    23822 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/container.py
--rw-r--r--   0 admin      (501) staff       (20)    51560 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/conv.py
--rw-r--r--   0 admin      (501) staff       (20)     2662 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/distance.py
--rw-r--r--   0 admin      (501) staff       (20)     8997 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/dropout.py
--rw-r--r--   0 admin      (501) staff       (20)     4861 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/flatten.py
--rw-r--r--   0 admin      (501) staff       (20)    12545 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/fold.py
--rw-r--r--   0 admin      (501) staff       (20)    13332 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/instancenorm.py
--rw-r--r--   0 admin      (501) staff       (20)     6191 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/linear.py
--rw-r--r--   0 admin      (501) staff       (20)    77226 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/loss.py
--rw-r--r--   0 admin      (501) staff       (20)     7100 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/module.py
--rw-r--r--   0 admin      (501) staff       (20)     9717 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/normalization.py
--rw-r--r--   0 admin      (501) staff       (20)    16584 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/padding.py
--rw-r--r--   0 admin      (501) staff       (20)     1728 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/pixelshuffle.py
--rw-r--r--   0 admin      (501) staff       (20)    48072 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/pooling.py
--rw-r--r--   0 admin      (501) staff       (20)    48452 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/rnn.py
--rw-r--r--   0 admin      (501) staff       (20)    17824 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/sparse.py
--rw-r--r--   0 admin      (501) staff       (20)    17745 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/transformer.py
--rw-r--r--   0 admin      (501) staff       (20)    10086 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/upsampling.py
--rw-r--r--   0 admin      (501) staff       (20)      957 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/modules/utils.py
--rw-r--r--   0 admin      (501) staff       (20)     2734 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/parameter.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:10.649534 batorch-1.0.38/batorch/nn/utils/
--rw-r--r--   0 admin      (501) staff       (20)      409 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/utils/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     2914 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/utils/clip_grad.py
--rw-r--r--   0 admin      (501) staff       (20)     3027 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/utils/convert_parameters.py
--rw-r--r--   0 admin      (501) staff       (20)      813 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/utils/fusion.py
--rw-r--r--   0 admin      (501) staff       (20)     3801 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/utils/memory_format.py
--rw-r--r--   0 admin      (501) staff       (20)    52652 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/utils/prune.py
--rw-r--r--   0 admin      (501) staff       (20)    17955 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/utils/rnn.py
--rw-r--r--   0 admin      (501) staff       (20)    13674 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/utils/spectral_norm.py
--rw-r--r--   0 admin      (501) staff       (20)     4287 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/nn/utils/weight_norm.py
--rw-r--r--   0 admin      (501) staff       (20)    20603 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/optimizer.py
--rwxr-xr-x   0 admin      (501) staff       (20)   106172 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/tensor.py
--rw-r--r--   0 admin      (501) staff       (20)    45557 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/tensor2.py
--rw-r--r--   0 admin      (501) staff       (20)    24015 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/tensorfunc.py
--rw-r--r--   0 admin      (501) staff       (20)     9875 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/torch_namespace.py
--rw-r--r--   0 admin      (501) staff       (20)    13174 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch/torchext.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:10.643120 batorch-1.0.38/batorch.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     4301 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     2082 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       21 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       20 2023-07-06 12:58:10.000000 batorch-1.0.38/batorch.egg-info/top_level.txt
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:10.651314 batorch-1.0.38/micomputing/
--rw-r--r--   0 admin      (501) staff       (20)     2360 2023-07-06 12:58:08.000000 batorch-1.0.38/micomputing/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-06 12:58:09.000000 batorch-1.0.38/micomputing/data.py
--rw-r--r--   0 admin      (501) staff       (20)    38276 2023-07-06 12:58:09.000000 batorch-1.0.38/micomputing/funcs.py
--rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-06 12:58:08.000000 batorch-1.0.38/micomputing/metrics.py
--rwxr-xr-x   0 admin      (501) staff       (20)    33404 2023-07-06 12:58:09.000000 batorch-1.0.38/micomputing/micfunctions.so
--rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-06 12:58:09.000000 batorch-1.0.38/micomputing/network.py
--rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-06 12:58:08.000000 batorch-1.0.38/micomputing/plot.py
--rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-06 12:58:09.000000 batorch-1.0.38/micomputing/stdio.py
--rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-06 12:58:09.000000 batorch-1.0.38/micomputing/test.py
--rw-r--r--   0 admin      (501) staff       (20)    98904 2023-07-06 12:58:09.000000 batorch-1.0.38/micomputing/trans.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:10.651943 batorch-1.0.38/micomputing/zxhtools/
--rw-r--r--   0 admin      (501) staff       (20)     7454 2023-07-06 12:58:09.000000 batorch-1.0.38/micomputing/zxhtools/TRS.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:10.652552 batorch-1.0.38/micomputing/zxhtools/__pycache__/
--rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-06 12:58:09.000000 batorch-1.0.38/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-06 12:58:09.000000 batorch-1.0.38/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     9153 2023-07-06 12:58:09.000000 batorch-1.0.38/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc
--rw-r--r--   0 admin      (501) staff       (20)     8988 2023-07-06 12:58:09.000000 batorch-1.0.38/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     8071 2023-07-06 12:58:09.000000 batorch-1.0.38/micomputing/zxhtools/exec.py
--rw-r--r--   0 admin      (501) staff       (20)      507 2023-07-06 12:58:09.000000 batorch-1.0.38/micomputing/zxhtools/image2.AFF
--rw-r--r--   0 admin      (501) staff       (20)    21032 2023-07-06 12:58:09.000000 batorch-1.0.38/micomputing/zxhtools/image2.FFD
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-06 12:58:10.653031 batorch-1.0.38/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     4176 2023-07-06 12:58:10.000000 batorch-1.0.38/setup_batorch.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:00:04.631155 batorch-1.0.39/
+-rw-r--r--   0 admin      (501) staff       (20)     4301 2023-07-06 14:00:04.631008 batorch-1.0.39/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     3509 2023-07-06 14:00:04.000000 batorch-1.0.39/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:00:04.623265 batorch-1.0.39/batorch/
+-rw-r--r--   0 admin      (501) staff       (20)    20267 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     7640 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/device.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:00:04.625368 batorch-1.0.39/batorch/nn/
+-rw-r--r--   0 admin      (501) staff       (20)      343 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1599 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/_reduction.py
+-rw-r--r--   0 admin      (501) staff       (20)     1766 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/common_types.py
+-rw-r--r--   0 admin      (501) staff       (20)   186195 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/functional.py
+-rw-r--r--   0 admin      (501) staff       (20)    14006 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/grad.py
+-rw-r--r--   0 admin      (501) staff       (20)    18207 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/init.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:00:04.629440 batorch-1.0.39/batorch/nn/modules/
+-rw-r--r--   0 admin      (501) staff       (20)     4618 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     7250 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/_functions.py
+-rw-r--r--   0 admin      (501) staff       (20)    48520 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/activation.py
+-rw-r--r--   0 admin      (501) staff       (20)    10997 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/adaptive.py
+-rw-r--r--   0 admin      (501) staff       (20)    25981 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/batchnorm.py
+-rw-r--r--   0 admin      (501) staff       (20)    23822 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/container.py
+-rw-r--r--   0 admin      (501) staff       (20)    51560 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/conv.py
+-rw-r--r--   0 admin      (501) staff       (20)     2662 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/distance.py
+-rw-r--r--   0 admin      (501) staff       (20)     8997 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/dropout.py
+-rw-r--r--   0 admin      (501) staff       (20)     4861 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/flatten.py
+-rw-r--r--   0 admin      (501) staff       (20)    12545 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/fold.py
+-rw-r--r--   0 admin      (501) staff       (20)    13332 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/instancenorm.py
+-rw-r--r--   0 admin      (501) staff       (20)     6191 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/linear.py
+-rw-r--r--   0 admin      (501) staff       (20)    77226 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/loss.py
+-rw-r--r--   0 admin      (501) staff       (20)     7100 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/module.py
+-rw-r--r--   0 admin      (501) staff       (20)     9717 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/normalization.py
+-rw-r--r--   0 admin      (501) staff       (20)    16584 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/padding.py
+-rw-r--r--   0 admin      (501) staff       (20)     1728 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/pixelshuffle.py
+-rw-r--r--   0 admin      (501) staff       (20)    48072 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/pooling.py
+-rw-r--r--   0 admin      (501) staff       (20)    48452 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/rnn.py
+-rw-r--r--   0 admin      (501) staff       (20)    17824 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/sparse.py
+-rw-r--r--   0 admin      (501) staff       (20)    17745 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/transformer.py
+-rw-r--r--   0 admin      (501) staff       (20)    10086 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/upsampling.py
+-rw-r--r--   0 admin      (501) staff       (20)      957 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/modules/utils.py
+-rw-r--r--   0 admin      (501) staff       (20)     2734 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/parameter.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:00:04.630756 batorch-1.0.39/batorch/nn/utils/
+-rw-r--r--   0 admin      (501) staff       (20)      409 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/utils/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2914 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/utils/clip_grad.py
+-rw-r--r--   0 admin      (501) staff       (20)     3027 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/utils/convert_parameters.py
+-rw-r--r--   0 admin      (501) staff       (20)      813 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/utils/fusion.py
+-rw-r--r--   0 admin      (501) staff       (20)     3801 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/utils/memory_format.py
+-rw-r--r--   0 admin      (501) staff       (20)    52652 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/utils/prune.py
+-rw-r--r--   0 admin      (501) staff       (20)    17955 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/utils/rnn.py
+-rw-r--r--   0 admin      (501) staff       (20)    13674 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/utils/spectral_norm.py
+-rw-r--r--   0 admin      (501) staff       (20)     4287 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/nn/utils/weight_norm.py
+-rw-r--r--   0 admin      (501) staff       (20)    20603 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/optimizer.py
+-rwxr-xr-x   0 admin      (501) staff       (20)   106144 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/tensor.py
+-rw-r--r--   0 admin      (501) staff       (20)    45557 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/tensor2.py
+-rw-r--r--   0 admin      (501) staff       (20)    24015 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/tensorfunc.py
+-rw-r--r--   0 admin      (501) staff       (20)     9875 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/torch_namespace.py
+-rw-r--r--   0 admin      (501) staff       (20)    13174 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch/torchext.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 14:00:04.624248 batorch-1.0.39/batorch.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     4301 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     1520 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       21 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)        8 2023-07-06 14:00:04.000000 batorch-1.0.39/batorch.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-06 14:00:04.631209 batorch-1.0.39/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     4176 2023-07-06 14:00:04.000000 batorch-1.0.39/setup_batorch.py
```

### Comparing `batorch-1.0.38/PKG-INFO` & `batorch-1.0.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batorch
-Version: 1.0.38
+Version: 1.0.39
 Summary: 'batorch' is an extension of package torch, for tensors with batch dimensions. 
 Home-page: https://github.com/Bertie97/PyZMyc/batorch
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # batorch
```

### Comparing `batorch-1.0.38/README.md` & `batorch-1.0.39/README.md`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/__init__.py` & `batorch-1.0.39/batorch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,38 +2,41 @@
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = 'batorch',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.0.37',
+    version = '1.0.38',
     contact = 'bertiezhou@163.com',
     keywords = ['torch', 'batch', 'batched data'],
     description = "'batorch' is an extension of package torch, for tensors with batch dimensions. ",
     requires = ['pycamia', 'torch', 'pynvml'],
-    update = '2023-07-05 17:05:58'
+    update = '2023-07-06 20:58:09'
 ).check()
 
 import torch
 distributed = torch.distributed
 autograd = torch.autograd
 random = torch.random
 optim = torch.optim
 utils = torch.utils
 linalg = torch.linalg
 from .torchext import __all__
 for f in __all__:
     exec(f"from .torchext import {f}")
     setattr(torch, f, eval(f))
+    
+if torch.backends.mps.is_available(): from .device import MPS
+if torch.cuda.is_available(): from .device import GPU, GPUs
 
 from .device import free_memory_amount, all_memory_amount, AutoDevice
 from .tensorfunc import crop_as, pad, decimal, divide, equals, matpow, matprod, dot, down_scale, gaussian_kernel, norm, norm2, Fnorm, Fnorm2, frobenius_norm, meannorm, meannorm2, mean_norm, mean_norm2, Jacobian, grad_image, image_grid, up_scale, one_hot, permute_space, skew_symmetric, cross_matrix, uncross_matrix, summary, display #*
 from .optimizer import CSGD, CADAM, Optimization, train, test #*
-from .tensor import CPU, GPU, GPUs, Tensor, Size, set_device, get_device, to_device, turn_on_autodevice, turn_off_autodevice, get_cpu_memory_used, get_gpu_memory_used, inv, diag, batch_tensor, channel_tensor, zeros, zeros_like, ones, ones_like, empty, empty_like, rand, rand_like, randn, randn_like, full, full_like, randint, randint_like, eye, eye_as, eye_like, cat, stack, t, unsqueeze, squeeze, tensor, tr, trace, AVG, AggregationType, AliasDb, Any, AnyType, Argument, ArgumentSpec, AwaitType, BFloat16Storage, BFloat16Tensor, BenchmarkConfig, BenchmarkExecutionStats, Block, BoolStorage, BoolTensor, BoolType, BufferDict, ByteStorage, ByteTensor, CallStack, Callable, Capsule, CharStorage, CharTensor, ClassType, Code, CompilationUnit, CompleteArgumentSpec, ComplexDoubleStorage, ComplexFloatStorage, ComplexType, ConcreteModuleType, ConcreteModuleTypeBuilder, DeepCopyMemoTable, DeserializationStorageContext, DeviceObjType, Dict, DictType, DisableTorchFunction, DisableTorchFunctionSubclass, DispatchKey, DispatchKeySet, DoubleStorage, DoubleTensor, EnumType, ErrorReport, ExcludeDispatchKeyGuard, ExecutionPlan, FatalError, FileCheck, FloatStorage, FloatTensor, FloatType, FunctionSchema, Future, FutureType, Gradient, Graph, GraphExecutorState, HalfStorage, HalfTensor, IODescriptor, InferredType, IntStorage, IntTensor, IntType, InterfaceType, JITException, ListType, LiteScriptModule, LockingLogger, LoggerBase, LongStorage, LongTensor, ModuleDict, Node, NoneType, NoopLogger, NumberType, OperatorInfo, Optional, OptionalType, PRIVATE_OPS, ParameterDict, PyObjectType, PyTorchFileReader, PyTorchFileWriter, QInt32Storage, QInt8Storage, QUInt2x4Storage, QUInt4x2Storage, QUInt8Storage, RRefType, ScriptClass, ScriptClassFunction, ScriptDict, ScriptDictIterator, ScriptDictKeyIterator, ScriptFunction, ScriptList, ScriptListIterator, ScriptMethod, ScriptModule, ScriptModuleSerializer, ScriptObject, ScriptObjectProperty, SerializationStorageContext, Set, ShortStorage, ShortTensor, StaticModule, Storage, StorageBase, Stream, StreamObjType, StringType, SymBool, SymBoolType, SymFloat, SymInt, SymIntType, TYPE_CHECKING, Tag, TensorType, ThroughputBenchmark, TracingState, Tuple, TupleType, TypedStorage, USE_GLOBAL_DEPS, USE_RTLD_GLOBAL_WITH_LIBTORCH, Union, UnionType, UntypedStorage, Use, Value, _C, _GLOBAL_DEVICE_CONTEXT, _TorchCompileInductorWrapper, _TorchCompileWrapper, _TritonLibrary, _VF, __annotations__, __config__, __future__, __getattr__, __path__, __version__, _adaptive_avg_pool2d, _adaptive_avg_pool3d, _add_batch_dim, _add_relu, _add_relu_, _addmm_activation, _aminmax, _amp_foreach_non_finite_check_and_unscale_, _amp_update_scale_, _assert, _assert_async, _assert_tensor_metadata, _awaits, _batch_norm_impl_index, _cast_Byte, _cast_Char, _cast_Double, _cast_Float, _cast_Half, _cast_Int, _cast_Long, _cast_Short, _check, _check_index, _check_not_implemented, _check_tensor_all, _check_tensor_all_with, _check_type, _check_value, _check_with, _choose_qparams_per_tensor, _chunk_grad_outputs_efficient_attention, _classes, _coalesce, _compile, _compute_linear_combination, _conj, _conj_copy, _conj_physical, _convert_indices_from_coo_to_csr, _convert_indices_from_csr_to_coo, _convolution, _convolution_mode, _copy_from, _copy_from_and_resize, _ctc_loss, _cudnn_ctc_loss, _cudnn_init_dropout_state, _cudnn_rnn, _cudnn_rnn_flatten_weight, _cufft_clear_plan_cache, _cufft_get_plan_cache_max_size, _cufft_get_plan_cache_size, _cufft_set_plan_cache_max_size, _cummax_helper, _cummin_helper, _custom_op, _debug_has_internal_overlap, _decomp, _deprecated_attrs, _dim_arange, _dirichlet_grad, _disable_dynamo, _disable_functionalization, _dispatch, _efficientzerotensor, _embedding_bag, _embedding_bag_forward_only, _empty_affine_quantized, _empty_per_channel_affine_quantized, _enable_functionalization, _euclidean_dist, _fake_quantize_learnable_per_channel_affine, _fake_quantize_learnable_per_tensor_affine, _fake_quantize_per_tensor_affine_cachemask_tensor_qparams, _fft_c2c, _fft_c2r, _fft_r2c, _fill_mem_eff_dropout_mask_, _foobar, _foreach_abs, _foreach_abs_, _foreach_acos, _foreach_acos_, _foreach_add, _foreach_add_, _foreach_addcdiv, _foreach_addcdiv_, _foreach_addcmul, _foreach_addcmul_, _foreach_asin, _foreach_asin_, _foreach_atan, _foreach_atan_, _foreach_ceil, _foreach_ceil_, _foreach_clamp_max, _foreach_clamp_max_, _foreach_clamp_min, _foreach_clamp_min_, _foreach_cos, _foreach_cos_, _foreach_cosh, _foreach_cosh_, _foreach_div, _foreach_div_, _foreach_erf, _foreach_erf_, _foreach_erfc, _foreach_erfc_, _foreach_exp, _foreach_exp_, _foreach_expm1, _foreach_expm1_, _foreach_floor, _foreach_floor_, _foreach_frac, _foreach_frac_, _foreach_lerp, _foreach_lerp_, _foreach_lgamma, _foreach_lgamma_, _foreach_log, _foreach_log10, _foreach_log10_, _foreach_log1p, _foreach_log1p_, _foreach_log2, _foreach_log2_, _foreach_log_, _foreach_maximum, _foreach_maximum_, _foreach_minimum, _foreach_minimum_, _foreach_mul, _foreach_mul_, _foreach_neg, _foreach_neg_, _foreach_norm, _foreach_pow, _foreach_pow_, _foreach_reciprocal, _foreach_reciprocal_, _foreach_round, _foreach_round_, _foreach_sigmoid, _foreach_sigmoid_, _foreach_sin, _foreach_sin_, _foreach_sinh, _foreach_sinh_, _foreach_sqrt, _foreach_sqrt_, _foreach_sub, _foreach_sub_, _foreach_tan, _foreach_tan_, _foreach_tanh, _foreach_tanh_, _foreach_trunc, _foreach_trunc_, _foreach_zero_, _freeze_functional_tensor, _from_functional_tensor, _functional_assert_async, _functional_sym_constrain_range, _functionalize_has_metadata_mutation, _functorch, _fused_adam_, _fused_adamw_, _fused_dropout, _fused_moving_avg_obs_fq_helper, _fused_sdp_choice, _fw_primal_copy, _grid_sampler_2d_cpu_fallback, _guards, _has_compatible_shallow_copy_type, _histogramdd_bin_edges, _histogramdd_from_bin_cts, _histogramdd_from_bin_tensors, _import_dotted_name, _index_put_impl_, _indices_copy, _initExtension, _int_mm, _is_all_true, _is_any_true, _is_functional_tensor, _is_zerotensor, _jit_internal, _lazy_modules, _linalg_check_errors, _linalg_det, _linalg_eigh, _linalg_slogdet, _linalg_solve_ex, _linalg_svd, _linalg_utils, _load_global_deps, _lobpcg, _log_softmax, _log_softmax_backward_data, _logcumsumexp, _logging, _lowrank, _lstm_mps, _lu_with_info, _make_dep_token, _make_dual, _make_dual_copy, _make_per_channel_quantized_tensor, _make_per_tensor_quantized_tensor, _masked_scale, _masked_softmax, _meta_registrations, _mkldnn, _mkldnn_reshape, _mkldnn_transpose, _mkldnn_transpose_, _mps_convolution, _mps_convolution_transpose, _namedtensor_internals, _native_batch_norm_legit, _native_batch_norm_legit_no_training, _native_multi_head_attention, _neg_view, _neg_view_copy, _nested_from_padded, _nested_from_padded_and_nested_example, _nested_tensor_from_mask, _nested_tensor_from_mask_left_aligned, _nested_tensor_from_tensor_list, _nested_tensor_softmax_with_shape, _nnpack_available, _nnpack_spatial_convolution, _ops, _pack_padded_sequence, _pad_packed_sequence, _pin_memory, _preload_cuda_deps, _prelu_kernel, _prims, _prims_common, _propagate_xla_data, _refs, _register_device_module, _remove_batch_dim, _reshape_alias_copy, _reshape_from_tensor, _resize_output_, _rowwise_prune, _running_with_deploy, _sample_dirichlet, _saturate_weight_to_fp16, _scaled_dot_product_attention_math, _scaled_dot_product_efficient_attention, _scaled_dot_product_flash_attention, _segment_reduce, _shape_as_tensor, _sobol_engine_draw, _sobol_engine_ff_, _sobol_engine_initialize_state_, _sobol_engine_scramble_, _softmax, _softmax_backward_data, _sources, _sparse_broadcast_to, _sparse_broadcast_to_copy, _sparse_coo_tensor_unsafe, _sparse_csr_prod, _sparse_csr_sum, _sparse_log_softmax_backward_data, _sparse_softmax_backward_data, _sparse_sparse_matmul, _sparse_sum, _stack, _standard_gamma, _standard_gamma_grad, _storage_classes, _structured_sparse_linear, _subclasses, _sync, _tensor, _tensor_classes, _tensor_str, _test_autograd_multiple_dispatch, _test_autograd_multiple_dispatch_view, _test_autograd_multiple_dispatch_view_copy, _test_check_tensor, _test_functorch_fallback, _test_serialization_subcmul, _to_cpu, _to_functional_tensor, _transform_bias_rescale_qkv, _transformer_encoder_layer_fwd, _trilinear, _triton_multi_head_attention, _triton_scaled_dot_attention, _unique, _unique2, _unpack_dual, _unsafe_index, _unsafe_index_put, _use_cudnn_ctc_loss, _use_cudnn_rnn_flatten_weight, _utils, _utils_internal, _validate_compressed_sparse_indices, _validate_sparse_bsc_tensor_args, _validate_sparse_bsr_tensor_args, _validate_sparse_compressed_tensor_args, _validate_sparse_coo_tensor_args, _validate_sparse_csc_tensor_args, _validate_sparse_csr_tensor_args, _values_copy, _vmap_internals, _warn_typed_storage_removal, _weight_norm, _weight_norm_interface, _weights_only_unpickler, abs, abs_, absolute, acos, acos_, acosh, acosh_, adaptive_avg_pool1d, adaptive_max_pool1d, add, addbmm, addcdiv, addcmul, addmm, addmv, addmv_, addr, adjoint, affine_grid_generator, alias_copy, align_tensors, all, allclose, alpha_dropout, alpha_dropout_, amax, amin, aminmax, amp, angle, any, ao, arange, arccos, arccos_, arccosh, arccosh_, arcsin, arcsin_, arcsinh, arcsinh_, arctan, arctan2, arctan_, arctanh, arctanh_, are_deterministic_algorithms_enabled, argmax, argmin, argsort, argwhere, as_strided, as_strided_, as_strided_copy, as_strided_scatter, as_tensor, asarray, asin, asin_, asinh, asinh_, atan, atan2, atan_, atanh, atanh_, atleast_1d, atleast_2d, atleast_3d, attr, autocast, autocast_decrement_nesting, autocast_increment_nesting, autograd, avg_pool1d, backends, baddbmm, bartlett_window, batch_norm, batch_norm_backward_elemt, batch_norm_backward_reduce, batch_norm_elemt, batch_norm_gather_stats, batch_norm_gather_stats_with_counts, batch_norm_stats, batch_norm_update_stats, bernoulli, bfloat16, bilinear, binary_cross_entropy_with_logits, bincount, binomial, bits16, bits1x8, bits2x4, bits4x2, bits8, bitwise_and, bitwise_left_shift, bitwise_not, bitwise_or, bitwise_right_shift, bitwise_xor, blackman_window, block_diag, bmm, bool, broadcast_shapes, broadcast_tensors, broadcast_to, bucketize, can_cast, candidate, cartesian_prod, ccol_indices_copy, cdist, cdouble, ceil, ceil_, celu, celu_, cfloat, chain_matmul, chalf, channel_shuffle, channels_last, channels_last_3d, cholesky, cholesky_inverse, cholesky_solve, choose_qparams_optimized, chunk, clamp, clamp_, clamp_max, clamp_max_, clamp_min, clamp_min_, classes, classproperty, clear_autocast_cache, clip, clip_, clone, col_indices_copy, column_stack, combinations, compile, compiled_with_cxx11_abi, compiler, complex, complex128, complex32, complex64, concat, concatenate, conj, conj_physical, conj_physical_, constant_pad_nd, contiguous_format, conv1d, conv2d, conv3d, conv_tbc, conv_transpose1d, conv_transpose2d, conv_transpose3d, convolution, copysign, corrcoef, cos, cos_, cosh, cosh_, cosine_embedding_loss, cosine_similarity, count_nonzero, cov, cpp, cpu, cross, crow_indices_copy, ctc_loss, ctypes, cuda, cudnn_affine_grid_generator, cudnn_batch_norm, cudnn_convolution, cudnn_convolution_add_relu, cudnn_convolution_relu, cudnn_convolution_transpose, cudnn_grid_sampler, cudnn_is_acceptable, cummax, cummin, cumprod, cumsum, cumulative_trapezoid, default_generator, deg2rad, deg2rad_, dequantize, det, detach, detach_, detach_copy, device, diag_embed, diagflat, diagonal, diagonal_copy, diagonal_scatter, diff, digamma, dist, distributed, distributions, div, divide, dot, double, dropout, dropout_, dsmm, dsplit, dstack, dtype, e, eig, einsum, embedding, embedding_bag, embedding_renorm_, empty_permuted, empty_quantized, empty_strided, enable_grad, eq, equal, erf, erf_, erfc, erfc_, erfinv, exp, exp2, exp2_, exp_, expand_copy, expm1, expm1_, fake_quantize_per_channel_affine, fake_quantize_per_tensor_affine, fbgemm_linear_fp16_weight, fbgemm_linear_fp16_weight_fp32_activation, fbgemm_linear_int8_weight, fbgemm_linear_int8_weight_fp32_activation, fbgemm_linear_quantize_weight, fbgemm_pack_gemm_matrix_fp16, fbgemm_pack_quantized_matrix, feature_alpha_dropout, feature_alpha_dropout_, feature_dropout, feature_dropout_, fft, fill, fill_, finfo, fix, fix_, flatten, flip, fliplr, flipud, float, float16, float32, float64, float_power, floor, floor_, floor_divide, fmax, fmin, fmod, fork, frac, frac_, frexp, frobenius_norm, from_dlpack, from_file, from_numpy, frombuffer, functional, fused_moving_avg_obs_fake_quant, futures, fx, gather, gcd, gcd_, ge, geqrf, ger, get_autocast_cpu_dtype, get_autocast_gpu_dtype, get_autocast_ipu_dtype, get_autocast_xla_dtype, get_default_dtype, get_deterministic_debug_mode, get_file_path, get_float32_matmul_precision, get_num_interop_threads, get_num_threads, get_rng_state, gradient, greater, greater_equal, grid_sampler, grid_sampler_2d, grid_sampler_3d, group_norm, gru, gru_cell, gt, half, hamming_window, hann_window, hardshrink, has_lapack, has_mkl, has_openmp, has_spectral, heaviside, hinge_embedding_loss, histc, histogram, histogramdd, hsmm, hsplit, hspmm, hstack, hub, hypot, i0, i0_, igamma, igammac, iinfo, imag, import_ir_module, import_ir_module_from_buffer, index_add, index_copy, index_fill, index_put, index_put_, index_reduce, index_select, indices_copy, inf, inference_mode, init_num_threads, initial_seed, inner, inspect, instance_norm, int, int16, int32, int64, int8, int_repr, inverse, is_anomaly_check_nan_enabled, is_anomaly_enabled, is_autocast_cache_enabled, is_autocast_cpu_enabled, is_autocast_enabled, is_autocast_ipu_enabled, is_autocast_xla_enabled, is_complex, is_conj, is_deterministic_algorithms_warn_only_enabled, is_distributed, is_floating_point, is_grad_enabled, is_inference, is_inference_mode_enabled, is_neg, is_nonzero, is_same_size, is_signed, is_storage, is_tensor, is_vulkan_available, is_warn_always_enabled, isclose, isfinite, isin, isinf, isnan, isneginf, isposinf, isreal, istft, jit, kaiser_window, kl_div, kron, kthvalue, layer_norm, layout, lcm, lcm_, ldexp, ldexp_, le, legacy_contiguous_format, lerp, less, less_equal, lgamma, library, linalg, linspace, load, lobpcg, log, log10, log10_, log1p, log1p_, log2, log2_, log_, log_softmax, logaddexp, logaddexp2, logcumsumexp, logdet, logical_and, logical_not, logical_or, logical_xor, logit, logit_, logspace, logsumexp, long, lstm, lstm_cell, lstsq, lt, lu, lu_solve, lu_unpack, manual_seed, margin_ranking_loss, masked, masked_fill, masked_scatter, masked_select, math, matmul, matrix_exp, matrix_power, matrix_rank, max, max_pool1d, max_pool1d_with_indices, max_pool2d, max_pool3d, maximum, mean, median, memory_format, merge_type_from_type_comment, meshgrid, min, minimum, miopen_batch_norm, miopen_convolution, miopen_convolution_add_relu, miopen_convolution_relu, miopen_convolution_transpose, miopen_depthwise_convolution, miopen_rnn, mkldnn_adaptive_avg_pool2d, mkldnn_convolution, mkldnn_linear_backward_weights, mkldnn_max_pool2d, mkldnn_max_pool3d, mkldnn_rnn_layer, mm, mode, moveaxis, movedim, mps, msort, mul, multinomial, multiply, multiprocessing, mv, mvlgamma, name, nan, nan_to_num, nan_to_num_, nanmean, nanmedian, nanquantile, nansum, narrow, narrow_copy, native_batch_norm, native_channel_shuffle, native_dropout, native_group_norm, native_layer_norm, native_norm, ne, neg, neg_, negative, negative_, nested, nextafter, nn, no_grad, nonzero, nonzero_static, norm, norm_except_dim, normal, not_equal, nuclear_norm, numel, obj, onnx, ops, optim, orgqr, ormqr, os, outer, overrides, package, pairwise_distance, parse_ir, parse_schema, parse_type_comment, pca_lowrank, pdist, per_channel_affine, per_channel_affine_float_qparams, per_channel_symmetric, per_tensor_affine, per_tensor_symmetric, permute, permute_copy, pi, pinverse, pixel_shuffle, pixel_unshuffle, platform, poisson, poisson_nll_loss, polar, polygamma, positive, pow, prelu, prepare_multiprocessing_environment, preserve_format, prod, profiler, promote_types, put, py_float, py_int, q_per_channel_axis, q_per_channel_scales, q_per_channel_zero_points, q_scale, q_zero_point, qint32, qint8, qr, qscheme, quantile, quantization, quantize_per_channel, quantize_per_tensor, quantize_per_tensor_dynamic, quantized_batch_norm, quantized_gru, quantized_gru_cell, quantized_lstm, quantized_lstm_cell, quantized_max_pool1d, quantized_max_pool2d, quantized_max_pool3d, quantized_rnn_relu_cell, quantized_rnn_tanh_cell, quasirandom, quint2x4, quint4x2, quint8, rad2deg, rad2deg_, random, randperm, range, ravel, read_vitals, real, reciprocal, reciprocal_, relu, relu_, remainder, renorm, repeat_interleave, reshape, resize_as_, resize_as_sparse_, resolve_conj, resolve_neg, result_type, return_types, rnn_relu, rnn_relu_cell, rnn_tanh, rnn_tanh_cell, roll, rot90, round, round_, row_indices_copy, row_stack, rrelu, rrelu_, rsqrt, rsqrt_, rsub, saddmm, save, scalar_tensor, scatter, scatter_add, scatter_reduce, searchsorted, seed, segment_reduce, select, select_copy, select_scatter, selu, selu_, serialization, set_anomaly_enabled, set_autocast_cache_enabled, set_autocast_cpu_dtype, set_autocast_cpu_enabled, set_autocast_enabled, set_autocast_gpu_dtype, set_autocast_ipu_dtype, set_autocast_ipu_enabled, set_autocast_xla_dtype, set_autocast_xla_enabled, set_default_device, set_default_dtype, set_default_tensor_type, set_deterministic_debug_mode, set_float32_matmul_precision, set_flush_denormal, set_grad_enabled, set_num_interop_threads, set_num_threads, set_printoptions, set_rng_state, set_vital, set_warn_always, sgn, short, sigmoid, sigmoid_, sign, signal, signbit, sin, sin_, sinc, sinc_, sinh, sinh_, slice_copy, slice_scatter, slogdet, smm, softmax, solve, sort, sparse, sparse_bsc, sparse_bsc_tensor, sparse_bsr, sparse_bsr_tensor, sparse_compressed_tensor, sparse_coo, sparse_coo_tensor, sparse_csc, sparse_csc_tensor, sparse_csr, sparse_csr_tensor, special, split, split_copy, split_with_sizes, split_with_sizes_copy, spmm, sqrt, sqrt_, square, square_, squeeze_copy, sspaddmm, std, std_mean, stft, storage, strided, sub, subtract, sum, svd, svd_lowrank, swapaxes, swapdims, sym_constrain_range, sym_float, sym_int, sym_max, sym_min, sym_not, symeig, t_copy, take, take_along_dim, tan, tan_, tanh, tanh_, tensor_split, tensordot, testing, textwrap, threshold, threshold_, tile, to_dlpack, topk, torch_version, transpose, transpose_copy, trapezoid, trapz, triangular_solve, tril, tril_indices, triplet_margin_loss, triu, triu_indices, true_divide, trunc, trunc_, types, uint8, unbind, unbind_copy, unflatten, unfold_copy, unify_type_list, unique, unique_consecutive, unsafe_chunk, unsafe_split, unsafe_split_with_sizes, unsqueeze_copy, use_deterministic_algorithms, utils, values_copy, vander, var, var_mean, vdot, version, view_as_complex, view_as_complex_copy, view_as_real, view_as_real_copy, view_copy, vitals_enabled, vmap, vsplit, vstack, wait, where, windows, xlogy, xlogy_, zero_ #**
+from .tensor import CPU, Tensor, Size, set_device, get_device, to_device, turn_on_autodevice, turn_off_autodevice, get_cpu_memory_used, get_gpu_memory_used, inv, diag, batch_tensor, channel_tensor, zeros, zeros_like, ones, ones_like, empty, empty_like, rand, rand_like, randn, randn_like, full, full_like, randint, randint_like, eye, eye_as, eye_like, cat, stack, t, unsqueeze, squeeze, tensor, tr, trace, AVG, AggregationType, AliasDb, Any, AnyType, Argument, ArgumentSpec, AwaitType, BFloat16Storage, BFloat16Tensor, BenchmarkConfig, BenchmarkExecutionStats, Block, BoolStorage, BoolTensor, BoolType, BufferDict, ByteStorage, ByteTensor, CallStack, Callable, Capsule, CharStorage, CharTensor, ClassType, Code, CompilationUnit, CompleteArgumentSpec, ComplexDoubleStorage, ComplexFloatStorage, ComplexType, ConcreteModuleType, ConcreteModuleTypeBuilder, DeepCopyMemoTable, DeserializationStorageContext, DeviceObjType, Dict, DictType, DisableTorchFunction, DisableTorchFunctionSubclass, DispatchKey, DispatchKeySet, DoubleStorage, DoubleTensor, EnumType, ErrorReport, ExcludeDispatchKeyGuard, ExecutionPlan, FatalError, FileCheck, FloatStorage, FloatTensor, FloatType, FunctionSchema, Future, FutureType, Gradient, Graph, GraphExecutorState, HalfStorage, HalfTensor, IODescriptor, InferredType, IntStorage, IntTensor, IntType, InterfaceType, JITException, ListType, LiteScriptModule, LockingLogger, LoggerBase, LongStorage, LongTensor, ModuleDict, Node, NoneType, NoopLogger, NumberType, OperatorInfo, Optional, OptionalType, PRIVATE_OPS, ParameterDict, PyObjectType, PyTorchFileReader, PyTorchFileWriter, QInt32Storage, QInt8Storage, QUInt2x4Storage, QUInt4x2Storage, QUInt8Storage, RRefType, ScriptClass, ScriptClassFunction, ScriptDict, ScriptDictIterator, ScriptDictKeyIterator, ScriptFunction, ScriptList, ScriptListIterator, ScriptMethod, ScriptModule, ScriptModuleSerializer, ScriptObject, ScriptObjectProperty, SerializationStorageContext, Set, ShortStorage, ShortTensor, StaticModule, Storage, StorageBase, Stream, StreamObjType, StringType, SymBool, SymBoolType, SymFloat, SymInt, SymIntType, TYPE_CHECKING, Tag, TensorType, ThroughputBenchmark, TracingState, Tuple, TupleType, TypedStorage, USE_GLOBAL_DEPS, USE_RTLD_GLOBAL_WITH_LIBTORCH, Union, UnionType, UntypedStorage, Use, Value, _C, _GLOBAL_DEVICE_CONTEXT, _TorchCompileInductorWrapper, _TorchCompileWrapper, _TritonLibrary, _VF, __annotations__, __config__, __future__, __getattr__, __path__, __version__, _adaptive_avg_pool2d, _adaptive_avg_pool3d, _add_batch_dim, _add_relu, _add_relu_, _addmm_activation, _aminmax, _amp_foreach_non_finite_check_and_unscale_, _amp_update_scale_, _assert, _assert_async, _assert_tensor_metadata, _awaits, _batch_norm_impl_index, _cast_Byte, _cast_Char, _cast_Double, _cast_Float, _cast_Half, _cast_Int, _cast_Long, _cast_Short, _check, _check_index, _check_not_implemented, _check_tensor_all, _check_tensor_all_with, _check_type, _check_value, _check_with, _choose_qparams_per_tensor, _chunk_grad_outputs_efficient_attention, _classes, _coalesce, _compile, _compute_linear_combination, _conj, _conj_copy, _conj_physical, _convert_indices_from_coo_to_csr, _convert_indices_from_csr_to_coo, _convolution, _convolution_mode, _copy_from, _copy_from_and_resize, _ctc_loss, _cudnn_ctc_loss, _cudnn_init_dropout_state, _cudnn_rnn, _cudnn_rnn_flatten_weight, _cufft_clear_plan_cache, _cufft_get_plan_cache_max_size, _cufft_get_plan_cache_size, _cufft_set_plan_cache_max_size, _cummax_helper, _cummin_helper, _custom_op, _debug_has_internal_overlap, _decomp, _deprecated_attrs, _dim_arange, _dirichlet_grad, _disable_dynamo, _disable_functionalization, _dispatch, _efficientzerotensor, _embedding_bag, _embedding_bag_forward_only, _empty_affine_quantized, _empty_per_channel_affine_quantized, _enable_functionalization, _euclidean_dist, _fake_quantize_learnable_per_channel_affine, _fake_quantize_learnable_per_tensor_affine, _fake_quantize_per_tensor_affine_cachemask_tensor_qparams, _fft_c2c, _fft_c2r, _fft_r2c, _fill_mem_eff_dropout_mask_, _foobar, _foreach_abs, _foreach_abs_, _foreach_acos, _foreach_acos_, _foreach_add, _foreach_add_, _foreach_addcdiv, _foreach_addcdiv_, _foreach_addcmul, _foreach_addcmul_, _foreach_asin, _foreach_asin_, _foreach_atan, _foreach_atan_, _foreach_ceil, _foreach_ceil_, _foreach_clamp_max, _foreach_clamp_max_, _foreach_clamp_min, _foreach_clamp_min_, _foreach_cos, _foreach_cos_, _foreach_cosh, _foreach_cosh_, _foreach_div, _foreach_div_, _foreach_erf, _foreach_erf_, _foreach_erfc, _foreach_erfc_, _foreach_exp, _foreach_exp_, _foreach_expm1, _foreach_expm1_, _foreach_floor, _foreach_floor_, _foreach_frac, _foreach_frac_, _foreach_lerp, _foreach_lerp_, _foreach_lgamma, _foreach_lgamma_, _foreach_log, _foreach_log10, _foreach_log10_, _foreach_log1p, _foreach_log1p_, _foreach_log2, _foreach_log2_, _foreach_log_, _foreach_maximum, _foreach_maximum_, _foreach_minimum, _foreach_minimum_, _foreach_mul, _foreach_mul_, _foreach_neg, _foreach_neg_, _foreach_norm, _foreach_pow, _foreach_pow_, _foreach_reciprocal, _foreach_reciprocal_, _foreach_round, _foreach_round_, _foreach_sigmoid, _foreach_sigmoid_, _foreach_sin, _foreach_sin_, _foreach_sinh, _foreach_sinh_, _foreach_sqrt, _foreach_sqrt_, _foreach_sub, _foreach_sub_, _foreach_tan, _foreach_tan_, _foreach_tanh, _foreach_tanh_, _foreach_trunc, _foreach_trunc_, _foreach_zero_, _freeze_functional_tensor, _from_functional_tensor, _functional_assert_async, _functional_sym_constrain_range, _functionalize_has_metadata_mutation, _functorch, _fused_adam_, _fused_adamw_, _fused_dropout, _fused_moving_avg_obs_fq_helper, _fused_sdp_choice, _fw_primal_copy, _grid_sampler_2d_cpu_fallback, _guards, _has_compatible_shallow_copy_type, _histogramdd_bin_edges, _histogramdd_from_bin_cts, _histogramdd_from_bin_tensors, _import_dotted_name, _index_put_impl_, _indices_copy, _initExtension, _int_mm, _is_all_true, _is_any_true, _is_functional_tensor, _is_zerotensor, _jit_internal, _lazy_modules, _linalg_check_errors, _linalg_det, _linalg_eigh, _linalg_slogdet, _linalg_solve_ex, _linalg_svd, _linalg_utils, _load_global_deps, _lobpcg, _log_softmax, _log_softmax_backward_data, _logcumsumexp, _logging, _lowrank, _lstm_mps, _lu_with_info, _make_dep_token, _make_dual, _make_dual_copy, _make_per_channel_quantized_tensor, _make_per_tensor_quantized_tensor, _masked_scale, _masked_softmax, _meta_registrations, _mkldnn, _mkldnn_reshape, _mkldnn_transpose, _mkldnn_transpose_, _mps_convolution, _mps_convolution_transpose, _namedtensor_internals, _native_batch_norm_legit, _native_batch_norm_legit_no_training, _native_multi_head_attention, _neg_view, _neg_view_copy, _nested_from_padded, _nested_from_padded_and_nested_example, _nested_tensor_from_mask, _nested_tensor_from_mask_left_aligned, _nested_tensor_from_tensor_list, _nested_tensor_softmax_with_shape, _nnpack_available, _nnpack_spatial_convolution, _ops, _pack_padded_sequence, _pad_packed_sequence, _pin_memory, _preload_cuda_deps, _prelu_kernel, _prims, _prims_common, _propagate_xla_data, _refs, _register_device_module, _remove_batch_dim, _reshape_alias_copy, _reshape_from_tensor, _resize_output_, _rowwise_prune, _running_with_deploy, _sample_dirichlet, _saturate_weight_to_fp16, _scaled_dot_product_attention_math, _scaled_dot_product_efficient_attention, _scaled_dot_product_flash_attention, _segment_reduce, _shape_as_tensor, _sobol_engine_draw, _sobol_engine_ff_, _sobol_engine_initialize_state_, _sobol_engine_scramble_, _softmax, _softmax_backward_data, _sources, _sparse_broadcast_to, _sparse_broadcast_to_copy, _sparse_coo_tensor_unsafe, _sparse_csr_prod, _sparse_csr_sum, _sparse_log_softmax_backward_data, _sparse_softmax_backward_data, _sparse_sparse_matmul, _sparse_sum, _stack, _standard_gamma, _standard_gamma_grad, _storage_classes, _structured_sparse_linear, _subclasses, _sync, _tensor, _tensor_classes, _tensor_str, _test_autograd_multiple_dispatch, _test_autograd_multiple_dispatch_view, _test_autograd_multiple_dispatch_view_copy, _test_check_tensor, _test_functorch_fallback, _test_serialization_subcmul, _to_cpu, _to_functional_tensor, _transform_bias_rescale_qkv, _transformer_encoder_layer_fwd, _trilinear, _triton_multi_head_attention, _triton_scaled_dot_attention, _unique, _unique2, _unpack_dual, _unsafe_index, _unsafe_index_put, _use_cudnn_ctc_loss, _use_cudnn_rnn_flatten_weight, _utils, _utils_internal, _validate_compressed_sparse_indices, _validate_sparse_bsc_tensor_args, _validate_sparse_bsr_tensor_args, _validate_sparse_compressed_tensor_args, _validate_sparse_coo_tensor_args, _validate_sparse_csc_tensor_args, _validate_sparse_csr_tensor_args, _values_copy, _vmap_internals, _warn_typed_storage_removal, _weight_norm, _weight_norm_interface, _weights_only_unpickler, abs, abs_, absolute, acos, acos_, acosh, acosh_, adaptive_avg_pool1d, adaptive_max_pool1d, add, addbmm, addcdiv, addcmul, addmm, addmv, addmv_, addr, adjoint, affine_grid_generator, alias_copy, align_tensors, all, allclose, alpha_dropout, alpha_dropout_, amax, amin, aminmax, amp, angle, any, ao, arange, arccos, arccos_, arccosh, arccosh_, arcsin, arcsin_, arcsinh, arcsinh_, arctan, arctan2, arctan_, arctanh, arctanh_, are_deterministic_algorithms_enabled, argmax, argmin, argsort, argwhere, as_strided, as_strided_, as_strided_copy, as_strided_scatter, as_tensor, asarray, asin, asin_, asinh, asinh_, atan, atan2, atan_, atanh, atanh_, atleast_1d, atleast_2d, atleast_3d, attr, autocast, autocast_decrement_nesting, autocast_increment_nesting, autograd, avg_pool1d, backends, baddbmm, bartlett_window, batch_norm, batch_norm_backward_elemt, batch_norm_backward_reduce, batch_norm_elemt, batch_norm_gather_stats, batch_norm_gather_stats_with_counts, batch_norm_stats, batch_norm_update_stats, bernoulli, bfloat16, bilinear, binary_cross_entropy_with_logits, bincount, binomial, bits16, bits1x8, bits2x4, bits4x2, bits8, bitwise_and, bitwise_left_shift, bitwise_not, bitwise_or, bitwise_right_shift, bitwise_xor, blackman_window, block_diag, bmm, bool, broadcast_shapes, broadcast_tensors, broadcast_to, bucketize, can_cast, candidate, cartesian_prod, ccol_indices_copy, cdist, cdouble, ceil, ceil_, celu, celu_, cfloat, chain_matmul, chalf, channel_shuffle, channels_last, channels_last_3d, cholesky, cholesky_inverse, cholesky_solve, choose_qparams_optimized, chunk, clamp, clamp_, clamp_max, clamp_max_, clamp_min, clamp_min_, classes, classproperty, clear_autocast_cache, clip, clip_, clone, col_indices_copy, column_stack, combinations, compile, compiled_with_cxx11_abi, compiler, complex, complex128, complex32, complex64, concat, concatenate, conj, conj_physical, conj_physical_, constant_pad_nd, contiguous_format, conv1d, conv2d, conv3d, conv_tbc, conv_transpose1d, conv_transpose2d, conv_transpose3d, convolution, copysign, corrcoef, cos, cos_, cosh, cosh_, cosine_embedding_loss, cosine_similarity, count_nonzero, cov, cpp, cpu, cross, crow_indices_copy, ctc_loss, ctypes, cuda, cudnn_affine_grid_generator, cudnn_batch_norm, cudnn_convolution, cudnn_convolution_add_relu, cudnn_convolution_relu, cudnn_convolution_transpose, cudnn_grid_sampler, cudnn_is_acceptable, cummax, cummin, cumprod, cumsum, cumulative_trapezoid, default_generator, deg2rad, deg2rad_, dequantize, det, detach, detach_, detach_copy, device, diag_embed, diagflat, diagonal, diagonal_copy, diagonal_scatter, diff, digamma, dist, distributed, distributions, div, divide, dot, double, dropout, dropout_, dsmm, dsplit, dstack, dtype, e, eig, einsum, embedding, embedding_bag, embedding_renorm_, empty_permuted, empty_quantized, empty_strided, enable_grad, eq, equal, erf, erf_, erfc, erfc_, erfinv, exp, exp2, exp2_, exp_, expand_copy, expm1, expm1_, fake_quantize_per_channel_affine, fake_quantize_per_tensor_affine, fbgemm_linear_fp16_weight, fbgemm_linear_fp16_weight_fp32_activation, fbgemm_linear_int8_weight, fbgemm_linear_int8_weight_fp32_activation, fbgemm_linear_quantize_weight, fbgemm_pack_gemm_matrix_fp16, fbgemm_pack_quantized_matrix, feature_alpha_dropout, feature_alpha_dropout_, feature_dropout, feature_dropout_, fft, fill, fill_, finfo, fix, fix_, flatten, flip, fliplr, flipud, float, float16, float32, float64, float_power, floor, floor_, floor_divide, fmax, fmin, fmod, fork, frac, frac_, frexp, frobenius_norm, from_dlpack, from_file, from_numpy, frombuffer, functional, fused_moving_avg_obs_fake_quant, futures, fx, gather, gcd, gcd_, ge, geqrf, ger, get_autocast_cpu_dtype, get_autocast_gpu_dtype, get_autocast_ipu_dtype, get_autocast_xla_dtype, get_default_dtype, get_deterministic_debug_mode, get_file_path, get_float32_matmul_precision, get_num_interop_threads, get_num_threads, get_rng_state, gradient, greater, greater_equal, grid_sampler, grid_sampler_2d, grid_sampler_3d, group_norm, gru, gru_cell, gt, half, hamming_window, hann_window, hardshrink, has_lapack, has_mkl, has_openmp, has_spectral, heaviside, hinge_embedding_loss, histc, histogram, histogramdd, hsmm, hsplit, hspmm, hstack, hub, hypot, i0, i0_, igamma, igammac, iinfo, imag, import_ir_module, import_ir_module_from_buffer, index_add, index_copy, index_fill, index_put, index_put_, index_reduce, index_select, indices_copy, inf, inference_mode, init_num_threads, initial_seed, inner, inspect, instance_norm, int, int16, int32, int64, int8, int_repr, inverse, is_anomaly_check_nan_enabled, is_anomaly_enabled, is_autocast_cache_enabled, is_autocast_cpu_enabled, is_autocast_enabled, is_autocast_ipu_enabled, is_autocast_xla_enabled, is_complex, is_conj, is_deterministic_algorithms_warn_only_enabled, is_distributed, is_floating_point, is_grad_enabled, is_inference, is_inference_mode_enabled, is_neg, is_nonzero, is_same_size, is_signed, is_storage, is_tensor, is_vulkan_available, is_warn_always_enabled, isclose, isfinite, isin, isinf, isnan, isneginf, isposinf, isreal, istft, jit, kaiser_window, kl_div, kron, kthvalue, layer_norm, layout, lcm, lcm_, ldexp, ldexp_, le, legacy_contiguous_format, lerp, less, less_equal, lgamma, library, linalg, linspace, load, lobpcg, log, log10, log10_, log1p, log1p_, log2, log2_, log_, log_softmax, logaddexp, logaddexp2, logcumsumexp, logdet, logical_and, logical_not, logical_or, logical_xor, logit, logit_, logspace, logsumexp, long, lstm, lstm_cell, lstsq, lt, lu, lu_solve, lu_unpack, manual_seed, margin_ranking_loss, masked, masked_fill, masked_scatter, masked_select, math, matmul, matrix_exp, matrix_power, matrix_rank, max, max_pool1d, max_pool1d_with_indices, max_pool2d, max_pool3d, maximum, mean, median, memory_format, merge_type_from_type_comment, meshgrid, min, minimum, miopen_batch_norm, miopen_convolution, miopen_convolution_add_relu, miopen_convolution_relu, miopen_convolution_transpose, miopen_depthwise_convolution, miopen_rnn, mkldnn_adaptive_avg_pool2d, mkldnn_convolution, mkldnn_linear_backward_weights, mkldnn_max_pool2d, mkldnn_max_pool3d, mkldnn_rnn_layer, mm, mode, moveaxis, movedim, mps, msort, mul, multinomial, multiply, multiprocessing, mv, mvlgamma, name, nan, nan_to_num, nan_to_num_, nanmean, nanmedian, nanquantile, nansum, narrow, narrow_copy, native_batch_norm, native_channel_shuffle, native_dropout, native_group_norm, native_layer_norm, native_norm, ne, neg, neg_, negative, negative_, nested, nextafter, nn, no_grad, nonzero, nonzero_static, norm, norm_except_dim, normal, not_equal, nuclear_norm, numel, obj, onnx, ops, optim, orgqr, ormqr, os, outer, overrides, package, pairwise_distance, parse_ir, parse_schema, parse_type_comment, pca_lowrank, pdist, per_channel_affine, per_channel_affine_float_qparams, per_channel_symmetric, per_tensor_affine, per_tensor_symmetric, permute, permute_copy, pi, pinverse, pixel_shuffle, pixel_unshuffle, platform, poisson, poisson_nll_loss, polar, polygamma, positive, pow, prelu, prepare_multiprocessing_environment, preserve_format, prod, profiler, promote_types, put, py_float, py_int, q_per_channel_axis, q_per_channel_scales, q_per_channel_zero_points, q_scale, q_zero_point, qint32, qint8, qr, qscheme, quantile, quantization, quantize_per_channel, quantize_per_tensor, quantize_per_tensor_dynamic, quantized_batch_norm, quantized_gru, quantized_gru_cell, quantized_lstm, quantized_lstm_cell, quantized_max_pool1d, quantized_max_pool2d, quantized_max_pool3d, quantized_rnn_relu_cell, quantized_rnn_tanh_cell, quasirandom, quint2x4, quint4x2, quint8, rad2deg, rad2deg_, random, randperm, range, ravel, read_vitals, real, reciprocal, reciprocal_, relu, relu_, remainder, renorm, repeat_interleave, reshape, resize_as_, resize_as_sparse_, resolve_conj, resolve_neg, result_type, return_types, rnn_relu, rnn_relu_cell, rnn_tanh, rnn_tanh_cell, roll, rot90, round, round_, row_indices_copy, row_stack, rrelu, rrelu_, rsqrt, rsqrt_, rsub, saddmm, save, scalar_tensor, scatter, scatter_add, scatter_reduce, searchsorted, seed, segment_reduce, select, select_copy, select_scatter, selu, selu_, serialization, set_anomaly_enabled, set_autocast_cache_enabled, set_autocast_cpu_dtype, set_autocast_cpu_enabled, set_autocast_enabled, set_autocast_gpu_dtype, set_autocast_ipu_dtype, set_autocast_ipu_enabled, set_autocast_xla_dtype, set_autocast_xla_enabled, set_default_device, set_default_dtype, set_default_tensor_type, set_deterministic_debug_mode, set_float32_matmul_precision, set_flush_denormal, set_grad_enabled, set_num_interop_threads, set_num_threads, set_printoptions, set_rng_state, set_vital, set_warn_always, sgn, short, sigmoid, sigmoid_, sign, signal, signbit, sin, sin_, sinc, sinc_, sinh, sinh_, slice_copy, slice_scatter, slogdet, smm, softmax, solve, sort, sparse, sparse_bsc, sparse_bsc_tensor, sparse_bsr, sparse_bsr_tensor, sparse_compressed_tensor, sparse_coo, sparse_coo_tensor, sparse_csc, sparse_csc_tensor, sparse_csr, sparse_csr_tensor, special, split, split_copy, split_with_sizes, split_with_sizes_copy, spmm, sqrt, sqrt_, square, square_, squeeze_copy, sspaddmm, std, std_mean, stft, storage, strided, sub, subtract, sum, svd, svd_lowrank, swapaxes, swapdims, sym_constrain_range, sym_float, sym_int, sym_max, sym_min, sym_not, symeig, t_copy, take, take_along_dim, tan, tan_, tanh, tanh_, tensor_split, tensordot, testing, textwrap, threshold, threshold_, tile, to_dlpack, topk, torch_version, transpose, transpose_copy, trapezoid, trapz, triangular_solve, tril, tril_indices, triplet_margin_loss, triu, triu_indices, true_divide, trunc, trunc_, types, uint8, unbind, unbind_copy, unflatten, unfold_copy, unify_type_list, unique, unique_consecutive, unsafe_chunk, unsafe_split, unsafe_split_with_sizes, unsqueeze_copy, use_deterministic_algorithms, utils, values_copy, vander, var, var_mean, vdot, version, view_as_complex, view_as_complex_copy, view_as_real, view_as_real_copy, view_copy, vitals_enabled, vmap, vsplit, vstack, wait, where, windows, xlogy, xlogy_, zero_ #**
 from . import nn
 
 import math
 e = tensor(math.e)
 nan = tensor(math.nan)
 inf = tensor(math.inf)
 pi = tensor(math.pi)
```

### Comparing `batorch-1.0.38/batorch/device.py` & `batorch-1.0.39/batorch/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,30 @@
     package = "batorch",
     fileinfo = "The inherited tensor from 'torch' with batch.",
     requires = ["pycamia", "torch", "pynvml"]
 )
 
 __all__ = """
     CPU
-    GPU
-    GPUs
     AutoDevice
     FixedDevice
     free_memory_amount
     all_memory_amount
 """.split()
 
-GPU_priority = ['cuda', 'mps']
-
 import os, torch
 with __info__:
     import pynvml, psutil
     from pycamia import alias, ByteSize
 
+GPU_priority = ['cuda', 'mps']
+is_available = dict(
+    cuda = torch.cuda.is_available(),
+    mps = torch.backends.mps.is_available(),
+)
 GB = 1.074e+9
 warning_free_memory_threshold = eval(os.environ.get('CUDA_RUN_MEMORY', '5')) # Run with at lease *GB
 
 free_memory_amount = None
 all_memory_amount = None
 
 @alias("free_memory_amount", amount="free")
@@ -95,15 +96,15 @@
     @property
     def working_memory(self):
         return ByteSize(free_memory_amount(self.main_device_id))
 
     def auto_select(self):
         self.auto = False
         for gpu_family in GPU_priority:
-            if gpu_family == 'cuda' and torch.cuda.is_available():
+            if gpu_family == 'cuda' and is_available['cuda']:
                 self.available_gpu_ids = list(range(torch.cuda.device_count()))
                 available_gpus_memory = [free_memory_amount(i) for i in self.available_gpu_ids]
 
                 threshold = warning_free_memory_threshold if self.required_memory is None else self.required_memory / self.required_devices / 2
                 sorted_memory = sorted(enumerate(available_gpus_memory), key=lambda x: -x[1])
                 candidates = [(i, m) for i, m in sorted_memory if m > threshold * GB][:self.required_devices]
                 if len(candidates) > 0: most_available_gpus, most_available_gpu_memory = zip(*candidates)
@@ -125,15 +126,15 @@
                     print(f"Total free memory: {sum(most_available_gpu_memory) / GB:.5} GB. ")
                     if not self.always_proceed:
                         tag = input("Do you want to proceed? [yes/no/y/n]:")
                         if 'y' not in tag.lower(): raise RuntimeError("Not enough free devices left.")
                 if self.verbose: print(f"Setting working devices: {most_available_gpus}, main device: {most_available_gpus[0]}. proceeding...")
                 self._working_devices = [f"cuda:{i}" for i in most_available_gpus]
                 break
-            elif gpu_family == 'mps' and torch.backends.mps.is_available():
+            elif gpu_family == 'mps' and is_available['mps']:
                 self._working_devices = ['mps']
                 self.required_devices = 1
                 break
         else:
             if self.verbose: print("Warning: cannot find any gpu, using cpu instead. ")
             self._working_devices = ['cpu']
             self.required_devices = 1
@@ -168,10 +169,14 @@
         return x
     
 class FixedDevice(AutoDevice):
     def __init__(self, *devices, required_devices=1, auto=False, required_memory=None, verbose=False):
         super().__init__(*devices, required_devices=required_devices, auto=auto, required_memory=required_memory, verbose=verbose) 
 
 CPU = FixedDevice(torch.device("cpu"))
-mps = FixedDevice(torch.device("mps"))
-GPU = FixedDevice(torch.device("cuda:0"))
-GPUs = [FixedDevice(torch.device(f"cuda:{i}")) for i in range(torch.cuda.device_count())]
+if is_available['mps']:
+    __all__.append('MPS')
+    MPS = FixedDevice(torch.device("mps"))
+if is_available['cuda']:
+    __all__.append('GPU', 'GPUs')
+    GPU = FixedDevice(torch.device("cuda:0"))
+    GPUs = [FixedDevice(torch.device(f"cuda:{i}")) for i in range(torch.cuda.device_count())]
```

### Comparing `batorch-1.0.38/batorch/nn/_reduction.py` & `batorch-1.0.39/batorch/nn/_reduction.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/common_types.py` & `batorch-1.0.39/batorch/nn/common_types.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/functional.py` & `batorch-1.0.39/batorch/nn/functional.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/grad.py` & `batorch-1.0.39/batorch/nn/grad.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/init.py` & `batorch-1.0.39/batorch/nn/init.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/__init__.py` & `batorch-1.0.39/batorch/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/_functions.py` & `batorch-1.0.39/batorch/nn/modules/_functions.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/activation.py` & `batorch-1.0.39/batorch/nn/modules/activation.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/adaptive.py` & `batorch-1.0.39/batorch/nn/modules/adaptive.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/batchnorm.py` & `batorch-1.0.39/batorch/nn/modules/batchnorm.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/container.py` & `batorch-1.0.39/batorch/nn/modules/container.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/conv.py` & `batorch-1.0.39/batorch/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/distance.py` & `batorch-1.0.39/batorch/nn/modules/distance.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/dropout.py` & `batorch-1.0.39/batorch/nn/modules/dropout.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/flatten.py` & `batorch-1.0.39/batorch/nn/modules/flatten.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/fold.py` & `batorch-1.0.39/batorch/nn/modules/fold.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/instancenorm.py` & `batorch-1.0.39/batorch/nn/modules/instancenorm.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/linear.py` & `batorch-1.0.39/batorch/nn/modules/linear.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/loss.py` & `batorch-1.0.39/batorch/nn/modules/loss.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/module.py` & `batorch-1.0.39/batorch/nn/modules/module.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/normalization.py` & `batorch-1.0.39/batorch/nn/modules/normalization.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/padding.py` & `batorch-1.0.39/batorch/nn/modules/padding.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/pixelshuffle.py` & `batorch-1.0.39/batorch/nn/modules/pixelshuffle.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/pooling.py` & `batorch-1.0.39/batorch/nn/modules/pooling.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/rnn.py` & `batorch-1.0.39/batorch/nn/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/sparse.py` & `batorch-1.0.39/batorch/nn/modules/sparse.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/transformer.py` & `batorch-1.0.39/batorch/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/upsampling.py` & `batorch-1.0.39/batorch/nn/modules/upsampling.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/modules/utils.py` & `batorch-1.0.39/batorch/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/parameter.py` & `batorch-1.0.39/batorch/nn/parameter.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/utils/clip_grad.py` & `batorch-1.0.39/batorch/nn/utils/clip_grad.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/utils/convert_parameters.py` & `batorch-1.0.39/batorch/nn/utils/convert_parameters.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/utils/fusion.py` & `batorch-1.0.39/batorch/nn/utils/fusion.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/utils/memory_format.py` & `batorch-1.0.39/batorch/nn/utils/memory_format.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/utils/prune.py` & `batorch-1.0.39/batorch/nn/utils/prune.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/utils/rnn.py` & `batorch-1.0.39/batorch/nn/utils/rnn.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/utils/spectral_norm.py` & `batorch-1.0.39/batorch/nn/utils/spectral_norm.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/nn/utils/weight_norm.py` & `batorch-1.0.39/batorch/nn/utils/weight_norm.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/optimizer.py` & `batorch-1.0.39/batorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/tensor.py` & `batorch-1.0.39/batorch/tensor.py`

 * *Files identical despite different names*

```diff
@@ -6,16 +6,14 @@
     package = "batorch",
     fileinfo = "The inherited tensor from 'torch' with batch.",
     requires = "torch"
 )
 
 __all__ = """
     CPU
-    GPU
-    GPUs
     Tensor
     Size
     set_device
     get_device
     to_device
     turn_on_autodevice
     turn_off_autodevice
@@ -26,15 +24,15 @@
     batch_tensor
     channel_tensor
 """.split()
 
 import builtins, sys
 from functools import wraps
 from typing import Generator
-from .device import GB, CPU, GPU, GPUs, AutoDevice, FixedDevice
+from .device import GB, CPU, AutoDevice, FixedDevice
 
 with __info__:
     import torch
     from pycamia import ByteSize
     from pycamia import avouch, alias, execblock
     from pycamia import get_alphas, arg_tuple, max_argmax
     from pycamia import argmax as _argmax, item, to_list
```

### Comparing `batorch-1.0.38/batorch/tensor2.py` & `batorch-1.0.39/batorch/tensor2.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/tensorfunc.py` & `batorch-1.0.39/batorch/tensorfunc.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/torch_namespace.py` & `batorch-1.0.39/batorch/torch_namespace.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch/torchext.py` & `batorch-1.0.39/batorch/torchext.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.38/batorch.egg-info/PKG-INFO` & `batorch-1.0.39/batorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batorch
-Version: 1.0.38
+Version: 1.0.39
 Summary: 'batorch' is an extension of package torch, for tensors with batch dimensions. 
 Home-page: https://github.com/Bertie97/PyZMyc/batorch
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # batorch
```

### Comparing `batorch-1.0.38/setup_batorch.py` & `batorch-1.0.39/setup_batorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'batorch',
-	version = '1.0.38',
+	version = '1.0.39',
 	keywords = ['pip', 'pymyc', 'batorch', 'torch', 'batch', 'batched data'],
 	description = "'batorch' is an extension of package torch, for tensors with batch dimensions. ",
 	long_description = '# batorch\n\n## Introduction\n\n[batorch](https://github.com/Bertie97/pyctlib/tree/main/batorch) is a package affiliated to project [`PyCAMIA`](https://github.com/Bertie97/pycamia). We encapsulated a new type on top of `torch` tensers, which we call it `batorch.Tensor`. It has the same function as `torch.Tensor`, but it can automatically select the device it was on and provide batch or channel dimensions. Also, we try to provide more useful module for torch users to make deep learning to be implemented more easily. It relies `python v3.6+` with `torch v 1.7.0+`. ***Note that `torch v1.7.0` was released in 2020,*** *and it is necessary for this package as the inheritance behavior for this version is different from previous versions.* Most original `torch` functions should be able to be applied for `batorch` tensors. \n\n> Special features for `batorch` are still under development. If unknown errors pop our, please use traditional `torch` code to bypass it and meanwhile it would be very kind of you to let us know if anything is needed: please contact us by [e-mail](https://github.com/Bertie97/pycamia#Contributors). \n\n```python\n>>> import batorch as bt\n>>> import batorch.nn as nn\n>>> bt.turn_off_autodevice()\n>>> bt.manual_seed(0)\n<torch._C.Generator object at 0x1071b6730>\n>>> t = bt.randn([3000], 400, requires_grad=True)\n>>> LP = nn.Linear(400, 400)\n>>> a = LP(t)\n>>> a.sum().sum().backward()\n>>> print(t.grad)\nTensor([[-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702],\n        [-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702],\n        [-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702],\n        ...,\n        [-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702],\n        [-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702],\n        [-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702]], shape=batorch.Size([3000], 400))\n```\n\n`batorch` has all of following appealing features:\n\n1. **Auto assign** the tensors to available `GPU` **device** by default. \n2. Use `[nbatch]` or `{nchannel}` to specify **the batch and channel dimensions**. i.e. `tp.rand([4], {2}, 20, 30)` returns a 2-channel feature tensor of $20\\times30$ matrices with batch size 4. One may also use `tensor.batch_dimension` to access (or assign) batch dimension, channel dimension can be operated likewise. If you find it hard to remember the symbol, just remember brackets enclose paralleled items in matrices hence it represents the batch dimension for paralleled calculation; braces enclose equation systems which are highly related hence it represents the channel (or feature) dimension. \n3. Batch and channel dimension can help **auto matching the sizes** of two tensors in operations. For example, tensors of sizes `(3, [2], 4)` and `(3, 4)` can be automatically added together with axis of size 3 and 4 matched together. Some methods will also use this information. Sampling, for example, will take the batch dimension as priority.\n4. The tensor object is **compatible with original `torch` functions**. \n\n## Installation\n\nThis package can be installed by `pip install batorch` or moving the source code to the directory of python libraries (the source code can be downloaded on [github](https://github.com/Bertie97/pycamia) or [PyPI](https://pypi.org/project/batorch/)). \n\n```shell\npip install batorch\n```\n\n## Usages\n\nNot available yet, one may check the codes for usages.\n\n## Acknowledgment\n\n@ Yuncheng Zhou: Developer\n@ Yiteng Zhang: Important functions extraction',
 	long_description_content_type = 'text/markdown',
 	license = 'MIT Licence',
 	url = 'https://github.com/Bertie97/PyZMyc/batorch',
 	author = 'Yuncheng Zhou',
```

