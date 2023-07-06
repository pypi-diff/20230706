# Comparing `tmp/bytetrade-recommend-model-sdk-0.0.23.tar.gz` & `tmp/bytetrade-recommend-model-sdk-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.23.tar", last modified: Mon Jul  3 09:57:44 2023, max compression
+gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.24.tar", last modified: Thu Jul  6 02:18:17 2023, max compression
```

## Comparing `bytetrade-recommend-model-sdk-0.0.23.tar` & `bytetrade-recommend-model-sdk-0.0.24.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 09:57:44.061485 bytetrade-recommend-model-sdk-0.0.23/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.23/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-03 09:57:44.061485 bytetrade-recommend-model-sdk-0.0.23/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.23/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 09:57:44.057485 bytetrade-recommend-model-sdk-0.0.23/bytetrade_recommend_model_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-03 09:57:44.000000 bytetrade-recommend-model-sdk-0.0.23/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2178 2023-07-03 09:57:44.000000 bytetrade-recommend-model-sdk-0.0.23/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-03 09:57:44.000000 bytetrade-recommend-model-sdk-0.0.23/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-07-03 09:57:44.000000 bytetrade-recommend-model-sdk-0.0.23/bytetrade_recommend_model_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-03 09:57:44.000000 bytetrade-recommend-model-sdk-0.0.23/bytetrade_recommend_model_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 09:57:44.057485 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 09:57:44.057485 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/embeddings/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/embeddings/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      489 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/embeddings/bert_embedding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/embeddings/embedding_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/embeddings/word2vec_embedding.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 09:57:44.057485 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 09:57:44.057485 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/config/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/config/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/config/content_similar_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/config/dnn_click_predictor_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/config/mind_base_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 09:57:44.057485 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/dataset/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/dataset/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2719 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 09:57:44.057485 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/eval/__init_.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/eval/eval_operation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11667 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 09:57:44.057485 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/exp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/exp/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11826 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/experiment_enum.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 09:57:44.061485 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10026 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/model/content_similar_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2330 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 09:57:44.061485 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/proto_class/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/proto_class/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17830 2023-07-03 09:21:19.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/proto_class/embedding_pb2.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 09:57:44.061485 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/recommend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/recommend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3354 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/recommend/recommend_common_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/recommend/recommend_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/recommend/time_weight_decay_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 09:57:44.061485 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1901 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/resources/model_management.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 09:57:44.061485 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/tools/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/tools/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5147 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/tools/aws_s3_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/tools/common_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27513 2023-07-03 09:24:37.000000 bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/tools/model_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-03 09:57:44.061485 bytetrade-recommend-model-sdk-0.0.23/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-07-03 09:55:06.000000 bytetrade-recommend-model-sdk-0.0.23/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.359712 bytetrade-recommend-model-sdk-0.0.24/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-06 02:18:17.359712 bytetrade-recommend-model-sdk-0.0.24/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/bytetrade_recommend_model_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-06 02:18:17.000000 bytetrade-recommend-model-sdk-0.0.24/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2178 2023-07-06 02:18:17.000000 bytetrade-recommend-model-sdk-0.0.24/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-06 02:18:17.000000 bytetrade-recommend-model-sdk-0.0.24/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-07-06 02:18:17.000000 bytetrade-recommend-model-sdk-0.0.24/bytetrade_recommend_model_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-06 02:18:17.000000 bytetrade-recommend-model-sdk-0.0.24/bytetrade_recommend_model_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/embeddings/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/embeddings/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      489 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/embeddings/bert_embedding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/embeddings/embedding_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/embeddings/word2vec_embedding.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/config/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/config/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/config/content_similar_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/config/dnn_click_predictor_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/config/mind_base_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2719 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/eval/__init_.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/eval/eval_operation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11667 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/exp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/exp/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11826 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/experiment_enum.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10528 2023-07-06 00:59:59.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/model/content_similar_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2330 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.355712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/proto_class/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/proto_class/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17830 2023-07-03 09:21:19.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/proto_class/embedding_pb2.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.359712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/recommend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/recommend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3354 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/recommend/recommend_common_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/recommend/recommend_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/recommend/time_weight_decay_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.359712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1901 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/resources/model_management.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 02:18:17.359712 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/tools/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/tools/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5147 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/tools/aws_s3_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/tools/common_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27513 2023-07-03 09:24:37.000000 bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/tools/model_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-06 02:18:17.359712 bytetrade-recommend-model-sdk-0.0.24/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-07-06 02:12:13.000000 bytetrade-recommend-model-sdk-0.0.24/setup.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.23/README.md` & `bytetrade-recommend-model-sdk-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt` & `bytetrade-recommend-model-sdk-0.0.24/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/embeddings/embedding_tool.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/embeddings/embedding_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/embeddings/word2vec_embedding.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/embeddings/word2vec_embedding.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/config/content_similar_config.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/config/content_similar_config.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/eval/eval_operation.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/eval/eval_operation.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/model/content_similar_model.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/model/content_similar_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,30 +177,40 @@
         if len(current_list_embedding) > self.__config.num_clicked_news_a_user:
             current_list_embedding = current_list_embedding[:self.__config.num_clicked_news_a_user]
         stack_candidate_embedding = np.stack(current_list_embedding)
         
         user_embedding = stack_candidate_embedding.sum(axis=0,keepdims=True)
         return user_embedding
             
