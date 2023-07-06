# Comparing `tmp/mljar-supervised-1.0.0.tar.gz` & `tmp/mljar-supervised-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mljar-supervised-1.0.0.tar", last modified: Mon Jun 26 13:38:22 2023, max compression
+gzip compressed data, was "mljar-supervised-1.0.1.tar", last modified: Thu Jul  6 13:24:39 2023, max compression
```

## Comparing `mljar-supervised-1.0.0.tar` & `mljar-supervised-1.0.1.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1073 2022-03-28 10:53:20.000000 mljar-supervised-1.0.0/LICENSE
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       47 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/MANIFEST.in
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26713 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    22164 2023-06-26 11:22:02.000000 mljar-supervised-1.0.0/README.md
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.905047 mljar-supervised-1.0.0/mljar_supervised.egg-info/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26713 2023-06-26 13:38:22.000000 mljar-supervised-1.0.0/mljar_supervised.egg-info/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3461 2023-06-26 13:38:22.000000 mljar-supervised-1.0.0/mljar_supervised.egg-info/SOURCES.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-06-26 13:38:22.000000 mljar-supervised-1.0.0/mljar_supervised.egg-info/dependency_links.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      310 2023-06-26 13:38:22.000000 mljar-supervised-1.0.0/mljar_supervised.egg-info/requires.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       11 2023-06-26 13:38:22.000000 mljar-supervised-1.0.0/mljar_supervised.egg-info/top_level.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      309 2023-06-26 11:10:20.000000 mljar-supervised-1.0.0/requirements.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       48 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/requirements_dev.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/setup.cfg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1213 2023-06-26 13:37:16.000000 mljar-supervised-1.0.0/setup.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.905047 mljar-supervised-1.0.0/supervised/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2023-06-26 13:37:44.000000 mljar-supervised-1.0.0/supervised/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.905047 mljar-supervised-1.0.0/supervised/algorithms/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/algorithms/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4172 2021-09-02 10:34:57.000000 mljar-supervised-1.0.0/supervised/algorithms/algorithm.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2524 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/baseline.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    14472 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/catboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9168 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/decision_tree.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5170 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/extra_trees.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      911 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/algorithms/factory.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3550 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/knn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12114 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/lightgbm.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5972 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/linear.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4792 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/nn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5406 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/random_forest.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2349 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/registry.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6108 2023-06-26 08:29:57.000000 mljar-supervised-1.0.0/supervised/algorithms/sklearn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12628 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/xgboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26161 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/automl.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   100170 2023-06-26 11:40:41.000000 mljar-supervised-1.0.0/supervised/base_automl.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/supervised/callbacks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/callbacks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      592 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/callbacks/callback.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1027 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/callbacks/callback_list.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9058 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/callbacks/early_stopping.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1700 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/callbacks/learner_time_constraint.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      607 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/callbacks/max_iters_constraint.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1867 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/callbacks/metric_logger.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      932 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/callbacks/terminate_on_nan.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3351 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/callbacks/total_time_constraint.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    23009 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/ensemble.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      546 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/exceptions.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/supervised/fairness/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-06-26 08:29:57.000000 mljar-supervised-1.0.0/supervised/fairness/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26295 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/fairness/metrics.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15058 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/fairness/optimization.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4049 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/fairness/plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3863 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/fairness/report.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-06-26 08:29:57.000000 mljar-supervised-1.0.0/supervised/fairness/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    29363 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/model_framework.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/supervised/preprocessing/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/preprocessing/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3563 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/preprocessing/datetime_transformer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12634 2023-06-26 11:40:03.000000 mljar-supervised-1.0.0/supervised/preprocessing/eda.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      889 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/preprocessing/encoding_selector.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1509 2023-06-26 08:29:57.000000 mljar-supervised-1.0.0/supervised/preprocessing/exclude_missing_target.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    10747 2023-06-26 11:40:03.000000 mljar-supervised-1.0.0/supervised/preprocessing/goldenfeatures_transformer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3866 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/preprocessing/kmeans_transformer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2458 2023-06-26 11:40:07.000000 mljar-supervised-1.0.0/supervised/preprocessing/label_binarizer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1804 2022-12-30 13:35:06.000000 mljar-supervised-1.0.0/supervised/preprocessing/label_encoder.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1613 2023-06-26 08:29:57.000000 mljar-supervised-1.0.0/supervised/preprocessing/loo_encoder.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26512 2023-06-26 11:40:03.000000 mljar-supervised-1.0.0/supervised/preprocessing/preprocessing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4658 2023-06-26 11:40:03.000000 mljar-supervised-1.0.0/supervised/preprocessing/preprocessing_categorical.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3759 2023-06-26 11:40:03.000000 mljar-supervised-1.0.0/supervised/preprocessing/preprocessing_missing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4038 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/preprocessing/preprocessing_utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3664 2023-06-26 11:40:03.000000 mljar-supervised-1.0.0/supervised/preprocessing/scale.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2603 2021-09-30 14:10:40.000000 mljar-supervised-1.0.0/supervised/preprocessing/text_transformer.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/supervised/tuner/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/tuner/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2584 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/tuner/data_info.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2409 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/tuner/hill_climbing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    58739 2023-06-26 11:40:41.000000 mljar-supervised-1.0.0/supervised/tuner/mljar_tuner.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/supervised/tuner/optuna/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5634 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/catboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2635 2022-12-30 13:09:00.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/extra_trees.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2054 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/knn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5999 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/lightgbm.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2260 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/nn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2637 2022-12-30 13:09:15.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/random_forest.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11488 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/tuner.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4824 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/xgboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6389 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/tuner/preprocessing_tuner.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      564 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/tuner/random_parameters.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8974 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/tuner/time_controller.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/supervised/utils/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      184 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/utils/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    37134 2023-06-26 11:40:41.000000 mljar-supervised-1.0.0/supervised/utils/additional_metrics.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7895 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/utils/additional_plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5409 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/utils/automl_plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1052 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/utils/common.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      524 2021-09-17 07:39:41.000000 mljar-supervised-1.0.0/supervised/utils/config.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      173 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/utils/constants.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1481 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/utils/data_validation.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3204 2021-09-02 10:34:57.000000 mljar-supervised-1.0.0/supervised/utils/importance.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4949 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/utils/leaderboard_plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4880 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/utils/learning_curves.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    13752 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/utils/metric.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12099 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/utils/shap.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      463 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/utils/subsample.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      628 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/utils/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/supervised/validation/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/validation/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1211 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/validation/validation_step.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      264 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/validation/validator_base.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4267 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/validation/validator_custom.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5611 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/validation/validator_kfold.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4788 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/validation/validator_split.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-07-06 13:24:39.836086 mljar-supervised-1.0.1/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1073 2022-03-28 10:53:20.000000 mljar-supervised-1.0.1/LICENSE
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       47 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/MANIFEST.in
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    29496 2023-07-06 13:24:39.836086 mljar-supervised-1.0.1/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    24483 2023-06-27 12:06:31.000000 mljar-supervised-1.0.1/README.md
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-07-06 13:24:39.828086 mljar-supervised-1.0.1/mljar_supervised.egg-info/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    29496 2023-07-06 13:24:39.000000 mljar-supervised-1.0.1/mljar_supervised.egg-info/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3461 2023-07-06 13:24:39.000000 mljar-supervised-1.0.1/mljar_supervised.egg-info/SOURCES.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-07-06 13:24:39.000000 mljar-supervised-1.0.1/mljar_supervised.egg-info/dependency_links.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      310 2023-07-06 13:24:39.000000 mljar-supervised-1.0.1/mljar_supervised.egg-info/requires.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       11 2023-07-06 13:24:39.000000 mljar-supervised-1.0.1/mljar_supervised.egg-info/top_level.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      309 2023-06-26 11:10:20.000000 mljar-supervised-1.0.1/requirements.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       48 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/requirements_dev.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-07-06 13:24:39.836086 mljar-supervised-1.0.1/setup.cfg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1213 2023-07-06 13:21:55.000000 mljar-supervised-1.0.1/setup.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-07-06 13:24:39.828086 mljar-supervised-1.0.1/supervised/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2023-07-06 13:22:03.000000 mljar-supervised-1.0.1/supervised/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-07-06 13:24:39.832086 mljar-supervised-1.0.1/supervised/algorithms/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/algorithms/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4172 2021-09-02 10:34:57.000000 mljar-supervised-1.0.1/supervised/algorithms/algorithm.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2524 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/algorithms/baseline.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    14472 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/algorithms/catboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9168 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/algorithms/decision_tree.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5170 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/algorithms/extra_trees.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      911 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/algorithms/factory.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3550 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/algorithms/knn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12114 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/algorithms/lightgbm.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5972 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/algorithms/linear.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4792 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/algorithms/nn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5406 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/algorithms/random_forest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2349 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/algorithms/registry.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6108 2023-06-26 08:29:57.000000 mljar-supervised-1.0.1/supervised/algorithms/sklearn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12628 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/algorithms/xgboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26144 2023-07-04 14:07:03.000000 mljar-supervised-1.0.1/supervised/automl.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   100170 2023-06-26 11:40:41.000000 mljar-supervised-1.0.1/supervised/base_automl.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-07-06 13:24:39.832086 mljar-supervised-1.0.1/supervised/callbacks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/callbacks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      592 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/callbacks/callback.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1027 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/callbacks/callback_list.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9058 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/callbacks/early_stopping.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1700 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/callbacks/learner_time_constraint.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      607 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/callbacks/max_iters_constraint.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1867 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/callbacks/metric_logger.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      932 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/callbacks/terminate_on_nan.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3351 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/callbacks/total_time_constraint.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    23009 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/ensemble.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      546 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/exceptions.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-07-06 13:24:39.832086 mljar-supervised-1.0.1/supervised/fairness/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-06-26 08:29:57.000000 mljar-supervised-1.0.1/supervised/fairness/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26303 2023-07-04 08:54:29.000000 mljar-supervised-1.0.1/supervised/fairness/metrics.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15057 2023-07-04 08:41:29.000000 mljar-supervised-1.0.1/supervised/fairness/optimization.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4049 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/fairness/plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3863 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/fairness/report.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-06-26 08:29:57.000000 mljar-supervised-1.0.1/supervised/fairness/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    29363 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/model_framework.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-07-06 13:24:39.832086 mljar-supervised-1.0.1/supervised/preprocessing/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/preprocessing/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3563 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/preprocessing/datetime_transformer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12634 2023-06-26 11:40:03.000000 mljar-supervised-1.0.1/supervised/preprocessing/eda.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      889 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/preprocessing/encoding_selector.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1509 2023-06-26 08:29:57.000000 mljar-supervised-1.0.1/supervised/preprocessing/exclude_missing_target.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    10747 2023-06-26 11:40:03.000000 mljar-supervised-1.0.1/supervised/preprocessing/goldenfeatures_transformer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3866 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/preprocessing/kmeans_transformer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2458 2023-06-26 11:40:07.000000 mljar-supervised-1.0.1/supervised/preprocessing/label_binarizer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1804 2022-12-30 13:35:06.000000 mljar-supervised-1.0.1/supervised/preprocessing/label_encoder.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1613 2023-06-26 08:29:57.000000 mljar-supervised-1.0.1/supervised/preprocessing/loo_encoder.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26512 2023-06-26 11:40:03.000000 mljar-supervised-1.0.1/supervised/preprocessing/preprocessing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4658 2023-06-26 11:40:03.000000 mljar-supervised-1.0.1/supervised/preprocessing/preprocessing_categorical.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3759 2023-06-26 11:40:03.000000 mljar-supervised-1.0.1/supervised/preprocessing/preprocessing_missing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4038 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/preprocessing/preprocessing_utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3664 2023-06-26 11:40:03.000000 mljar-supervised-1.0.1/supervised/preprocessing/scale.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2603 2021-09-30 14:10:40.000000 mljar-supervised-1.0.1/supervised/preprocessing/text_transformer.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-07-06 13:24:39.832086 mljar-supervised-1.0.1/supervised/tuner/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/tuner/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2584 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/tuner/data_info.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2409 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/tuner/hill_climbing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    59383 2023-07-04 13:02:50.000000 mljar-supervised-1.0.1/supervised/tuner/mljar_tuner.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-07-06 13:24:39.832086 mljar-supervised-1.0.1/supervised/tuner/optuna/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/tuner/optuna/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5634 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/tuner/optuna/catboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2635 2022-12-30 13:09:00.000000 mljar-supervised-1.0.1/supervised/tuner/optuna/extra_trees.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2054 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/tuner/optuna/knn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5999 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/tuner/optuna/lightgbm.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2260 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/tuner/optuna/nn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2637 2022-12-30 13:09:15.000000 mljar-supervised-1.0.1/supervised/tuner/optuna/random_forest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11488 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/tuner/optuna/tuner.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4824 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/tuner/optuna/xgboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6389 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/tuner/preprocessing_tuner.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      564 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/tuner/random_parameters.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8974 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/tuner/time_controller.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-07-06 13:24:39.836086 mljar-supervised-1.0.1/supervised/utils/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      184 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/utils/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    37191 2023-07-04 07:57:29.000000 mljar-supervised-1.0.1/supervised/utils/additional_metrics.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7895 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/utils/additional_plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5409 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/utils/automl_plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1052 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/utils/common.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      524 2021-09-17 07:39:41.000000 mljar-supervised-1.0.1/supervised/utils/config.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      173 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/utils/constants.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1481 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/utils/data_validation.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3204 2021-09-02 10:34:57.000000 mljar-supervised-1.0.1/supervised/utils/importance.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4949 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/utils/leaderboard_plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4880 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/utils/learning_curves.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    13752 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/utils/metric.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12119 2023-07-06 13:19:56.000000 mljar-supervised-1.0.1/supervised/utils/shap.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      463 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/utils/subsample.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      628 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/utils/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-07-06 13:24:39.836086 mljar-supervised-1.0.1/supervised/validation/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/validation/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1211 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/validation/validation_step.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      264 2021-09-02 08:06:45.000000 mljar-supervised-1.0.1/supervised/validation/validator_base.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4267 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/validation/validator_custom.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5611 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/validation/validator_kfold.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4788 2023-06-26 11:40:40.000000 mljar-supervised-1.0.1/supervised/validation/validator_split.py
```

### Comparing `mljar-supervised-1.0.0/LICENSE` & `mljar-supervised-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/PKG-INFO` & `mljar-supervised-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mljar-supervised
-Version: 1.0.0
+Version: 1.0.1
 Summary: Automated Machine Learning for Humans
 Home-page: https://github.com/mljar/mljar-supervised
 Author: MLJAR, Sp. z o.o.
 Author-email: contact@mljar.com
 License: MIT
 Description: # MLJAR Automated Machine Learning for Humans
         
