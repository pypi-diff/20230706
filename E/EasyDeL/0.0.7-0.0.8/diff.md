# Comparing `tmp/EasyDeL-0.0.7.tar.gz` & `tmp/EasyDeL-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyDeL-0.0.7.tar", last modified: Fri Jun 30 18:02:36 2023, max compression
+gzip compressed data, was "EasyDeL-0.0.8.tar", last modified: Thu Jul  6 04:44:31 2023, max compression
```

## Comparing `EasyDeL-0.0.7.tar` & `EasyDeL-0.0.8.tar`

### file list

```diff
@@ -1,62 +1,66 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.055000 EasyDeL-0.0.7/
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDeL.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     6365 2023-06-30 18:02:35.000000 EasyDeL-0.0.7/EasyDeL.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1404 2023-06-30 18:02:35.000000 EasyDeL-0.0.7/EasyDeL.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-06-30 18:02:35.000000 EasyDeL-0.0.7/EasyDeL.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2023-06-30 18:02:35.000000 EasyDeL-0.0.7/EasyDeL.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-06-30 18:02:35.000000 EasyDeL-0.0.7/EasyDeL.egg-info/top_level.txt
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1712 2023-06-30 08:03:06.000000 EasyDeL-0.0.7/EasyDel/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/configs/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       78 2023-06-29 05:59:18.000000 EasyDeL-0.0.7/EasyDel/configs/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5646 2023-06-29 05:59:18.000000 EasyDeL-0.0.7/EasyDel/configs/configs.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1284 2023-06-30 08:03:06.000000 EasyDeL-0.0.7/EasyDel/modules/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/falcon/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       88 2023-06-15 12:27:13.000000 EasyDeL-0.0.7/EasyDel/modules/falcon/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    19533 2023-06-29 05:59:18.000000 EasyDeL-0.0.7/EasyDel/modules/falcon/modelling_falcon_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/gpt_j/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      130 2023-06-14 16:25:08.000000 EasyDeL-0.0.7/EasyDel/modules/gpt_j/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    31319 2023-06-14 16:25:08.000000 EasyDeL-0.0.7/EasyDel/modules/gpt_j/modelling_gpt_j_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/gpt_neo_x/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       94 2023-06-23 11:08:05.000000 EasyDeL-0.0.7/EasyDel/modules/gpt_neo_x/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    16080 2023-06-23 11:13:00.000000 EasyDeL-0.0.7/EasyDel/modules/gpt_neo_x/modelling_gpt_neo_x_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/llama/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      150 2023-06-14 16:42:09.000000 EasyDeL-0.0.7/EasyDel/modules/llama/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    34041 2023-06-27 16:24:48.000000 EasyDeL-0.0.7/EasyDel/modules/llama/modelling_llama_flax.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17266 2023-06-26 16:41:56.000000 EasyDeL-0.0.7/EasyDel/modules/llama/modelling_llama_pytorch.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/lucid_transformer/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       95 2023-06-14 16:25:08.000000 EasyDeL-0.0.7/EasyDel/modules/lucid_transformer/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    13472 2023-06-29 05:59:18.000000 EasyDeL-0.0.7/EasyDel/modules/lucid_transformer/modelling_lt_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/mosaic_mpt/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       76 2023-06-14 16:34:35.000000 EasyDeL-0.0.7/EasyDel/modules/mosaic_mpt/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17799 2023-06-22 04:42:44.000000 EasyDeL-0.0.7/EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/palm/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       76 2023-06-30 08:01:08.000000 EasyDeL-0.0.7/EasyDel/modules/palm/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    16353 2023-06-30 07:08:03.000000 EasyDeL-0.0.7/EasyDel/modules/palm/modelling_palm_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/t5/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       75 2023-06-30 08:01:08.000000 EasyDeL-0.0.7/EasyDel/modules/t5/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    59589 2023-06-30 07:56:15.000000 EasyDeL-0.0.7/EasyDel/modules/t5/modelling_t5_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/serve/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-18 16:37:39.000000 EasyDeL-0.0.7/EasyDel/serve/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1482 2023-06-18 16:37:39.000000 EasyDeL-0.0.7/EasyDel/serve/serve_utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.055000 EasyDeL-0.0.7/EasyDel/trainer/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      146 2023-06-26 17:06:26.000000 EasyDeL-0.0.7/EasyDel/trainer/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8944 2023-06-29 08:35:15.000000 EasyDeL-0.0.7/EasyDel/trainer/config.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    21478 2023-06-29 05:59:18.000000 EasyDeL-0.0.7/EasyDel/trainer/fsdp_train.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.055000 EasyDeL-0.0.7/EasyDel/utils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      402 2023-06-14 16:25:08.000000 EasyDeL-0.0.7/EasyDel/utils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      389 2023-06-14 16:25:08.000000 EasyDeL-0.0.7/EasyDel/utils/checker.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4584 2023-06-26 16:41:56.000000 EasyDeL-0.0.7/EasyDel/utils/utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.055000 EasyDeL-0.0.7/EasyDel/weight_convertor/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-06-15 13:20:11.000000 EasyDeL-0.0.7/EasyDel/weight_convertor/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     6215 2023-06-18 16:37:39.000000 EasyDeL-0.0.7/EasyDel/weight_convertor/falcon.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5077 2023-06-22 11:28:16.000000 EasyDeL-0.0.7/EasyDel/weight_convertor/llama.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9833 2023-06-18 16:37:39.000000 EasyDeL-0.0.7/EasyDel/weight_convertor/mpt.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      858 2023-06-18 16:37:39.000000 EasyDeL-0.0.7/EasyDel/weight_convertor/utils.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-14 16:25:08.000000 EasyDeL-0.0.7/LICENSE
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     6365 2023-06-30 18:02:36.055000 EasyDeL-0.0.7/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5471 2023-06-30 07:58:59.000000 EasyDeL-0.0.7/README.md
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      608 2023-06-23 10:45:58.000000 EasyDeL-0.0.7/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-30 18:02:36.055000 EasyDeL-0.0.7/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1124 2023-06-30 08:08:21.000000 EasyDeL-0.0.7/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.864133 EasyDeL-0.0.8/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.848134 EasyDeL-0.0.8/EasyDeL.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6365 2023-07-06 04:44:31.000000 EasyDeL-0.0.8/EasyDeL.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1512 2023-07-06 04:44:31.000000 EasyDeL-0.0.8/EasyDeL.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-07-06 04:44:31.000000 EasyDeL-0.0.8/EasyDeL.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2023-07-06 04:44:31.000000 EasyDeL-0.0.8/EasyDeL.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-07-06 04:44:31.000000 EasyDeL-0.0.8/EasyDeL.egg-info/top_level.txt
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.852134 EasyDeL-0.0.8/EasyDel/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1892 2023-07-06 04:43:45.000000 EasyDeL-0.0.8/EasyDel/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.852134 EasyDeL-0.0.8/EasyDel/configs/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       91 2023-07-06 04:35:58.000000 EasyDeL-0.0.8/EasyDel/configs/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9145 2023-07-06 04:35:58.000000 EasyDeL-0.0.8/EasyDel/configs/configs.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.852134 EasyDeL-0.0.8/EasyDel/modules/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1428 2023-07-06 04:25:19.000000 EasyDeL-0.0.8/EasyDel/modules/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.852134 EasyDeL-0.0.8/EasyDel/modules/falcon/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       88 2023-06-15 12:27:13.000000 EasyDeL-0.0.8/EasyDel/modules/falcon/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    19533 2023-06-29 05:59:18.000000 EasyDeL-0.0.8/EasyDel/modules/falcon/modelling_falcon_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.852134 EasyDeL-0.0.8/EasyDel/modules/gpt_j/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      130 2023-06-14 16:25:08.000000 EasyDeL-0.0.8/EasyDel/modules/gpt_j/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    31319 2023-06-14 16:25:08.000000 EasyDeL-0.0.8/EasyDel/modules/gpt_j/modelling_gpt_j_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.852134 EasyDeL-0.0.8/EasyDel/modules/gpt_neo_x/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       94 2023-06-23 11:08:05.000000 EasyDeL-0.0.8/EasyDel/modules/gpt_neo_x/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    16080 2023-06-23 11:13:00.000000 EasyDeL-0.0.8/EasyDel/modules/gpt_neo_x/modelling_gpt_neo_x_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.852134 EasyDeL-0.0.8/EasyDel/modules/llama/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      150 2023-06-14 16:42:09.000000 EasyDeL-0.0.8/EasyDel/modules/llama/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    34041 2023-06-27 16:24:48.000000 EasyDeL-0.0.8/EasyDel/modules/llama/modelling_llama_flax.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17266 2023-06-26 16:41:56.000000 EasyDeL-0.0.8/EasyDel/modules/llama/modelling_llama_pytorch.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.856134 EasyDeL-0.0.8/EasyDel/modules/lucid_transformer/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       95 2023-06-14 16:25:08.000000 EasyDeL-0.0.8/EasyDel/modules/lucid_transformer/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    13472 2023-06-29 05:59:18.000000 EasyDeL-0.0.8/EasyDel/modules/lucid_transformer/modelling_lt_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.856134 EasyDeL-0.0.8/EasyDel/modules/mosaic_mpt/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       76 2023-06-14 16:34:35.000000 EasyDeL-0.0.8/EasyDel/modules/mosaic_mpt/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17799 2023-06-22 04:42:44.000000 EasyDeL-0.0.8/EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.856134 EasyDeL-0.0.8/EasyDel/modules/opt/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       76 2023-07-06 04:25:19.000000 EasyDeL-0.0.8/EasyDel/modules/opt/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    29993 2023-07-06 04:19:00.000000 EasyDeL-0.0.8/EasyDel/modules/opt/modelling_opt_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.860134 EasyDeL-0.0.8/EasyDel/modules/palm/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       76 2023-06-30 08:01:08.000000 EasyDeL-0.0.8/EasyDel/modules/palm/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    16353 2023-06-30 07:08:03.000000 EasyDeL-0.0.8/EasyDel/modules/palm/modelling_palm_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.860134 EasyDeL-0.0.8/EasyDel/modules/t5/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       85 2023-07-06 04:19:25.000000 EasyDeL-0.0.8/EasyDel/modules/t5/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    59589 2023-06-30 07:56:15.000000 EasyDeL-0.0.8/EasyDel/modules/t5/modelling_t5_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.860134 EasyDeL-0.0.8/EasyDel/serve/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-18 16:37:39.000000 EasyDeL-0.0.8/EasyDel/serve/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1482 2023-06-18 16:37:39.000000 EasyDeL-0.0.8/EasyDel/serve/serve_utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.860134 EasyDeL-0.0.8/EasyDel/trainer/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      219 2023-07-06 04:43:45.000000 EasyDeL-0.0.8/EasyDel/trainer/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8944 2023-06-29 08:35:15.000000 EasyDeL-0.0.8/EasyDel/trainer/config.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    22483 2023-07-06 04:19:25.000000 EasyDeL-0.0.8/EasyDel/trainer/fsdp_train.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9443 2023-07-06 04:43:45.000000 EasyDeL-0.0.8/EasyDel/trainer/training_utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.860134 EasyDeL-0.0.8/EasyDel/utils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      402 2023-06-14 16:25:08.000000 EasyDeL-0.0.8/EasyDel/utils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      389 2023-06-14 16:25:08.000000 EasyDeL-0.0.8/EasyDel/utils/checker.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4584 2023-06-26 16:41:56.000000 EasyDeL-0.0.8/EasyDel/utils/utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.864133 EasyDeL-0.0.8/EasyDel/weight_convertor/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-06-15 13:20:11.000000 EasyDeL-0.0.8/EasyDel/weight_convertor/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6215 2023-06-18 16:37:39.000000 EasyDeL-0.0.8/EasyDel/weight_convertor/falcon.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5077 2023-06-22 11:28:16.000000 EasyDeL-0.0.8/EasyDel/weight_convertor/llama.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9833 2023-06-18 16:37:39.000000 EasyDeL-0.0.8/EasyDel/weight_convertor/mpt.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      858 2023-06-18 16:37:39.000000 EasyDeL-0.0.8/EasyDel/weight_convertor/utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-14 16:25:08.000000 EasyDeL-0.0.8/LICENSE
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6365 2023-07-06 04:44:31.864133 EasyDeL-0.0.8/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5471 2023-06-30 07:58:59.000000 EasyDeL-0.0.8/README.md
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      608 2023-06-23 10:45:58.000000 EasyDeL-0.0.8/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-07-06 04:44:31.864133 EasyDeL-0.0.8/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1124 2023-07-06 04:43:54.000000 EasyDeL-0.0.8/setup.py
```

### Comparing `EasyDeL-0.0.7/EasyDeL.egg-info/PKG-INFO` & `EasyDeL-0.0.8/EasyDeL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyDeL
-Version: 0.0.7
+Version: 0.0.8
 Summary: An open-source library to make training faster and more optimized in Jax/Flax
 Home-page: https://github.com/erfanzar/EasyDeL
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@eyahoo.com
 License: UNKNOWN
 Keywords: machine learning,deep learning,pytorch
 Platform: UNKNOWN
