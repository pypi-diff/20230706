# Comparing `tmp/landingai-0.0.8.tar.gz` & `tmp/landingai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingai-0.0.8.tar", max compression
+gzip compressed data, was "landingai-0.1.1.tar", max compression
```

## Comparing `landingai-0.0.8.tar` & `landingai-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,25 @@
--rw-r--r--   0        0        0     4098 2023-05-13 04:21:18.893710 landingai-0.0.8/README.md
--rw-r--r--   0        0        0       40 2023-05-11 23:35:20.932651 landingai-0.0.8/landingai/__init__.py
--rw-r--r--   0        0        0     3372 2023-05-12 22:53:01.555726 landingai-0.0.8/landingai/common.py
--rw-r--r--   0        0        0     7385 2023-05-13 03:23:15.112923 landingai-0.0.8/landingai/predict.py
--rw-r--r--   0        0        0     2107 2023-05-12 22:53:01.563372 landingai-0.0.8/landingai/visualize.py
--rw-r--r--   0        0        0     1194 2023-05-13 04:19:48.542411 landingai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4990 1970-01-01 00:00:00.000000 landingai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-06 21:38:20.297719 landingai-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     6741 2023-07-06 21:38:20.297719 landingai-0.1.1/README.md
+-rw-r--r--   0        0        0      354 2023-07-06 21:38:20.329719 landingai-0.1.1/landingai/__init__.py
+-rw-r--r--   0        0        0     6833 2023-07-06 21:38:20.329719 landingai-0.1.1/landingai/common.py
+-rw-r--r--   0        0        0       72 2023-07-06 21:38:20.329719 landingai-0.1.1/landingai/data_management/__init__.py
+-rw-r--r--   0        0        0     8458 2023-07-06 21:38:20.329719 landingai-0.1.1/landingai/data_management/client.py
+-rw-r--r--   0        0        0    19329 2023-07-06 21:38:20.329719 landingai-0.1.1/landingai/data_management/media.py
+-rw-r--r--   0        0        0     4236 2023-07-06 21:38:20.329719 landingai-0.1.1/landingai/data_management/metadata.py
+-rw-r--r--   0        0        0     2188 2023-07-06 21:38:20.329719 landingai-0.1.1/landingai/data_management/utils.py
+-rw-r--r--   0        0        0     9418 2023-07-06 21:38:20.329719 landingai-0.1.1/landingai/exceptions.py
+-rw-r--r--   0        0        0  1594400 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     6843 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/io.py
+-rw-r--r--   0        0        0      221 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/pipeline/__init__.py
+-rw-r--r--   0        0        0     5287 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/pipeline/image_source.py
+-rw-r--r--   0        0        0     4841 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/postprocess.py
+-rw-r--r--   0        0        0    25157 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/predict.py
+-rw-r--r--   0        0        0     6068 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/st_utils.py
+-rw-r--r--   0        0        0       40 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/storage/__init__.py
+-rw-r--r--   0        0        0     4374 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/storage/snowflake.py
+-rw-r--r--   0        0        0     1685 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/transform.py
+-rw-r--r--   0        0        0     1598 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/utils.py
+-rw-r--r--   0        0        0    23703 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/vision_pipeline.py
+-rw-r--r--   0        0        0    13403 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/visualize.py
+-rw-r--r--   0        0        0     2487 2023-07-06 21:38:21.005723 landingai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7986 1970-01-01 00:00:00.000000 landingai-0.1.1/PKG-INFO
```

