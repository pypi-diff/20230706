# Comparing `tmp/climate_learn-0.0.2.tar.gz` & `tmp/climate_learn-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climate_learn-0.0.2.tar", last modified: Tue Feb 21 18:52:06 2023, max compression
+gzip compressed data, was "climate_learn-1.0.0.tar", last modified: Thu Jul  6 14:34:24 2023, max compression
```

## Comparing `climate_learn-0.0.2.tar` & `climate_learn-1.0.0.tar`

### file list

```diff
@@ -1,56 +1,103 @@
-drwxr-xr-x   0 jason.jewik (22903) mintgrp  (21000)        0 2023-02-21 18:52:06.890004 climate_learn-0.0.2/
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     1147 2023-01-21 01:39:11.000000 climate_learn-0.0.2/LICENSE
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     4225 2023-02-21 18:52:06.890004 climate_learn-0.0.2/PKG-INFO
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     2488 2023-02-21 18:50:18.000000 climate_learn-0.0.2/README.md
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     2420 2023-02-21 18:49:19.000000 climate_learn-0.0.2/pyproject.toml
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)       38 2023-02-21 18:52:06.890004 climate_learn-0.0.2/setup.cfg
-drwxr-xr-x   0 jason.jewik (22903) mintgrp  (21000)        0 2023-02-21 18:52:06.886004 climate_learn-0.0.2/src/
-drwxr-xr-x   0 jason.jewik (22903) mintgrp  (21000)        0 2023-02-21 18:52:06.886004 climate_learn-0.0.2/src/climate_learn/
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)        0 2023-01-21 01:39:11.000000 climate_learn-0.0.2/src/climate_learn/__init__.py
-drwxr-xr-x   0 jason.jewik (22903) mintgrp  (21000)        0 2023-02-21 18:52:06.886004 climate_learn-0.0.2/src/climate_learn/data/
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)      132 2023-02-09 18:39:54.000000 climate_learn-0.0.2/src/climate_learn/data/__init__.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     1856 2023-02-09 18:39:54.000000 climate_learn-0.0.2/src/climate_learn/data/constants.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)    10022 2023-02-03 18:08:12.000000 climate_learn-0.0.2/src/climate_learn/data/download.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     7215 2023-02-21 18:06:40.000000 climate_learn-0.0.2/src/climate_learn/data/itermodule.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     6952 2023-02-21 18:06:40.000000 climate_learn-0.0.2/src/climate_learn/data/module.py
-drwxr-xr-x   0 jason.jewik (22903) mintgrp  (21000)        0 2023-02-21 18:52:06.890004 climate_learn-0.0.2/src/climate_learn/data/modules/
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)       59 2023-02-09 18:39:54.000000 climate_learn-0.0.2/src/climate_learn/data/modules/__init__.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     6044 2023-02-21 18:06:40.000000 climate_learn-0.0.2/src/climate_learn/data/modules/era5_iterdataset.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)    10697 2023-02-14 18:43:51.000000 climate_learn-0.0.2/src/climate_learn/data/modules/era5_module.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     7459 2023-02-09 18:39:54.000000 climate_learn-0.0.2/src/climate_learn/data/nc2npz.py
-drwxr-xr-x   0 jason.jewik (22903) mintgrp  (21000)        0 2023-02-21 18:52:06.890004 climate_learn-0.0.2/src/climate_learn/models/
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     1405 2023-01-21 01:39:11.000000 climate_learn-0.0.2/src/climate_learn/models/__init__.py
-drwxr-xr-x   0 jason.jewik (22903) mintgrp  (21000)        0 2023-02-21 18:52:06.890004 climate_learn-0.0.2/src/climate_learn/models/components/
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)       85 2023-01-21 01:39:11.000000 climate_learn-0.0.2/src/climate_learn/models/components/__init__.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     9477 2023-02-14 18:43:51.000000 climate_learn-0.0.2/src/climate_learn/models/components/cnn_blocks.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     1772 2023-02-21 18:06:40.000000 climate_learn-0.0.2/src/climate_learn/models/components/linear.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     2982 2023-02-21 18:06:40.000000 climate_learn-0.0.2/src/climate_learn/models/components/resnet.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     5879 2023-02-21 18:06:40.000000 climate_learn-0.0.2/src/climate_learn/models/components/unet.py
-drwxr-xr-x   0 jason.jewik (22903) mintgrp  (21000)        0 2023-02-21 18:52:06.890004 climate_learn-0.0.2/src/climate_learn/models/components/utils/
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)        0 2023-01-21 01:39:11.000000 climate_learn-0.0.2/src/climate_learn/models/components/utils/__init__.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     4198 2023-02-09 18:39:54.000000 climate_learn-0.0.2/src/climate_learn/models/components/utils/pos_embed.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     6867 2023-02-21 18:06:40.000000 climate_learn-0.0.2/src/climate_learn/models/components/vit.py
-drwxr-xr-x   0 jason.jewik (22903) mintgrp  (21000)        0 2023-02-21 18:52:06.890004 climate_learn-0.0.2/src/climate_learn/models/modules/
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)      118 2023-01-21 01:39:11.000000 climate_learn-0.0.2/src/climate_learn/models/modules/__init__.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     4814 2023-02-21 18:06:40.000000 climate_learn-0.0.2/src/climate_learn/models/modules/downscale.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     7959 2023-02-21 18:06:40.000000 climate_learn-0.0.2/src/climate_learn/models/modules/forecast.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     4291 2023-02-21 18:06:40.000000 climate_learn-0.0.2/src/climate_learn/models/modules/linear.py
-drwxr-xr-x   0 jason.jewik (22903) mintgrp  (21000)        0 2023-02-21 18:52:06.890004 climate_learn-0.0.2/src/climate_learn/models/modules/utils/
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)        0 2023-01-21 01:39:11.000000 climate_learn-0.0.2/src/climate_learn/models/modules/utils/__init__.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     4090 2023-02-21 18:06:40.000000 climate_learn-0.0.2/src/climate_learn/models/modules/utils/lr_scheduler.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     6178 2023-02-21 18:06:40.000000 climate_learn-0.0.2/src/climate_learn/models/modules/utils/metrics.py
-drwxr-xr-x   0 jason.jewik (22903) mintgrp  (21000)        0 2023-02-21 18:52:06.890004 climate_learn-0.0.2/src/climate_learn/training/
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)       44 2023-01-21 01:39:11.000000 climate_learn-0.0.2/src/climate_learn/training/__init__.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)      289 2023-02-21 18:06:40.000000 climate_learn-0.0.2/src/climate_learn/training/loggers.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     2092 2023-02-21 18:06:40.000000 climate_learn-0.0.2/src/climate_learn/training/train.py
-drwxr-xr-x   0 jason.jewik (22903) mintgrp  (21000)        0 2023-02-21 18:52:06.890004 climate_learn-0.0.2/src/climate_learn/utils/
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)       25 2023-01-21 01:39:11.000000 climate_learn-0.0.2/src/climate_learn/utils/__init__.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)      574 2023-01-31 17:51:41.000000 climate_learn-0.0.2/src/climate_learn/utils/data.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     1240 2023-01-21 01:39:11.000000 climate_learn-0.0.2/src/climate_learn/utils/datetime.py
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     5226 2023-02-21 18:06:51.000000 climate_learn-0.0.2/src/climate_learn/utils/visualize.py
-drwxr-xr-x   0 jason.jewik (22903) mintgrp  (21000)        0 2023-02-21 18:52:06.886004 climate_learn-0.0.2/src/climate_learn.egg-info/
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     4225 2023-02-21 18:52:06.000000 climate_learn-0.0.2/src/climate_learn.egg-info/PKG-INFO
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)     1627 2023-02-21 18:52:06.000000 climate_learn-0.0.2/src/climate_learn.egg-info/SOURCES.txt
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)        1 2023-02-21 18:52:06.000000 climate_learn-0.0.2/src/climate_learn.egg-info/dependency_links.txt
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)      316 2023-02-21 18:52:06.000000 climate_learn-0.0.2/src/climate_learn.egg-info/requires.txt
--rw-r--r--   0 jason.jewik (22903) mintgrp  (21000)       14 2023-02-21 18:52:06.000000 climate_learn-0.0.2/src/climate_learn.egg-info/top_level.txt
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.946820 climate_learn-1.0.0/
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1098 2023-07-06 14:33:52.000000 climate_learn-1.0.0/LICENSE
+-rw-rw-r--   0 jason     (1000) jason     (1000)     4222 2023-07-06 14:34:24.946820 climate_learn-1.0.0/PKG-INFO
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2659 2023-06-29 14:33:48.000000 climate_learn-1.0.0/README.md
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2245 2023-07-06 14:28:46.000000 climate_learn-1.0.0/pyproject.toml
+-rw-rw-r--   0 jason     (1000) jason     (1000)       38 2023-07-06 14:34:24.946820 climate_learn-1.0.0/setup.cfg
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.938820 climate_learn-1.0.0/src/
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.942820 climate_learn-1.0.0/src/climate_learn/
+-rw-rw-r--   0 jason     (1000) jason     (1000)      273 2023-07-03 14:52:59.000000 climate_learn-1.0.0/src/climate_learn/__init__.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.942820 climate_learn-1.0.0/src/climate_learn/data/
+-rw-rw-r--   0 jason     (1000) jason     (1000)      164 2023-06-21 03:40:45.000000 climate_learn-1.0.0/src/climate_learn/data/__init__.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.942820 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/
+-rw-rw-r--   0 jason     (1000) jason     (1000)      232 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/__init__.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.942820 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/args/
+-rw-rw-r--   0 jason     (1000) jason     (1000)      153 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/args/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2542 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/args/climate_dataset_args.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      681 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/args/era5_args.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2016 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/args/stacked_climate_dataset_args.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2333 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/climate_dataset.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.942820 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/cmip6/
+-rw-rw-r--   0 jason     (1000) jason     (1000)      868 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/cmip6/constants.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     7401 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/cmip6_iterdataset.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.942820 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/era5/
+-rw-rw-r--   0 jason     (1000) jason     (1000)       48 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/era5/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1675 2023-06-20 23:02:17.000000 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/era5/constants.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)    11613 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/era5/era5.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     7170 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/era5_continuous_iterdataset.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     7325 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/era5_iterdataset.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     3991 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/climate_dataset/stacked_climate_dataset.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     6715 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/climatebench_dataset.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     5284 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/data/climatebench_module.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.942820 climate_learn-1.0.0/src/climate_learn/data/dataset/
+-rw-rw-r--   0 jason     (1000) jason     (1000)      127 2023-04-13 22:58:31.000000 climate_learn-1.0.0/src/climate_learn/data/dataset/__init__.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.942820 climate_learn-1.0.0/src/climate_learn/data/dataset/args/
+-rw-rw-r--   0 jason     (1000) jason     (1000)       94 2023-04-13 22:58:31.000000 climate_learn-1.0.0/src/climate_learn/data/dataset/args/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1256 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/dataset/args/map_dataset_args.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1633 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/dataset/args/shard_dataset_args.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     7021 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/dataset/map_dataset.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)    14812 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/dataset/shard_dataset.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     6144 2023-07-05 20:40:04.000000 climate_learn-1.0.0/src/climate_learn/data/download.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)    10306 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/data/iterdataset.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)    12103 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/data/itermodule.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     3692 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/data/mapmodule.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     8790 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/module.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1904 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/data/npzdataset.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.942820 climate_learn-1.0.0/src/climate_learn/data/processing/
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2497 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/data/processing/climatebench.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1071 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/data/processing/cmip6_constants.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2326 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/data/processing/era5_constants.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     3027 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/data/processing/era5_cropped.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     7233 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/data/processing/era5_extreme.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     8055 2023-06-21 03:10:29.000000 climate_learn-1.0.0/src/climate_learn/data/processing/nc2npz.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     3622 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/data/processing/prism.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.946820 climate_learn-1.0.0/src/climate_learn/data/task/
+-rw-rw-r--   0 jason     (1000) jason     (1000)      158 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/task/__init__.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.946820 climate_learn-1.0.0/src/climate_learn/data/task/args/
+-rw-rw-r--   0 jason     (1000) jason     (1000)      124 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/task/args/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      611 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/task/args/downscaling_args.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1701 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/task/args/forecasting_args.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1259 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/task/args/task_args.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2503 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/task/downscaling.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     3078 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/task/forecasting.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     4127 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/data/task/task.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.946820 climate_learn-1.0.0/src/climate_learn/metrics/
+-rw-rw-r--   0 jason     (1000) jason     (1000)       96 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/metrics/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     8997 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/metrics/functional.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)    12839 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/metrics/metrics.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      867 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/metrics/utils.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.946820 climate_learn-1.0.0/src/climate_learn/models/
+-rw-rw-r--   0 jason     (1000) jason     (1000)       62 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/models/__init__.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.946820 climate_learn-1.0.0/src/climate_learn/models/hub/
+-rw-rw-r--   0 jason     (1000) jason     (1000)      282 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/models/hub/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      534 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/models/hub/climatology.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.946820 climate_learn-1.0.0/src/climate_learn/models/hub/components/
+-rw-rw-r--   0 jason     (1000) jason     (1000)     9477 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/models/hub/components/cnn_blocks.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     4198 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/models/hub/components/pos_embed.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      396 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/models/hub/interpolation.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      634 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/models/hub/linear_regression.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      699 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/models/hub/persistence.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2076 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/models/hub/resnet.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     4965 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/models/hub/unet.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      166 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/models/hub/utils.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     4043 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/models/hub/vit.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     3997 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/models/lr_scheduler.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     8061 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/models/module.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.946820 climate_learn-1.0.0/src/climate_learn/transforms/
+-rw-rw-r--   0 jason     (1000) jason     (1000)      102 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/transforms/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1014 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/transforms/denormalize.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      451 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/transforms/mask.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      182 2023-06-20 20:56:41.000000 climate_learn-1.0.0/src/climate_learn/transforms/registry.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.946820 climate_learn-1.0.0/src/climate_learn/utils/
+-rw-rw-r--   0 jason     (1000) jason     (1000)      407 2023-07-03 14:53:12.000000 climate_learn-1.0.0/src/climate_learn/utils/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)    17457 2023-07-03 14:50:40.000000 climate_learn-1.0.0/src/climate_learn/utils/loaders.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      574 2023-06-29 14:33:48.000000 climate_learn-1.0.0/src/climate_learn/utils/mc_dropout.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     6363 2023-06-29 14:49:49.000000 climate_learn-1.0.0/src/climate_learn/utils/visualize.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.942820 climate_learn-1.0.0/src/climate_learn.egg-info/
+-rw-rw-r--   0 jason     (1000) jason     (1000)     4222 2023-07-06 14:34:24.000000 climate_learn-1.0.0/src/climate_learn.egg-info/PKG-INFO
+-rw-rw-r--   0 jason     (1000) jason     (1000)     3530 2023-07-06 14:34:24.000000 climate_learn-1.0.0/src/climate_learn.egg-info/SOURCES.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)        1 2023-07-06 14:34:24.000000 climate_learn-1.0.0/src/climate_learn.egg-info/dependency_links.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)      365 2023-07-06 14:34:24.000000 climate_learn-1.0.0/src/climate_learn.egg-info/requires.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)       14 2023-07-06 14:34:24.000000 climate_learn-1.0.0/src/climate_learn.egg-info/top_level.txt
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-07-06 14:34:24.946820 climate_learn-1.0.0/tests/
+-rw-rw-r--   0 jason     (1000) jason     (1000)      485 2023-06-20 20:56:41.000000 climate_learn-1.0.0/tests/test_trainer.py
```

### Comparing `climate_learn-0.0.2/LICENSE` & `climate_learn-1.0.0/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# MIT License
-#
-#@title Copyright (c) 2021 CCAI Community Authors { display-mode: "form" }
-#
-# Permission is hereby granted, free of charge, to any person obtaining a
-# copy of this software and associated documentation files (the "Software"),
-# to deal in the Software without restriction, including without limitation
-# the rights to use, copy, modify, merge, publish, distribute, sublicense,
-# and/or sell copies of the Software, and to permit persons to whom the
-# Software is furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
-# THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-# DEALINGS IN THE SOFTWARE.
+MIT License
+
+Copyright (c) 2021-present Machine Intelligence Group at UCLA
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `climate_learn-0.0.2/PKG-INFO` & `climate_learn-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,62 @@
 Metadata-Version: 2.1
 Name: climate_learn
-Version: 0.0.2
-Summary: ClimateLearn: Benchmarking Machine Learning for Data-driven Climate Science
-Author-email: MINT at UCLA <jason.jewik@cs.ucla.edu>, Hritik Bansal <hbansal@g.ucla.edu>, Shashank Goel <shashankgoel@g.ucla.edu>, Siddharth Nandy <sidd.nandy@gmail.com>, Tung Nguyen <tungnd@g.ucla.edu>, Seongbin Park <shannonsbpark@gmail.com>, Jingchen Tang <tangtang1228@ucla.edu>, Jason Jewik <jason.jewik@cs.ucla.edu>, Aditya Grover <adityag@cs.ucla.edu>
+Version: 1.0.0
+Summary: ClimateLearn: Benchmarking Machine Learning for Weather and Climate Modeling
+Author-email: MINT at UCLA <jason.jewik@ucla.edu>, Tung Nguyen <tungnd@cs.ucla.edu>, Jason Jewik <jason.jewik@ucla.edu>, Hritik Bansal <hbansal@ucla.edu>, Prakhar Sharma <prakhar6sharma@gmail.com>, Aditya Grover <adityag@cs.ucla.edu>
 Project-URL: Source, https://github.com/aditya-grover/climate-learn
 Project-URL: Issue Tracker, https://github.com/aditya-grover/climate-learn/issues
 Project-URL: Documentation, https://climatelearn.readthedocs.io/en/latest/
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 <h1 align="center">ClimateLearn</h1>
 
 [![Documentation Status](https://readthedocs.org/projects/climatelearn/badge/?version=latest)](https://climatelearn.readthedocs.io/en/latest/?badge=latest)
 [![CI Build Status](https://github.com/aditya-grover/climate-learn/actions/workflows/ci.yaml/badge.svg)](https://github.com/aditya-grover/climate-learn/actions/workflows/ci.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WiNEK1BHsiGzo_bT9Fcm8lea2H_ghNfa)
+[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LcecQLgLtwaHOwbvJAxw9UjCxfM0RMrX?usp=sharing)
 
 **ClimateLearn** is a Python library for accessing state-of-the-art climate data and machine learning models in a standardized, straightforward way. This library provides access to multiple datasets, a zoo of baseline approaches, and a suite of metrics and visualizations for large-scale benchmarking of statistical downscaling and temporal forecasting methods. For further context on our past motivation and future plans, check out our announcement [blog post](https://aditya-grover.github.io/blog/2023/climate-learn/).
 
 ## Usage
 
-[**Python3**](https://www.python.org/) is required.
+[**Python 3.8+**](https://www.python.org/) is required. The xESMF package has to be installed separately since one of its dependencies, ESMpy, is available only through Conda.
 ```