```

### Comparing `EasyDeL-0.0.7/EasyDeL.egg-info/SOURCES.txt` & `EasyDeL-0.0.8/EasyDeL.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -20,23 +20,26 @@
 EasyDel/modules/llama/__init__.py
 EasyDel/modules/llama/modelling_llama_flax.py
 EasyDel/modules/llama/modelling_llama_pytorch.py
 EasyDel/modules/lucid_transformer/__init__.py
 EasyDel/modules/lucid_transformer/modelling_lt_flax.py
 EasyDel/modules/mosaic_mpt/__init__.py
 EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py
+EasyDel/modules/opt/__init__.py
+EasyDel/modules/opt/modelling_opt_flax.py
 EasyDel/modules/palm/__init__.py
 EasyDel/modules/palm/modelling_palm_flax.py
 EasyDel/modules/t5/__init__.py
 EasyDel/modules/t5/modelling_t5_flax.py
 EasyDel/serve/__init__.py
 EasyDel/serve/serve_utils.py
 EasyDel/trainer/__init__.py
 EasyDel/trainer/config.py
 EasyDel/trainer/fsdp_train.py
+EasyDel/trainer/training_utils.py
 EasyDel/utils/__init__.py
 EasyDel/utils/checker.py
 EasyDel/utils/utils.py
 EasyDel/weight_convertor/__init__.py
 EasyDel/weight_convertor/falcon.py
 EasyDel/weight_convertor/llama.py
 EasyDel/weight_convertor/mpt.py
