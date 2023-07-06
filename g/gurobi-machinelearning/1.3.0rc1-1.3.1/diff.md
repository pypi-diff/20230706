# Comparing `tmp/gurobi-machinelearning-1.3.0rc1.tar.gz` & `tmp/gurobi-machinelearning-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gurobi-machinelearning-1.3.0rc1.tar", last modified: Thu Jun  8 08:21:16 2023, max compression
+gzip compressed data, was "gurobi-machinelearning-1.3.1.tar", last modified: Thu Jul  6 10:36:37 2023, max compression
```

## Comparing `gurobi-machinelearning-1.3.0rc1.tar` & `gurobi-machinelearning-1.3.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.275817 gurobi-machinelearning-1.3.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-06-08 08:21:16.275817 gurobi-machinelearning-1.3.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-08 08:21:16.275817 gurobi-machinelearning-1.3.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.267817 gurobi-machinelearning-1.3.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.271817 gurobi-machinelearning-1.3.0rc1/src/gurobi_machinelearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-06-08 08:21:16.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_machinelearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-08 08:21:16.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_machinelearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:21:16.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_machinelearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 08:21:16.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_machinelearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 08:21:16.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_machinelearning.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.271817 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-08 08:21:09.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/add_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.271817 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/keras/keras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.271817 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/_var_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/base_predictor_constr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.271817 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/decision_tree/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/decision_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/decision_tree/decision_tree_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/get_convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.275817 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/neural_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/submodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/register_user_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/registered_predictors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.275817 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/base_regressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/decision_tree_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/mlpregressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/pls_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/predictors_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/random_forest_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/skgetter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.275817 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/torch/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.275817 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/xgboost/xgboost_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.719664 gurobi-machinelearning-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-06 10:36:37.719664 gurobi-machinelearning-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-06 10:36:37.719664 gurobi-machinelearning-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.715664 gurobi-machinelearning-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.715664 gurobi-machinelearning-1.3.1/src/gurobi_machinelearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-06 10:36:37.000000 gurobi-machinelearning-1.3.1/src/gurobi_machinelearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-06 10:36:37.000000 gurobi-machinelearning-1.3.1/src/gurobi_machinelearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:36:37.000000 gurobi-machinelearning-1.3.1/src/gurobi_machinelearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 10:36:37.000000 gurobi-machinelearning-1.3.1/src/gurobi_machinelearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 10:36:37.000000 gurobi-machinelearning-1.3.1/src/gurobi_machinelearning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.715664 gurobi-machinelearning-1.3.1/src/gurobi_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-06 10:36:30.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/add_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.715664 gurobi-machinelearning-1.3.1/src/gurobi_ml/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/keras/keras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.715664 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/_var_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/base_predictor_constr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.719664 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/decision_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/decision_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/decision_tree/decision_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/get_convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.719664 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/neural_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/submodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/register_user_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/registered_predictors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.719664 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/base_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/column_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/decision_tree_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/mlpregressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/pls_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/predictors_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/random_forest_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/skgetter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.719664 gurobi-machinelearning-1.3.1/src/gurobi_ml/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/torch/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.719664 gurobi-machinelearning-1.3.1/src/gurobi_ml/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/xgboost/xgboost_regressor.py
```

### Comparing `gurobi-machinelearning-1.3.0rc1/LICENSE` & `gurobi-machinelearning-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/PKG-INFO` & `gurobi-machinelearning-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobi-machinelearning
-Version: 1.3.0rc1
+Version: 1.3.1
 Summary: package to insert ML models in Gurobi
 Author: Gurobi Optimization LLC
 Maintainer: Pierre Bonami
 Maintainer-email: bonami@gurobi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Gurobi/gurobi-machinelearning
 Project-URL: Documentation, https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com