+conda install -c conda-forge xesmf
 pip install climate-learn
 ```
 
 ### Quickstart
-Please refer to this [Google Colab](https://colab.research.google.com/drive/1WiNEK1BHsiGzo_bT9Fcm8lea2H_ghNfa) for a tutorial-style exposition into developing your first models for forecasting and downscaling in ClimateLearn.
+We have a quickstart notebook in the `notebooks` folder titled `Quickstart.ipynb`. It is intended for use in Google Colab and can be launched by clicking the Google Colab badge above or this link: https://colab.research.google.com/drive/1LcecQLgLtwaHOwbvJAxw9UjCxfM0RMrX?usp=sharing.
 
-We previewed some key features of ClimateLearn at a spotlight tutorial in the "Tackling Climate Change with Machine Learning" Workshop at the Neural Information Processing Systems 2022 Conference. The slides and recorded talk can be found on [Climate Change AI's website](https://www.climatechange.ai/papers/neurips2022/114). 
+We also previewed some key features of ClimateLearn at a spotlight tutorial in the "Tackling Climate Change with Machine Learning" Workshop at the Neural Information Processing Systems 2022 Conference. The slides and recorded talk can be found on [Climate Change AI's website](https://www.climatechange.ai/papers/neurips2022/114).
 
 ### Documentation
 Find us on [ReadTheDocs](https://climatelearn.readthedocs.io/).
 
-### Integrations
-- [Weights & Biases](https://wandb.ai/site)
-
 ## About Us
 ClimateLearn is managed by the Machine Intelligence Group at UCLA, headed by [Professor Aditya Grover](https://aditya-grover.github.io).
 
 ## Contributing
 Contributions are welcome! See our [contributing guide](https://github.com/aditya-grover/climate-learn/blob/main/CONTRIBUTING.md).
 
 ## Citing ClimateLearn
```