```

### Comparing `EasyDeL-0.0.7/EasyDel/__init__.py` & `EasyDeL-0.0.8/EasyDel/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 if is_tensorflow_available():
     ...
 if is_flax_available():
     from .modules import FlaxLlamaModel, LlamaConfig, FlaxLlamaForCausalLM, LlamaModel, LlamaForCausalLM, \
         FlaxLTModelModule, FlaxLTConfig, FlaxLTForCausalLM, FlaxLTModel, GPTJConfig, FlaxGPTJModule, \
         FlaxGPTJForCausalLMModule, FlaxGPTJModel, FlaxGPTJForCausalLM, FlaxMptForCausalLM, MptConfig, FlaxMptModel, \
         FlaxFalconForCausalLM, FlaxFalconModel, FalconConfig, FlaxGPTNeoXForCausalLM, GPTNeoXConfig, FlaxGPTNeoXModel, \
-        FlaxT5ForConditionalGeneration, FlaxT5Model, FlaxPalmForCausalLM, PalmModel, PalmConfig
-from .trainer import finetuner, TrainArguments, fsdp_train_step
+        FlaxT5ForConditionalGeneration, FlaxT5Model, FlaxPalmForCausalLM, PalmModel, PalmConfig, T5Config, \
+        FlaxOPTForCausalLM, FlaxOPTModel, OPTConfig
+from .trainer import finetuner, TrainArguments, fsdp_train_step, get_training_modules
 
 __all__ = __version__, 'package_checker', 'is_jax_available', 'is_torch_available', 'is_flax_available', \
