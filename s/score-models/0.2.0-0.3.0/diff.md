# Comparing `tmp/score_models-0.2.0.tar.gz` & `tmp/score_models-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "score_models-0.2.0.tar", last modified: Thu Jul  6 06:30:46 2023, max compression
+gzip compressed data, was "score_models-0.3.0.tar", last modified: Thu Jul  6 14:09:29 2023, max compression
```

## Comparing `score_models-0.2.0.tar` & `score_models-0.3.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 06:30:46.695724 score_models-0.2.0/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      469 2023-07-06 06:30:46.695724 score_models-0.2.0/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5340 2023-07-06 06:22:09.000000 score_models-0.2.0/README.md
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       90 2023-07-05 04:03:53.000000 score_models-0.2.0/pyproject.toml
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 06:30:46.691724 score_models-0.2.0/score_models/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       94 2023-07-05 03:25:19.000000 score_models-0.2.0/score_models/__init__.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 06:30:46.691724 score_models-0.2.0/score_models/architectures/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-05 02:17:22.000000 score_models-0.2.0/score_models/architectures/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4923 2023-07-05 02:18:21.000000 score_models-0.2.0/score_models/architectures/ddpm.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3557 2023-07-06 06:27:36.000000 score_models-0.2.0/score_models/architectures/mlp.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    15113 2023-07-05 02:18:28.000000 score_models-0.2.0/score_models/architectures/ncsnpp.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    16600 2023-07-06 05:33:05.000000 score_models-0.2.0/score_models/base.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2035 2023-07-04 14:03:48.000000 score_models-0.2.0/score_models/definitions.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 06:30:46.695724 score_models-0.2.0/score_models/layers/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      686 2023-07-06 00:14:06.000000 score_models-0.2.0/score_models/layers/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3574 2023-07-06 00:26:11.000000 score_models-0.2.0/score_models/layers/attention_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      601 2023-07-04 06:17:32.000000 score_models-0.2.0/score_models/layers/combine.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2766 2023-03-05 17:43:23.000000 score_models-0.2.0/score_models/layers/conditional_batchnorm2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2279 2023-03-05 17:43:23.000000 score_models-0.2.0/score_models/layers/conditional_instancenorm2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2980 2023-03-05 17:43:23.000000 score_models-0.2.0/score_models/layers/conditional_instancenorm2d_plus.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2903 2023-03-05 17:43:23.000000 score_models-0.2.0/score_models/layers/conv1dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3120 2023-03-05 17:43:23.000000 score_models-0.2.0/score_models/layers/conv2dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3134 2023-07-04 04:38:49.000000 score_models-0.2.0/score_models/layers/conv3dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1111 2023-07-04 06:17:50.000000 score_models-0.2.0/score_models/layers/conv_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3354 2023-07-04 06:58:10.000000 score_models-0.2.0/score_models/layers/ddpm_resnet_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1950 2023-07-04 06:11:52.000000 score_models-0.2.0/score_models/layers/downsample.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3543 2023-03-05 17:43:23.000000 score_models-0.2.0/score_models/layers/ncsn_resnet_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      611 2023-03-05 17:43:23.000000 score_models-0.2.0/score_models/layers/projection_embedding.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3232 2023-07-04 06:42:28.000000 score_models-0.2.0/score_models/layers/resnet_block_biggan.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2447 2023-03-05 17:43:23.000000 score_models-0.2.0/score_models/layers/spectral_normalization.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      862 2023-03-05 17:43:23.000000 score_models-0.2.0/score_models/layers/squeeze_and_excitation.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2123 2023-07-04 03:51:29.000000 score_models-0.2.0/score_models/layers/style_gan_conv.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1957 2023-07-04 06:50:45.000000 score_models-0.2.0/score_models/layers/up_or_downsampling.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6493 2023-07-04 04:15:34.000000 score_models-0.2.0/score_models/layers/up_or_downsampling1d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7626 2023-07-04 04:18:13.000000 score_models-0.2.0/score_models/layers/up_or_downsampling2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7507 2023-07-04 06:39:32.000000 score_models-0.2.0/score_models/layers/up_or_downsampling3d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1485 2023-07-03 16:51:47.000000 score_models-0.2.0/score_models/layers/upfirdn1d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1720 2023-07-03 16:51:47.000000 score_models-0.2.0/score_models/layers/upfirdn2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2053 2023-07-03 16:51:47.000000 score_models-0.2.0/score_models/layers/upfirdn3d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1558 2023-07-04 06:02:46.000000 score_models-0.2.0/score_models/layers/upsample.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1590 2023-07-06 05:13:46.000000 score_models-0.2.0/score_models/score_model.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 06:30:46.695724 score_models-0.2.0/score_models/sde/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-04 05:26:17.000000 score_models-0.2.0/score_models/sde/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1268 2023-07-05 12:48:17.000000 score_models-0.2.0/score_models/sde/sde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1653 2023-07-05 12:48:37.000000 score_models-0.2.0/score_models/sde/vesde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1504 2023-07-05 12:48:40.000000 score_models-0.2.0/score_models/sde/vpsde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3672 2023-07-06 05:44:37.000000 score_models-0.2.0/score_models/utils.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 06:30:46.691724 score_models-0.2.0/score_models.egg-info/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      469 2023-07-06 06:30:46.000000 score_models-0.2.0/score_models.egg-info/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1715 2023-07-06 06:30:46.000000 score_models-0.2.0/score_models.egg-info/SOURCES.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-07-06 06:30:46.000000 score_models-0.2.0/score_models.egg-info/dependency_links.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       43 2023-07-06 06:30:46.000000 score_models-0.2.0/score_models.egg-info/requires.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       13 2023-07-06 06:30:46.000000 score_models-0.2.0/score_models.egg-info/top_level.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-07-06 06:30:46.695724 score_models-0.2.0/setup.cfg
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      722 2023-07-06 02:19:07.000000 score_models-0.2.0/setup.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 06:30:46.695724 score_models-0.2.0/tests/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1231 2023-07-06 01:58:54.000000 score_models-0.2.0/tests/test_architectures.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6839 2023-07-06 00:26:26.000000 score_models-0.2.0/tests/test_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1384 2023-07-06 03:48:36.000000 score_models-0.2.0/tests/test_loading_score.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3090 2023-07-06 04:00:33.000000 score_models-0.2.0/tests/test_training.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 14:09:29.392583 score_models-0.3.0/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6213 2023-07-06 14:09:29.392583 score_models-0.3.0/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5325 2023-07-06 13:52:29.000000 score_models-0.3.0/README.md
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       90 2023-07-06 13:52:30.000000 score_models-0.3.0/pyproject.toml
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 14:09:29.388583 score_models-0.3.0/score_models/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       94 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/__init__.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 14:09:29.392583 score_models-0.3.0/score_models/architectures/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/architectures/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4923 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/architectures/ddpm.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3557 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/architectures/mlp.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    15113 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/architectures/ncsnpp.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    16600 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/base.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2035 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/definitions.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 14:09:29.392583 score_models-0.3.0/score_models/layers/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      686 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3574 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/attention_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      601 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/combine.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2766 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/conditional_batchnorm2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2279 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/conditional_instancenorm2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2980 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/conditional_instancenorm2d_plus.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2903 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/conv1dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3120 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/conv2dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3134 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/conv3dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1111 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/conv_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3354 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/ddpm_resnet_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1950 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/downsample.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3543 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/ncsn_resnet_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      611 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/projection_embedding.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3232 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/resnet_block_biggan.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2447 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/spectral_normalization.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      862 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/squeeze_and_excitation.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2123 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/style_gan_conv.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1957 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/up_or_downsampling.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6493 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/up_or_downsampling1d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7626 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/up_or_downsampling2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7507 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/up_or_downsampling3d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1485 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/upfirdn1d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1720 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/upfirdn2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2053 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/upfirdn3d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1558 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/upsample.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1590 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/score_model.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 14:09:29.392583 score_models-0.3.0/score_models/sde/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/sde/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1268 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/sde/sde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1653 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/sde/vesde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1504 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/sde/vpsde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3672 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/utils.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 14:09:29.388583 score_models-0.3.0/score_models.egg-info/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6213 2023-07-06 14:09:29.000000 score_models-0.3.0/score_models.egg-info/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1715 2023-07-06 14:09:29.000000 score_models-0.3.0/score_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-07-06 14:09:29.000000 score_models-0.3.0/score_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       43 2023-07-06 14:09:29.000000 score_models-0.3.0/score_models.egg-info/requires.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       13 2023-07-06 14:09:29.000000 score_models-0.3.0/score_models.egg-info/top_level.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-07-06 14:09:29.392583 score_models-0.3.0/setup.cfg
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      880 2023-07-06 14:07:37.000000 score_models-0.3.0/setup.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 14:09:29.392583 score_models-0.3.0/tests/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1231 2023-07-06 13:52:30.000000 score_models-0.3.0/tests/test_architectures.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6839 2023-07-06 13:52:30.000000 score_models-0.3.0/tests/test_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1384 2023-07-06 13:52:30.000000 score_models-0.3.0/tests/test_loading_score.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3090 2023-07-06 13:52:30.000000 score_models-0.3.0/tests/test_training.py
```

### Comparing `score_models-0.2.0/README.md` & `score_models-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Score Models for Pytorch
 