@@ -15,62 +15,63 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![build and test](https://github.com/Gurobi/gurobi-machinelearning/actions/workflows/push.yml/badge.svg?branch=main)](https://github.com/Gurobi/gurobi-machinelearning/actions/workflows/push.yml?query=branch%3Amain++)
 [![build wheel](https://github.com/Gurobi/gurobi-machinelearning/actions/workflows/build_wheel.yml/badge.svg?branch=main)](https://github.com/Gurobi/gurobi-machinelearning/actions/workflows/build_wheel.yml?query=branch%3Amain++)
-![Python versions](https://img.shields.io/badge/python-3.9%20|%203.10-blue)
+![Python versions](https://img.shields.io/badge/python-3.9%20|%203.10%20|%203.11-blue)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/gurobi-machinelearning)](https://pypi.org/project/gurobi-machinelearning)
 [![ReadTheDocs](https://readthedocs.com/projects/gurobi-optimization-gurobi-machine-learning/badge/?version=stable)](https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com)
 [![Gurobi-forum](https://img.shields.io/badge/Help-Gurobi--Forum-red)](https://support.gurobi.com/hc/en-us/community/topics/10373864542609-GitHub-Projects)
 
 [![Gurobi](https://raw.githubusercontent.com/Gurobi/gurobi-machinelearning/main/docs/source/_static/image8.png)](https://www.gurobi.com)
 
 
 # Gurobi Machine Learning
 
 Gurobi Machine Learning is an [open-source](https://gurobi-machinelearning.readthedocs.io/en/stable/meta-license.html) python package to embed trained regression models in a [`gurobipy`](https://pypi.org/project/gurobipy/) model to be solved with the Gurobi solver.
 
-The package currently supports various [scikit-learn](https://scikit-learn.org/stable/) objects. It has limited support for the [Keras](https://keras.io/) API of [TensorFlow](https://www.tensorflow.org/) and [PyTorch](https://pytorch.org/). Only neural networks with ReLU activation can be used with these two packages.
+The package currently supports various [scikit-learn](https://scikit-learn.org/stable/) objects. It has limited support for the [Keras](https://keras.io/) API of [TensorFlow](https://www.tensorflow.org/), [PyTorch](https://pytorch.org/) and [XGBoost](https://www.xgboost.ai). Only neural networks with ReLU activation can be used with Keras and PyTorch.
 
 # Documentation
 
 The latest user manual is available on [readthedocs](https://gurobi-machinelearning.readthedocs.io/).
 
 # Contact us
 
 For questions related to using Gurobi Machine Learning please use [Gurobi's Forum](https://support.gurobi.com/hc/en-us/community/topics/10373864542609-GitHub-Projects).
 
-For reporting bugs, issues and feature request please
+For reporting bugs, issues and feature requests please
 [open an issue](https://github.com/Gurobi/gurobi-machinelearning/issues).
 
 If you encounter issues with Gurobi or ``gurobipy`` please contact
 [Gurobi Support](https://support.gurobi.com/hc/en-us).
 
 # Installation
 
 ## Dependencies
 
 `gurobi-machinelearning` requires the following:
 - Python >= 3.9
-- [`numpy`](https://pypi.org/project/numpy/) >= 1.22.0
+- [`numpy`](https://pypi.org/project/numpy/) >= 1.23.0
 - [`gurobipy`](https://pypi.org/project/gurobipy/) >= 10.0
 - [`scipy`](https://pypi.org/project/scipy/) >= 1.9.3
 
 The current version supports the following ML packages:
 - [`torch`](https://pypi.org/project/torch/)
 - [`scikit-learn`](https://pypi.org/project/scikit-learn)
 - [`tensorflow`](https://pypi.org/project/tensorflow)
+- [`XGBoost`](https://pypi.org/project/xgboost/)
 
 Installing these packages is only required if the predictor you want to insert uses them
 (i.e. to insert a Keras based predictor you need to have `tensorflow` installed).
 
-The up to date supported and tested versions of each package for the last release can be [found in the documentation](https://gurobi-machinelearning.readthedocs.io/en/1.1.x/firststeps-introduction.html#table-versions).
+The up to date supported and tested versions of each package for the last release can be [found in the documentation](https://gurobi-machinelearning.readthedocs.io/en/stable/firststeps-introduction.html#table-versions).
 
 ## Pip installation
 
 The easiest way to install `gurobi-machinelearning` is using `pip` in a virtual environment:
 ```shell
 (.venv) pip install gurobi-machinelearning
 ```
```

### Comparing `gurobi-machinelearning-1.3.0rc1/README.md` & `gurobi-machinelearning-1.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 [![build and test](https://github.com/Gurobi/gurobi-machinelearning/actions/workflows/push.yml/badge.svg?branch=main)](https://github.com/Gurobi/gurobi-machinelearning/actions/workflows/push.yml?query=branch%3Amain++)
 [![build wheel](https://github.com/Gurobi/gurobi-machinelearning/actions/workflows/build_wheel.yml/badge.svg?branch=main)](https://github.com/Gurobi/gurobi-machinelearning/actions/workflows/build_wheel.yml?query=branch%3Amain++)
-![Python versions](https://img.shields.io/badge/python-3.9%20|%203.10-blue)
+![Python versions](https://img.shields.io/badge/python-3.9%20|%203.10%20|%203.11-blue)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/gurobi-machinelearning)](https://pypi.org/project/gurobi-machinelearning)
 [![ReadTheDocs](https://readthedocs.com/projects/gurobi-optimization-gurobi-machine-learning/badge/?version=stable)](https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com)
 [![Gurobi-forum](https://img.shields.io/badge/Help-Gurobi--Forum-red)](https://support.gurobi.com/hc/en-us/community/topics/10373864542609-GitHub-Projects)
 
 [![Gurobi](https://raw.githubusercontent.com/Gurobi/gurobi-machinelearning/main/docs/source/_static/image8.png)](https://www.gurobi.com)
 
 
 # Gurobi Machine Learning
 
 Gurobi Machine Learning is an [open-source](https://gurobi-machinelearning.readthedocs.io/en/stable/meta-license.html) python package to embed trained regression models in a [`gurobipy`](https://pypi.org/project/gurobipy/) model to be solved with the Gurobi solver.
 
-The package currently supports various [scikit-learn](https://scikit-learn.org/stable/) objects. It has limited support for the [Keras](https://keras.io/) API of [TensorFlow](https://www.tensorflow.org/) and [PyTorch](https://pytorch.org/). Only neural networks with ReLU activation can be used with these two packages.
+The package currently supports various [scikit-learn](https://scikit-learn.org/stable/) objects. It has limited support for the [Keras](https://keras.io/) API of [TensorFlow](https://www.tensorflow.org/), [PyTorch](https://pytorch.org/) and [XGBoost](https://www.xgboost.ai). Only neural networks with ReLU activation can be used with Keras and PyTorch.
 
 # Documentation
 
 The latest user manual is available on [readthedocs](https://gurobi-machinelearning.readthedocs.io/).
 
 # Contact us
 
 For questions related to using Gurobi Machine Learning please use [Gurobi's Forum](https://support.gurobi.com/hc/en-us/community/topics/10373864542609-GitHub-Projects).
 
-For reporting bugs, issues and feature request please
+For reporting bugs, issues and feature requests please
 [open an issue](https://github.com/Gurobi/gurobi-machinelearning/issues).
 
 If you encounter issues with Gurobi or ``gurobipy`` please contact
 [Gurobi Support](https://support.gurobi.com/hc/en-us).
 
 # Installation
 
 ## Dependencies
 
 `gurobi-machinelearning` requires the following:
 - Python >= 3.9
-- [`numpy`](https://pypi.org/project/numpy/) >= 1.22.0
+- [`numpy`](https://pypi.org/project/numpy/) >= 1.23.0
 - [`gurobipy`](https://pypi.org/project/gurobipy/) >= 10.0
 - [`scipy`](https://pypi.org/project/scipy/) >= 1.9.3
 
 The current version supports the following ML packages:
 - [`torch`](https://pypi.org/project/torch/)
 - [`scikit-learn`](https://pypi.org/project/scikit-learn)
 - [`tensorflow`](https://pypi.org/project/tensorflow)
+- [`XGBoost`](https://pypi.org/project/xgboost/)
 
 Installing these packages is only required if the predictor you want to insert uses them
 (i.e. to insert a Keras based predictor you need to have `tensorflow` installed).
 
-The up to date supported and tested versions of each package for the last release can be [found in the documentation](https://gurobi-machinelearning.readthedocs.io/en/1.1.x/firststeps-introduction.html#table-versions).
+The up to date supported and tested versions of each package for the last release can be [found in the documentation](https://gurobi-machinelearning.readthedocs.io/en/stable/firststeps-introduction.html#table-versions).
 
 ## Pip installation
 
 The easiest way to install `gurobi-machinelearning` is using `pip` in a virtual environment:
 ```shell
 (.venv) pip install gurobi-machinelearning
 ```
```

### Comparing `gurobi-machinelearning-1.3.0rc1/pyproject.toml` & `gurobi-machinelearning-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gurobi-machinelearning"
-version = "1.3.0rc1"
+version = "1.3.1"
 description = "package to insert ML models in Gurobi"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text="Apache-2.0"}
 keywords = ["mathematical optimization", "gurobi", "scikit-learn", "pytorch", "tensorflow", "ml"]
 authors = [
   {name = "Gurobi Optimization LLC"}
```

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_machinelearning.egg-info/PKG-INFO` & `gurobi-machinelearning-1.3.1/src/gurobi_machinelearning.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobi-machinelearning
-Version: 1.3.0rc1
+Version: 1.3.1
 Summary: package to insert ML models in Gurobi
 Author: Gurobi Optimization LLC
 Maintainer: Pierre Bonami
 Maintainer-email: bonami@gurobi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Gurobi/gurobi-machinelearning
 Project-URL: Documentation, https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com
@@ -15,62 +15,63 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![build and test](https://github.com/Gurobi/gurobi-machinelearning/actions/workflows/push.yml/badge.svg?branch=main)](https://github.com/Gurobi/gurobi-machinelearning/actions/workflows/push.yml?query=branch%3Amain++)
 [![build wheel](https://github.com/Gurobi/gurobi-machinelearning/actions/workflows/build_wheel.yml/badge.svg?branch=main)](https://github.com/Gurobi/gurobi-machinelearning/actions/workflows/build_wheel.yml?query=branch%3Amain++)
-![Python versions](https://img.shields.io/badge/python-3.9%20|%203.10-blue)
+![Python versions](https://img.shields.io/badge/python-3.9%20|%203.10%20|%203.11-blue)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/gurobi-machinelearning)](https://pypi.org/project/gurobi-machinelearning)
 [![ReadTheDocs](https://readthedocs.com/projects/gurobi-optimization-gurobi-machine-learning/badge/?version=stable)](https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com)
 [![Gurobi-forum](https://img.shields.io/badge/Help-Gurobi--Forum-red)](https://support.gurobi.com/hc/en-us/community/topics/10373864542609-GitHub-Projects)
 
 [![Gurobi](https://raw.githubusercontent.com/Gurobi/gurobi-machinelearning/main/docs/source/_static/image8.png)](https://www.gurobi.com)
 
 
 # Gurobi Machine Learning
 
 Gurobi Machine Learning is an [open-source](https://gurobi-machinelearning.readthedocs.io/en/stable/meta-license.html) python package to embed trained regression models in a [`gurobipy`](https://pypi.org/project/gurobipy/) model to be solved with the Gurobi solver.
 
-The package currently supports various [scikit-learn](https://scikit-learn.org/stable/) objects. It has limited support for the [Keras](https://keras.io/) API of [TensorFlow](https://www.tensorflow.org/) and [PyTorch](https://pytorch.org/). Only neural networks with ReLU activation can be used with these two packages.
+The package currently supports various [scikit-learn](https://scikit-learn.org/stable/) objects. It has limited support for the [Keras](https://keras.io/) API of [TensorFlow](https://www.tensorflow.org/), [PyTorch](https://pytorch.org/) and [XGBoost](https://www.xgboost.ai). Only neural networks with ReLU activation can be used with Keras and PyTorch.
 
 # Documentation
 
 The latest user manual is available on [readthedocs](https://gurobi-machinelearning.readthedocs.io/).
 
 # Contact us
 
 For questions related to using Gurobi Machine Learning please use [Gurobi's Forum](https://support.gurobi.com/hc/en-us/community/topics/10373864542609-GitHub-Projects).
 
-For reporting bugs, issues and feature request please
+For reporting bugs, issues and feature requests please
 [open an issue](https://github.com/Gurobi/gurobi-machinelearning/issues).
 
 If you encounter issues with Gurobi or ``gurobipy`` please contact
 [Gurobi Support](https://support.gurobi.com/hc/en-us).
 
 # Installation
 
 ## Dependencies
 
 `gurobi-machinelearning` requires the following:
 - Python >= 3.9
-- [`numpy`](https://pypi.org/project/numpy/) >= 1.22.0
+- [`numpy`](https://pypi.org/project/numpy/) >= 1.23.0
 - [`gurobipy`](https://pypi.org/project/gurobipy/) >= 10.0
 - [`scipy`](https://pypi.org/project/scipy/) >= 1.9.3
 
 The current version supports the following ML packages:
 - [`torch`](https://pypi.org/project/torch/)
 - [`scikit-learn`](https://pypi.org/project/scikit-learn)
 - [`tensorflow`](https://pypi.org/project/tensorflow)
+- [`XGBoost`](https://pypi.org/project/xgboost/)
 
 Installing these packages is only required if the predictor you want to insert uses them
 (i.e. to insert a Keras based predictor you need to have `tensorflow` installed).
 
-The up to date supported and tested versions of each package for the last release can be [found in the documentation](https://gurobi-machinelearning.readthedocs.io/en/1.1.x/firststeps-introduction.html#table-versions).
+The up to date supported and tested versions of each package for the last release can be [found in the documentation](https://gurobi-machinelearning.readthedocs.io/en/stable/firststeps-introduction.html#table-versions).
 
 ## Pip installation
 
 The easiest way to install `gurobi-machinelearning` is using `pip` in a virtual environment:
 ```shell
 (.venv) pip install gurobi-machinelearning
 ```
```

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_machinelearning.egg-info/SOURCES.txt` & `gurobi-machinelearning-1.3.1/src/gurobi_machinelearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/__init__.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/_version.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/_version.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from importlib import metadata
 
 try:
     __version__ = metadata.version("gurobi_machinelearning")
 except metadata.PackageNotFoundError:
     __version__ = "dev"
 
-GIT_HASH = "f6a98a0a6ffe194679d00661f204c6204d55f882"
+GIT_HASH = "208bf12d2e054b02c2462de6446318be3e461520"
 
 
 def get_versions():
     """Get package version."""
     # Downloaded package with inserted git hash.
     if "Format" not in GIT_HASH:
         git_hash = f"-{GIT_HASH}"
```

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/add_predictor.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/add_predictor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/exceptions.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/keras/__init__.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/keras/keras.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/keras/keras.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/__init__.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/_var_utils.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/_var_utils.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/base_predictor_constr.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/base_predictor_constr.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/decision_tree/__init__.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/decision_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/decision_tree/decision_tree_model.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/decision_tree/decision_tree_model.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/get_convertor.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/get_convertor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/__init__.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/activations.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/activations.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/layers.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/layers.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/neural_net.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/neural_net.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/submodel.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/submodel.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/register_user_predictor.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/register_user_predictor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/registered_predictors.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/registered_predictors.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,28 +71,21 @@
         }
     return {}
 
 
 def keras_convertors():
     """Collect known Keras objects that can be embedded and the conversion class."""
     if "tensorflow" in sys.modules:
-        from keras.engine.functional import (  # pylint: disable=import-outside-toplevel
-            Functional,
-        )
-        from keras.engine.training import (  # pylint: disable=import-outside-toplevel
-            Model,
-        )
         from tensorflow import keras  # pylint: disable=import-outside-toplevel
 
         from .keras import add_keras_constr  # pylint: disable=import-outside-toplevel
 
         return {
             keras.Sequential: add_keras_constr,
-            Functional: add_keras_constr,
-            Model: add_keras_constr,
+            keras.Model: add_keras_constr,
         }
     return {}
 
 
 def registered_predictors():
     """Return the list of registered predictors."""
     convertors = {}
```

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/__init__.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/base_regressions.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/base_regressions.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/column_transformer.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/column_transformer.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/decision_tree_regressor.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/linear_regression.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/linear_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/logistic_regression.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/mlpregressor.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/mlpregressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/pipeline.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/pls_regression.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/pls_regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             **kwargs,
         )
 
     def add_regression_constr(self):
         """Add the prediction constraints to Gurobi."""
         x_mean = self.predictor._x_mean
         x_std = self.predictor._x_std
-        coefs = self.predictor._coef_.T
+        coefs = self.predictor.coef_.T
         intercept = self.predictor.intercept_
         self.gp_model.addConstr(
             self.output
             == self.input @ (coefs / x_std[:, np.newaxis])
             - x_mean / x_std @ coefs
             + intercept,
             name="plsreg",
```

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/predictors_list.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/predictors_list.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/preprocessing.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/random_forest_regressor.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/random_forest_regressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/skgetter.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/skgetter.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/torch/__init__.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/torch/sequential.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/torch/sequential.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/xgboost/__init__.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/xgboost/xgboost_regressor.py` & `gurobi-machinelearning-1.3.1/src/gurobi_ml/xgboost/xgboost_regressor.py`

 * *Files identical despite different names*