-    'is_tensorflow_available', "finetuner", "TrainArguments", "fsdp_train_step", \
+    'is_tensorflow_available', "finetuner", "TrainArguments", "fsdp_train_step", 'get_training_modules', \
     'LlamaConfig', 'LlamaForCausalLM', 'LlamaModel', 'FlaxLlamaForCausalLM', \
     'FlaxLlamaModel', 'FlaxGPTJModule', 'FlaxGPTJForCausalLMModule', \
     'FlaxGPTJModel', 'FlaxGPTJForCausalLM', 'GPTJConfig', \
     'FlaxLTModel', 'FlaxLTConfig', 'FlaxLTModelModule', 'FlaxLTForCausalLM', \
     "FlaxMptForCausalLM", "MptConfig", "FlaxMptModel", \
     "FlaxFalconForCausalLM", "FlaxFalconModel", "FalconConfig", \
     "FlaxGPTNeoXForCausalLM", "GPTNeoXConfig", "FlaxGPTNeoXModel", \
     "FlaxT5ForConditionalGeneration", "FlaxT5Model", \
-    "FlaxPalmForCausalLM", "PalmModel", "PalmConfig"
+    "FlaxPalmForCausalLM", "PalmModel", "PalmConfig", 'T5Config', \
+    "FlaxOPTForCausalLM", "FlaxOPTModel", "OPTConfig"
```

### Comparing `EasyDeL-0.0.7/EasyDel/configs/configs.py` & `EasyDeL-0.0.8/EasyDel/configs/configs.py`

 * *Files 24% similar despite different names*

```diff
@@ -203,7 +203,128 @@
         "n_layer": 60,
         "parallel_attn": True,
         "torch_dtype": "bfloat16",
         "use_cache": True,
         "vocab_size": 65024
     }
 }