+    def recall_empty(self,limit):
+        result_tuple_list = list()
+        for current_tuple in self.__base_document_id_to_created_at_tuple_list:
+            result_tuple_list.append((current_tuple[0],0.5))
+            if len(result_tuple_list) >= limit:
+                break
+        return result_tuple_list
     
     def recall(self,candidate_news_id_to_embedding,limit):
         """
         """
         if len(candidate_news_id_to_embedding) < 1:
-            result_tuple_list = list()
-            for current_tuple in self.__base_document_id_to_created_at_tuple_list:
-                result_tuple_list.append((current_tuple[0],0.5))
-                if len(result_tuple_list) >= limit:
-                    break
-            return result_tuple_list
+            self.__logger.debug(f'candidate_news_id_to_embedding length samll than 1')
+            return self.recall_empty(limit)
         
         self.__recommend_common_util.validate_candidate_document_id_to_item(candidate_news_id_to_embedding,self.__embedding_shape)
         user_embedding = self.get_user_vector(candidate_news_id_to_embedding)
         faiss.normalize_L2(user_embedding)
         consin_similar, nearest_indexes = self.__cosin_index.search(user_embedding, limit) # cosin similar,
         result_tuple_list = list()
         for current_similar,current_index in zip(consin_similar[0],nearest_indexes[0]):
               current_weight = (2 - (1 - current_similar)) * 1.0 / 2
+              if current_index not in self.__base_index_to_document_id:
+                  self.__logger.debug(f'current_index {current_index} is not exist')
+                  continue
               result_tuple_list.append((self.__base_index_to_document_id[current_index],current_weight))
+        
+        if len(result_tuple_list)  < 1:
+            self.__logger.debug('after complete result_tuple_list is small than 1')
+            return self.recall_empty(limit)
         return result_tuple_list
```

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/proto_class/embedding_pb2.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/proto_class/embedding_pb2.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/recommend/recommend_common_util.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/recommend/recommend_common_util.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/recommend/recommend_tool.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/recommend/recommend_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/recommend/time_weight_decay_tool.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/recommend/time_weight_decay_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/resources/model_management.json` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/resources/model_management.json`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/tools/aws_s3_tool.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/tools/aws_s3_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/tools/common_tool.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/tools/common_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/recommend_model_sdk/tools/model_tool.py` & `bytetrade-recommend-model-sdk-0.0.24/recommend_model_sdk/tools/model_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.23/setup.py` & `bytetrade-recommend-model-sdk-0.0.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 sys.path.append(os.path.dirname(__file__) + "/recommend-model")
 
 
 
 
 setup(
     name="bytetrade-recommend-model-sdk",
-    version="0.0.23",
+    version="0.0.24",
     # packages=find_packages(exclude="unit_test"),
     install_requires=[
         "pandas==2.0.0",
         "gensim==4.3.1",
         "protobuf==3.20.1",
         "nltk==3.8.1",
         "boto3"
```