@@ -39,14 +39,15 @@
         
         ## Table of Contents
         
          - [Automated Machine Learning](https://github.com/mljar/mljar-supervised#automated-machine-learning)
          - [What's good in it?](https://github.com/mljar/mljar-supervised#whats-good-in-it)
          - [Automatic Documentation](https://github.com/mljar/mljar-supervised#automatic-documentation)
          - [Available Modes](https://github.com/mljar/mljar-supervised#available-modes)
+         - [Fairness Aware Training](https://github.com/mljar/mljar-supervised#fairness-aware-training)
          - [Examples](https://github.com/mljar/mljar-supervised#examples)
          - [FAQ](https://github.com/mljar/mljar-supervised#faq)
          - [Documentation](https://github.com/mljar/mljar-supervised#documentation)
          - [Installation](https://github.com/mljar/mljar-supervised#installation)
          - [Demo](https://github.com/mljar/mljar-supervised#demo)
          - [Contributing](https://github.com/mljar/mljar-supervised#contributing)
          - [Cite](https://github.com/mljar/mljar-supervised#cite)
@@ -166,14 +167,16 @@
         
         It should be used when the performance is the most important and time is not limited.
         - It is using 10-fold CV
         - It is using: `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, and `CatBoost`. Those algorithms are tuned by `Optuna` framework for `optuna_time_budget` seconds, each. Algorithms are tuned with original data, without advanced feature engineering.
         - It is using advanced feature engineering, stacking and ensembling. The hyperparameters found for original data are reused with those steps.
         - It produces learning curves in the reports.
         
+        
+        
         ## How to save and load AutoML?
         
         All models in the AutoML are saved and loaded automatically. No need to call `save()` or `load()`.
         
         ### Example:
         
         #### Train AutoML
@@ -202,14 +205,69 @@
         
         - for binary classification: `logloss`, `auc`, `f1`, `average_precision`, `accuracy`- default is `logloss`
         - for mutliclass classification: `logloss`, `f1`, `accuracy` - default is `logloss`
         - for regression: `rmse`, `mse`, `mae`, `r2`, `mape`, `spearman`, `pearson` - default is `rmse`
         
         If you don't find `eval_metric` that you need, please add a new issue. We will add it.
         
+        
+        ## Fairness Aware Training
+        
+        Starting from version `1.0.0` AutoML can optimize Machine Learning pipline with sensitive features. There are following fairness releated arguments in the AutoML constructor:
+         - `fairness_metric` - metric which will be used to decide if the model is fair,
+         - `fairness_threshold` - threshold used in decision about model fairness,
+         - `privileged_groups` - privileged groups used in fairness metrics computation,
+         - `underprivileged_groups` - underprivileged groups used in fairness metrics computation.
+        
+        The `fit()` method accepts `sensitive_features`. When sensitive features are passed to AutoML, the best model will be selected among fair models only. In the AutoML reports additional information about fairness metrics will be added. The MLJAR AutoML supports two methods for bias mitigation:
+         - Sample Weighting - assigns weights to samples to treat samples equally,
+         - Smart Grid Search - similar to Sample Weighting where different weights are checked to optimize fairness metric.
+        
+        The fair ML bulding can be used with all algorithms including `Ensemble` and `Stacked Ensemble`. We support three Machine Learning tasks:
+         - binary classification,
+         - mutliclass classification,
+         - regression.
+        
+        Example code:
+        
+        
+        ```python
+        from sklearn.model_selection import train_test_split
+        from sklearn.datasets import fetch_openml
+        from supervised.automl import AutoML
+        
+        data = fetch_openml(data_id=1590, as_frame=True)
+        X = data.data
+        y = (data.target == ">50K") * 1
+        sensitive_features = X[["sex"]]
+        
+        X_train, X_test, y_train, y_test, S_train, S_test = train_test_split(
+            X, y, sensitive_features, stratify=y, test_size=0.75, random_state=42
+        )
+        
+        automl = AutoML(
+            algorithms=[
+                "Xgboost"
+            ],
+            train_ensemble=False,
+            fairness_metric="demographic_parity_ratio",  
+            fairness_threshold=0.8,
+            privileged_groups = [{"sex": "Male"}],
+            underprivileged_groups = [{"sex": "Female"}],
+        )
+        
+        automl.fit(X_train, y_train, sensitive_features=S_train)
+        ```
+        
+        You can read more about fairness aware AutoML training in our article https://mljar.com/blog/fairness-machine-learning/
+        
+        ![Fairness aware AutoML](https://raw.githubusercontent.com/mljar/visual-identity/main/automl/fairness-automl.gif)
+        
+        
+        
         # Examples
         
         ## :point_right: Binary Classification Example
         
         There is a simple interface available with `fit` and `predict` methods.
         
         ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mljar-supervised Version: 1.0.0 Summary: Automated
+Metadata-Version: 2.1 Name: mljar-supervised Version: 1.0.1 Summary: Automated
 Machine Learning for Humans Home-page: https://github.com/mljar/mljar-
 supervised Author: MLJAR, Sp. z o.o. Author-email: contact@mljar.com License:
 MIT Description: # MLJAR Automated Machine Learning for Humans [![Tests status]
 (https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml/
 badge.svg)](https://github.com/mljar/mljar-supervised/actions/workflows/run-
 tests.yml) [![PyPI version](https://badge.fury.io/py/mljar-supervised.svg)]
 (https://badge.fury.io/py/mljar-supervised) [![Anaconda-Server Badge](https://
@@ -22,71 +22,72 @@
 contact us by [email](https://mljar.com/contact/) for details
    [https://github.com/mljar/visual-identity/raw/main/robots/robot_docs.png]
 --- ## Table of Contents - [Automated Machine Learning](https://github.com/
 mljar/mljar-supervised#automated-machine-learning) - [What's good in it?]
 (https://github.com/mljar/mljar-supervised#whats-good-in-it) - [Automatic
 Documentation](https://github.com/mljar/mljar-supervised#automatic-
 documentation) - [Available Modes](https://github.com/mljar/mljar-
-supervised#available-modes) - [Examples](https://github.com/mljar/mljar-
-supervised#examples) - [FAQ](https://github.com/mljar/mljar-supervised#faq) -
-[Documentation](https://github.com/mljar/mljar-supervised#documentation) -
-[Installation](https://github.com/mljar/mljar-supervised#installation) - [Demo]
-(https://github.com/mljar/mljar-supervised#demo) - [Contributing](https://
-github.com/mljar/mljar-supervised#contributing) - [Cite](https://github.com/
-mljar/mljar-supervised#cite) - [License](https://github.com/mljar/mljar-
-supervised#license) - [Commercial support](https://github.com/mljar/mljar-
-supervised#commercial-support) - [MLJAR](https://github.com/mljar/mljar-
-supervised#mljar) # Automated Machine Learning The `mljar-supervised` is an
-Automated Machine Learning Python package that works with tabular data. It is
-designed to save time for a data scientist. It abstracts the common way to
-preprocess the data, construct the machine learning models, and perform hyper-
-parameters tuning to find the best model :trophy:. It is no black-box as you
-can see exactly how the ML pipeline is constructed (with a detailed Markdown
-report for each ML model). The `mljar-supervised` will help you with: -
-explaining and understanding your data (Automatic Exploratory Data Analysis), -
-trying many different machine learning models (Algorithm Selection and Hyper-
-Parameters tuning), - creating Markdown reports from analysis with details
-about all models (Automatic-Documentation), - saving, re-running and loading
-the analysis and ML models. It has four built-in modes of work: - `Explain`
-mode, which is ideal for explaining and understanding the data, with many data
-explanations, like decision trees visualization, linear models coefficients
-display, permutation importances and SHAP explanations of data, - `Perform` for
-building ML pipelines to use in production, - `Compete` mode that trains
-highly-tuned ML models with ensembling and stacking, with a purpose to use in
-ML competitions. - `Optuna` mode that can be used to search for highly-tuned ML
-models, should be used when the performance is the most important, and
-computation time is not limited (it is available from version `0.10.0`) Of
-course, you can further customize the details of each `mode` to meet the
-requirements. ## What's good in it? - It is using many algorithms: `Baseline`,
-`Linear`, `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, `CatBoost`,
-`Neural Networks`, and `Nearest Neighbors`. - It can compute Ensemble based on
-greedy algorithm from [Caruana paper](http://www.cs.cornell.edu/~alexn/papers/
-shotgun.icml04.revised.rev2.pdf). - It can stack models to build level 2
-ensemble (available in `Compete` mode or after setting `stack_models`
-parameter). - It can do features preprocessing, like: missing values imputation
-and converting categoricals. What is more, it can also handle target values
-preprocessing. - It can do advanced features engineering, like: [Golden
-Features](https://supervised.mljar.com/features/golden_features/), [Features
-Selection](https://supervised.mljar.com/features/features_selection/), Text and
-Time Transformations. - It can tune hyper-parameters with `not-so-random-
-search` algorithm (random-search over defined set of values) and hill climbing
-to fine-tune final models. - It can compute the `Baseline` for your data. That
-you will know if you need Machine Learning or not! - It has extensive
-explanations. This package is training simple `Decision Trees` with `max_depth
-<= 5`, so you can easily visualize them with amazing [dtreeviz](https://
-github.com/parrt/dtreeviz) to better understand your data. - The `mljar-
-supervised` is using simple linear regression and include its coefficients in
-the summary report, so you can check which features are used the most in the
-linear model. - It cares about explainability of models: for every algorithm,
-the feature importance is computed based on permutation. Additionally, for
-every algorithm the SHAP explanations are computed: feature importance,
-dependence plots, and decision plots (explanations can be switched off with
-`explain_level` parameter). - There is automatic documentation for every ML
-experiment run with AutoML. The `mljar-supervised` creates markdown reports
-from AutoML training full of ML details, metrics and charts.
+supervised#available-modes) - [Fairness Aware Training](https://github.com/
+mljar/mljar-supervised#fairness-aware-training) - [Examples](https://
+github.com/mljar/mljar-supervised#examples) - [FAQ](https://github.com/mljar/
+mljar-supervised#faq) - [Documentation](https://github.com/mljar/mljar-
+supervised#documentation) - [Installation](https://github.com/mljar/mljar-
+supervised#installation) - [Demo](https://github.com/mljar/mljar-
+supervised#demo) - [Contributing](https://github.com/mljar/mljar-
+supervised#contributing) - [Cite](https://github.com/mljar/mljar-
+supervised#cite) - [License](https://github.com/mljar/mljar-supervised#license)
+- [Commercial support](https://github.com/mljar/mljar-supervised#commercial-
+support) - [MLJAR](https://github.com/mljar/mljar-supervised#mljar) # Automated
+Machine Learning The `mljar-supervised` is an Automated Machine Learning Python
+package that works with tabular data. It is designed to save time for a data
+scientist. It abstracts the common way to preprocess the data, construct the
+machine learning models, and perform hyper-parameters tuning to find the best
+model :trophy:. It is no black-box as you can see exactly how the ML pipeline
+is constructed (with a detailed Markdown report for each ML model). The `mljar-
+supervised` will help you with: - explaining and understanding your data
+(Automatic Exploratory Data Analysis), - trying many different machine learning
+models (Algorithm Selection and Hyper-Parameters tuning), - creating Markdown
+reports from analysis with details about all models (Automatic-Documentation),
+- saving, re-running and loading the analysis and ML models. It has four built-
+in modes of work: - `Explain` mode, which is ideal for explaining and
+understanding the data, with many data explanations, like decision trees
+visualization, linear models coefficients display, permutation importances and
+SHAP explanations of data, - `Perform` for building ML pipelines to use in
+production, - `Compete` mode that trains highly-tuned ML models with ensembling
+and stacking, with a purpose to use in ML competitions. - `Optuna` mode that
+can be used to search for highly-tuned ML models, should be used when the
+performance is the most important, and computation time is not limited (it is
+available from version `0.10.0`) Of course, you can further customize the
+details of each `mode` to meet the requirements. ## What's good in it? - It is
+using many algorithms: `Baseline`, `Linear`, `Random Forest`, `Extra Trees`,
+`LightGBM`, `Xgboost`, `CatBoost`, `Neural Networks`, and `Nearest Neighbors`.
+- It can compute Ensemble based on greedy algorithm from [Caruana paper](http:/
+/www.cs.cornell.edu/~alexn/papers/shotgun.icml04.revised.rev2.pdf). - It can
+stack models to build level 2 ensemble (available in `Compete` mode or after
+setting `stack_models` parameter). - It can do features preprocessing, like:
+missing values imputation and converting categoricals. What is more, it can
+also handle target values preprocessing. - It can do advanced features
+engineering, like: [Golden Features](https://supervised.mljar.com/features/
+golden_features/), [Features Selection](https://supervised.mljar.com/features/
+features_selection/), Text and Time Transformations. - It can tune hyper-
+parameters with `not-so-random-search` algorithm (random-search over defined
+set of values) and hill climbing to fine-tune final models. - It can compute
+the `Baseline` for your data. That you will know if you need Machine Learning
+or not! - It has extensive explanations. This package is training simple
+`Decision Trees` with `max_depth <= 5`, so you can easily visualize them with
+amazing [dtreeviz](https://github.com/parrt/dtreeviz) to better understand your
+data. - The `mljar-supervised` is using simple linear regression and include
+its coefficients in the summary report, so you can check which features are
+used the most in the linear model. - It cares about explainability of models:
+for every algorithm, the feature importance is computed based on permutation.
+Additionally, for every algorithm the SHAP explanations are computed: feature
+importance, dependence plots, and decision plots (explanations can be switched
+off with `explain_level` parameter). - There is automatic documentation for
+every ML experiment run with AutoML. The `mljar-supervised` creates markdown
+reports from AutoML training full of ML details, metrics and charts.
      [https://raw.githubusercontent.com/mljar/visual-identity/main/media/
                                 infograph.png]
 # Automatic Documentation ## The AutoML Report The report from running AutoML
 will contain the table with infomation about each model score and time needed
 to train the model. For each model there is a link, which you can click to see
 model's details. The performance of all ML models is presented as scatter and
 box plots so you can visually inspect which algorithms perform the best :
@@ -143,28 +144,57 @@
 same training code after the interruption and AutoML reloads already trained
 models and finish the training. ## Supported evaluation metrics (`eval_metric`
 argument in `AutoML()`) - for binary classification: `logloss`, `auc`, `f1`,
 `average_precision`, `accuracy`- default is `logloss` - for mutliclass
 classification: `logloss`, `f1`, `accuracy` - default is `logloss` - for
 regression: `rmse`, `mse`, `mae`, `r2`, `mape`, `spearman`, `pearson` - default
 is `rmse` If you don't find `eval_metric` that you need, please add a new
-issue. We will add it. # Examples ## :point_right: Binary Classification
-Example There is a simple interface available with `fit` and `predict` methods.
-```python import pandas as pd from sklearn.model_selection import
-train_test_split from supervised.automl import AutoML df = pd.read_csv( "https:
-//raw.githubusercontent.com/pplonski/datasets-for-start/master/adult/data.csv",
-skipinitialspace=True, ) X_train, X_test, y_train, y_test = train_test_split
-( df[df.columns[:-1]], df["income"], test_size=0.25 ) automl = AutoML()
-automl.fit(X_train, y_train) predictions = automl.predict(X_test) ``` AutoML
-`fit` will print: ```py Create directory AutoML_1 AutoML task to be solved:
-binary_classification AutoML will use algorithms: ['Baseline', 'Linear',
-'Decision Tree', 'Random Forest', 'Xgboost', 'Neural Network'] AutoML will
-optimize for metric: logloss 1_Baseline final logloss 0.5519845471086654 time
-0.08 seconds 2_DecisionTree final logloss 0.3655910192804364 time 10.28 seconds
-3_Linear final logloss 0.38139916864708445 time 3.19 seconds
+issue. We will add it. ## Fairness Aware Training Starting from version `1.0.0`
+AutoML can optimize Machine Learning pipline with sensitive features. There are
+following fairness releated arguments in the AutoML constructor: -
+`fairness_metric` - metric which will be used to decide if the model is fair, -
+`fairness_threshold` - threshold used in decision about model fairness, -
+`privileged_groups` - privileged groups used in fairness metrics computation, -
+`underprivileged_groups` - underprivileged groups used in fairness metrics
+computation. The `fit()` method accepts `sensitive_features`. When sensitive
+features are passed to AutoML, the best model will be selected among fair
+models only. In the AutoML reports additional information about fairness
+metrics will be added. The MLJAR AutoML supports two methods for bias
+mitigation: - Sample Weighting - assigns weights to samples to treat samples
+equally, - Smart Grid Search - similar to Sample Weighting where different
+weights are checked to optimize fairness metric. The fair ML bulding can be
+used with all algorithms including `Ensemble` and `Stacked Ensemble`. We
+support three Machine Learning tasks: - binary classification, - mutliclass
+classification, - regression. Example code: ```python from
+sklearn.model_selection import train_test_split from sklearn.datasets import
+fetch_openml from supervised.automl import AutoML data = fetch_openml
+(data_id=1590, as_frame=True) X = data.data y = (data.target == ">50K") * 1
+sensitive_features = X[["sex"]] X_train, X_test, y_train, y_test, S_train,
+S_test = train_test_split( X, y, sensitive_features, stratify=y,
+test_size=0.75, random_state=42 ) automl = AutoML( algorithms=[ "Xgboost" ],
+train_ensemble=False, fairness_metric="demographic_parity_ratio",
+fairness_threshold=0.8, privileged_groups = [{"sex": "Male"}],
+underprivileged_groups = [{"sex": "Female"}], ) automl.fit(X_train, y_train,
+sensitive_features=S_train) ``` You can read more about fairness aware AutoML
+training in our article https://mljar.com/blog/fairness-machine-learning/ !
+[Fairness aware AutoML](https://raw.githubusercontent.com/mljar/visual-
+identity/main/automl/fairness-automl.gif) # Examples ## :point_right: Binary
+Classification Example There is a simple interface available with `fit` and
+`predict` methods. ```python import pandas as pd from sklearn.model_selection
+import train_test_split from supervised.automl import AutoML df = pd.read_csv
+( "https://raw.githubusercontent.com/pplonski/datasets-for-start/master/adult/
+data.csv", skipinitialspace=True, ) X_train, X_test, y_train, y_test =
+train_test_split( df[df.columns[:-1]], df["income"], test_size=0.25 ) automl =
+AutoML() automl.fit(X_train, y_train) predictions = automl.predict(X_test) ```
+AutoML `fit` will print: ```py Create directory AutoML_1 AutoML task to be
+solved: binary_classification AutoML will use algorithms: ['Baseline',
+'Linear', 'Decision Tree', 'Random Forest', 'Xgboost', 'Neural Network'] AutoML
+will optimize for metric: logloss 1_Baseline final logloss 0.5519845471086654
+time 0.08 seconds 2_DecisionTree final logloss 0.3655910192804364 time 10.28
+seconds 3_Linear final logloss 0.38139916864708445 time 3.19 seconds
 4_Default_RandomForest final logloss 0.2975204390214936 time 79.19 seconds
 5_Default_Xgboost final logloss 0.2731086827200411 time 5.17 seconds
 6_Default_NeuralNetwork final logloss 0.319812276905242 time 21.19 seconds
 Ensemble final logloss 0.2731086821194617 time 1.43 seconds ``` - the AutoML
 results in [Markdown report](https://github.com/mljar/mljar-examples/tree/
 master/Income_classification/AutoML_1#automl-leaderboard) - the Xgboost
 [Markdown report](https://github.com/mljar/mljar-examples/blob/master/
```

### Comparing `mljar-supervised-1.0.0/README.md` & `mljar-supervised-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 ## Table of Contents
 
  - [Automated Machine Learning](https://github.com/mljar/mljar-supervised#automated-machine-learning)
  - [What's good in it?](https://github.com/mljar/mljar-supervised#whats-good-in-it)
  - [Automatic Documentation](https://github.com/mljar/mljar-supervised#automatic-documentation)
  - [Available Modes](https://github.com/mljar/mljar-supervised#available-modes)
+ - [Fairness Aware Training](https://github.com/mljar/mljar-supervised#fairness-aware-training)
  - [Examples](https://github.com/mljar/mljar-supervised#examples)
  - [FAQ](https://github.com/mljar/mljar-supervised#faq)
  - [Documentation](https://github.com/mljar/mljar-supervised#documentation)
  - [Installation](https://github.com/mljar/mljar-supervised#installation)
  - [Demo](https://github.com/mljar/mljar-supervised#demo)
  - [Contributing](https://github.com/mljar/mljar-supervised#contributing)
  - [Cite](https://github.com/mljar/mljar-supervised#cite)
@@ -158,14 +159,16 @@
 
 It should be used when the performance is the most important and time is not limited.
 - It is using 10-fold CV
 - It is using: `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, and `CatBoost`. Those algorithms are tuned by `Optuna` framework for `optuna_time_budget` seconds, each. Algorithms are tuned with original data, without advanced feature engineering.
 - It is using advanced feature engineering, stacking and ensembling. The hyperparameters found for original data are reused with those steps.
 - It produces learning curves in the reports.
 
+
+
 ## How to save and load AutoML?
 
 All models in the AutoML are saved and loaded automatically. No need to call `save()` or `load()`.
 
 ### Example:
 
 #### Train AutoML
@@ -194,14 +197,69 @@
 
 - for binary classification: `logloss`, `auc`, `f1`, `average_precision`, `accuracy`- default is `logloss`
 - for mutliclass classification: `logloss`, `f1`, `accuracy` - default is `logloss`
 - for regression: `rmse`, `mse`, `mae`, `r2`, `mape`, `spearman`, `pearson` - default is `rmse`
 
 If you don't find `eval_metric` that you need, please add a new issue. We will add it.
 
+
+## Fairness Aware Training
+
+Starting from version `1.0.0` AutoML can optimize Machine Learning pipline with sensitive features. There are following fairness releated arguments in the AutoML constructor:
+ - `fairness_metric` - metric which will be used to decide if the model is fair,
+ - `fairness_threshold` - threshold used in decision about model fairness,
+ - `privileged_groups` - privileged groups used in fairness metrics computation,
+ - `underprivileged_groups` - underprivileged groups used in fairness metrics computation.
+
+The `fit()` method accepts `sensitive_features`. When sensitive features are passed to AutoML, the best model will be selected among fair models only. In the AutoML reports additional information about fairness metrics will be added. The MLJAR AutoML supports two methods for bias mitigation:
+ - Sample Weighting - assigns weights to samples to treat samples equally,
+ - Smart Grid Search - similar to Sample Weighting where different weights are checked to optimize fairness metric.
+
+The fair ML bulding can be used with all algorithms including `Ensemble` and `Stacked Ensemble`. We support three Machine Learning tasks:
+ - binary classification,
+ - mutliclass classification,
+ - regression.
+
+Example code:
+
+
+```python
+from sklearn.model_selection import train_test_split
+from sklearn.datasets import fetch_openml
+from supervised.automl import AutoML
+
+data = fetch_openml(data_id=1590, as_frame=True)
+X = data.data
+y = (data.target == ">50K") * 1
+sensitive_features = X[["sex"]]
+
+X_train, X_test, y_train, y_test, S_train, S_test = train_test_split(
+    X, y, sensitive_features, stratify=y, test_size=0.75, random_state=42
+)
+
+automl = AutoML(
+    algorithms=[
+        "Xgboost"
+    ],
+    train_ensemble=False,
+    fairness_metric="demographic_parity_ratio",  
+    fairness_threshold=0.8,
+    privileged_groups = [{"sex": "Male"}],
+    underprivileged_groups = [{"sex": "Female"}],
+)
+
+automl.fit(X_train, y_train, sensitive_features=S_train)
+```
+
+You can read more about fairness aware AutoML training in our article https://mljar.com/blog/fairness-machine-learning/
+
+![Fairness aware AutoML](https://raw.githubusercontent.com/mljar/visual-identity/main/automl/fairness-automl.gif)
+
+
+
 # Examples
 
 ## :point_right: Binary Classification Example
 
 There is a simple interface available with `fit` and `predict` methods.
 
 ```python
```

#### html2text {}

```diff
@@ -19,71 +19,72 @@
 contact us by [email](https://mljar.com/contact/) for details
    [https://github.com/mljar/visual-identity/raw/main/robots/robot_docs.png]
 --- ## Table of Contents - [Automated Machine Learning](https://github.com/
 mljar/mljar-supervised#automated-machine-learning) - [What's good in it?]
 (https://github.com/mljar/mljar-supervised#whats-good-in-it) - [Automatic
 Documentation](https://github.com/mljar/mljar-supervised#automatic-
 documentation) - [Available Modes](https://github.com/mljar/mljar-
-supervised#available-modes) - [Examples](https://github.com/mljar/mljar-
-supervised#examples) - [FAQ](https://github.com/mljar/mljar-supervised#faq) -
-[Documentation](https://github.com/mljar/mljar-supervised#documentation) -
-[Installation](https://github.com/mljar/mljar-supervised#installation) - [Demo]
-(https://github.com/mljar/mljar-supervised#demo) - [Contributing](https://
-github.com/mljar/mljar-supervised#contributing) - [Cite](https://github.com/
-mljar/mljar-supervised#cite) - [License](https://github.com/mljar/mljar-
-supervised#license) - [Commercial support](https://github.com/mljar/mljar-
-supervised#commercial-support) - [MLJAR](https://github.com/mljar/mljar-
-supervised#mljar) # Automated Machine Learning The `mljar-supervised` is an
-Automated Machine Learning Python package that works with tabular data. It is
-designed to save time for a data scientist. It abstracts the common way to
-preprocess the data, construct the machine learning models, and perform hyper-
-parameters tuning to find the best model :trophy:. It is no black-box as you
-can see exactly how the ML pipeline is constructed (with a detailed Markdown
-report for each ML model). The `mljar-supervised` will help you with: -
-explaining and understanding your data (Automatic Exploratory Data Analysis), -
-trying many different machine learning models (Algorithm Selection and Hyper-
-Parameters tuning), - creating Markdown reports from analysis with details
-about all models (Automatic-Documentation), - saving, re-running and loading
-the analysis and ML models. It has four built-in modes of work: - `Explain`
-mode, which is ideal for explaining and understanding the data, with many data
-explanations, like decision trees visualization, linear models coefficients
-display, permutation importances and SHAP explanations of data, - `Perform` for
-building ML pipelines to use in production, - `Compete` mode that trains
-highly-tuned ML models with ensembling and stacking, with a purpose to use in
-ML competitions. - `Optuna` mode that can be used to search for highly-tuned ML
-models, should be used when the performance is the most important, and
-computation time is not limited (it is available from version `0.10.0`) Of
-course, you can further customize the details of each `mode` to meet the
-requirements. ## What's good in it? - It is using many algorithms: `Baseline`,
-`Linear`, `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, `CatBoost`,
-`Neural Networks`, and `Nearest Neighbors`. - It can compute Ensemble based on
-greedy algorithm from [Caruana paper](http://www.cs.cornell.edu/~alexn/papers/
-shotgun.icml04.revised.rev2.pdf). - It can stack models to build level 2
-ensemble (available in `Compete` mode or after setting `stack_models`
-parameter). - It can do features preprocessing, like: missing values imputation
-and converting categoricals. What is more, it can also handle target values
-preprocessing. - It can do advanced features engineering, like: [Golden
-Features](https://supervised.mljar.com/features/golden_features/), [Features
-Selection](https://supervised.mljar.com/features/features_selection/), Text and
-Time Transformations. - It can tune hyper-parameters with `not-so-random-
-search` algorithm (random-search over defined set of values) and hill climbing
-to fine-tune final models. - It can compute the `Baseline` for your data. That
-you will know if you need Machine Learning or not! - It has extensive
-explanations. This package is training simple `Decision Trees` with `max_depth
-<= 5`, so you can easily visualize them with amazing [dtreeviz](https://
-github.com/parrt/dtreeviz) to better understand your data. - The `mljar-
-supervised` is using simple linear regression and include its coefficients in
-the summary report, so you can check which features are used the most in the
-linear model. - It cares about explainability of models: for every algorithm,
-the feature importance is computed based on permutation. Additionally, for
-every algorithm the SHAP explanations are computed: feature importance,
-dependence plots, and decision plots (explanations can be switched off with
-`explain_level` parameter). - There is automatic documentation for every ML
-experiment run with AutoML. The `mljar-supervised` creates markdown reports
-from AutoML training full of ML details, metrics and charts.
+supervised#available-modes) - [Fairness Aware Training](https://github.com/
+mljar/mljar-supervised#fairness-aware-training) - [Examples](https://
+github.com/mljar/mljar-supervised#examples) - [FAQ](https://github.com/mljar/
+mljar-supervised#faq) - [Documentation](https://github.com/mljar/mljar-
+supervised#documentation) - [Installation](https://github.com/mljar/mljar-
+supervised#installation) - [Demo](https://github.com/mljar/mljar-
+supervised#demo) - [Contributing](https://github.com/mljar/mljar-
+supervised#contributing) - [Cite](https://github.com/mljar/mljar-
+supervised#cite) - [License](https://github.com/mljar/mljar-supervised#license)
+- [Commercial support](https://github.com/mljar/mljar-supervised#commercial-
+support) - [MLJAR](https://github.com/mljar/mljar-supervised#mljar) # Automated
+Machine Learning The `mljar-supervised` is an Automated Machine Learning Python
+package that works with tabular data. It is designed to save time for a data
+scientist. It abstracts the common way to preprocess the data, construct the
+machine learning models, and perform hyper-parameters tuning to find the best
+model :trophy:. It is no black-box as you can see exactly how the ML pipeline
+is constructed (with a detailed Markdown report for each ML model). The `mljar-
+supervised` will help you with: - explaining and understanding your data
+(Automatic Exploratory Data Analysis), - trying many different machine learning
+models (Algorithm Selection and Hyper-Parameters tuning), - creating Markdown
+reports from analysis with details about all models (Automatic-Documentation),
+- saving, re-running and loading the analysis and ML models. It has four built-
+in modes of work: - `Explain` mode, which is ideal for explaining and
+understanding the data, with many data explanations, like decision trees
+visualization, linear models coefficients display, permutation importances and
+SHAP explanations of data, - `Perform` for building ML pipelines to use in
+production, - `Compete` mode that trains highly-tuned ML models with ensembling
+and stacking, with a purpose to use in ML competitions. - `Optuna` mode that
+can be used to search for highly-tuned ML models, should be used when the
+performance is the most important, and computation time is not limited (it is
+available from version `0.10.0`) Of course, you can further customize the
+details of each `mode` to meet the requirements. ## What's good in it? - It is
+using many algorithms: `Baseline`, `Linear`, `Random Forest`, `Extra Trees`,
+`LightGBM`, `Xgboost`, `CatBoost`, `Neural Networks`, and `Nearest Neighbors`.
+- It can compute Ensemble based on greedy algorithm from [Caruana paper](http:/
+/www.cs.cornell.edu/~alexn/papers/shotgun.icml04.revised.rev2.pdf). - It can
+stack models to build level 2 ensemble (available in `Compete` mode or after
+setting `stack_models` parameter). - It can do features preprocessing, like:
+missing values imputation and converting categoricals. What is more, it can
+also handle target values preprocessing. - It can do advanced features
+engineering, like: [Golden Features](https://supervised.mljar.com/features/
+golden_features/), [Features Selection](https://supervised.mljar.com/features/
+features_selection/), Text and Time Transformations. - It can tune hyper-
+parameters with `not-so-random-search` algorithm (random-search over defined
+set of values) and hill climbing to fine-tune final models. - It can compute
+the `Baseline` for your data. That you will know if you need Machine Learning
+or not! - It has extensive explanations. This package is training simple
+`Decision Trees` with `max_depth <= 5`, so you can easily visualize them with
+amazing [dtreeviz](https://github.com/parrt/dtreeviz) to better understand your
+data. - The `mljar-supervised` is using simple linear regression and include
+its coefficients in the summary report, so you can check which features are
+used the most in the linear model. - It cares about explainability of models:
+for every algorithm, the feature importance is computed based on permutation.
+Additionally, for every algorithm the SHAP explanations are computed: feature
+importance, dependence plots, and decision plots (explanations can be switched
+off with `explain_level` parameter). - There is automatic documentation for
+every ML experiment run with AutoML. The `mljar-supervised` creates markdown
+reports from AutoML training full of ML details, metrics and charts.
      [https://raw.githubusercontent.com/mljar/visual-identity/main/media/
                                 infograph.png]
 # Automatic Documentation ## The AutoML Report The report from running AutoML
 will contain the table with infomation about each model score and time needed
 to train the model. For each model there is a link, which you can click to see
 model's details. The performance of all ML models is presented as scatter and
 box plots so you can visually inspect which algorithms perform the best :
@@ -140,28 +141,57 @@
 same training code after the interruption and AutoML reloads already trained
 models and finish the training. ## Supported evaluation metrics (`eval_metric`
 argument in `AutoML()`) - for binary classification: `logloss`, `auc`, `f1`,
 `average_precision`, `accuracy`- default is `logloss` - for mutliclass
 classification: `logloss`, `f1`, `accuracy` - default is `logloss` - for
 regression: `rmse`, `mse`, `mae`, `r2`, `mape`, `spearman`, `pearson` - default
 is `rmse` If you don't find `eval_metric` that you need, please add a new
-issue. We will add it. # Examples ## :point_right: Binary Classification
-Example There is a simple interface available with `fit` and `predict` methods.
-```python import pandas as pd from sklearn.model_selection import
-train_test_split from supervised.automl import AutoML df = pd.read_csv( "https:
-//raw.githubusercontent.com/pplonski/datasets-for-start/master/adult/data.csv",
-skipinitialspace=True, ) X_train, X_test, y_train, y_test = train_test_split
-( df[df.columns[:-1]], df["income"], test_size=0.25 ) automl = AutoML()
-automl.fit(X_train, y_train) predictions = automl.predict(X_test) ``` AutoML
-`fit` will print: ```py Create directory AutoML_1 AutoML task to be solved:
-binary_classification AutoML will use algorithms: ['Baseline', 'Linear',
-'Decision Tree', 'Random Forest', 'Xgboost', 'Neural Network'] AutoML will
-optimize for metric: logloss 1_Baseline final logloss 0.5519845471086654 time
-0.08 seconds 2_DecisionTree final logloss 0.3655910192804364 time 10.28 seconds
-3_Linear final logloss 0.38139916864708445 time 3.19 seconds
+issue. We will add it. ## Fairness Aware Training Starting from version `1.0.0`
+AutoML can optimize Machine Learning pipline with sensitive features. There are
+following fairness releated arguments in the AutoML constructor: -
+`fairness_metric` - metric which will be used to decide if the model is fair, -
+`fairness_threshold` - threshold used in decision about model fairness, -
+`privileged_groups` - privileged groups used in fairness metrics computation, -
+`underprivileged_groups` - underprivileged groups used in fairness metrics
+computation. The `fit()` method accepts `sensitive_features`. When sensitive
+features are passed to AutoML, the best model will be selected among fair
+models only. In the AutoML reports additional information about fairness
+metrics will be added. The MLJAR AutoML supports two methods for bias
+mitigation: - Sample Weighting - assigns weights to samples to treat samples
+equally, - Smart Grid Search - similar to Sample Weighting where different
+weights are checked to optimize fairness metric. The fair ML bulding can be
+used with all algorithms including `Ensemble` and `Stacked Ensemble`. We
+support three Machine Learning tasks: - binary classification, - mutliclass
+classification, - regression. Example code: ```python from
+sklearn.model_selection import train_test_split from sklearn.datasets import
+fetch_openml from supervised.automl import AutoML data = fetch_openml
+(data_id=1590, as_frame=True) X = data.data y = (data.target == ">50K") * 1
+sensitive_features = X[["sex"]] X_train, X_test, y_train, y_test, S_train,
+S_test = train_test_split( X, y, sensitive_features, stratify=y,
+test_size=0.75, random_state=42 ) automl = AutoML( algorithms=[ "Xgboost" ],
+train_ensemble=False, fairness_metric="demographic_parity_ratio",
+fairness_threshold=0.8, privileged_groups = [{"sex": "Male"}],
+underprivileged_groups = [{"sex": "Female"}], ) automl.fit(X_train, y_train,
+sensitive_features=S_train) ``` You can read more about fairness aware AutoML
+training in our article https://mljar.com/blog/fairness-machine-learning/ !
+[Fairness aware AutoML](https://raw.githubusercontent.com/mljar/visual-
+identity/main/automl/fairness-automl.gif) # Examples ## :point_right: Binary
+Classification Example There is a simple interface available with `fit` and
+`predict` methods. ```python import pandas as pd from sklearn.model_selection
+import train_test_split from supervised.automl import AutoML df = pd.read_csv
+( "https://raw.githubusercontent.com/pplonski/datasets-for-start/master/adult/
+data.csv", skipinitialspace=True, ) X_train, X_test, y_train, y_test =
+train_test_split( df[df.columns[:-1]], df["income"], test_size=0.25 ) automl =
+AutoML() automl.fit(X_train, y_train) predictions = automl.predict(X_test) ```
+AutoML `fit` will print: ```py Create directory AutoML_1 AutoML task to be
+solved: binary_classification AutoML will use algorithms: ['Baseline',
+'Linear', 'Decision Tree', 'Random Forest', 'Xgboost', 'Neural Network'] AutoML
+will optimize for metric: logloss 1_Baseline final logloss 0.5519845471086654
+time 0.08 seconds 2_DecisionTree final logloss 0.3655910192804364 time 10.28
+seconds 3_Linear final logloss 0.38139916864708445 time 3.19 seconds
 4_Default_RandomForest final logloss 0.2975204390214936 time 79.19 seconds
 5_Default_Xgboost final logloss 0.2731086827200411 time 5.17 seconds
 6_Default_NeuralNetwork final logloss 0.319812276905242 time 21.19 seconds
 Ensemble final logloss 0.2731086821194617 time 1.43 seconds ``` - the AutoML
 results in [Markdown report](https://github.com/mljar/mljar-examples/tree/
 master/Income_classification/AutoML_1#automl-leaderboard) - the Xgboost
 [Markdown report](https://github.com/mljar/mljar-examples/blob/master/
```

### Comparing `mljar-supervised-1.0.0/mljar_supervised.egg-info/PKG-INFO` & `mljar-supervised-1.0.1/mljar_supervised.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mljar-supervised
-Version: 1.0.0
+Version: 1.0.1
 Summary: Automated Machine Learning for Humans
 Home-page: https://github.com/mljar/mljar-supervised
 Author: MLJAR, Sp. z o.o.
 Author-email: contact@mljar.com
 License: MIT
 Description: # MLJAR Automated Machine Learning for Humans
         
@@ -39,14 +39,15 @@
         
         ## Table of Contents
         
          - [Automated Machine Learning](https://github.com/mljar/mljar-supervised#automated-machine-learning)
          - [What's good in it?](https://github.com/mljar/mljar-supervised#whats-good-in-it)
          - [Automatic Documentation](https://github.com/mljar/mljar-supervised#automatic-documentation)
          - [Available Modes](https://github.com/mljar/mljar-supervised#available-modes)
+         - [Fairness Aware Training](https://github.com/mljar/mljar-supervised#fairness-aware-training)
          - [Examples](https://github.com/mljar/mljar-supervised#examples)
          - [FAQ](https://github.com/mljar/mljar-supervised#faq)
          - [Documentation](https://github.com/mljar/mljar-supervised#documentation)
          - [Installation](https://github.com/mljar/mljar-supervised#installation)
          - [Demo](https://github.com/mljar/mljar-supervised#demo)
          - [Contributing](https://github.com/mljar/mljar-supervised#contributing)
          - [Cite](https://github.com/mljar/mljar-supervised#cite)
@@ -166,14 +167,16 @@
         
         It should be used when the performance is the most important and time is not limited.
         - It is using 10-fold CV
         - It is using: `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, and `CatBoost`. Those algorithms are tuned by `Optuna` framework for `optuna_time_budget` seconds, each. Algorithms are tuned with original data, without advanced feature engineering.
         - It is using advanced feature engineering, stacking and ensembling. The hyperparameters found for original data are reused with those steps.
         - It produces learning curves in the reports.
         
+        
+        
         ## How to save and load AutoML?
         
         All models in the AutoML are saved and loaded automatically. No need to call `save()` or `load()`.
         
         ### Example:
         
         #### Train AutoML
@@ -202,14 +205,69 @@
         
         - for binary classification: `logloss`, `auc`, `f1`, `average_precision`, `accuracy`- default is `logloss`
         - for mutliclass classification: `logloss`, `f1`, `accuracy` - default is `logloss`
         - for regression: `rmse`, `mse`, `mae`, `r2`, `mape`, `spearman`, `pearson` - default is `rmse`
         
         If you don't find `eval_metric` that you need, please add a new issue. We will add it.
         
+        
+        ## Fairness Aware Training
+        
+        Starting from version `1.0.0` AutoML can optimize Machine Learning pipline with sensitive features. There are following fairness releated arguments in the AutoML constructor:
+         - `fairness_metric` - metric which will be used to decide if the model is fair,
+         - `fairness_threshold` - threshold used in decision about model fairness,
+         - `privileged_groups` - privileged groups used in fairness metrics computation,
+         - `underprivileged_groups` - underprivileged groups used in fairness metrics computation.
+        
+        The `fit()` method accepts `sensitive_features`. When sensitive features are passed to AutoML, the best model will be selected among fair models only. In the AutoML reports additional information about fairness metrics will be added. The MLJAR AutoML supports two methods for bias mitigation:
+         - Sample Weighting - assigns weights to samples to treat samples equally,
+         - Smart Grid Search - similar to Sample Weighting where different weights are checked to optimize fairness metric.
+        
+        The fair ML bulding can be used with all algorithms including `Ensemble` and `Stacked Ensemble`. We support three Machine Learning tasks:
+         - binary classification,
+         - mutliclass classification,
+         - regression.
+        
+        Example code:
+        
+        
+        ```python
+        from sklearn.model_selection import train_test_split
+        from sklearn.datasets import fetch_openml
+        from supervised.automl import AutoML
+        
+        data = fetch_openml(data_id=1590, as_frame=True)
+        X = data.data
+        y = (data.target == ">50K") * 1
+        sensitive_features = X[["sex"]]
+        
+        X_train, X_test, y_train, y_test, S_train, S_test = train_test_split(
+            X, y, sensitive_features, stratify=y, test_size=0.75, random_state=42
+        )
+        
+        automl = AutoML(
+            algorithms=[
+                "Xgboost"
+            ],
+            train_ensemble=False,
+            fairness_metric="demographic_parity_ratio",  
+            fairness_threshold=0.8,
+            privileged_groups = [{"sex": "Male"}],
+            underprivileged_groups = [{"sex": "Female"}],
+        )
+        
+        automl.fit(X_train, y_train, sensitive_features=S_train)
+        ```
+        
+        You can read more about fairness aware AutoML training in our article https://mljar.com/blog/fairness-machine-learning/
+        
+        ![Fairness aware AutoML](https://raw.githubusercontent.com/mljar/visual-identity/main/automl/fairness-automl.gif)
+        
+        
+        
         # Examples
         
         ## :point_right: Binary Classification Example
         
         There is a simple interface available with `fit` and `predict` methods.
         
         ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mljar-supervised Version: 1.0.0 Summary: Automated
+Metadata-Version: 2.1 Name: mljar-supervised Version: 1.0.1 Summary: Automated
 Machine Learning for Humans Home-page: https://github.com/mljar/mljar-
 supervised Author: MLJAR, Sp. z o.o. Author-email: contact@mljar.com License:
 MIT Description: # MLJAR Automated Machine Learning for Humans [![Tests status]
 (https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml/
 badge.svg)](https://github.com/mljar/mljar-supervised/actions/workflows/run-
 tests.yml) [![PyPI version](https://badge.fury.io/py/mljar-supervised.svg)]
 (https://badge.fury.io/py/mljar-supervised) [![Anaconda-Server Badge](https://
@@ -22,71 +22,72 @@
 contact us by [email](https://mljar.com/contact/) for details
    [https://github.com/mljar/visual-identity/raw/main/robots/robot_docs.png]
 --- ## Table of Contents - [Automated Machine Learning](https://github.com/
 mljar/mljar-supervised#automated-machine-learning) - [What's good in it?]
 (https://github.com/mljar/mljar-supervised#whats-good-in-it) - [Automatic
 Documentation](https://github.com/mljar/mljar-supervised#automatic-
 documentation) - [Available Modes](https://github.com/mljar/mljar-
-supervised#available-modes) - [Examples](https://github.com/mljar/mljar-
-supervised#examples) - [FAQ](https://github.com/mljar/mljar-supervised#faq) -
-[Documentation](https://github.com/mljar/mljar-supervised#documentation) -
-[Installation](https://github.com/mljar/mljar-supervised#installation) - [Demo]
-(https://github.com/mljar/mljar-supervised#demo) - [Contributing](https://
-github.com/mljar/mljar-supervised#contributing) - [Cite](https://github.com/
-mljar/mljar-supervised#cite) - [License](https://github.com/mljar/mljar-
-supervised#license) - [Commercial support](https://github.com/mljar/mljar-
-supervised#commercial-support) - [MLJAR](https://github.com/mljar/mljar-
-supervised#mljar) # Automated Machine Learning The `mljar-supervised` is an
-Automated Machine Learning Python package that works with tabular data. It is
-designed to save time for a data scientist. It abstracts the common way to
-preprocess the data, construct the machine learning models, and perform hyper-
-parameters tuning to find the best model :trophy:. It is no black-box as you
-can see exactly how the ML pipeline is constructed (with a detailed Markdown
-report for each ML model). The `mljar-supervised` will help you with: -
-explaining and understanding your data (Automatic Exploratory Data Analysis), -
-trying many different machine learning models (Algorithm Selection and Hyper-
-Parameters tuning), - creating Markdown reports from analysis with details
-about all models (Automatic-Documentation), - saving, re-running and loading
-the analysis and ML models. It has four built-in modes of work: - `Explain`
-mode, which is ideal for explaining and understanding the data, with many data
-explanations, like decision trees visualization, linear models coefficients
-display, permutation importances and SHAP explanations of data, - `Perform` for
-building ML pipelines to use in production, - `Compete` mode that trains
-highly-tuned ML models with ensembling and stacking, with a purpose to use in
-ML competitions. - `Optuna` mode that can be used to search for highly-tuned ML
-models, should be used when the performance is the most important, and
-computation time is not limited (it is available from version `0.10.0`) Of
-course, you can further customize the details of each `mode` to meet the
-requirements. ## What's good in it? - It is using many algorithms: `Baseline`,
-`Linear`, `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, `CatBoost`,
-`Neural Networks`, and `Nearest Neighbors`. - It can compute Ensemble based on
-greedy algorithm from [Caruana paper](http://www.cs.cornell.edu/~alexn/papers/
-shotgun.icml04.revised.rev2.pdf). - It can stack models to build level 2
-ensemble (available in `Compete` mode or after setting `stack_models`
-parameter). - It can do features preprocessing, like: missing values imputation
-and converting categoricals. What is more, it can also handle target values
-preprocessing. - It can do advanced features engineering, like: [Golden
-Features](https://supervised.mljar.com/features/golden_features/), [Features
-Selection](https://supervised.mljar.com/features/features_selection/), Text and
-Time Transformations. - It can tune hyper-parameters with `not-so-random-
-search` algorithm (random-search over defined set of values) and hill climbing
-to fine-tune final models. - It can compute the `Baseline` for your data. That
-you will know if you need Machine Learning or not! - It has extensive
-explanations. This package is training simple `Decision Trees` with `max_depth
-<= 5`, so you can easily visualize them with amazing [dtreeviz](https://
-github.com/parrt/dtreeviz) to better understand your data. - The `mljar-
-supervised` is using simple linear regression and include its coefficients in
-the summary report, so you can check which features are used the most in the
-linear model. - It cares about explainability of models: for every algorithm,
-the feature importance is computed based on permutation. Additionally, for
-every algorithm the SHAP explanations are computed: feature importance,
-dependence plots, and decision plots (explanations can be switched off with
-`explain_level` parameter). - There is automatic documentation for every ML
-experiment run with AutoML. The `mljar-supervised` creates markdown reports
-from AutoML training full of ML details, metrics and charts.
+supervised#available-modes) - [Fairness Aware Training](https://github.com/
+mljar/mljar-supervised#fairness-aware-training) - [Examples](https://
+github.com/mljar/mljar-supervised#examples) - [FAQ](https://github.com/mljar/
+mljar-supervised#faq) - [Documentation](https://github.com/mljar/mljar-
+supervised#documentation) - [Installation](https://github.com/mljar/mljar-
+supervised#installation) - [Demo](https://github.com/mljar/mljar-
+supervised#demo) - [Contributing](https://github.com/mljar/mljar-
+supervised#contributing) - [Cite](https://github.com/mljar/mljar-
+supervised#cite) - [License](https://github.com/mljar/mljar-supervised#license)
+- [Commercial support](https://github.com/mljar/mljar-supervised#commercial-
+support) - [MLJAR](https://github.com/mljar/mljar-supervised#mljar) # Automated
+Machine Learning The `mljar-supervised` is an Automated Machine Learning Python
+package that works with tabular data. It is designed to save time for a data
+scientist. It abstracts the common way to preprocess the data, construct the
+machine learning models, and perform hyper-parameters tuning to find the best
+model :trophy:. It is no black-box as you can see exactly how the ML pipeline
+is constructed (with a detailed Markdown report for each ML model). The `mljar-
+supervised` will help you with: - explaining and understanding your data
+(Automatic Exploratory Data Analysis), - trying many different machine learning
+models (Algorithm Selection and Hyper-Parameters tuning), - creating Markdown
+reports from analysis with details about all models (Automatic-Documentation),
+- saving, re-running and loading the analysis and ML models. It has four built-
+in modes of work: - `Explain` mode, which is ideal for explaining and
+understanding the data, with many data explanations, like decision trees
+visualization, linear models coefficients display, permutation importances and
+SHAP explanations of data, - `Perform` for building ML pipelines to use in
+production, - `Compete` mode that trains highly-tuned ML models with ensembling
+and stacking, with a purpose to use in ML competitions. - `Optuna` mode that
+can be used to search for highly-tuned ML models, should be used when the
+performance is the most important, and computation time is not limited (it is
+available from version `0.10.0`) Of course, you can further customize the
+details of each `mode` to meet the requirements. ## What's good in it? - It is
+using many algorithms: `Baseline`, `Linear`, `Random Forest`, `Extra Trees`,
+`LightGBM`, `Xgboost`, `CatBoost`, `Neural Networks`, and `Nearest Neighbors`.
+- It can compute Ensemble based on greedy algorithm from [Caruana paper](http:/
+/www.cs.cornell.edu/~alexn/papers/shotgun.icml04.revised.rev2.pdf). - It can
+stack models to build level 2 ensemble (available in `Compete` mode or after
+setting `stack_models` parameter). - It can do features preprocessing, like:
+missing values imputation and converting categoricals. What is more, it can
+also handle target values preprocessing. - It can do advanced features
+engineering, like: [Golden Features](https://supervised.mljar.com/features/
+golden_features/), [Features Selection](https://supervised.mljar.com/features/
+features_selection/), Text and Time Transformations. - It can tune hyper-
+parameters with `not-so-random-search` algorithm (random-search over defined
+set of values) and hill climbing to fine-tune final models. - It can compute
+the `Baseline` for your data. That you will know if you need Machine Learning
+or not! - It has extensive explanations. This package is training simple
+`Decision Trees` with `max_depth <= 5`, so you can easily visualize them with
+amazing [dtreeviz](https://github.com/parrt/dtreeviz) to better understand your
+data. - The `mljar-supervised` is using simple linear regression and include
+its coefficients in the summary report, so you can check which features are
+used the most in the linear model. - It cares about explainability of models:
+for every algorithm, the feature importance is computed based on permutation.
+Additionally, for every algorithm the SHAP explanations are computed: feature
+importance, dependence plots, and decision plots (explanations can be switched
+off with `explain_level` parameter). - There is automatic documentation for
+every ML experiment run with AutoML. The `mljar-supervised` creates markdown
+reports from AutoML training full of ML details, metrics and charts.
      [https://raw.githubusercontent.com/mljar/visual-identity/main/media/
                                 infograph.png]
 # Automatic Documentation ## The AutoML Report The report from running AutoML
 will contain the table with infomation about each model score and time needed
 to train the model. For each model there is a link, which you can click to see
 model's details. The performance of all ML models is presented as scatter and
 box plots so you can visually inspect which algorithms perform the best :
@@ -143,28 +144,57 @@
 same training code after the interruption and AutoML reloads already trained
 models and finish the training. ## Supported evaluation metrics (`eval_metric`
 argument in `AutoML()`) - for binary classification: `logloss`, `auc`, `f1`,
 `average_precision`, `accuracy`- default is `logloss` - for mutliclass
 classification: `logloss`, `f1`, `accuracy` - default is `logloss` - for
 regression: `rmse`, `mse`, `mae`, `r2`, `mape`, `spearman`, `pearson` - default
 is `rmse` If you don't find `eval_metric` that you need, please add a new
-issue. We will add it. # Examples ## :point_right: Binary Classification
-Example There is a simple interface available with `fit` and `predict` methods.
-```python import pandas as pd from sklearn.model_selection import
-train_test_split from supervised.automl import AutoML df = pd.read_csv( "https:
-//raw.githubusercontent.com/pplonski/datasets-for-start/master/adult/data.csv",
-skipinitialspace=True, ) X_train, X_test, y_train, y_test = train_test_split
-( df[df.columns[:-1]], df["income"], test_size=0.25 ) automl = AutoML()
-automl.fit(X_train, y_train) predictions = automl.predict(X_test) ``` AutoML
-`fit` will print: ```py Create directory AutoML_1 AutoML task to be solved:
-binary_classification AutoML will use algorithms: ['Baseline', 'Linear',
-'Decision Tree', 'Random Forest', 'Xgboost', 'Neural Network'] AutoML will
-optimize for metric: logloss 1_Baseline final logloss 0.5519845471086654 time
-0.08 seconds 2_DecisionTree final logloss 0.3655910192804364 time 10.28 seconds
-3_Linear final logloss 0.38139916864708445 time 3.19 seconds
+issue. We will add it. ## Fairness Aware Training Starting from version `1.0.0`
+AutoML can optimize Machine Learning pipline with sensitive features. There are
+following fairness releated arguments in the AutoML constructor: -
+`fairness_metric` - metric which will be used to decide if the model is fair, -
+`fairness_threshold` - threshold used in decision about model fairness, -
+`privileged_groups` - privileged groups used in fairness metrics computation, -
+`underprivileged_groups` - underprivileged groups used in fairness metrics
+computation. The `fit()` method accepts `sensitive_features`. When sensitive
+features are passed to AutoML, the best model will be selected among fair
+models only. In the AutoML reports additional information about fairness
+metrics will be added. The MLJAR AutoML supports two methods for bias
+mitigation: - Sample Weighting - assigns weights to samples to treat samples
+equally, - Smart Grid Search - similar to Sample Weighting where different
+weights are checked to optimize fairness metric. The fair ML bulding can be
+used with all algorithms including `Ensemble` and `Stacked Ensemble`. We
+support three Machine Learning tasks: - binary classification, - mutliclass
+classification, - regression. Example code: ```python from
+sklearn.model_selection import train_test_split from sklearn.datasets import
+fetch_openml from supervised.automl import AutoML data = fetch_openml
+(data_id=1590, as_frame=True) X = data.data y = (data.target == ">50K") * 1
+sensitive_features = X[["sex"]] X_train, X_test, y_train, y_test, S_train,
+S_test = train_test_split( X, y, sensitive_features, stratify=y,
+test_size=0.75, random_state=42 ) automl = AutoML( algorithms=[ "Xgboost" ],
+train_ensemble=False, fairness_metric="demographic_parity_ratio",
+fairness_threshold=0.8, privileged_groups = [{"sex": "Male"}],
+underprivileged_groups = [{"sex": "Female"}], ) automl.fit(X_train, y_train,
+sensitive_features=S_train) ``` You can read more about fairness aware AutoML
+training in our article https://mljar.com/blog/fairness-machine-learning/ !
+[Fairness aware AutoML](https://raw.githubusercontent.com/mljar/visual-
+identity/main/automl/fairness-automl.gif) # Examples ## :point_right: Binary
+Classification Example There is a simple interface available with `fit` and
+`predict` methods. ```python import pandas as pd from sklearn.model_selection
+import train_test_split from supervised.automl import AutoML df = pd.read_csv
+( "https://raw.githubusercontent.com/pplonski/datasets-for-start/master/adult/
+data.csv", skipinitialspace=True, ) X_train, X_test, y_train, y_test =
+train_test_split( df[df.columns[:-1]], df["income"], test_size=0.25 ) automl =
+AutoML() automl.fit(X_train, y_train) predictions = automl.predict(X_test) ```
+AutoML `fit` will print: ```py Create directory AutoML_1 AutoML task to be
+solved: binary_classification AutoML will use algorithms: ['Baseline',
+'Linear', 'Decision Tree', 'Random Forest', 'Xgboost', 'Neural Network'] AutoML
+will optimize for metric: logloss 1_Baseline final logloss 0.5519845471086654
+time 0.08 seconds 2_DecisionTree final logloss 0.3655910192804364 time 10.28
+seconds 3_Linear final logloss 0.38139916864708445 time 3.19 seconds
 4_Default_RandomForest final logloss 0.2975204390214936 time 79.19 seconds
 5_Default_Xgboost final logloss 0.2731086827200411 time 5.17 seconds
 6_Default_NeuralNetwork final logloss 0.319812276905242 time 21.19 seconds
 Ensemble final logloss 0.2731086821194617 time 1.43 seconds ``` - the AutoML
 results in [Markdown report](https://github.com/mljar/mljar-examples/tree/
 master/Income_classification/AutoML_1#automl-leaderboard) - the Xgboost
 [Markdown report](https://github.com/mljar/mljar-examples/blob/master/
```

### Comparing `mljar-supervised-1.0.0/mljar_supervised.egg-info/SOURCES.txt` & `mljar-supervised-1.0.1/mljar_supervised.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/setup.py` & `mljar-supervised-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mljar-supervised",
-    version="1.0.0",
+    version="1.0.1",
     description="Automated Machine Learning for Humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mljar/mljar-supervised",
     author="MLJAR, Sp. z o.o.",
     author_email="contact@mljar.com",
     license="MIT",
```

### Comparing `mljar-supervised-1.0.0/supervised/algorithms/algorithm.py` & `mljar-supervised-1.0.1/supervised/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/algorithms/baseline.py` & `mljar-supervised-1.0.1/supervised/algorithms/baseline.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/algorithms/catboost.py` & `mljar-supervised-1.0.1/supervised/algorithms/catboost.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/algorithms/decision_tree.py` & `mljar-supervised-1.0.1/supervised/algorithms/decision_tree.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/algorithms/extra_trees.py` & `mljar-supervised-1.0.1/supervised/algorithms/extra_trees.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/algorithms/factory.py` & `mljar-supervised-1.0.1/supervised/algorithms/factory.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/algorithms/knn.py` & `mljar-supervised-1.0.1/supervised/algorithms/knn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/algorithms/lightgbm.py` & `mljar-supervised-1.0.1/supervised/algorithms/lightgbm.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/algorithms/linear.py` & `mljar-supervised-1.0.1/supervised/algorithms/linear.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/algorithms/nn.py` & `mljar-supervised-1.0.1/supervised/algorithms/nn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/algorithms/random_forest.py` & `mljar-supervised-1.0.1/supervised/algorithms/random_forest.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/algorithms/registry.py` & `mljar-supervised-1.0.1/supervised/algorithms/registry.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/algorithms/sklearn.py` & `mljar-supervised-1.0.1/supervised/algorithms/sklearn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/algorithms/xgboost.py` & `mljar-supervised-1.0.1/supervised/algorithms/xgboost.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/automl.py` & `mljar-supervised-1.0.1/supervised/automl.py`

 * *Files 0% similar despite different names*

```diff
@@ -416,15 +416,15 @@
             y (numpy.ndarray or pandas.Series): Training targets
 
             sample_weight (numpy.ndarray or pandas.Series): Training sample weights
 
             cv (iterable or list): List or iterable with (train, validation) splits representing array of indices.
                 It is used only with custom validation (`validation_strategy={'validation_type': 'custom'}`).
 
-            sensitive_features (numpy.ndarray or pandas.Series or pandas.DataFrame): Sensitive features to learn fair models
+            sensitive_features (pandas.Series or pandas.DataFrame): Sensitive features to learn fair models
 
         Returns:
             AutoML object: Returns `self`
         """
         return self._fit(X, y, sample_weight, cv, sensitive_features)
 
     def predict(self, X: Union[List, numpy.ndarray, pandas.DataFrame]) -> numpy.ndarray:
```

### Comparing `mljar-supervised-1.0.0/supervised/base_automl.py` & `mljar-supervised-1.0.1/supervised/base_automl.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/callbacks/callback.py` & `mljar-supervised-1.0.1/supervised/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/callbacks/callback_list.py` & `mljar-supervised-1.0.1/supervised/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/callbacks/early_stopping.py` & `mljar-supervised-1.0.1/supervised/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/callbacks/learner_time_constraint.py` & `mljar-supervised-1.0.1/supervised/callbacks/learner_time_constraint.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/callbacks/max_iters_constraint.py` & `mljar-supervised-1.0.1/supervised/callbacks/max_iters_constraint.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/callbacks/metric_logger.py` & `mljar-supervised-1.0.1/supervised/callbacks/metric_logger.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/callbacks/terminate_on_nan.py` & `mljar-supervised-1.0.1/supervised/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/callbacks/total_time_constraint.py` & `mljar-supervised-1.0.1/supervised/callbacks/total_time_constraint.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/ensemble.py` & `mljar-supervised-1.0.1/supervised/ensemble.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/exceptions.py` & `mljar-supervised-1.0.1/supervised/exceptions.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/fairness/metrics.py` & `mljar-supervised-1.0.1/supervised/fairness/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         predicted_labels,
         sensitive_features,
         fairness_metric,
         fairness_threshold,
         privileged_groups=[],
         underprivileged_groups=[],
         previous_fairness_optimization=None,
-    ):
+    ):        
         target = np.array(target).ravel()
         preds = np.array(predicted_labels)
 
         fairness_metrics = {}
 
         for col in sensitive_features.columns:
             col_name = col[10:]  # skip 'senstive_'
```

### Comparing `mljar-supervised-1.0.0/supervised/fairness/optimization.py` & `mljar-supervised-1.0.1/supervised/fairness/optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
         return {
             "selection_rates": selection_rates,
             "previous_weights": previous_weights,
             "weights": weights,
             "total_dp_ratio": total_dp_ratio,
             "step": step,
-            "fairness_threshold": fairness_threshold,
+            "fairness_threshold": fairness_threshold
         }
 
     @staticmethod
     def regression(
         target,
         predictions,
         sensitive_features,
```

### Comparing `mljar-supervised-1.0.0/supervised/fairness/plots.py` & `mljar-supervised-1.0.1/supervised/fairness/plots.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/fairness/report.py` & `mljar-supervised-1.0.1/supervised/fairness/report.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/fairness/utils.py` & `mljar-supervised-1.0.1/supervised/fairness/utils.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/model_framework.py` & `mljar-supervised-1.0.1/supervised/model_framework.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/preprocessing/datetime_transformer.py` & `mljar-supervised-1.0.1/supervised/preprocessing/datetime_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/preprocessing/eda.py` & `mljar-supervised-1.0.1/supervised/preprocessing/eda.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/preprocessing/encoding_selector.py` & `mljar-supervised-1.0.1/supervised/preprocessing/encoding_selector.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/preprocessing/exclude_missing_target.py` & `mljar-supervised-1.0.1/supervised/preprocessing/exclude_missing_target.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/preprocessing/goldenfeatures_transformer.py` & `mljar-supervised-1.0.1/supervised/preprocessing/goldenfeatures_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/preprocessing/kmeans_transformer.py` & `mljar-supervised-1.0.1/supervised/preprocessing/kmeans_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/preprocessing/label_binarizer.py` & `mljar-supervised-1.0.1/supervised/preprocessing/label_binarizer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/preprocessing/label_encoder.py` & `mljar-supervised-1.0.1/supervised/preprocessing/label_encoder.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/preprocessing/loo_encoder.py` & `mljar-supervised-1.0.1/supervised/preprocessing/loo_encoder.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/preprocessing/preprocessing.py` & `mljar-supervised-1.0.1/supervised/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/preprocessing/preprocessing_categorical.py` & `mljar-supervised-1.0.1/supervised/preprocessing/preprocessing_categorical.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/preprocessing/preprocessing_missing.py` & `mljar-supervised-1.0.1/supervised/preprocessing/preprocessing_missing.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/preprocessing/preprocessing_utils.py` & `mljar-supervised-1.0.1/supervised/preprocessing/preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/preprocessing/scale.py` & `mljar-supervised-1.0.1/supervised/preprocessing/scale.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/preprocessing/text_transformer.py` & `mljar-supervised-1.0.1/supervised/preprocessing/text_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/tuner/data_info.py` & `mljar-supervised-1.0.1/supervised/tuner/data_info.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/tuner/hill_climbing.py` & `mljar-supervised-1.0.1/supervised/tuner/hill_climbing.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/tuner/mljar_tuner.py` & `mljar-supervised-1.0.1/supervised/tuner/mljar_tuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import copy
 import json
 import numpy as np
 import pandas as pd
 
 from sklearn.preprocessing import OneHotEncoder
+from supervised.preprocessing.label_encoder import LabelEncoder
 
 from supervised.tuner.random_parameters import RandomParameters
 from supervised.algorithms.registry import AlgorithmsRegistry
 from supervised.preprocessing.preprocessing_categorical import PreprocessingCategorical
 from supervised.tuner.preprocessing_tuner import PreprocessingTuner
 from supervised.tuner.hill_climbing import HillClimbing
 from supervised.algorithms.registry import (
@@ -291,14 +292,25 @@
         # get sensitive features for all samples
         sensitive_features_path = os.path.join(results_path, "sensitive_features.data")
         sensitive_features = load_data(sensitive_features_path)
 
         # get target
         y_path = os.path.join(results_path, "y.data")
         target = np.array(load_data(y_path)["target"])
+        
+        # we operate here on full target data (for all samples)
+        # we can't load preprocessed targets from other place
+        # we need to perform preprocessing here 
+        if df_models.shape[0] > 0:
+            target_preprocessing = df_models["model"].iloc[0].params.get("preprocessing", {}).get("target_preprocessing", {})
+            if PreprocessingCategorical.CONVERT_INTEGER in target_preprocessing:
+                cat_y = LabelEncoder(try_to_fit_numeric=True)
+                cat_y.fit(target)
+                target = cat_y.transform(target)
+        
 
         sensitive_columns = list(sensitive_features.columns)
 
         for i in range(df_models.shape[0]):
             model_type = df_models["model_type"].iloc[i]
 
             if df_models["model_type"].iloc[i] in ["Baseline"]:
```

### Comparing `mljar-supervised-1.0.0/supervised/tuner/optuna/catboost.py` & `mljar-supervised-1.0.1/supervised/tuner/optuna/catboost.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/tuner/optuna/extra_trees.py` & `mljar-supervised-1.0.1/supervised/tuner/optuna/extra_trees.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/tuner/optuna/knn.py` & `mljar-supervised-1.0.1/supervised/tuner/optuna/knn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/tuner/optuna/lightgbm.py` & `mljar-supervised-1.0.1/supervised/tuner/optuna/lightgbm.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/tuner/optuna/nn.py` & `mljar-supervised-1.0.1/supervised/tuner/optuna/nn.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/tuner/optuna/random_forest.py` & `mljar-supervised-1.0.1/supervised/tuner/optuna/random_forest.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/tuner/optuna/tuner.py` & `mljar-supervised-1.0.1/supervised/tuner/optuna/tuner.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/tuner/optuna/xgboost.py` & `mljar-supervised-1.0.1/supervised/tuner/optuna/xgboost.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/tuner/preprocessing_tuner.py` & `mljar-supervised-1.0.1/supervised/tuner/preprocessing_tuner.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/tuner/random_parameters.py` & `mljar-supervised-1.0.1/supervised/tuner/random_parameters.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/tuner/time_controller.py` & `mljar-supervised-1.0.1/supervised/tuner/time_controller.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/utils/additional_metrics.py` & `mljar-supervised-1.0.1/supervised/utils/additional_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,14 +217,15 @@
                 f"Predicted as {negative_label}",
                 f"Predicted as {positive_label}",
             ],
             index=[f"Labeled as {negative_label}", f"Labeled as {positive_label}"],
         )
 
         predicted_labels = pd.Series((predictions.ravel() > threshold).astype(int))
+        predicted_labels_01 = predicted_labels.copy()
         predicted_probas = pd.DataFrame(
             {"proba_0": 1 - predictions.ravel(), "proba_1": predictions.ravel()}
         )
 
         if mapping is not None:
             labeled_target = target["target"].map(mapping)
             predicted_labels = predicted_labels.map(mapping)
@@ -241,15 +242,15 @@
                 labeled_target, predicted_labels, predicted_probas
             ),
         }
 
         if sensitive_features is not None:
             metrics["fairness_metrics"] = FairnessMetrics.binary_classification(
                 target,
-                predicted_labels,
+                predicted_labels_01,
                 sensitive_features,
                 fairness_metric,
                 fairness_threshold,
                 privileged_groups,
                 underprivileged_groups,
                 previous_fairness_optimization,
             )
```

### Comparing `mljar-supervised-1.0.0/supervised/utils/additional_plots.py` & `mljar-supervised-1.0.1/supervised/utils/additional_plots.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/utils/automl_plots.py` & `mljar-supervised-1.0.1/supervised/utils/automl_plots.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/utils/common.py` & `mljar-supervised-1.0.1/supervised/utils/common.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/utils/config.py` & `mljar-supervised-1.0.1/supervised/utils/config.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/utils/data_validation.py` & `mljar-supervised-1.0.1/supervised/utils/data_validation.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/utils/importance.py` & `mljar-supervised-1.0.1/supervised/utils/importance.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/utils/leaderboard_plots.py` & `mljar-supervised-1.0.1/supervised/utils/leaderboard_plots.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/utils/learning_curves.py` & `mljar-supervised-1.0.1/supervised/utils/learning_curves.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/utils/metric.py` & `mljar-supervised-1.0.1/supervised/utils/metric.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/utils/shap.py` & `mljar-supervised-1.0.1/supervised/utils/shap.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,17 +241,18 @@
                     X_vald,
                     y_vald,
                     model_file_path,
                     learner_name,
                     class_names,
                 )
         except Exception as e:
-            print(
-                f"Exception while producing SHAP explanations. {str(e)}\nContinuing ..."
-            )
+            pass
+            #print(
+            #    f"Exception while producing SHAP explanations. {str(e)}\nContinuing ..."
+            #)
 
     @staticmethod
     def decisions_regression(
         df_preds,
         shap_values,
         expected_value,
         X_vald,
```

### Comparing `mljar-supervised-1.0.0/supervised/utils/utils.py` & `mljar-supervised-1.0.1/supervised/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/validation/validation_step.py` & `mljar-supervised-1.0.1/supervised/validation/validation_step.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/validation/validator_custom.py` & `mljar-supervised-1.0.1/supervised/validation/validator_custom.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/validation/validator_kfold.py` & `mljar-supervised-1.0.1/supervised/validation/validator_kfold.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-1.0.0/supervised/validation/validator_split.py` & `mljar-supervised-1.0.1/supervised/validation/validator_split.py`

 * *Files identical despite different names*