+
+opt_configs = {
+    '1.3b': {
+        {
+            "activation_dropout": 0.0,
+            "activation_function": "relu",
+            "attention_dropout": 0.0,
+            "bos_token_id": 2,
+            "do_layer_norm_before": True,
+            "dropout": 0.1,
+            "eos_token_id": 2,
+            "ffn_dim": 8192,
+            "hidden_size": 2048,
+            "init_std": 0.02,
+            "layerdrop": 0.0,
+            "max_position_embeddings": 2048,
+            "model_type": "opt",
+            "num_attention_heads": 32,
+            "num_hidden_layers": 24,
+            "pad_token_id": 1,
+            "prefix": "</s>",
+            "use_cache": True,
+            "vocab_size": 50272,
+            "word_embed_proj_dim": 2048
+        }
+    },
+    '6.7b': {
+        "_remove_final_layer_norm": False,
+        "activation_dropout": 0.0,
+        "activation_function": "relu",
+        "attention_dropout": 0.0,
+        "bos_token_id": 2,
+        "do_layer_norm_before": True,
+        "dropout": 0.1,
+        "eos_token_id": 2,
+        "ffn_dim": 16384,
+        "hidden_size": 4096,
+        "init_std": 0.02,
+        "layerdrop": 0.0,
+        "max_position_embeddings": 2048,
+        "model_type": "opt",
+        "num_attention_heads": 32,
+        "num_hidden_layers": 32,
+        "pad_token_id": 1,
+        "prefix": "</s>",
+        "use_cache": True,
+        "vocab_size": 50272,
+        "word_embed_proj_dim": 4096
+    },
+    '66b': {
+        "_remove_final_layer_norm": False,
+        "activation_dropout": 0.0,
+        "activation_function": "relu",
+        "attention_dropout": 0.0,
+        "bos_token_id": 2,
+        "do_layer_norm_before": True,
+        "dropout": 0.1,
+        "eos_token_id": 2,
+        "ffn_dim": 36864,
+        "hidden_size": 9216,
+        "init_std": 0.02,
+        "layerdrop": 0.0,
+        "max_position_embeddings": 2048,
+        "model_type": "opt",
+        "num_attention_heads": 72,
+        "num_hidden_layers": 64,
+        "pad_token_id": 1,
+        "prefix": "</s>",
+        "use_cache": True,
+        "vocab_size": 50272,
+        "word_embed_proj_dim": 9216
+    },
+    '13b': {
+        "_name_or_path": "facebook/opt-13b",
+        "_remove_final_layer_norm": False,
+        "activation_dropout": 0.0,
+        "activation_function": "relu",
+        "attention_dropout": 0.0,
+        "bos_token_id": 2,
+        "do_layer_norm_before": True,
+        "dropout": 0.1,
+        "eos_token_id": 2,
+        "ffn_dim": 20480,
+        "hidden_size": 5120,
+        "init_std": 0.02,
+        "layerdrop": 0.0,
+        "max_position_embeddings": 2048,
+        "model_type": "opt",
+        "num_attention_heads": 40,
+        "num_hidden_layers": 40,
+        "output_projection": True,
+        "pad_token_id": 1,
+        "prefix": "</s>",
+        "use_cache": True,
+        "vocab_size": 50272,
+        "word_embed_proj_dim": 5120
+    },
+    '350m': {
+        "activation_dropout": 0.0,
+        "activation_function": "relu",
+        "attention_dropout": 0.0,
+        "bos_token_id": 2,
+        "do_layer_norm_before": False,
+        "dropout": 0.1,
+        "eos_token_id": 2,
+        "ffn_dim": 4096,
+        "hidden_size": 1024,
+        "init_std": 0.02,
+        "layerdrop": 0.0,
+        "max_position_embeddings": 2048,
+        "model_type": "opt",
+        "num_attention_heads": 16,
+        "num_hidden_layers": 24,
+        "pad_token_id": 1,
+        "prefix": "</s>",
+        "use_cache": True,
+        "vocab_size": 50272,
+        "word_embed_proj_dim": 512
+
+    }
+}
```

### Comparing `EasyDeL-0.0.7/EasyDel/modules/__init__.py` & `EasyDeL-0.0.8/EasyDel/modules/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from .llama import LlamaConfig, LlamaModel, LlamaForCausalLM, FlaxLlamaModel, FlaxLlamaForCausalLM
 from .gpt_j import FlaxGPTJModule, FlaxGPTJForCausalLMModule, FlaxGPTJModel, FlaxGPTJForCausalLM, GPTJConfig
 from .lucid_transformer import FlaxLTModel, FlaxLTConfig, FlaxLTModelModule, FlaxLTForCausalLM
 from .mosaic_mpt import MptConfig, FlaxMptModel, FlaxMptForCausalLM
 from .falcon import FalconConfig, FlaxFalconModel, FlaxFalconForCausalLM
 from .gpt_neo_x import FlaxGPTNeoXForCausalLM, GPTNeoXConfig, FlaxGPTNeoXModel
 from .palm import PalmConfig, PalmModel, FlaxPalmForCausalLM
