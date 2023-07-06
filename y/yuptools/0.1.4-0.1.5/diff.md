# Comparing `tmp/yuptools-0.1.4.tar.gz` & `tmp/yuptools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuptools-0.1.4.tar", last modified: Fri Jun 30 03:59:32 2023, max compression
+gzip compressed data, was "yuptools-0.1.5.tar", last modified: Thu Jul  6 03:09:12 2023, max compression
```

## Comparing `yuptools-0.1.4.tar` & `yuptools-0.1.5.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:32.966681 yuptools-0.1.4/
--rw-rw-rw-   0        0        0     1088 2023-04-21 08:53:14.000000 yuptools-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     3198 2023-06-30 03:59:32.965678 yuptools-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2957 2023-06-30 03:58:56.000000 yuptools-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 03:59:32.967674 yuptools-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-30 03:58:56.000000 yuptools-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:30.647202 yuptools-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:30.728983 yuptools-0.1.4/src/yuptools/
--rw-rw-rw-   0        0        0      240 2023-05-21 22:00:40.000000 yuptools-0.1.4/src/yuptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:30.884680 yuptools-0.1.4/src/yuptools/attacks/
--rw-rw-rw-   0        0        0       43 2023-05-21 01:50:37.000000 yuptools-0.1.4/src/yuptools/attacks/__init__.py
--rw-rw-rw-   0        0        0     1943 2023-05-23 23:07:37.000000 yuptools-0.1.4/src/yuptools/attacks/fgsm.py
--rw-rw-rw-   0        0        0     2872 2023-05-22 04:35:07.000000 yuptools-0.1.4/src/yuptools/attacks/ifgsm.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:31.018128 yuptools-0.1.4/src/yuptools/datasets/
--rw-rw-rw-   0        0        0       86 2023-05-25 12:15:58.000000 yuptools-0.1.4/src/yuptools/datasets/__init__.py
--rw-rw-rw-   0        0        0     4145 2023-05-25 08:06:05.000000 yuptools-0.1.4/src/yuptools/datasets/base.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:31.418743 yuptools-0.1.4/src/yuptools/datasets/class_labels/
--rw-rw-rw-   0        0        0       17 2023-05-25 12:15:58.000000 yuptools-0.1.4/src/yuptools/datasets/class_labels/__init__.py
--rw-rw-rw-   0        0        0      191 2023-04-19 07:36:49.000000 yuptools-0.1.4/src/yuptools/datasets/class_labels/cifar10.py
--rw-rw-rw-   0        0        0     1935 2023-04-19 07:36:49.000000 yuptools-0.1.4/src/yuptools/datasets/class_labels/cifar100.py
--rw-rw-rw-   0        0        0      207 2023-04-20 00:48:17.000000 yuptools-0.1.4/src/yuptools/datasets/class_labels/fashionmnist.py
--rw-rw-rw-   0        0        0    18494 2023-04-19 10:46:55.000000 yuptools-0.1.4/src/yuptools/datasets/class_labels/imagenet.py
--rw-rw-rw-   0        0        0      151 2023-04-20 00:52:35.000000 yuptools-0.1.4/src/yuptools/datasets/class_labels/mnist.py
--rw-rw-rw-   0        0        0     9466 2023-05-21 01:56:33.000000 yuptools-0.1.4/src/yuptools/datasets/image_classification.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:31.540416 yuptools-0.1.4/src/yuptools/models/
--rw-rw-rw-   0        0        0       97 2023-05-23 23:21:32.000000 yuptools-0.1.4/src/yuptools/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:31.787755 yuptools-0.1.4/src/yuptools/models/classification/
--rw-rw-rw-   0        0        0       67 2023-05-19 05:42:06.000000 yuptools-0.1.4/src/yuptools/models/classification/__init__.py
--rw-rw-rw-   0        0        0     5499 2023-05-22 03:46:27.000000 yuptools-0.1.4/src/yuptools/models/classification/base.py
--rw-rw-rw-   0        0        0     1146 2023-05-19 04:08:19.000000 yuptools-0.1.4/src/yuptools/models/classification/config.py
--rw-rw-rw-   0        0        0     3122 2023-06-26 07:32:05.000000 yuptools-0.1.4/src/yuptools/models/classification/models.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:31.940511 yuptools-0.1.4/src/yuptools/models/classification/nets/
--rw-rw-rw-   0        0        0       86 2023-03-22 22:54:35.000000 yuptools-0.1.4/src/yuptools/models/classification/nets/__init__.py
--rw-rw-rw-   0        0        0     7111 2023-03-03 05:35:17.000000 yuptools-0.1.4/src/yuptools/models/classification/nets/deit.py
--rw-rw-rw-   0        0        0     6904 2023-03-03 05:35:17.000000 yuptools-0.1.4/src/yuptools/models/classification/nets/mixer.py
--rw-rw-rw-   0        0        0    23022 2023-03-03 05:35:17.000000 yuptools-0.1.4/src/yuptools/models/classification/nets/poolformer.py
--rw-rw-rw-   0        0        0    11940 2023-03-03 05:35:17.000000 yuptools-0.1.4/src/yuptools/models/classification/nets/pvt.py
--rw-rw-rw-   0        0        0      919 2023-05-19 04:46:33.000000 yuptools-0.1.4/src/yuptools/models/classification/warnings.py
--rw-rw-rw-   0        0        0      705 2023-05-19 02:49:58.000000 yuptools-0.1.4/src/yuptools/models/classification/weights.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:32.117039 yuptools-0.1.4/src/yuptools/models/replace/
--rw-rw-rw-   0        0        0       68 2023-05-19 06:29:29.000000 yuptools-0.1.4/src/yuptools/models/replace/__init__.py
--rw-rw-rw-   0        0        0      420 2023-05-19 06:26:47.000000 yuptools-0.1.4/src/yuptools/models/replace/activation.py
--rw-rw-rw-   0        0        0     1457 2023-05-21 00:57:35.000000 yuptools-0.1.4/src/yuptools/models/replace/base.py
--rw-rw-rw-   0        0        0     2034 2023-05-19 06:26:47.000000 yuptools-0.1.4/src/yuptools/models/replace/common.py
--rw-rw-rw-   0        0        0      270 2023-05-19 06:26:47.000000 yuptools-0.1.4/src/yuptools/models/replace/config.py
--rw-rw-rw-   0        0        0     1879 2023-05-19 06:26:47.000000 yuptools-0.1.4/src/yuptools/models/replace/normalization.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:32.228408 yuptools-0.1.4/src/yuptools/models/test/
--rw-rw-rw-   0        0        0       79 2023-05-25 13:39:36.000000 yuptools-0.1.4/src/yuptools/models/test/__init__.py
--rw-rw-rw-   0        0        0     1297 2023-05-25 12:37:07.000000 yuptools-0.1.4/src/yuptools/models/test/accuracy.py
--rw-rw-rw-   0        0        0     3232 2023-05-25 14:07:05.000000 yuptools-0.1.4/src/yuptools/models/test/calibration.py
--rw-rw-rw-   0        0        0     2933 2023-05-24 00:54:12.000000 yuptools-0.1.4/src/yuptools/models/test/linearity.py
--rw-rw-rw-   0        0        0     2464 2023-05-23 23:49:47.000000 yuptools-0.1.4/src/yuptools/models/xray.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:32.340645 yuptools-0.1.4/src/yuptools/plotlib/
--rw-rw-rw-   0        0        0       43 2023-05-31 07:59:55.000000 yuptools-0.1.4/src/yuptools/plotlib/__init__.py
--rw-rw-rw-   0        0        0     2039 2023-05-31 08:53:42.000000 yuptools-0.1.4/src/yuptools/plotlib/bar.py
--rw-rw-rw-   0        0        0     4146 2023-05-31 08:42:30.000000 yuptools-0.1.4/src/yuptools/plotlib/base.py
--rw-rw-rw-   0        0        0     1492 2023-04-21 08:19:35.000000 yuptools-0.1.4/src/yuptools/plotlib/common.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:32.518945 yuptools-0.1.4/src/yuptools/tools/
--rw-rw-rw-   0        0        0      128 2023-05-25 07:16:55.000000 yuptools-0.1.4/src/yuptools/tools/__init__.py
--rw-rw-rw-   0        0        0      287 2023-05-17 21:43:57.000000 yuptools-0.1.4/src/yuptools/tools/attrtools.py
--rw-rw-rw-   0        0        0     1881 2023-05-25 09:04:38.000000 yuptools-0.1.4/src/yuptools/tools/dictools.py
--rw-rw-rw-   0        0        0     1589 2023-05-24 00:34:34.000000 yuptools-0.1.4/src/yuptools/tools/linalgtools.py
--rw-rw-rw-   0        0        0     1482 2023-05-19 01:20:48.000000 yuptools-0.1.4/src/yuptools/tools/listools.py
--rw-rw-rw-   0        0        0     1295 2023-05-17 19:18:18.000000 yuptools-0.1.4/src/yuptools/tools/pathtools.py
--rw-rw-rw-   0        0        0      627 2023-05-22 04:21:26.000000 yuptools-0.1.4/src/yuptools/tools/randtools.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:32.713816 yuptools-0.1.4/src/yuptools/train/
--rw-rw-rw-   0        0        0      152 2023-05-25 08:33:17.000000 yuptools-0.1.4/src/yuptools/train/__init__.py
--rw-rw-rw-   0        0        0     9748 2023-05-25 09:22:49.000000 yuptools-0.1.4/src/yuptools/train/base.py
--rw-rw-rw-   0        0        0      663 2023-05-25 07:46:49.000000 yuptools-0.1.4/src/yuptools/train/criterion.py
--rw-rw-rw-   0        0        0      509 2023-05-25 06:43:18.000000 yuptools-0.1.4/src/yuptools/train/dataloader.py
--rw-rw-rw-   0        0        0     2323 2023-05-25 07:46:00.000000 yuptools-0.1.4/src/yuptools/train/optimizer.py
--rw-rw-rw-   0        0        0     2687 2023-05-25 07:01:42.000000 yuptools-0.1.4/src/yuptools/train/scheduler.py
--rw-rw-rw-   0        0        0      627 2023-05-25 09:22:44.000000 yuptools-0.1.4/src/yuptools/train/trainer.py
--rw-rw-rw-   0        0        0     4104 2023-05-25 07:01:42.000000 yuptools-0.1.4/src/yuptools/train/warmup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:32.859493 yuptools-0.1.4/src/yuptools/travel/
--rw-rw-rw-   0        0        0       49 2023-05-22 03:34:24.000000 yuptools-0.1.4/src/yuptools/travel/__init__.py
--rw-rw-rw-   0        0        0      633 2023-06-26 03:54:06.000000 yuptools-0.1.4/src/yuptools/travel/config.py
--rw-rw-rw-   0        0        0     4784 2023-06-26 04:02:22.000000 yuptools-0.1.4/src/yuptools/travel/direction.py
--rw-rw-rw-   0        0        0     2826 2023-05-22 08:02:00.000000 yuptools-0.1.4/src/yuptools/travel/footprint.py
--rw-rw-rw-   0        0        0     5795 2023-05-22 07:50:16.000000 yuptools-0.1.4/src/yuptools/travel/travel.py
--rw-rw-rw-   0        0        0      675 2023-05-22 03:25:19.000000 yuptools-0.1.4/src/yuptools/travel/warnings.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:32.879117 yuptools-0.1.4/src/yuptools/web/
--rw-rw-rw-   0        0        0       23 2023-05-21 21:08:21.000000 yuptools-0.1.4/src/yuptools/web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:32.943737 yuptools-0.1.4/src/yuptools/web/chrome/
--rw-rw-rw-   0        0        0       23 2023-05-21 21:08:21.000000 yuptools-0.1.4/src/yuptools/web/chrome/__init__.py
--rw-rw-rw-   0        0        0      129 2023-05-21 21:14:42.000000 yuptools-0.1.4/src/yuptools/web/chrome/config.py
--rw-rw-rw-   0        0        0     4115 2023-05-21 21:14:42.000000 yuptools-0.1.4/src/yuptools/web/chrome/driver.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:59:30.779796 yuptools-0.1.4/src/yuptools.egg-info/
--rw-rw-rw-   0        0        0     3198 2023-06-30 03:59:30.000000 yuptools-0.1.4/src/yuptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2601 2023-06-30 03:59:30.000000 yuptools-0.1.4/src/yuptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 03:59:30.000000 yuptools-0.1.4/src/yuptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-06-30 03:59:30.000000 yuptools-0.1.4/src/yuptools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-30 03:59:30.000000 yuptools-0.1.4/src/yuptools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:12.970279 yuptools-0.1.5/
+-rw-rw-rw-   0        0        0     1088 2023-04-21 08:53:14.000000 yuptools-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     3198 2023-07-06 03:09:12.969282 yuptools-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2957 2023-07-06 02:38:18.000000 yuptools-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 03:09:12.970279 yuptools-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-07-06 02:38:18.000000 yuptools-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:07.374738 yuptools-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:07.583166 yuptools-0.1.5/src/yuptools/
+-rw-rw-rw-   0        0        0      240 2023-05-21 22:00:40.000000 yuptools-0.1.5/src/yuptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:08.089270 yuptools-0.1.5/src/yuptools/attacks/
+-rw-rw-rw-   0        0        0       43 2023-05-21 01:50:37.000000 yuptools-0.1.5/src/yuptools/attacks/__init__.py
+-rw-rw-rw-   0        0        0     1943 2023-05-23 23:07:37.000000 yuptools-0.1.5/src/yuptools/attacks/fgsm.py
+-rw-rw-rw-   0        0        0     2872 2023-05-22 04:35:07.000000 yuptools-0.1.5/src/yuptools/attacks/ifgsm.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:08.531937 yuptools-0.1.5/src/yuptools/datasets/
+-rw-rw-rw-   0        0        0       86 2023-05-25 12:15:58.000000 yuptools-0.1.5/src/yuptools/datasets/__init__.py
+-rw-rw-rw-   0        0        0     4145 2023-05-25 08:06:05.000000 yuptools-0.1.5/src/yuptools/datasets/base.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:09.167704 yuptools-0.1.5/src/yuptools/datasets/class_labels/
+-rw-rw-rw-   0        0        0       17 2023-05-25 12:15:58.000000 yuptools-0.1.5/src/yuptools/datasets/class_labels/__init__.py
+-rw-rw-rw-   0        0        0      191 2023-04-19 07:36:49.000000 yuptools-0.1.5/src/yuptools/datasets/class_labels/cifar10.py
+-rw-rw-rw-   0        0        0     1935 2023-04-19 07:36:49.000000 yuptools-0.1.5/src/yuptools/datasets/class_labels/cifar100.py
+-rw-rw-rw-   0        0        0      207 2023-04-20 00:48:17.000000 yuptools-0.1.5/src/yuptools/datasets/class_labels/fashionmnist.py
+-rw-rw-rw-   0        0        0    18494 2023-04-19 10:46:55.000000 yuptools-0.1.5/src/yuptools/datasets/class_labels/imagenet.py
+-rw-rw-rw-   0        0        0      151 2023-04-20 00:52:35.000000 yuptools-0.1.5/src/yuptools/datasets/class_labels/mnist.py
+-rw-rw-rw-   0        0        0     9466 2023-05-21 01:56:33.000000 yuptools-0.1.5/src/yuptools/datasets/image_classification.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:09.300151 yuptools-0.1.5/src/yuptools/models/
+-rw-rw-rw-   0        0        0       97 2023-05-23 23:21:32.000000 yuptools-0.1.5/src/yuptools/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:09.720694 yuptools-0.1.5/src/yuptools/models/classification/
+-rw-rw-rw-   0        0        0       67 2023-05-19 05:42:06.000000 yuptools-0.1.5/src/yuptools/models/classification/__init__.py
+-rw-rw-rw-   0        0        0     5499 2023-05-22 03:46:27.000000 yuptools-0.1.5/src/yuptools/models/classification/base.py
+-rw-rw-rw-   0        0        0     1146 2023-05-19 04:08:19.000000 yuptools-0.1.5/src/yuptools/models/classification/config.py
+-rw-rw-rw-   0        0        0     3122 2023-06-26 07:32:05.000000 yuptools-0.1.5/src/yuptools/models/classification/models.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:10.076670 yuptools-0.1.5/src/yuptools/models/classification/nets/
+-rw-rw-rw-   0        0        0       86 2023-03-22 22:54:35.000000 yuptools-0.1.5/src/yuptools/models/classification/nets/__init__.py
+-rw-rw-rw-   0        0        0     7111 2023-03-03 05:35:17.000000 yuptools-0.1.5/src/yuptools/models/classification/nets/deit.py
+-rw-rw-rw-   0        0        0     6904 2023-03-03 05:35:17.000000 yuptools-0.1.5/src/yuptools/models/classification/nets/mixer.py
+-rw-rw-rw-   0        0        0    23022 2023-03-03 05:35:17.000000 yuptools-0.1.5/src/yuptools/models/classification/nets/poolformer.py
+-rw-rw-rw-   0        0        0    11940 2023-03-03 05:35:17.000000 yuptools-0.1.5/src/yuptools/models/classification/nets/pvt.py
+-rw-rw-rw-   0        0        0      919 2023-05-19 04:46:33.000000 yuptools-0.1.5/src/yuptools/models/classification/warnings.py
+-rw-rw-rw-   0        0        0      705 2023-05-19 02:49:58.000000 yuptools-0.1.5/src/yuptools/models/classification/weights.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:10.472174 yuptools-0.1.5/src/yuptools/models/replace/
+-rw-rw-rw-   0        0        0       68 2023-05-19 06:29:29.000000 yuptools-0.1.5/src/yuptools/models/replace/__init__.py
+-rw-rw-rw-   0        0        0      420 2023-05-19 06:26:47.000000 yuptools-0.1.5/src/yuptools/models/replace/activation.py
+-rw-rw-rw-   0        0        0     1457 2023-05-21 00:57:35.000000 yuptools-0.1.5/src/yuptools/models/replace/base.py
+-rw-rw-rw-   0        0        0     2034 2023-05-19 06:26:47.000000 yuptools-0.1.5/src/yuptools/models/replace/common.py
+-rw-rw-rw-   0        0        0      270 2023-05-19 06:26:47.000000 yuptools-0.1.5/src/yuptools/models/replace/config.py
+-rw-rw-rw-   0        0        0     1879 2023-05-19 06:26:47.000000 yuptools-0.1.5/src/yuptools/models/replace/normalization.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:10.734201 yuptools-0.1.5/src/yuptools/models/test/
+-rw-rw-rw-   0        0        0       79 2023-05-25 13:39:36.000000 yuptools-0.1.5/src/yuptools/models/test/__init__.py
+-rw-rw-rw-   0        0        0     1297 2023-05-25 12:37:07.000000 yuptools-0.1.5/src/yuptools/models/test/accuracy.py
+-rw-rw-rw-   0        0        0     3232 2023-05-25 14:07:05.000000 yuptools-0.1.5/src/yuptools/models/test/calibration.py
+-rw-rw-rw-   0        0        0     2933 2023-05-24 00:54:12.000000 yuptools-0.1.5/src/yuptools/models/test/linearity.py
+-rw-rw-rw-   0        0        0     2464 2023-05-23 23:49:47.000000 yuptools-0.1.5/src/yuptools/models/xray.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:11.035933 yuptools-0.1.5/src/yuptools/plotlib/
+-rw-rw-rw-   0        0        0       43 2023-05-31 07:59:55.000000 yuptools-0.1.5/src/yuptools/plotlib/__init__.py
+-rw-rw-rw-   0        0        0     2039 2023-05-31 08:53:42.000000 yuptools-0.1.5/src/yuptools/plotlib/bar.py
+-rw-rw-rw-   0        0        0     4146 2023-05-31 08:42:30.000000 yuptools-0.1.5/src/yuptools/plotlib/base.py
+-rw-rw-rw-   0        0        0     1492 2023-04-21 08:19:35.000000 yuptools-0.1.5/src/yuptools/plotlib/common.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:11.640707 yuptools-0.1.5/src/yuptools/tools/
+-rw-rw-rw-   0        0        0      128 2023-05-25 07:16:55.000000 yuptools-0.1.5/src/yuptools/tools/__init__.py
+-rw-rw-rw-   0        0        0      287 2023-05-17 21:43:57.000000 yuptools-0.1.5/src/yuptools/tools/attrtools.py
+-rw-rw-rw-   0        0        0     1881 2023-05-25 09:04:38.000000 yuptools-0.1.5/src/yuptools/tools/dictools.py
+-rw-rw-rw-   0        0        0     1589 2023-05-24 00:34:34.000000 yuptools-0.1.5/src/yuptools/tools/linalgtools.py
+-rw-rw-rw-   0        0        0     1482 2023-05-19 01:20:48.000000 yuptools-0.1.5/src/yuptools/tools/listools.py
+-rw-rw-rw-   0        0        0     1295 2023-05-17 19:18:18.000000 yuptools-0.1.5/src/yuptools/tools/pathtools.py
+-rw-rw-rw-   0        0        0      627 2023-05-22 04:21:26.000000 yuptools-0.1.5/src/yuptools/tools/randtools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:12.268935 yuptools-0.1.5/src/yuptools/train/
+-rw-rw-rw-   0        0        0      152 2023-05-25 08:33:17.000000 yuptools-0.1.5/src/yuptools/train/__init__.py
+-rw-rw-rw-   0        0        0     9748 2023-05-25 09:22:49.000000 yuptools-0.1.5/src/yuptools/train/base.py
+-rw-rw-rw-   0        0        0      663 2023-05-25 07:46:49.000000 yuptools-0.1.5/src/yuptools/train/criterion.py
+-rw-rw-rw-   0        0        0      509 2023-05-25 06:43:18.000000 yuptools-0.1.5/src/yuptools/train/dataloader.py
+-rw-rw-rw-   0        0        0     2323 2023-05-25 07:46:00.000000 yuptools-0.1.5/src/yuptools/train/optimizer.py
+-rw-rw-rw-   0        0        0     2687 2023-05-25 07:01:42.000000 yuptools-0.1.5/src/yuptools/train/scheduler.py
+-rw-rw-rw-   0        0        0      627 2023-05-25 09:22:44.000000 yuptools-0.1.5/src/yuptools/train/trainer.py
+-rw-rw-rw-   0        0        0     4104 2023-05-25 07:01:42.000000 yuptools-0.1.5/src/yuptools/train/warmup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:12.670757 yuptools-0.1.5/src/yuptools/travel/
+-rw-rw-rw-   0        0        0       75 2023-07-06 02:38:18.000000 yuptools-0.1.5/src/yuptools/travel/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-06-26 03:54:06.000000 yuptools-0.1.5/src/yuptools/travel/config.py
+-rw-rw-rw-   0        0        0     4784 2023-06-26 04:02:22.000000 yuptools-0.1.5/src/yuptools/travel/direction.py
+-rw-rw-rw-   0        0        0     2826 2023-05-22 08:02:00.000000 yuptools-0.1.5/src/yuptools/travel/footprint.py
+-rw-rw-rw-   0        0        0     5795 2023-05-22 07:50:16.000000 yuptools-0.1.5/src/yuptools/travel/travel.py
+-rw-rw-rw-   0        0        0      675 2023-05-22 03:25:19.000000 yuptools-0.1.5/src/yuptools/travel/warnings.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:12.740211 yuptools-0.1.5/src/yuptools/web/
+-rw-rw-rw-   0        0        0       23 2023-05-21 21:08:21.000000 yuptools-0.1.5/src/yuptools/web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:12.941243 yuptools-0.1.5/src/yuptools/web/chrome/
+-rw-rw-rw-   0        0        0       23 2023-05-21 21:08:21.000000 yuptools-0.1.5/src/yuptools/web/chrome/__init__.py
+-rw-rw-rw-   0        0        0      129 2023-05-21 21:14:42.000000 yuptools-0.1.5/src/yuptools/web/chrome/config.py
+-rw-rw-rw-   0        0        0     4115 2023-05-21 21:14:42.000000 yuptools-0.1.5/src/yuptools/web/chrome/driver.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:09:07.658748 yuptools-0.1.5/src/yuptools.egg-info/
+-rw-rw-rw-   0        0        0     3198 2023-07-06 03:09:07.000000 yuptools-0.1.5/src/yuptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2601 2023-07-06 03:09:07.000000 yuptools-0.1.5/src/yuptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 03:09:07.000000 yuptools-0.1.5/src/yuptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-07-06 03:09:07.000000 yuptools-0.1.5/src/yuptools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 03:09:07.000000 yuptools-0.1.5/src/yuptools.egg-info/top_level.txt
```

### Comparing `yuptools-0.1.4/LICENSE` & `yuptools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/PKG-INFO` & `yuptools-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuptools
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://github.com/yupeeee/YupTools
 Author: Juyeop Kim
 Author-email: juyeopkim@yonsei.ac.kr
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -13,15 +13,15 @@
 YupTools is a Python package based on PyTorch.
 
 ---
 
 
 ## Installation
 