### Comparing `climate_learn-0.0.2/README.md` & `climate_learn-1.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 <h1 align="center">ClimateLearn</h1>
 
 [![Documentation Status](https://readthedocs.org/projects/climatelearn/badge/?version=latest)](https://climatelearn.readthedocs.io/en/latest/?badge=latest)
 [![CI Build Status](https://github.com/aditya-grover/climate-learn/actions/workflows/ci.yaml/badge.svg)](https://github.com/aditya-grover/climate-learn/actions/workflows/ci.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WiNEK1BHsiGzo_bT9Fcm8lea2H_ghNfa)
+[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LcecQLgLtwaHOwbvJAxw9UjCxfM0RMrX?usp=sharing)
 
 **ClimateLearn** is a Python library for accessing state-of-the-art climate data and machine learning models in a standardized, straightforward way. This library provides access to multiple datasets, a zoo of baseline approaches, and a suite of metrics and visualizations for large-scale benchmarking of statistical downscaling and temporal forecasting methods. For further context on our past motivation and future plans, check out our announcement [blog post](https://aditya-grover.github.io/blog/2023/climate-learn/).
 
 ## Usage
 
-[**Python3**](https://www.python.org/) is required.
+[**Python 3.8+**](https://www.python.org/) is required. The xESMF package has to be installed separately since one of its dependencies, ESMpy, is available only through Conda.
 ```
+conda install -c conda-forge xesmf
 pip install climate-learn
 ```
 
 ### Quickstart
-Please refer to this [Google Colab](https://colab.research.google.com/drive/1WiNEK1BHsiGzo_bT9Fcm8lea2H_ghNfa) for a tutorial-style exposition into developing your first models for forecasting and downscaling in ClimateLearn.
+We have a quickstart notebook in the `notebooks` folder titled `Quickstart.ipynb`. It is intended for use in Google Colab and can be launched by clicking the Google Colab badge above or this link: https://colab.research.google.com/drive/1LcecQLgLtwaHOwbvJAxw9UjCxfM0RMrX?usp=sharing.
 
-We previewed some key features of ClimateLearn at a spotlight tutorial in the "Tackling Climate Change with Machine Learning" Workshop at the Neural Information Processing Systems 2022 Conference. The slides and recorded talk can be found on [Climate Change AI's website](https://www.climatechange.ai/papers/neurips2022/114). 
+We also previewed some key features of ClimateLearn at a spotlight tutorial in the "Tackling Climate Change with Machine Learning" Workshop at the Neural Information Processing Systems 2022 Conference. The slides and recorded talk can be found on [Climate Change AI's website](https://www.climatechange.ai/papers/neurips2022/114).
 
 ### Documentation
 Find us on [ReadTheDocs](https://climatelearn.readthedocs.io/).
 
-### Integrations
-- [Weights & Biases](https://wandb.ai/site)
-
 ## About Us
 ClimateLearn is managed by the Machine Intelligence Group at UCLA, headed by [Professor Aditya Grover](https://aditya-grover.github.io).
 
 ## Contributing
 Contributions are welcome! See our [contributing guide](https://github.com/aditya-grover/climate-learn/blob/main/CONTRIBUTING.md).
 
 ## Citing ClimateLearn
```

### Comparing `climate_learn-0.0.2/pyproject.toml` & `climate_learn-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "climate_learn"
-version = "0.0.2"
+version = "1.0.0"
 authors = [
-    { name = "MINT at UCLA", email = "jason.jewik@cs.ucla.edu" },
-    { name = "Hritik Bansal", email = "hbansal@g.ucla.edu" },
-    { name = "Shashank Goel", email = "shashankgoel@g.ucla.edu" },
-    { name = "Siddharth Nandy", email = "sidd.nandy@gmail.com" },
-    { name = "Tung Nguyen", email = "tungnd@g.ucla.edu" },
-    { name = "Seongbin Park", email = "shannonsbpark@gmail.com" },
-    { name = "Jingchen Tang", email = "tangtang1228@ucla.edu" },
-    { name = "Jason Jewik", email = "jason.jewik@cs.ucla.edu" },
+    { name = "MINT at UCLA", email = "jason.jewik@ucla.edu" },
+    { name = "Tung Nguyen", email = "tungnd@cs.ucla.edu" },
+    { name = "Jason Jewik", email = "jason.jewik@ucla.edu" },
+    { name = "Hritik Bansal", email = "hbansal@ucla.edu" },    
+    { name = "Prakhar Sharma", email = "prakhar6sharma@gmail.com" },
     { name = "Aditya Grover", email = "adityag@cs.ucla.edu" },
 ]
-description = "ClimateLearn: Benchmarking Machine Learning for Data-driven Climate Science"
+description = "ClimateLearn: Benchmarking Machine Learning for Weather and Climate Modeling"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Atmospheric Science",
     "Topic :: Software Development",
@@ -40,26 +36,29 @@
 ]
 dependencies = [    
     "cdsapi>=0.5.1",
     "dask>=2022.2.0",
     "importlib-metadata==4.13.0",
     "matplotlib>=3.5.3",
     "netcdf4>=1.6.2",
-    "pytorch-lightning>=1.9.0", 
+    "pytorch-lightning>=1.9.0",
     "scikit-learn>=1.0.2",
-    "timm>=0.6.12",
+    "timm==0.9.2",
+    "tensorboard==2.11.2",
     "wandb>=0.13.9",
     "xarray>=0.20.2",
+    "rasterio>=1.3.7"
 ]
 
 [project.optional-dependencies]
 dev = [
     "black>=23.1.0",    
     "flake8>=3.9.2",
     "pytest>=7.2.1",
+    "properscoring",
     "build",
     "twine"
 ]
 docs = [
     "ipython>=7.34.0",
     "nbsphinx>=0.8.12",
     "sphinx>=5.3.0",
```

### Comparing `climate_learn-0.0.2/src/climate_learn/data/constants.py` & `climate_learn-1.0.0/src/climate_learn/data/processing/era5_constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-NAME_TO_CMIP = {
-    "geopotential": "zg",
-    "u_component_of_wind": "ua",
-    "v_component_of_wind": "va",
-    "temperature": "ta",
-    "relative_humidity": "r",
-    "specific_humidity": "hus",
-}
-
 NAME_TO_VAR = {
     "2m_temperature": "t2m",
     "10m_u_component_of_wind": "u10",
     "10m_v_component_of_wind": "v10",
     "mean_sea_level_pressure": "msl",
     "surface_pressure": "sp",
     "toa_incident_solar_radiation": "tisr",
@@ -52,17 +43,38 @@
     "temperature",
     "relative_humidity",
     "specific_humidity",
     "vorticity",
     "potential_vorticity",
 ]
 
+VAR_TO_UNIT = {
+    "2m_temperature": "K",
+    "10m_u_component_of_wind": "m/s",
+    "10m_v_component_of_wind": "m/s",
+    "mean_sea_level_pressure": "Pa",
+    "surface_pressure": "Pa",
+    "toa_incident_solar_radiation": "J/m^2",
+    "total_precipitation": "m",
+    "total_cloud_cover": None, # dimensionless
+    "land_sea_mask": None, # dimensionless
+    "orography": None, # dimensionless
+    "geopotential": "m^2/s^2",
+    "u_component_of_wind": "m/s",
+    "v_component_of_wind": "m/s",
+    "temperature": "K",
+    "relative_humidity": "%",
+    "specific_humidity": "kg/kg",
+    "voriticity": "1/s",
+    "potential_vorticity": "K m^2 / (kg s)"
+}
+
 DEFAULT_PRESSURE_LEVELS = [50, 250, 500, 600, 700, 850, 925]
 
-CONSTANTS = ["orography", "lsm", "slt", "lat2d", "lon2d"]
+CONSTANTS = ["orography", "land_sea_mask", "slt", "lattitude", "longitude"]
 
 NAME_LEVEL_TO_VAR_LEVEL = {}
 
 for var in SINGLE_LEVEL_VARS:
     NAME_LEVEL_TO_VAR_LEVEL[var] = NAME_TO_VAR[var]
 
 for var in PRESSURE_LEVEL_VARS:
```

### Comparing `climate_learn-0.0.2/src/climate_learn/data/modules/era5_iterdataset.py` & `climate_learn-1.0.0/src/climate_learn/data/climate_dataset/cmip6_iterdataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -55,115 +55,142 @@
                 rank = 0
                 world_size = 1
             else:
                 rank = torch.distributed.get_rank()
                 world_size = torch.distributed.get_world_size()
             num_workers_per_ddp = worker_info.num_workers
             num_shards = num_workers_per_ddp * world_size
-            per_worker = int(math.floor(n_files / float(num_shards)))
+            per_worker = n_files // num_shards
             worker_id = rank * num_workers_per_ddp + worker_info.id
             iter_start = worker_id * per_worker
             iter_end = iter_start + per_worker
 
         for idx in range(iter_start, iter_end):
             path_inp = self.inp_file_list[idx]
             path_out = self.out_file_list[idx]
             inp = np.load(path_inp)
             if path_out == path_inp:
                 out = inp
             else:
                 out = np.load(path_out)
-            yield {k: inp[k] for k in self.variables}, {
-                k: out[k] for k in self.out_variables
+            yield {k: np.squeeze(inp[k], axis=1) for k in self.variables}, {
+                k: np.squeeze(out[k], axis=1) for k in self.out_variables
             }, self.variables, self.out_variables
 
 
 class Forecast(IterableDataset):
     def __init__(
         self, dataset: NpyReader, pred_range: int = 6, history: int = 3, window: int = 6
     ) -> None:
         super().__init__()
         self.dataset = dataset
-        self.pred_range = pred_range
+        assert pred_range % 6 == 0
+        self.pred_range = pred_range // 6
         self.history = history
-        self.window = window
+        assert window % 6 == 0
+        self.window = window // 6
 
     def __iter__(self):
         for inp_data, out_data, variables, out_variables in self.dataset:
-            x = np.concatenate(
-                [inp_data[k].astype(np.float32) for k in inp_data.keys()], axis=1
-            )
-            x = torch.from_numpy(x)
-            y = np.concatenate(
-                [out_data[k].astype(np.float32) for k in out_data.keys()], axis=1
-            )
-            y = torch.from_numpy(y)
-
-            inputs = x.unsqueeze(0).repeat_interleave(self.history, dim=0)
-            for t in range(self.history):
-                inputs[t] = inputs[t].roll(-t * self.window, dims=0)
+            inp_data = {
+                k: torch.from_numpy(inp_data[k].astype(np.float32))
+                .unsqueeze(0)
+                .repeat_interleave(self.history, dim=0)
+                for k in inp_data.keys()
+            }
+            out_data = {
+                k: torch.from_numpy(out_data[k].astype(np.float32))
+                for k in out_data.keys()
+            }
+            for key in inp_data.keys():
+                for t in range(self.history):
+                    inp_data[key][t] = inp_data[key][t].roll(-t * self.window, dims=0)
 
             last_idx = -((self.history - 1) * self.window + self.pred_range)
 
-            inputs = inputs[:, :last_idx].transpose(0, 1)  # N, T, C, H, W
+            inp_data = {
+                k: inp_data[k][:, :last_idx].transpose(0, 1)
+                for k in inp_data.keys()  # N, T, H, W
+            }
 
-            predict_ranges = (
-                torch.ones(inputs.shape[0]).to(torch.long) * self.pred_range
-            )
+            inp_data_len = inp_data[variables[0]].size(0)
+
+            predict_ranges = torch.ones(inp_data_len).to(torch.long) * self.pred_range
             output_ids = (
-                torch.arange(inputs.shape[0])
+                torch.arange(inp_data_len)
                 + (self.history - 1) * self.window
                 + predict_ranges
             )
-            outputs = y[output_ids]
-
-            yield inputs, outputs, variables, out_variables
+            out_data = {k: out_data[k][output_ids] for k in out_data.keys()}
+            yield inp_data, out_data, variables, out_variables
 
 
 class Downscale(IterableDataset):
     def __init__(self, dataset: NpyReader) -> None:
         super().__init__()
         self.dataset = dataset
 
     def __iter__(self):
         for inp_data, out_data, variables, out_variables in self.dataset:
-            x = np.concatenate(
-                [inp_data[k].astype(np.float32) for k in inp_data.keys()], axis=1
-            )
-            x = torch.from_numpy(x)
-            y = np.concatenate(
-                [out_data[k].astype(np.float32) for k in out_data.keys()], axis=1
-            )
-            y = torch.from_numpy(y)
-
-            yield x, y, variables, out_variables
+            inp_data = {
+                k: torch.from_numpy(inp_data[k].astype(np.float32))
+                for k in inp_data.keys()
+            }
+            out_data = {
+                k: torch.from_numpy(out_data[k].astype(np.float32))
+                for k in out_data.keys()
+            }
+            yield inp_data, out_data, variables, out_variables
 
 
 class IndividualDataIter(IterableDataset):
     def __init__(
         self,
         dataset: Union[Forecast, Downscale],
         transforms: torch.nn.Module,
         output_transforms: torch.nn.Module,
+        subsample: int = 6,
     ):
         super().__init__()
         self.dataset = dataset
         self.transforms = transforms
         self.output_transforms = output_transforms
+        self.subsample = subsample
 
     def __iter__(self):
         for inp, out, variables, out_variables in self.dataset:
-            assert inp.shape[0] == out.shape[0]
-            for i in range(inp.shape[0]):
+            inp_shapes = set([inp[k].shape[0] for k in inp.keys()])
+            out_shapes = set([out[k].shape[0] for k in out.keys()])
+            assert len(inp_shapes) == 1
+            assert len(out_shapes) == 1
+            inp_len = next(iter(inp_shapes))
+            out_len = next(iter(out_shapes))
+            assert inp_len == out_len
+            for i in range(0, inp_len, self.subsample):
+                x = {k: inp[k][i] for k in inp.keys()}
+                y = {k: out[k][i] for k in out.keys()}
                 if self.transforms is not None:
-                    yield self.transforms(inp[i]), self.output_transforms(
-                        out[i]
-                    ), variables, out_variables
-                else:
-                    yield inp[i], out[i], variables, out_variables
+                    if isinstance(self.dataset, Forecast):
+                        x = {
+                            k: self.transforms[k](x[k].unsqueeze(1)).squeeze(1)
+                            for k in x.keys()
+                        }
+                    elif isinstance(self.dataset, Downscale):
+                        x = {
+                            k: self.transforms[k](x[k].unsqueeze(0)).squeeze(0)
+                            for k in x.keys()
+                        }
+                    else:
+                        raise RuntimeError(f"Not supported task.")
+                if self.output_transforms is not None:
+                    y = {
+                        k: self.output_transforms[k](y[k].unsqueeze(0)).squeeze(0)
+                        for k in y.keys()
+                    }
+                yield x, y, variables, out_variables
 
 
 class ShuffleIterableDataset(IterableDataset):
     def __init__(self, dataset: IndividualDataIter, buffer_size: int) -> None:
         super().__init__()
         assert buffer_size > 0
         self.dataset = dataset
```

### Comparing `climate_learn-0.0.2/src/climate_learn/data/nc2npz.py` & `climate_learn-1.0.0/src/climate_learn/data/processing/nc2npz.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # Standard library
 import glob
 import os
 
-# Local application
-from .constants import DEFAULT_PRESSURE_LEVELS, NAME_TO_VAR, VAR_TO_NAME, CONSTANTS
-
 # Third party
 import numpy as np
 import xarray as xr
 import netCDF4 as nc
 from tqdm import tqdm
 
+# Local application
+from .era5_constants import (
+    DEFAULT_PRESSURE_LEVELS,
+    NAME_TO_VAR,
+    VAR_TO_NAME,
+    CONSTANTS,
+)
+
 HOURS_PER_YEAR = 8736  # 8760 --> 8736 which is dividable by 16
 
 
 def nc2np(path, variables, years, save_dir, partition, num_shards_per_year):
     os.makedirs(os.path.join(save_dir, partition), exist_ok=True)
 
     if partition == "train":
@@ -54,15 +59,23 @@
                 ps, combine="by_coords", parallel=True
             )  # dataset for a single variable
             code = NAME_TO_VAR[var]
 
             if len(ds[code].shape) == 3:  # surface level variables
                 ds[code] = ds[code].expand_dims("val", axis=1)
                 # remove the last 24 hours if this year has 366 days
-                np_vars[var] = ds[code].to_numpy()[-HOURS_PER_YEAR:]
+                if code == "tp":  # accumulate 6 hours and log transform
+                    tp = ds[code].to_numpy()
+                    tp_cum_6hrs = np.cumsum(tp, axis=0)
+                    tp_cum_6hrs[6:] = tp_cum_6hrs[6:] - tp_cum_6hrs[:-6]
+                    eps = 0.001
+                    tp_cum_6hrs = np.log(eps + tp_cum_6hrs) - np.log(eps)
+                    np_vars[var] = tp_cum_6hrs[-HOURS_PER_YEAR:]
+                else:
+                    np_vars[var] = ds[code].to_numpy()[-HOURS_PER_YEAR:]
 
                 if partition == "train":
                     # compute mean and std of each var in each year
                     var_mean_yearly = np_vars[var].mean(axis=(0, 2, 3))
                     var_std_yearly = np_vars[var].std(axis=(0, 2, 3))
                     if var not in normalize_mean:
                         normalize_mean[var] = [var_mean_yearly]
@@ -132,14 +145,16 @@
                     + (mean**2).mean(axis=0)
                     - mean.mean(axis=0) ** 2
                 )
                 std = np.sqrt(variance)
                 # E[X] = E[E[X|Y]]
                 mean = mean.mean(axis=0)
                 normalize_mean[var] = mean
+                if var == "total_precipitation":
+                    normalize_mean[var] = np.zeros_like(normalize_mean[var])
                 normalize_std[var] = std
 
         np.savez(os.path.join(save_dir, "normalize_mean.npz"), **normalize_mean)
         np.savez(os.path.join(save_dir, "normalize_std.npz"), **normalize_std)
 
     for var in climatology.keys():
         climatology[var] = np.stack(climatology[var], axis=0)
```

### Comparing `climate_learn-0.0.2/src/climate_learn/models/components/cnn_blocks.py` & `climate_learn-1.0.0/src/climate_learn/models/hub/components/cnn_blocks.py`

 * *Files identical despite different names*

### Comparing `climate_learn-0.0.2/src/climate_learn/models/components/unet.py` & `climate_learn-1.0.0/src/climate_learn/models/hub/unet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,69 @@
-from math import log
-from typing import List, Tuple, Union
+# Standard library
+from typing import Iterable
 
-import torch
-from torch import nn
-from torch.distributions.normal import Normal
-from .cnn_blocks import (
-    PeriodicConv2D,
+# Local application
+from .utils import register
+from .components.cnn_blocks import (
     DownBlock,
-    UpBlock,
-    MiddleBlock,
     Downsample,
+    MiddleBlock,
+    PeriodicConv2D,
+    UpBlock,
     Upsample,
 )
 
-# Large based on https://github.com/labmlai/annotated_deep_learning_paper_implementations/blob/master/labml_nn/diffusion/ddpm/unet.py
-# MIT License
+# Third party
+import torch
+from torch import nn
 
 
+@register("unet")
 class Unet(nn.Module):
     def __init__(
         self,
         in_channels,
+        out_channels,
         history=1,
         hidden_channels=64,
         activation="leaky",
-        out_channels=None,
         norm: bool = True,
         dropout: float = 0.1,
-        ch_mults: Union[Tuple[int, ...], List[int]] = (1, 2, 2, 4),
-        is_attn: Union[Tuple[bool, ...], List[bool]] = (False, False, False, False),
+        ch_mults: Iterable[int] = (1, 2, 2, 4),
+        is_attn: Iterable[bool] = (False, False, False, False),
         mid_attn: bool = False,
         n_blocks: int = 2,
     ) -> None:
         super().__init__()
         self.prob_type = None
-        self.in_channels = in_channels
-        if out_channels is None:
-            out_channels = in_channels
+        self.in_channels = in_channels * history
         self.out_channels = out_channels
         self.hidden_channels = hidden_channels
 
         if activation == "gelu":
             self.activation = nn.GELU()
         elif activation == "relu":
             self.activation = nn.ReLU()
         elif activation == "silu":
             self.activation = nn.SiLU()
         elif activation == "leaky":
             self.activation = nn.LeakyReLU(0.3)
         else:
             raise NotImplementedError(f"Activation {activation} not implemented")
 
-        # Number of resolutions
-        n_resolutions = len(ch_mults)
-
-        insize = self.in_channels * history
-        n_channels = hidden_channels
-        # Project image into feature map
-        self.image_proj = PeriodicConv2D(insize, n_channels, kernel_size=7, padding=3)
+        self.image_proj = PeriodicConv2D(
+            self.in_channels, self.hidden_channels, kernel_size=7, padding=3
+        )
 
         # #### First half of U-Net - decreasing resolution
         down = []
         # Number of channels
-        out_channels = in_channels = n_channels
+        out_channels = in_channels = self.hidden_channels
         # For each resolution
+        n_resolutions = len(ch_mults)
         for i in range(n_resolutions):
             # Number of output channels at this resolution
             out_channels = in_channels * ch_mults[i]
             # Add `n_blocks`
             for _ in range(n_blocks):
                 down.append(
                     DownBlock(
@@ -132,59 +128,34 @@
             if i > 0:
                 up.append(Upsample(in_channels))
 
         # Combine the set of modules
         self.up = nn.ModuleList(up)
 
         if norm:
-            self.norm = nn.BatchNorm2d(n_channels)
+            self.norm = nn.BatchNorm2d(self.hidden_channels)
         else:
             self.norm = nn.Identity()
-        out_channels = self.out_channels
-        self.final = PeriodicConv2D(in_channels, out_channels, kernel_size=7, padding=3)
+        self.final = PeriodicConv2D(
+            in_channels, self.out_channels, kernel_size=7, padding=3
+        )
 
-    def predict(self, x):
-        if len(x.shape) == 5:  # history
+    def forward(self, x):
+        if len(x.shape) == 5:  # x.shape = [B,T,C,H,W]
             x = x.flatten(1, 2)
+        # x.shape = [B,T*C,H,W]
         x = self.image_proj(x)
-
         h = [x]
         for m in self.down:
             x = m(x)
             h.append(x)
-
         x = self.middle(x)
-
         for m in self.up:
             if isinstance(m, Upsample):
                 x = m(x)
             else:
                 # Get the skip connection from first half of U-Net and concatenate
                 s = h.pop()
                 x = torch.cat((x, s), dim=1)
                 x = m(x)
-
-        pred = self.final(self.activation(self.norm(x)))
-
-        return pred
-
-    def forward(
-        self, x: torch.Tensor, y: torch.Tensor, out_variables, metric, lat, log_postfix
-    ):
-        # B, C, H, W
-        pred = self.predict(x)
-        return (
-            [
-                m(pred, y, out_variables, lat=lat, log_postfix=log_postfix)
-                for m in metric
-            ],
-            x,
-        )
-
-    def evaluate(
-        self, x, y, variables, out_variables, transform, metrics, lat, clim, log_postfix
-    ):
-        pred = self.predict(x)
-        return [
-            m(pred, y, transform, out_variables, lat, clim, log_postfix)
-            for m in metrics
-        ], pred
+        yhat = self.final(self.activation(self.norm(x)))
+        return yhat
```

### Comparing `climate_learn-0.0.2/src/climate_learn/models/components/utils/pos_embed.py` & `climate_learn-1.0.0/src/climate_learn/models/hub/components/pos_embed.py`

 * *Files identical despite different names*

### Comparing `climate_learn-0.0.2/src/climate_learn/models/modules/utils/lr_scheduler.py` & `climate_learn-1.0.0/src/climate_learn/models/lr_scheduler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import math
 import warnings
 from typing import List
 
-# from pytorch_lightning.utilities.cli import LR_SCHEDULER_REGISTRY
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler
 
 
-# @LR_SCHEDULER_REGISTRY
 class LinearWarmupCosineAnnealingLR(_LRScheduler):
     """Sets the learning rate of each parameter group to follow a linear warmup schedule between
     warmup_start_lr and base_lr followed by a cosine annealing schedule between base_lr and
     eta_min."""
 
     def __init__(
         self,
```

### Comparing `climate_learn-0.0.2/src/climate_learn.egg-info/PKG-INFO` & `climate_learn-1.0.0/src/climate_learn.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,62 @@
 Metadata-Version: 2.1
 Name: climate-learn
-Version: 0.0.2
-Summary: ClimateLearn: Benchmarking Machine Learning for Data-driven Climate Science
-Author-email: MINT at UCLA <jason.jewik@cs.ucla.edu>, Hritik Bansal <hbansal@g.ucla.edu>, Shashank Goel <shashankgoel@g.ucla.edu>, Siddharth Nandy <sidd.nandy@gmail.com>, Tung Nguyen <tungnd@g.ucla.edu>, Seongbin Park <shannonsbpark@gmail.com>, Jingchen Tang <tangtang1228@ucla.edu>, Jason Jewik <jason.jewik@cs.ucla.edu>, Aditya Grover <adityag@cs.ucla.edu>
+Version: 1.0.0
+Summary: ClimateLearn: Benchmarking Machine Learning for Weather and Climate Modeling
+Author-email: MINT at UCLA <jason.jewik@ucla.edu>, Tung Nguyen <tungnd@cs.ucla.edu>, Jason Jewik <jason.jewik@ucla.edu>, Hritik Bansal <hbansal@ucla.edu>, Prakhar Sharma <prakhar6sharma@gmail.com>, Aditya Grover <adityag@cs.ucla.edu>
 Project-URL: Source, https://github.com/aditya-grover/climate-learn
 Project-URL: Issue Tracker, https://github.com/aditya-grover/climate-learn/issues
 Project-URL: Documentation, https://climatelearn.readthedocs.io/en/latest/
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 <h1 align="center">ClimateLearn</h1>
 
 [![Documentation Status](https://readthedocs.org/projects/climatelearn/badge/?version=latest)](https://climatelearn.readthedocs.io/en/latest/?badge=latest)
 [![CI Build Status](https://github.com/aditya-grover/climate-learn/actions/workflows/ci.yaml/badge.svg)](https://github.com/aditya-grover/climate-learn/actions/workflows/ci.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WiNEK1BHsiGzo_bT9Fcm8lea2H_ghNfa)
+[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LcecQLgLtwaHOwbvJAxw9UjCxfM0RMrX?usp=sharing)
 
 **ClimateLearn** is a Python library for accessing state-of-the-art climate data and machine learning models in a standardized, straightforward way. This library provides access to multiple datasets, a zoo of baseline approaches, and a suite of metrics and visualizations for large-scale benchmarking of statistical downscaling and temporal forecasting methods. For further context on our past motivation and future plans, check out our announcement [blog post](https://aditya-grover.github.io/blog/2023/climate-learn/).
 
 ## Usage
 
-[**Python3**](https://www.python.org/) is required.
+[**Python 3.8+**](https://www.python.org/) is required. The xESMF package has to be installed separately since one of its dependencies, ESMpy, is available only through Conda.
 ```
+conda install -c conda-forge xesmf
 pip install climate-learn
 ```
 
 ### Quickstart
-Please refer to this [Google Colab](https://colab.research.google.com/drive/1WiNEK1BHsiGzo_bT9Fcm8lea2H_ghNfa) for a tutorial-style exposition into developing your first models for forecasting and downscaling in ClimateLearn.
+We have a quickstart notebook in the `notebooks` folder titled `Quickstart.ipynb`. It is intended for use in Google Colab and can be launched by clicking the Google Colab badge above or this link: https://colab.research.google.com/drive/1LcecQLgLtwaHOwbvJAxw9UjCxfM0RMrX?usp=sharing.
 
-We previewed some key features of ClimateLearn at a spotlight tutorial in the "Tackling Climate Change with Machine Learning" Workshop at the Neural Information Processing Systems 2022 Conference. The slides and recorded talk can be found on [Climate Change AI's website](https://www.climatechange.ai/papers/neurips2022/114). 
+We also previewed some key features of ClimateLearn at a spotlight tutorial in the "Tackling Climate Change with Machine Learning" Workshop at the Neural Information Processing Systems 2022 Conference. The slides and recorded talk can be found on [Climate Change AI's website](https://www.climatechange.ai/papers/neurips2022/114).
 
 ### Documentation
 Find us on [ReadTheDocs](https://climatelearn.readthedocs.io/).
 
-### Integrations
-- [Weights & Biases](https://wandb.ai/site)
-
 ## About Us
 ClimateLearn is managed by the Machine Intelligence Group at UCLA, headed by [Professor Aditya Grover](https://aditya-grover.github.io).
 
 ## Contributing
 Contributions are welcome! See our [contributing guide](https://github.com/aditya-grover/climate-learn/blob/main/CONTRIBUTING.md).
 
 ## Citing ClimateLearn
```