-from .t5 import FlaxT5ForConditionalGeneration, FlaxT5Model
+from .t5 import FlaxT5ForConditionalGeneration, FlaxT5Model, T5Config
+from .opt import FlaxOPTForCausalLM, FlaxOPTModel, OPTConfig
 
 __all__ = ['LlamaConfig', 'LlamaForCausalLM', 'LlamaModel', 'FlaxLlamaForCausalLM', 'FlaxLlamaModel',
            'FlaxGPTJModule', 'FlaxGPTJForCausalLMModule', 'FlaxGPTJModel', 'FlaxGPTJForCausalLM', 'GPTJConfig',
            'FlaxLTModel', 'FlaxLTConfig', 'FlaxLTModelModule', 'FlaxLTForCausalLM',
            "MptConfig", "FlaxMptModel", "FlaxMptForCausalLM",
            "FalconConfig", "FlaxFalconModel", "FlaxFalconForCausalLM",
            "FlaxGPTNeoXForCausalLM", "GPTNeoXConfig", "FlaxGPTNeoXModel",
            "FlaxT5ForConditionalGeneration", "FlaxT5Model",
-           "PalmConfig", "PalmModel", "FlaxPalmForCausalLM"
-
+           "PalmConfig", "PalmModel", "FlaxPalmForCausalLM", 'T5Config',
+           "FlaxOPTForCausalLM", "FlaxOPTModel", "OPTConfig"
            ]
```

### Comparing `EasyDeL-0.0.7/EasyDel/modules/falcon/modelling_falcon_flax.py` & `EasyDeL-0.0.8/EasyDel/modules/falcon/modelling_falcon_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/EasyDel/modules/gpt_j/modelling_gpt_j_flax.py` & `EasyDeL-0.0.8/EasyDel/modules/gpt_j/modelling_gpt_j_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/EasyDel/modules/gpt_neo_x/modelling_gpt_neo_x_flax.py` & `EasyDeL-0.0.8/EasyDel/modules/gpt_neo_x/modelling_gpt_neo_x_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/EasyDel/modules/llama/modelling_llama_flax.py` & `EasyDeL-0.0.8/EasyDel/modules/llama/modelling_llama_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/EasyDel/modules/llama/modelling_llama_pytorch.py` & `EasyDeL-0.0.8/EasyDel/modules/llama/modelling_llama_pytorch.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/EasyDel/modules/lucid_transformer/modelling_lt_flax.py` & `EasyDeL-0.0.8/EasyDel/modules/lucid_transformer/modelling_lt_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py` & `EasyDeL-0.0.8/EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/EasyDel/modules/palm/modelling_palm_flax.py` & `EasyDeL-0.0.8/EasyDel/modules/palm/modelling_palm_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/EasyDel/modules/t5/modelling_t5_flax.py` & `EasyDeL-0.0.8/EasyDel/modules/t5/modelling_t5_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/EasyDel/serve/serve_utils.py` & `EasyDeL-0.0.8/EasyDel/serve/serve_utils.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/EasyDel/trainer/config.py` & `EasyDeL-0.0.8/EasyDel/trainer/config.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/EasyDel/trainer/fsdp_train.py` & `EasyDeL-0.0.8/EasyDel/trainer/fsdp_train.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,28 @@
 from jax.experimental.pjit import pjit, with_sharding_constraint, PartitionSpec
 from flax.training import train_state
 from jax import numpy as jnp
 from torch.utils.data import DataLoader
 from fjutils import match_partition_rules, make_shard_and_gather_fns, StreamingCheckpointer, count_params
 
 
