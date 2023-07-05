# Comparing `tmp/data_understand-0.0.1.tar.gz` & `tmp/data_understand-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_understand-0.0.1.tar", last modified: Wed Jun 28 22:24:32 2023, max compression
+gzip compressed data, was "data_understand-0.0.2.tar", last modified: Wed Jul  5 23:40:25 2023, max compression
```

## Comparing `data_understand-0.0.1.tar` & `data_understand-0.0.2.tar`

### file list

```diff
@@ -1,69 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:24:31.996607 data_understand-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-28 22:23:39.000000 data_understand-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-06-28 22:24:31.996607 data_understand-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-28 22:23:39.000000 data_understand-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:24:31.992607 data_understand-0.0.1/data_understand/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:24:31.992607 data_understand-0.0.1/data_understand/class_imbalance/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/class_imbalance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/class_imbalance/imbalance.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:24:31.992607 data_understand-0.0.1/data_understand/dataset_characteristics/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/dataset_characteristics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/dataset_characteristics/characteristics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:24:31.992607 data_understand-0.0.1/data_understand/dataset_statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/dataset_statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/dataset_statistics/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:24:31.992607 data_understand-0.0.1/data_understand/feature_correlation/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/feature_correlation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/feature_correlation/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/input_validations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/jupyter_notebook_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:24:31.992607 data_understand-0.0.1/data_understand/load_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/load_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/load_dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/pdf_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:24:31.992607 data_understand-0.0.1/data_understand/target_characteristics/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/target_characteristics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/target_characteristics/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:24:31.992607 data_understand-0.0.1/data_understand/value_distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/value_distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/value_distributions/box_plot_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/value_distributions/cat_frequency_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/value_distributions/distribution_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/value_distributions/histogram_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-28 22:23:39.000000 data_understand-0.0.1/data_understand/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:24:31.992607 data_understand-0.0.1/data_understand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-06-28 22:24:31.000000 data_understand-0.0.1/data_understand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-28 22:24:31.000000 data_understand-0.0.1/data_understand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 22:24:31.000000 data_understand-0.0.1/data_understand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-28 22:24:31.000000 data_understand-0.0.1/data_understand.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-28 22:24:31.000000 data_understand-0.0.1/data_understand.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 22:24:31.000000 data_understand-0.0.1/data_understand.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 22:23:39.000000 data_understand-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 22:24:31.996607 data_understand-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-28 22:23:39.000000 data_understand-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:24:31.992607 data_understand-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:24:31.996607 data_understand-0.0.1/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/e2e/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/e2e/test_e2e_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/e2e/test_e2e_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:24:31.996607 data_understand-0.0.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/unit/test_box_plot_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/unit/test_categorical_frequency_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/unit/test_characteristics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/unit/test_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/unit/test_histogram_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/unit/test_imbalance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/unit/test_input_validations.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/unit/test_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/unit/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/unit/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-28 22:23:39.000000 data_understand-0.0.1/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.699728 data_understand-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-05 23:39:29.000000 data_understand-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-05 23:40:25.699728 data_understand-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-07-05 23:39:29.000000 data_understand-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.695728 data_understand-0.0.2/data_understand/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.695728 data_understand-0.0.2/data_understand/class_imbalance/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/class_imbalance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/class_imbalance/imbalance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.695728 data_understand-0.0.2/data_understand/dataset_characteristics/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/dataset_characteristics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/dataset_characteristics/characteristics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.699728 data_understand-0.0.2/data_understand/dataset_statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/dataset_statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/dataset_statistics/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.699728 data_understand-0.0.2/data_understand/feature_correlation/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/feature_correlation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/feature_correlation/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/input_validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/jupyter_notebook_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.699728 data_understand-0.0.2/data_understand/load_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/load_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/load_dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/pdf_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.699728 data_understand-0.0.2/data_understand/target_characteristics/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/target_characteristics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/target_characteristics/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.699728 data_understand-0.0.2/data_understand/value_distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/value_distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/value_distributions/box_plot_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/value_distributions/cat_frequency_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/value_distributions/distribution_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/value_distributions/histogram_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.695728 data_understand-0.0.2/data_understand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-05 23:40:25.000000 data_understand-0.0.2/data_understand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-05 23:40:25.000000 data_understand-0.0.2/data_understand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 23:40:25.000000 data_understand-0.0.2/data_understand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-05 23:40:25.000000 data_understand-0.0.2/data_understand.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-05 23:40:25.000000 data_understand-0.0.2/data_understand.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 23:40:25.000000 data_understand-0.0.2/data_understand.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-05 23:39:29.000000 data_understand-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 23:40:25.699728 data_understand-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-05 23:39:29.000000 data_understand-0.0.2/setup.py
```

### Comparing `data_understand-0.0.1/LICENSE` & `data_understand-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.1/PKG-INFO` & `data_understand-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: data_understand
-Version: 0.0.1
+Version: 0.0.2
 Summary: Utility package for generating insights for datasets
 Home-page: https://github.com/ggupta2005/data.understand
 Author: Gaurav Gupta
 Author-email: ggupta2005@gmail.com
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # data.understand
+![PyPI data-understand](https://img.shields.io/pypi/v/data-understand)
+[![Downloads](https://static.pepy.tech/badge/data-understand)](https://pepy.tech/project/data-understand)
+[![Run Python E2E Tests](https://github.com/ggupta2005/data.understand/actions/workflows/python-e2e-tests.yml/badge.svg)](https://github.com/ggupta2005/data.understand/actions/workflows/python-e2e-tests.yml)
+[![Run Python Unit Tests](https://github.com/ggupta2005/data.understand/actions/workflows/python-unit-tests.yml/badge.svg)](https://github.com/ggupta2005/data.understand/actions/workflows/python-unit-tests.yml)
 
-As data scientists and machine learning engineers, we are often required to execute various data science tasks like loading up the dataset into a pandas dataframe, inspecting the columns/rows in the dataset, visualizing the distribution of values, finding feature correlations and determining if there are imbalances in the dataset. Often these tasks are repetitive and involves creating multiple jupyter notebooks, making sure we manage these jupyter notebooks separately with different handles to the location of input dataset. How about you have one tool which could take the directory location of your dataset and generate the boring logic for you to execute and learn the same insights about your dataset. All you need to do is to install this tool in your local python environment and then execute the tool from a command line.
+As data scientists and machine learning engineers, we are often required to execute various data science tasks like loading up the dataset into a pandas dataframe, inspecting the columns/rows in the dataset, visualizing the distribution of values, finding feature correlations and determining if there are any sort of imbalances in the dataset. Often these tasks are repetitive and involve creating multiple jupyter notebooks and we have to manage these jupyter notebooks separately with different handles to the location of input dataset. How about you have one tool which could take the directory location of your dataset and generate the boring aforementioned logic for you to execute and learn the same insights about your dataset. All you need to do is to install this tool in your local python environment and then execute the tool from a command line.
 
-You can install the package `data_understand` from pypi using the following command:-
+You can install the package `data-understand` from pypi using the following command:-
 
 ```
 pip install data-understand
 ```
 
 Once you have installed the tool locally, you can then look at the various options of the CLI tool:-
 
@@ -48,15 +51,15 @@
   -j, --generate_jupyter_notebook
                         Generate jupyter notebook file for understanding of data
 ```
 
 In order to generate both PDF report and jupyter notebook you can execute the following CLI command:-
 
 ```
-data_understand -f adult_dataset.csv -t income -p -j
+data_understand --file_name adult_dataset.csv --target_column income --generate_pdf --generate_jupyter_notebook
 ========================================================================================================================
 ========================================================================================================================
 The parsed arguments are:- 
 file_name: adult_dataset.csv
 target_column: income
 generate_pdf: True
 generate_jupyter_notebook: True
@@ -74,8 +77,8 @@
 Time taken: 0.0 min 0.053841799999986506 sec
 ========================================================================================================================
 Successfully generated PDF report and jupyter notebook
 Time taken: 0.0 min 7.485209299999951 sec
 ========================================================================================================================
 ```
 
-This would generate the jupyter notebook and PDF report in the same directory location as your dataset.
+This would generate the jupyter notebook and PDF report in the same directory location as your dataset. You can execute the cells in the jupyter notebook to generate various insights and graphs on the fly or you can read through the PDF report to learn about various aspects of your dataset.
```

### Comparing `data_understand-0.0.1/README.md` & `data_understand-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # data.understand
+![PyPI data-understand](https://img.shields.io/pypi/v/data-understand)
+[![Downloads](https://static.pepy.tech/badge/data-understand)](https://pepy.tech/project/data-understand)
+[![Run Python E2E Tests](https://github.com/ggupta2005/data.understand/actions/workflows/python-e2e-tests.yml/badge.svg)](https://github.com/ggupta2005/data.understand/actions/workflows/python-e2e-tests.yml)
+[![Run Python Unit Tests](https://github.com/ggupta2005/data.understand/actions/workflows/python-unit-tests.yml/badge.svg)](https://github.com/ggupta2005/data.understand/actions/workflows/python-unit-tests.yml)
 
-As data scientists and machine learning engineers, we are often required to execute various data science tasks like loading up the dataset into a pandas dataframe, inspecting the columns/rows in the dataset, visualizing the distribution of values, finding feature correlations and determining if there are imbalances in the dataset. Often these tasks are repetitive and involves creating multiple jupyter notebooks, making sure we manage these jupyter notebooks separately with different handles to the location of input dataset. How about you have one tool which could take the directory location of your dataset and generate the boring logic for you to execute and learn the same insights about your dataset. All you need to do is to install this tool in your local python environment and then execute the tool from a command line.
+As data scientists and machine learning engineers, we are often required to execute various data science tasks like loading up the dataset into a pandas dataframe, inspecting the columns/rows in the dataset, visualizing the distribution of values, finding feature correlations and determining if there are any sort of imbalances in the dataset. Often these tasks are repetitive and involve creating multiple jupyter notebooks and we have to manage these jupyter notebooks separately with different handles to the location of input dataset. How about you have one tool which could take the directory location of your dataset and generate the boring aforementioned logic for you to execute and learn the same insights about your dataset. All you need to do is to install this tool in your local python environment and then execute the tool from a command line.
 
-You can install the package `data_understand` from pypi using the following command:-
+You can install the package `data-understand` from pypi using the following command:-
 
 ```
 pip install data-understand
 ```
 
 Once you have installed the tool locally, you can then look at the various options of the CLI tool:-
 
@@ -28,15 +32,15 @@
   -j, --generate_jupyter_notebook
                         Generate jupyter notebook file for understanding of data
 ```
 
 In order to generate both PDF report and jupyter notebook you can execute the following CLI command:-
 
 ```
-data_understand -f adult_dataset.csv -t income -p -j
+data_understand --file_name adult_dataset.csv --target_column income --generate_pdf --generate_jupyter_notebook
 ========================================================================================================================
 ========================================================================================================================
 The parsed arguments are:- 
 file_name: adult_dataset.csv
 target_column: income
 generate_pdf: True
 generate_jupyter_notebook: True
@@ -54,8 +58,8 @@
 Time taken: 0.0 min 0.053841799999986506 sec
 ========================================================================================================================
 Successfully generated PDF report and jupyter notebook
 Time taken: 0.0 min 7.485209299999951 sec
 ========================================================================================================================
 ```
 
-This would generate the jupyter notebook and PDF report in the same directory location as your dataset.
+This would generate the jupyter notebook and PDF report in the same directory location as your dataset. You can execute the cells in the jupyter notebook to generate various insights and graphs on the fly or you can read through the PDF report to learn about various aspects of your dataset.
```

### Comparing `data_understand-0.0.1/data_understand/class_imbalance/imbalance.py` & `data_understand-0.0.2/data_understand/class_imbalance/imbalance.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.1/data_understand/dataset_characteristics/__init__.py` & `data_understand-0.0.2/data_understand/dataset_characteristics/__init__.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.1/data_understand/dataset_characteristics/characteristics.py` & `data_understand-0.0.2/data_understand/dataset_characteristics/characteristics.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.1/data_understand/dataset_statistics/statistics.py` & `data_understand-0.0.2/data_understand/dataset_statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.1/data_understand/feature_correlation/__init__.py` & `data_understand-0.0.2/data_understand/feature_correlation/__init__.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.1/data_understand/feature_correlation/correlation.py` & `data_understand-0.0.2/data_understand/feature_correlation/correlation.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.1/data_understand/jupyter_notebook_generator.py` & `data_understand-0.0.2/data_understand/jupyter_notebook_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
             source=(
                 "## Find target column imbalances in "
                 "classification scenarios\n" + CLASS_IMBALANCE_MESSAGE
             )
         ),
         v4.new_markdown_cell(source=class_imbalance_markdown),
         v4.new_code_cell(source=class_imbalance_code),
-        v4.new_markdown_cell(source="## References\n" + REFERENCES_MESSAGE)
+        v4.new_markdown_cell(source="## References\n" + REFERENCES_MESSAGE),
     ]
 
     with open(args.file_name + ".ipynb", "w") as f:
         nbformat.write(nb, f)
     print(
         "Successfully generated jupyter notebook for the dataset in "
         + args.file_name
```

### Comparing `data_understand-0.0.1/data_understand/load_dataset/dataset.py` & `data_understand-0.0.2/data_understand/load_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.1/data_understand/main.py` & `data_understand-0.0.2/data_understand/main.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.1/data_understand/messages.py` & `data_understand-0.0.2/data_understand/messages.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.1/data_understand/pdf_generator.py` & `data_understand-0.0.2/data_understand/pdf_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,16 +120,16 @@
         if multi_line:
             self.multi_cell(0, 10, message, markdown=True)
         else:
             self.cell(0, 10, message)
         self.ln()
 
     def _add_table(
-            self, message: str,
-            dataset_as_tuples: Tuple[Tuple[Any]]) -> None:
+        self, message: str, dataset_as_tuples: Tuple[Tuple[Any]]
+    ) -> None:
         """Add a table to the PDF report.
 
         :param message: The message to be added before the table.
         :type message: str
         :param dataset_as_tuples: The dataset to be added as a table.
         :type dataset_as_tuples: Tuple[Tuple[Any]]
         :return: None
@@ -264,24 +264,24 @@
                 self.add_page()
                 page_index = 0
 
             if page_index % 2 == 0:
                 self.image(
                     saved_file_name_list[index],
                     Align.L,
-                    y=40 + (page_index // 2) * 90,
+                    y=60 + (page_index // 2) * 90,
                     w=90,
                     h=90,
                     title=title,
                 )
             else:
                 self.image(
                     saved_file_name_list[index],
                     Align.R,
-                    y=40 + (page_index // 2) * 90,
+                    y=60 + (page_index // 2) * 90,
                     w=90,
                     h=90,
                     title=title,
                 )
             os.remove(saved_file_name_list[index])
 
             page_index += 1
```

### Comparing `data_understand-0.0.1/data_understand/target_characteristics/target.py` & `data_understand-0.0.2/data_understand/target_characteristics/target.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.1/data_understand/utils.py` & `data_understand-0.0.2/data_understand/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     """Measure the time taken by a function to execute via a decorator.
 
     :param compute_func: Function to be decorated
     :type compute_func: function
     :return: Decorated function
     :rtype: function
     """
+
     def compute_wrapper(*args, **kwargs):
         """Print the time taken by a function to execute and return result.
 
         :param args: Arguments to be passed to the function
         :type args: list
         :param kwargs: Keyword arguments to be passed to the function
         :type kwargs: dict
```

### Comparing `data_understand-0.0.1/data_understand/value_distributions/__init__.py` & `data_understand-0.0.2/data_understand/value_distributions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 """Module for computing value distributions."""
 
 from .box_plot_distribution import (
     generate_box_plot_distributions,
     get_jupyter_nb_code_to_generate_box_plot_distributions,
     save_box_plot_distributions)
 from .cat_frequency_distribution import (
```

### Comparing `data_understand-0.0.1/data_understand/value_distributions/box_plot_distribution.py` & `data_understand-0.0.2/data_understand/value_distributions/box_plot_distribution.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.1/data_understand/value_distributions/cat_frequency_distribution.py` & `data_understand-0.0.2/data_understand/value_distributions/cat_frequency_distribution.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.1/data_understand/value_distributions/distribution_utils.py` & `data_understand-0.0.2/data_understand/value_distributions/distribution_utils.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.1/data_understand/value_distributions/histogram_distribution.py` & `data_understand-0.0.2/data_understand/value_distributions/histogram_distribution.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.1/data_understand.egg-info/PKG-INFO` & `data_understand-0.0.2/data_understand.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: data-understand
-Version: 0.0.1
+Version: 0.0.2
 Summary: Utility package for generating insights for datasets
 Home-page: https://github.com/ggupta2005/data.understand
 Author: Gaurav Gupta
 Author-email: ggupta2005@gmail.com
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # data.understand
+![PyPI data-understand](https://img.shields.io/pypi/v/data-understand)
+[![Downloads](https://static.pepy.tech/badge/data-understand)](https://pepy.tech/project/data-understand)
+[![Run Python E2E Tests](https://github.com/ggupta2005/data.understand/actions/workflows/python-e2e-tests.yml/badge.svg)](https://github.com/ggupta2005/data.understand/actions/workflows/python-e2e-tests.yml)
+[![Run Python Unit Tests](https://github.com/ggupta2005/data.understand/actions/workflows/python-unit-tests.yml/badge.svg)](https://github.com/ggupta2005/data.understand/actions/workflows/python-unit-tests.yml)
 
-As data scientists and machine learning engineers, we are often required to execute various data science tasks like loading up the dataset into a pandas dataframe, inspecting the columns/rows in the dataset, visualizing the distribution of values, finding feature correlations and determining if there are imbalances in the dataset. Often these tasks are repetitive and involves creating multiple jupyter notebooks, making sure we manage these jupyter notebooks separately with different handles to the location of input dataset. How about you have one tool which could take the directory location of your dataset and generate the boring logic for you to execute and learn the same insights about your dataset. All you need to do is to install this tool in your local python environment and then execute the tool from a command line.
+As data scientists and machine learning engineers, we are often required to execute various data science tasks like loading up the dataset into a pandas dataframe, inspecting the columns/rows in the dataset, visualizing the distribution of values, finding feature correlations and determining if there are any sort of imbalances in the dataset. Often these tasks are repetitive and involve creating multiple jupyter notebooks and we have to manage these jupyter notebooks separately with different handles to the location of input dataset. How about you have one tool which could take the directory location of your dataset and generate the boring aforementioned logic for you to execute and learn the same insights about your dataset. All you need to do is to install this tool in your local python environment and then execute the tool from a command line.
 
-You can install the package `data_understand` from pypi using the following command:-
+You can install the package `data-understand` from pypi using the following command:-
 
 ```
 pip install data-understand
 ```
 
 Once you have installed the tool locally, you can then look at the various options of the CLI tool:-
 
@@ -48,15 +51,15 @@
   -j, --generate_jupyter_notebook
                         Generate jupyter notebook file for understanding of data
 ```
 
 In order to generate both PDF report and jupyter notebook you can execute the following CLI command:-
 
 ```
-data_understand -f adult_dataset.csv -t income -p -j
+data_understand --file_name adult_dataset.csv --target_column income --generate_pdf --generate_jupyter_notebook
 ========================================================================================================================
 ========================================================================================================================
 The parsed arguments are:- 
 file_name: adult_dataset.csv
 target_column: income
 generate_pdf: True
 generate_jupyter_notebook: True
@@ -74,8 +77,8 @@
 Time taken: 0.0 min 0.053841799999986506 sec
 ========================================================================================================================
 Successfully generated PDF report and jupyter notebook
 Time taken: 0.0 min 7.485209299999951 sec
 ========================================================================================================================
 ```
 
-This would generate the jupyter notebook and PDF report in the same directory location as your dataset.
+This would generate the jupyter notebook and PDF report in the same directory location as your dataset. You can execute the cells in the jupyter notebook to generate various insights and graphs on the fly or you can read through the PDF report to learn about various aspects of your dataset.
```

### Comparing `data_understand-0.0.1/setup.py` & `data_understand-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,19 +20,18 @@
     version=version,  # noqa: F821
     author="Gaurav Gupta",
     author_email="ggupta2005@gmail.com",
     description="Utility package for generating insights for datasets",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ggupta2005/data.understand",
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(exclude=['tests*']),
     python_requires=">=3.6",
     install_requires=install_requires,
     classifiers=[
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `data_understand-0.0.1/tests/unit/test_input_validations.py` & `data_understand-0.0.2/data_understand/input_validations.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,90 +1,69 @@
+"""Module for validating the user input parameters."""
+
 import os
-from argparse import Namespace
+from typing import Any
 
 import pandas as pd
-import pytest
 from raiutils.exceptions import UserErrorException
 
-from data_understand.input_validations import validate_input_parameters
 
+def validate_input_parameters(args: Any) -> None:
+    """Validate the input parameters.
+
+    The function validates the input parameters and raises an exception if
+    the input parameters are not valid. The function validates the following
+    parameters:
+
+    1. The file name is not None.
+    2. The target column name is not None.
+    3. The file name is a CSV file.
+    4. The file name exists.
+    5. Able to read the file as a pandas DataFrame.
+    6. The target column name exists in the dataset.
+
+    param args: The input parameters.
+    type args: Any
+    return: None
+    """
+    # Read all parameters
+    file_name = args.file_name
+    target_column = args.target_column
+
+    if file_name is None:
+        raise UserErrorException(
+            "A valid file name {0} is required. "
+            "Please provide a valid file path.".format(args.file_name)
+        )
 
-@pytest.fixture()
-def args():
-    return Namespace(file_name="test_file.csv", target_column="target")
+    if target_column is None:
+        raise UserErrorException("A valid target column name is required.")
 
+    if not isinstance(file_name, str):
+        raise UserErrorException("The file_name given is not string")
 
-class TestInputValidations:
-    def test_valid_input_parameters(self, args):
-        # Create a test CSV file and add a target column
-        test_df = pd.DataFrame(
-            {"col1": [1, 2, 3], "col2": [4, 5, 6], "target": [0, 1, 0]}
+    if not file_name.endswith(".csv"):
+        raise UserErrorException(
+            "The file {} is not a CSV file. "
+            "Please provide a CSV file.".format(file_name)
         )
-        test_df.to_csv(args.file_name, index=False)
-
-        # Test the function with valid input parameters
-        assert validate_input_parameters(args) is None
 
-        # Remove the test file
-        os.remove(args.file_name)
+    if not os.path.exists(file_name):
+        raise UserErrorException(
+            "The file {} doesn't exists.".format(file_name)
+        )
 
-    def test_missing_file_name(self, args):
-        args.file_name = None
-        with pytest.raises(
-            UserErrorException,
-            match="A valid file name None is required. "
-            "Please provide a valid file path.",
-        ):
-            validate_input_parameters(args)
-
-    def test_missing_target_column(self, args):
-        args.target_column = None
-        with pytest.raises(
-            UserErrorException, match="A valid target column name is required."
-        ):
-            validate_input_parameters(args)
-
-    def test_nonexistent_file_name(self, args):
-        args.file_name = "nonexistent_file.csv"
-        with pytest.raises(
-            UserErrorException,
-            match="The file nonexistent_file.csv doesn't exists.",
-        ):
-            validate_input_parameters(args)
-
-    def test_non_csv_file_name(self, args):
-        args.file_name = "test_file.txt"
-        with pytest.raises(
-            UserErrorException,
-            match="The file test_file.txt is not a CSV file. "
-            "Please provide a CSV file.",
-        ):
-            validate_input_parameters(args)
-
-    def test_invalid_csv_file(self, args):
-        # Create a test file with invalid CSV format
-        with open(args.file_name, "w") as f:
-            f.write("col1,col2,col3\n1,2,3\n4,5\n7,8,9,10")
-
-        with pytest.raises(
-            UserErrorException,
-            match=f"Unable to read CSV file {args.file_name} as "
-            "a pandas DataFrame",
-        ):
-            validate_input_parameters(args)
-
-        # Remove the test file
-        os.remove(args.file_name)
-
-    def test_nonexistent_target_column(self, args):
-        # Create a test CSV file without a target column
-        test_df = pd.DataFrame({"col1": [1, 2, 3], "col2": [4, 5, 6]})
-        test_df.to_csv(args.file_name, index=False)
-
-        with pytest.raises(
-            UserErrorException,
-            match="The target column name target doesn't exist in dataset.",
-        ):
-            validate_input_parameters(args)
+    try:
+        df = pd.read_csv(file_name)
+    except Exception:
+        raise UserErrorException(
+            "Unable to read CSV file {0} as a pandas DataFrame".format(
+                file_name
+            )
+        )
 
-        # Remove the test file
-        os.remove(args.file_name)
+    if target_column not in df.columns.tolist():
+        raise UserErrorException(
+            "The target column name {0} doesn't exist in dataset.".format(
+                target_column
+            )
+        )
```

