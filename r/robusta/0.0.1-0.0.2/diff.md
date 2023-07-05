# Comparing `tmp/robusta-0.0.1.tar.gz` & `tmp/robusta-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/robusta-0.0.1.tar", last modified: Fri Feb 28 18:11:41 2020, max compression
+gzip compressed data, was "robusta-0.0.2.tar", last modified: Wed Jul  5 23:05:56 2023, max compression
```

## Comparing `robusta-0.0.1.tar` & `robusta-0.0.2.tar`

### file list

```diff
@@ -1,83 +1,42 @@
-drwxr-xr-x   0 sophin     (501) staff       (20)        0 2020-02-28 18:11:41.475591 robusta-0.0.1/
--rw-r--r--   0 sophin     (501) staff       (20)      484 2020-02-28 18:11:41.475274 robusta-0.0.1/PKG-INFO
--rwxr-xr-x   0 sophin     (501) staff       (20)       22 2020-02-28 17:37:25.000000 robusta-0.0.1/README.md
-drwxr-xr-x   0 sophin     (501) staff       (20)        0 2020-02-28 18:11:41.441646 robusta-0.0.1/crossval/
--rw-r--r--   0 sophin     (501) staff       (20)      708 2020-02-11 02:27:19.000000 robusta-0.0.1/crossval/__init__.py
--rw-r--r--   0 sophin     (501) staff       (20)     2750 2020-02-11 02:02:16.000000 robusta-0.0.1/crossval/_curve.py
--rw-r--r--   0 sophin     (501) staff       (20)    13503 2020-02-23 12:25:29.000000 robusta-0.0.1/crossval/_predict.py
--rw-r--r--   0 sophin     (501) staff       (20)     2827 2020-02-12 04:11:42.000000 robusta-0.0.1/crossval/_verbose.py
--rw-r--r--   0 sophin     (501) staff       (20)     3706 2020-01-31 11:37:16.000000 robusta-0.0.1/crossval/compare.py
--rw-r--r--   0 sophin     (501) staff       (20)    19618 2020-02-13 16:51:46.000000 robusta-0.0.1/crossval/crossval.py
--rw-r--r--   0 sophin     (501) staff       (20)     4886 2020-02-19 02:14:43.000000 robusta-0.0.1/crossval/plot.py
--rw-r--r--   0 sophin     (501) staff       (20)     3730 2020-01-17 00:42:52.000000 robusta-0.0.1/crossval/results.py
--rw-r--r--   0 sophin     (501) staff       (20)     2175 2019-10-11 00:29:19.000000 robusta-0.0.1/crossval/saveload.py
--rw-r--r--   0 sophin     (501) staff       (20)    14349 2020-02-03 11:13:05.000000 robusta-0.0.1/crossval/schemes.py
-drwxr-xr-x   0 sophin     (501) staff       (20)        0 2020-02-28 18:11:41.444079 robusta-0.0.1/importance/
--rw-r--r--   0 sophin     (501) staff       (20)      317 2020-02-02 23:17:08.000000 robusta-0.0.1/importance/__init__.py
--rw-r--r--   0 sophin     (501) staff       (20)      718 2019-10-29 18:06:03.000000 robusta-0.0.1/importance/importance.py
--rw-r--r--   0 sophin     (501) staff       (20)    16151 2020-02-20 17:06:26.000000 robusta-0.0.1/importance/permutation.py
--rw-r--r--   0 sophin     (501) staff       (20)      833 2020-01-06 20:07:01.000000 robusta-0.0.1/importance/plot.py
--rw-r--r--   0 sophin     (501) staff       (20)     6003 2020-02-19 03:16:11.000000 robusta-0.0.1/importance/shuffle.py
-drwxr-xr-x   0 sophin     (501) staff       (20)        0 2020-02-28 18:11:41.446731 robusta-0.0.1/linear_model/
--rw-r--r--   0 sophin     (501) staff       (20)      192 2020-01-25 07:25:00.000000 robusta-0.0.1/linear_model/__init__.py
--rwxr-xr-x   0 sophin     (501) staff       (20)     5605 2020-01-25 07:52:33.000000 robusta-0.0.1/linear_model/blend.py
--rw-r--r--   0 sophin     (501) staff       (20)     5176 2020-01-25 08:09:21.000000 robusta-0.0.1/linear_model/caruana.py
--rwxr-xr-x   0 sophin     (501) staff       (20)     3831 2019-12-06 01:30:47.000000 robusta-0.0.1/linear_model/nng.py
-drwxr-xr-x   0 sophin     (501) staff       (20)        0 2020-02-28 18:11:41.450783 robusta-0.0.1/optimizer/
--rwxr-xr-x   0 sophin     (501) staff       (20)      206 2019-10-30 03:02:32.000000 robusta-0.0.1/optimizer/__init__.py
--rw-r--r--   0 sophin     (501) staff       (20)      471 2019-10-30 03:38:46.000000 robusta-0.0.1/optimizer/_plot.py
--rwxr-xr-x   0 sophin     (501) staff       (20)     2162 2019-10-30 03:34:02.000000 robusta-0.0.1/optimizer/_verbose.py
--rwxr-xr-x   0 sophin     (501) staff       (20)    12235 2019-11-11 22:28:50.000000 robusta-0.0.1/optimizer/base.py
--rw-r--r--   0 sophin     (501) staff       (20)     1061 2019-11-11 22:30:26.000000 robusta-0.0.1/optimizer/grid.py
--rw-r--r--   0 sophin     (501) staff       (20)     2431 2019-11-11 22:30:37.000000 robusta-0.0.1/optimizer/optuna.py
-drwxr-xr-x   0 sophin     (501) staff       (20)        0 2020-02-28 18:11:41.454742 robusta-0.0.1/outliers/
--rw-r--r--   0 sophin     (501) staff       (20)      360 2019-05-08 17:42:31.000000 robusta-0.0.1/outliers/__init__.py
--rw-r--r--   0 sophin     (501) staff       (20)      362 2019-05-06 12:06:24.000000 robusta-0.0.1/outliers/base.py
--rw-r--r--   0 sophin     (501) staff       (20)     1311 2019-05-06 10:38:27.000000 robusta-0.0.1/outliers/divided.py
--rw-r--r--   0 sophin     (501) staff       (20)      611 2019-05-06 10:39:06.000000 robusta-0.0.1/outliers/sklearn.py
--rw-r--r--   0 sophin     (501) staff       (20)      858 2019-05-08 17:42:35.000000 robusta-0.0.1/outliers/supervised.py
-drwxr-xr-x   0 sophin     (501) staff       (20)        0 2020-02-28 18:11:41.457671 robusta-0.0.1/pipeline/
--rwxr-xr-x   0 sophin     (501) staff       (20)      294 2019-04-28 08:50:48.000000 robusta-0.0.1/pipeline/__init__.py
--rwxr-xr-x   0 sophin     (501) staff       (20)     9322 2019-09-17 19:25:11.000000 robusta-0.0.1/pipeline/_column_transformer.py
--rwxr-xr-x   0 sophin     (501) staff       (20)     5544 2019-10-28 13:39:43.000000 robusta-0.0.1/pipeline/_feature_union.py
--rwxr-xr-x   0 sophin     (501) staff       (20)     1713 2020-02-02 03:17:50.000000 robusta-0.0.1/pipeline/_pipeline.py
--rwxr-xr-x   0 sophin     (501) staff       (20)     3398 2019-10-23 08:56:35.000000 robusta-0.0.1/pipeline/_target.py
-drwxr-xr-x   0 sophin     (501) staff       (20)        0 2020-02-28 18:11:41.462192 robusta-0.0.1/preprocessing/
--rwxr-xr-x   0 sophin     (501) staff       (20)     1554 2020-01-25 08:10:03.000000 robusta-0.0.1/preprocessing/__init__.py
--rwxr-xr-x   0 sophin     (501) staff       (20)    12755 2020-02-20 18:16:02.000000 robusta-0.0.1/preprocessing/base.py
--rwxr-xr-x   0 sophin     (501) staff       (20)    11988 2019-12-14 04:00:53.000000 robusta-0.0.1/preprocessing/category.py
--rw-r--r--   0 sophin     (501) staff       (20)     1622 2019-12-04 14:21:58.000000 robusta-0.0.1/preprocessing/datetime.py
--rwxr-xr-x   0 sophin     (501) staff       (20)    20368 2019-12-31 11:51:14.000000 robusta-0.0.1/preprocessing/numeric.py
--rw-r--r--   0 sophin     (501) staff       (20)     6587 2019-11-13 17:32:39.000000 robusta-0.0.1/preprocessing/target.py
-drwxr-xr-x   0 sophin     (501) staff       (20)        0 2020-02-28 18:11:41.464047 robusta-0.0.1/robusta.egg-info/
--rw-r--r--   0 sophin     (501) staff       (20)      484 2020-02-28 18:11:41.000000 robusta-0.0.1/robusta.egg-info/PKG-INFO
--rw-r--r--   0 sophin     (501) staff       (20)     1459 2020-02-28 18:11:41.000000 robusta-0.0.1/robusta.egg-info/SOURCES.txt
--rw-r--r--   0 sophin     (501) staff       (20)        1 2020-02-28 18:11:41.000000 robusta-0.0.1/robusta.egg-info/dependency_links.txt
--rw-r--r--   0 sophin     (501) staff       (20)      114 2020-02-28 18:11:41.000000 robusta-0.0.1/robusta.egg-info/top_level.txt
-drwxr-xr-x   0 sophin     (501) staff       (20)        0 2020-02-28 18:11:41.469519 robusta-0.0.1/selector/
--rwxr-xr-x   0 sophin     (501) staff       (20)      792 2020-02-02 23:10:39.000000 robusta-0.0.1/selector/__init__.py
--rw-r--r--   0 sophin     (501) staff       (20)     1534 2019-12-22 21:08:20.000000 robusta-0.0.1/selector/_plot.py
--rw-r--r--   0 sophin     (501) staff       (20)     3553 2020-02-02 23:42:13.000000 robusta-0.0.1/selector/_subset.py
--rw-r--r--   0 sophin     (501) staff       (20)     1980 2020-02-02 23:37:25.000000 robusta-0.0.1/selector/_verbose.py
--rw-r--r--   0 sophin     (501) staff       (20)     6732 2020-02-11 19:22:30.000000 robusta-0.0.1/selector/base.py
--rw-r--r--   0 sophin     (501) staff       (20)     4093 2020-02-11 19:22:28.000000 robusta-0.0.1/selector/exhaustive.py
--rw-r--r--   0 sophin     (501) staff       (20)     5875 2019-11-02 00:36:25.000000 robusta-0.0.1/selector/from_model.py
--rw-r--r--   0 sophin     (501) staff       (20)    10478 2020-02-11 19:23:03.000000 robusta-0.0.1/selector/genetic.py
--rw-r--r--   0 sophin     (501) staff       (20)     7666 2020-02-11 19:23:22.000000 robusta-0.0.1/selector/greed.py
--rw-r--r--   0 sophin     (501) staff       (20)     6098 2020-02-11 19:23:35.000000 robusta-0.0.1/selector/random.py
--rw-r--r--   0 sophin     (501) staff       (20)    10426 2020-02-13 17:02:17.000000 robusta-0.0.1/selector/rfe.py
--rw-r--r--   0 sophin     (501) staff       (20)     3757 2020-02-11 19:24:29.000000 robusta-0.0.1/selector/sas.py
-drwxr-xr-x   0 sophin     (501) staff       (20)        0 2020-02-28 18:11:41.470510 robusta-0.0.1/semi_supervised/
--rw-r--r--   0 sophin     (501) staff       (20)       65 2019-12-02 18:48:20.000000 robusta-0.0.1/semi_supervised/__init__.py
--rw-r--r--   0 sophin     (501) staff       (20)     2944 2019-12-03 04:05:18.000000 robusta-0.0.1/semi_supervised/pseudo_label.py
--rw-r--r--   0 sophin     (501) staff       (20)       38 2020-02-28 18:11:41.475696 robusta-0.0.1/setup.cfg
--rw-r--r--   0 sophin     (501) staff       (20)      636 2020-02-28 18:11:26.000000 robusta-0.0.1/setup.py
-drwxr-xr-x   0 sophin     (501) staff       (20)        0 2020-02-28 18:11:41.472731 robusta-0.0.1/testing/
--rwxr-xr-x   0 sophin     (501) staff       (20)      393 2019-11-11 21:06:38.000000 robusta-0.0.1/testing/__init__.py
--rw-r--r--   0 sophin     (501) staff       (20)     7288 2020-02-10 01:55:20.000000 robusta-0.0.1/testing/estimators.py
--rw-r--r--   0 sophin     (501) staff       (20)     9767 2019-11-11 22:09:14.000000 robusta-0.0.1/testing/params.py
--rwxr-xr-x   0 sophin     (501) staff       (20)     5410 2020-02-09 19:56:57.000000 robusta-0.0.1/testing/utils.py
-drwxr-xr-x   0 sophin     (501) staff       (20)        0 2020-02-28 18:11:41.474517 robusta-0.0.1/utils/
--rw-r--r--   0 sophin     (501) staff       (20)       44 2019-10-11 15:15:47.000000 robusta-0.0.1/utils/__init__.py
--rw-r--r--   0 sophin     (501) staff       (20)     1118 2019-10-19 19:38:22.000000 robusta-0.0.1/utils/_timer.py
--rw-r--r--   0 sophin     (501) staff       (20)     2328 2019-12-22 19:16:13.000000 robusta-0.0.1/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:05:56.609211 robusta-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-07-05 23:05:40.000000 robusta-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-07-05 23:05:40.000000 robusta-0.0.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-07-05 23:05:56.609211 robusta-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-07-05 23:05:40.000000 robusta-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-05 23:05:40.000000 robusta-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:05:56.605211 robusta-0.0.2/robusta/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:05:56.609211 robusta-0.0.2/robusta/batchnorm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/batchnorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/batchnorm/bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/batchnorm/stages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:05:56.609211 robusta-0.0.2/robusta/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33424 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/datasets/imagenet200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23779 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/datasets/imageneta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/datasets/imagenetc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/datasets/imagenetr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:05:56.609211 robusta-0.0.2/robusta/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/models/BiT_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/models/fixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/models/imagenet_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/models/resnet_gn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:05:56.609211 robusta-0.0.2/robusta/selflearning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/selflearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/selflearning/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-05 23:05:40.000000 robusta-0.0.2/robusta/selflearning/nn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:05:56.605211 robusta-0.0.2/robusta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-07-05 23:05:56.000000 robusta-0.0.2/robusta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-05 23:05:56.000000 robusta-0.0.2/robusta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 23:05:56.000000 robusta-0.0.2/robusta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 23:05:56.000000 robusta-0.0.2/robusta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-05 23:05:56.000000 robusta-0.0.2/robusta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-05 23:05:56.609211 robusta-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:05:56.609211 robusta-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-05 23:05:40.000000 robusta-0.0.2/test/test_batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-05 23:05:40.000000 robusta-0.0.2/test/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-05 23:05:40.000000 robusta-0.0.2/test/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 23:05:40.000000 robusta-0.0.2/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 23:05:40.000000 robusta-0.0.2/test/test_selflearning.py
```