-def fsdp_train_step(state, batch):
+def fsdp_train_step(state, batch, label_in_the_field=False, scope_logits=True):
     batch = with_sharding_constraint(batch, PartitionSpec(('dp', 'fsdp')))
 
     def calculate_loss(params):
         logits = state.apply_fn(params=params, **batch,
                                 return_dict=True).logits
-        loss = optax.softmax_cross_entropy_with_integer_labels(logits=logits[..., :-1, :],
-                                                               labels=batch['input_ids'][..., 1:])
+        if label_in_the_field:
+            loss = optax.softmax_cross_entropy_with_integer_labels(
+                logits=logits[..., :-1, :] if scope_logits else logits,
+                labels=batch['label'])
+        else:
+            loss = optax.softmax_cross_entropy_with_integer_labels(
+                logits=logits[..., :-1, :] if scope_logits else logits,
+                labels=batch['input_ids'][..., 1:])
         loss = jnp.mean(loss)
         return loss
 
     grad_fn = jax.value_and_grad(calculate_loss, has_aux=False)
     loss__, grad = grad_fn(state.params)
     state = state.apply_gradients(grads=grad)
     return state, loss__
@@ -90,15 +96,17 @@
         extra_configs=None,
         ids_to_pop_from_dataset=[],
         remove_ckpt_after_load: bool = False,
         model_class=None,
         configs_to_init_model_class=None,
         do_last_save: bool = True,
         model_parameters=None,
-        do_shard_fns=True
+        do_shard_fns: bool = True,
+        label_in_the_field: bool = False,
+        scope_logits: bool = True
 ) -> OutputFineTuner:
     if extra_configs is None:
         extra_configs = {}
     timer = Timers(
         use_wandb=False,
         tensorboard_writer=training_arguments.get_board()
     )
@@ -188,15 +196,15 @@
         create_train_state_from_params,
         in_shardings=(train_state_partition_spec.params,),
         out_shardings=train_state_partition_spec,
         donate_argnums=(0,)
     )
     sharded_train_step_fn = pjit(
         fsdp_train_step,
-        in_shardings=(train_state_partition_spec, PartitionSpec()),
+        in_shardings=(train_state_partition_spec, PartitionSpec(), PartitionSpec(), PartitionSpec()),
         out_shardings=(train_state_partition_spec, PartitionSpec()),
         donate_argnums=(0, 0, 0),
     )
     sharded_predict = pjit(predict, out_shardings=PartitionSpec(),
                            in_shardings=(train_state_partition_spec, PartitionSpec()))
     mesh = training_arguments.get_mesh()
     training_arguments.ckpt_path_exists()
@@ -239,15 +247,16 @@
                 for batch in dataloader_train:
                     i += 1
                     if i < max_steps_train:
 
                         _ = batch.pop('token_type_ids', None)
                         for i in ids_to_pop_from_dataset:
                             _ = batch.pop(i, None)