-[![PyPI version](https://badge.fury.io/py/torch_score_models.svg)](https://badge.fury.io/py/torch_score_models)
+[![PyPI version](https://badge.fury.io/py/score_models.svg)](https://badge.fury.io/py/score_models)
 [![codecov](https://codecov.io/gh/AlexandreAdam/torch_score_models/branch/dev/graph/badge.svg)](https://codecov.io/gh/AlexandreAdam/torch_score_models)
 
-0
-
 A storage for score-based models. The `ScoreModel` interface gives access to the following utilities
 - Simple initialisation of MLP, NCSN++ and DDPM neural network architectures
 - A fit method to train the score model on a dataset using Denoising Score Matching (DSM).
 - A sampling method based on an Euler-Maruyama discretisation of an SDE. 
 - A simple interface to train an energy model using DSM
 
 This repository is mainly intended for personal use.
```

### Comparing `score_models-0.2.0/score_models/architectures/ddpm.py` & `score_models-0.3.0/score_models/architectures/ddpm.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/architectures/mlp.py` & `score_models-0.3.0/score_models/architectures/mlp.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/architectures/ncsnpp.py` & `score_models-0.3.0/score_models/architectures/ncsnpp.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/base.py` & `score_models-0.3.0/score_models/base.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/definitions.py` & `score_models-0.3.0/score_models/definitions.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/__init__.py` & `score_models-0.3.0/score_models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/attention_block.py` & `score_models-0.3.0/score_models/layers/attention_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/combine.py` & `score_models-0.3.0/score_models/layers/combine.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/conditional_batchnorm2d.py` & `score_models-0.3.0/score_models/layers/conditional_batchnorm2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/conditional_instancenorm2d.py` & `score_models-0.3.0/score_models/layers/conditional_instancenorm2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/conditional_instancenorm2d_plus.py` & `score_models-0.3.0/score_models/layers/conditional_instancenorm2d_plus.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/conv1dsame.py` & `score_models-0.3.0/score_models/layers/conv1dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/conv2dsame.py` & `score_models-0.3.0/score_models/layers/conv2dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/conv3dsame.py` & `score_models-0.3.0/score_models/layers/conv3dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/conv_layers.py` & `score_models-0.3.0/score_models/layers/conv_layers.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/ddpm_resnet_block.py` & `score_models-0.3.0/score_models/layers/ddpm_resnet_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/downsample.py` & `score_models-0.3.0/score_models/layers/downsample.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/ncsn_resnet_block.py` & `score_models-0.3.0/score_models/layers/ncsn_resnet_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/projection_embedding.py` & `score_models-0.3.0/score_models/layers/projection_embedding.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/resnet_block_biggan.py` & `score_models-0.3.0/score_models/layers/resnet_block_biggan.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/spectral_normalization.py` & `score_models-0.3.0/score_models/layers/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/squeeze_and_excitation.py` & `score_models-0.3.0/score_models/layers/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/style_gan_conv.py` & `score_models-0.3.0/score_models/layers/style_gan_conv.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/up_or_downsampling.py` & `score_models-0.3.0/score_models/layers/up_or_downsampling.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/up_or_downsampling1d.py` & `score_models-0.3.0/score_models/layers/up_or_downsampling1d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/up_or_downsampling2d.py` & `score_models-0.3.0/score_models/layers/up_or_downsampling2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/up_or_downsampling3d.py` & `score_models-0.3.0/score_models/layers/up_or_downsampling3d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/upfirdn1d.py` & `score_models-0.3.0/score_models/layers/upfirdn1d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/upfirdn2d.py` & `score_models-0.3.0/score_models/layers/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/upfirdn3d.py` & `score_models-0.3.0/score_models/layers/upfirdn3d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/layers/upsample.py` & `score_models-0.3.0/score_models/layers/upsample.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/score_model.py` & `score_models-0.3.0/score_models/score_model.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/sde/sde.py` & `score_models-0.3.0/score_models/sde/sde.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/sde/vesde.py` & `score_models-0.3.0/score_models/sde/vesde.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/sde/vpsde.py` & `score_models-0.3.0/score_models/sde/vpsde.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models/utils.py` & `score_models-0.3.0/score_models/utils.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/score_models.egg-info/SOURCES.txt` & `score_models-0.3.0/score_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/tests/test_architectures.py` & `score_models-0.3.0/tests/test_architectures.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/tests/test_layers.py` & `score_models-0.3.0/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/tests/test_loading_score.py` & `score_models-0.3.0/tests/test_loading_score.py`

 * *Files identical despite different names*

### Comparing `score_models-0.2.0/tests/test_training.py` & `score_models-0.3.0/tests/test_training.py`

 * *Files identical despite different names*