-Latest version: 0.1.4 <br>
+Latest version: 0.1.5 <br>
 **Note: [Manual installation of PyTorch](https://pytorch.org/get-started/locally/) is required.**
 ```
 pip install yuptools==0.1.4
 ```
 
 
 ### Requirements
```

### Comparing `yuptools-0.1.4/README.md` & `yuptools-0.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 YupTools is a Python package based on PyTorch.
 
 ---
 
 
 ## Installation
 
-Latest version: 0.1.4 <br>
+Latest version: 0.1.5 <br>
 **Note: [Manual installation of PyTorch](https://pytorch.org/get-started/locally/) is required.**
 ```
 pip install yuptools==0.1.4
 ```
 
 
 ### Requirements
```

### Comparing `yuptools-0.1.4/setup.py` & `yuptools-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="yuptools",
-    version="0.1.4",
+    version="0.1.5",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Juyeop Kim",
     author_email="juyeopkim@yonsei.ac.kr",
     url="https://github.com/yupeeee/YupTools",
     license="MIT",
```

### Comparing `yuptools-0.1.4/src/yuptools/attacks/fgsm.py` & `yuptools-0.1.5/src/yuptools/attacks/fgsm.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/attacks/ifgsm.py` & `yuptools-0.1.5/src/yuptools/attacks/ifgsm.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/datasets/base.py` & `yuptools-0.1.5/src/yuptools/datasets/base.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/datasets/class_labels/cifar100.py` & `yuptools-0.1.5/src/yuptools/datasets/class_labels/cifar100.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/datasets/class_labels/imagenet.py` & `yuptools-0.1.5/src/yuptools/datasets/class_labels/imagenet.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/datasets/image_classification.py` & `yuptools-0.1.5/src/yuptools/datasets/image_classification.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/models/classification/base.py` & `yuptools-0.1.5/src/yuptools/models/classification/base.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/models/classification/config.py` & `yuptools-0.1.5/src/yuptools/models/classification/config.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/models/classification/models.py` & `yuptools-0.1.5/src/yuptools/models/classification/models.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/models/classification/nets/deit.py` & `yuptools-0.1.5/src/yuptools/models/classification/nets/deit.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/models/classification/nets/mixer.py` & `yuptools-0.1.5/src/yuptools/models/classification/nets/mixer.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/models/classification/nets/poolformer.py` & `yuptools-0.1.5/src/yuptools/models/classification/nets/poolformer.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/models/classification/nets/pvt.py` & `yuptools-0.1.5/src/yuptools/models/classification/nets/pvt.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/models/classification/warnings.py` & `yuptools-0.1.5/src/yuptools/models/classification/warnings.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/models/classification/weights.py` & `yuptools-0.1.5/src/yuptools/models/classification/weights.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/models/replace/base.py` & `yuptools-0.1.5/src/yuptools/models/replace/base.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/models/replace/common.py` & `yuptools-0.1.5/src/yuptools/models/replace/common.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/models/replace/normalization.py` & `yuptools-0.1.5/src/yuptools/models/replace/normalization.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/models/test/accuracy.py` & `yuptools-0.1.5/src/yuptools/models/test/accuracy.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/models/test/calibration.py` & `yuptools-0.1.5/src/yuptools/models/test/calibration.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/models/test/linearity.py` & `yuptools-0.1.5/src/yuptools/models/test/linearity.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/models/xray.py` & `yuptools-0.1.5/src/yuptools/models/xray.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/plotlib/bar.py` & `yuptools-0.1.5/src/yuptools/plotlib/bar.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/plotlib/base.py` & `yuptools-0.1.5/src/yuptools/plotlib/base.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/plotlib/common.py` & `yuptools-0.1.5/src/yuptools/plotlib/common.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/tools/dictools.py` & `yuptools-0.1.5/src/yuptools/tools/dictools.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/tools/linalgtools.py` & `yuptools-0.1.5/src/yuptools/tools/linalgtools.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/tools/listools.py` & `yuptools-0.1.5/src/yuptools/tools/listools.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/tools/pathtools.py` & `yuptools-0.1.5/src/yuptools/tools/pathtools.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/tools/randtools.py` & `yuptools-0.1.5/src/yuptools/tools/randtools.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/train/base.py` & `yuptools-0.1.5/src/yuptools/train/base.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/train/criterion.py` & `yuptools-0.1.5/src/yuptools/train/criterion.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/train/optimizer.py` & `yuptools-0.1.5/src/yuptools/train/optimizer.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/train/scheduler.py` & `yuptools-0.1.5/src/yuptools/train/scheduler.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/train/trainer.py` & `yuptools-0.1.5/src/yuptools/train/trainer.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/train/warmup.py` & `yuptools-0.1.5/src/yuptools/train/warmup.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/travel/config.py` & `yuptools-0.1.5/src/yuptools/travel/config.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/travel/direction.py` & `yuptools-0.1.5/src/yuptools/travel/direction.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/travel/footprint.py` & `yuptools-0.1.5/src/yuptools/travel/footprint.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/travel/travel.py` & `yuptools-0.1.5/src/yuptools/travel/travel.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/travel/warnings.py` & `yuptools-0.1.5/src/yuptools/travel/warnings.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools/web/chrome/driver.py` & `yuptools-0.1.5/src/yuptools/web/chrome/driver.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.4/src/yuptools.egg-info/PKG-INFO` & `yuptools-0.1.5/src/yuptools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuptools
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://github.com/yupeeee/YupTools
 Author: Juyeop Kim
 Author-email: juyeopkim@yonsei.ac.kr
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -13,15 +13,15 @@
 YupTools is a Python package based on PyTorch.
 
 ---
 
 
 ## Installation
 
-Latest version: 0.1.4 <br>
+Latest version: 0.1.5 <br>
 **Note: [Manual installation of PyTorch](https://pytorch.org/get-started/locally/) is required.**
 ```
 pip install yuptools==0.1.4
 ```
 
 
 ### Requirements
```

### Comparing `yuptools-0.1.4/src/yuptools.egg-info/SOURCES.txt` & `yuptools-0.1.5/src/yuptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