-                        sharded_train_state_, loss = sharded_train_step_fn(sharded_train_state_, batch)
+                        sharded_train_state_, loss = sharded_train_step_fn(sharded_train_state_, batch,
+                                                                           label_in_the_field, scope_logits)
                         losses.append(loss)
                         learning_rates.append(scheduler(i).tolist())
                         pbar.update(1)
                         # clear_output(True)
                         if use_wandb:
                             wandb_runtime.log(
                                 {'loss': loss.tolist(),
@@ -313,15 +322,17 @@
         fully_fsdp=True,
         use_wandb: bool = True,
         custom_rule=None,
         extra_configs=None,
         ids_to_pop_from_dataset=[],
         model_class=None,
         configs_to_init_model_class=None,
-        do_last_save: bool = True
+        do_last_save: bool = True,
+        label_in_the_field=False,
+        scope_logits=True
 ) -> OutputFineTuner:
     if extra_configs is None:
         extra_configs = {}
     timer = Timers(
         use_wandb=False,
         tensorboard_writer=training_arguments.get_board()
     )
@@ -416,56 +427,65 @@
         create_train_state_from_params,
         in_shardings=(train_state_partition_spec.params,),
         out_shardings=train_state_partition_spec,
         donate_argnums=(0,)
     )
     sharded_train_step_fn = pjit(
         fsdp_train_step,
-        in_shardings=(train_state_partition_spec, PartitionSpec()),
+        in_shardings=(train_state_partition_spec, PartitionSpec(), PartitionSpec(), PartitionSpec()),
         out_shardings=(train_state_partition_spec, PartitionSpec()),
         donate_argnums=(0, 0, 0),
     )
     sharded_predict = pjit(predict, out_shardings=PartitionSpec(),
                            in_shardings=(train_state_partition_spec, PartitionSpec()))
     mesh = training_arguments.get_mesh()
     training_arguments.ckpt_path_exists()
     ckpt_streamer = training_arguments.get_streaming_checkpointer()
     timer(
         'creating functions'
     ).stop()
     timer.log(['creating functions'])
+
     with mesh:
         timer(
             'loading parameters'
         ).start()
         shard_fns, gather_fns = make_shard_and_gather_fns(train_state_partition_spec, dtype_specs=dtype)
         params = sharded_init_fn()
 
         sharded_train_state_ = sharded_create_from_params_fn(params)
         timer(
             'loading parameters'
         ).stop()
         timer.log(['loading parameters'])
         count_params(sharded_train_state_.params)
-
+        if use_wandb:
+            wandb_runtime.log(
+                {
+                    'model billion parameters': sum(
+                        i.size for i in
+                        jax.tree_util.tree_flatten(flax.core.unfreeze(sharded_train_state_.params))[0]) / 1e9
+                }
+            )
         timer.write(timer.timers.keys(), 0)
         pbar = tqdm(total=max_steps_train)
         i = sharded_train_state_.step.tolist()
         losses = []
         pbar.update(sharded_train_state_.step.tolist())
         learning_rates = []
         for ep in range(training_arguments.num_train_epochs):
             for batch in dataloader_train:
                 i += 1
                 if i < max_steps_train:
 
                     _ = batch.pop('token_type_ids', None)
                     for i in ids_to_pop_from_dataset:
                         _ = batch.pop(i, None)
-                    sharded_train_state_, loss = sharded_train_step_fn(sharded_train_state_, batch)
+                    sharded_train_state_, loss = sharded_train_step_fn(sharded_train_state_, batch,
+                                                                       label_in_the_field, scope_logits)
                     losses.append(loss)
                     learning_rates.append(scheduler(i).tolist())
                     pbar.update(1)
                     # clear_output(True)
                     if use_wandb:
                         wandb_runtime.log(
                             {'loss': loss.tolist(),
```

### Comparing `EasyDeL-0.0.7/EasyDel/utils/utils.py` & `EasyDeL-0.0.8/EasyDel/utils/utils.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/EasyDel/weight_convertor/falcon.py` & `EasyDeL-0.0.8/EasyDel/weight_convertor/falcon.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/EasyDel/weight_convertor/llama.py` & `EasyDeL-0.0.8/EasyDel/weight_convertor/llama.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/EasyDel/weight_convertor/mpt.py` & `EasyDeL-0.0.8/EasyDel/weight_convertor/mpt.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/EasyDel/weight_convertor/utils.py` & `EasyDeL-0.0.8/EasyDel/weight_convertor/utils.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/LICENSE` & `EasyDeL-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/PKG-INFO` & `EasyDeL-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyDeL
-Version: 0.0.7
+Version: 0.0.8
 Summary: An open-source library to make training faster and more optimized in Jax/Flax
 Home-page: https://github.com/erfanzar/EasyDeL
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@eyahoo.com
 License: UNKNOWN
 Keywords: machine learning,deep learning,pytorch
 Platform: UNKNOWN
```

### Comparing `EasyDeL-0.0.7/README.md` & `EasyDeL-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/pyproject.toml` & `EasyDeL-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.7/setup.py` & `EasyDeL-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='EasyDeL',
-    version='0.0.7',
+    version='0.0.8',
     author='Erfan Zare Chavoshi',
     author_email='erfanzare82@eyahoo.com',
     description='An open-source library to make training faster and more optimized in Jax/Flax',
     url='https://github.com/erfanzar/EasyDeL',
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

