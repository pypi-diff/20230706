# Comparing `tmp/reddit_experiments-1.6.0.tar.gz` & `tmp/reddit_experiments-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit_experiments-1.6.0.tar", last modified: Tue Jun 27 21:43:19 2023, max compression
+gzip compressed data, was "reddit_experiments-1.7.0.tar", last modified: Thu Jul  6 18:57:22 2023, max compression
```

## Comparing `reddit_experiments-1.6.0.tar` & `reddit_experiments-1.7.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.843564 reddit_experiments-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.811563 reddit_experiments-1.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.815563 reddit_experiments-1.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/.github/workflows/python-package.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-27 21:43:19.843564 reddit_experiments-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.819563 reddit_experiments-1.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.819563 reddit_experiments-1.6.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    53651 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/docs/images/ddg-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/docs/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.819563 reddit_experiments-1.6.0/docs/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/docs/legacy/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.819563 reddit_experiments-1.6.0/reddit_decider/
--rw-r--r--   0 runner    (1001) docker     (123)    46119 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_decider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_decider/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.819563 reddit_experiments-1.6.0/reddit_experiments/
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.819563 reddit_experiments-1.6.0/reddit_experiments/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/providers/feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/providers/forced_variant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/providers/r2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/providers/simple_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.819563 reddit_experiments-1.6.0/reddit_experiments/targeting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/targeting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/targeting/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/targeting/tree_targeting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.823563 reddit_experiments-1.6.0/reddit_experiments/variant_sets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/variant_sets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/variant_sets/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/variant_sets/multi_variant_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/variant_sets/range_variant_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/variant_sets/rollout_variant_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/variant_sets/single_variant_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.819563 reddit_experiments-1.6.0/reddit_experiments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-27 21:43:19.000000 reddit_experiments-1.6.0/reddit_experiments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-27 21:43:19.000000 reddit_experiments-1.6.0/reddit_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:43:19.000000 reddit_experiments-1.6.0/reddit_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-27 21:43:19.000000 reddit_experiments-1.6.0/reddit_experiments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-27 21:43:19.000000 reddit_experiments-1.6.0/reddit_experiments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:43:19.000000 reddit_experiments-1.6.0/reddit_experiments.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/requirements-transitive.txt
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-27 21:43:19.843564 reddit_experiments-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.823563 reddit_experiments-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    78782 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/decider_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    38015 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/experiment_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.823563 reddit_experiments-1.6.0/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/providers/feature_flag_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/providers/forced_variant_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/providers/r2_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/providers/simple_experiment_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.823563 reddit_experiments-1.6.0/tests/providers/variant_sets/
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/providers/variant_sets/multi_variant_set_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/providers/variant_sets/range_variant_set_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/providers/variant_sets/rollout_variant_set_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/providers/variant_sets/single_variant_set_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.823563 reddit_experiments-1.6.0/tests/range_variant_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.843564 reddit_experiments-1.6.0/tests/range_variant_tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   154451 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/range_variant_tests/data/original_zk_config.json
--rw-r--r--   0 runner    (1001) docker     (123) 14213529 2023-06-27 21:43:04.000000 reddit_experiments-1.6.0/tests/range_variant_tests/data/output.json
--rw-r--r--   0 runner    (1001) docker     (123)   163729 2023-06-27 21:43:04.000000 reddit_experiments-1.6.0/tests/range_variant_tests/data/range_variant_zk_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-27 21:43:04.000000 reddit_experiments-1.6.0/tests/range_variant_tests/range_variant_parity_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.843564 reddit_experiments-1.6.0/tests/targeting/
--rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-06-27 21:43:04.000000 reddit_experiments-1.6.0/tests/targeting/tree_targeting_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.603658 reddit_experiments-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.575658 reddit_experiments-1.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.579658 reddit_experiments-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/.github/workflows/python-package.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-06 18:57:22.603658 reddit_experiments-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.579658 reddit_experiments-1.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.583658 reddit_experiments-1.7.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    53651 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/docs/images/ddg-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/docs/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.583658 reddit_experiments-1.7.0/docs/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/docs/legacy/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.583658 reddit_experiments-1.7.0/reddit_decider/
+-rw-r--r--   0 runner    (1001) docker     (123)    46770 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_decider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_decider/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.583658 reddit_experiments-1.7.0/reddit_experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.583658 reddit_experiments-1.7.0/reddit_experiments/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/providers/feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/providers/forced_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/providers/r2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/providers/simple_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.583658 reddit_experiments-1.7.0/reddit_experiments/targeting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/targeting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/targeting/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/targeting/tree_targeting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.583658 reddit_experiments-1.7.0/reddit_experiments/variant_sets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/variant_sets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/variant_sets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/variant_sets/multi_variant_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/variant_sets/range_variant_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/variant_sets/rollout_variant_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/reddit_experiments/variant_sets/single_variant_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.583658 reddit_experiments-1.7.0/reddit_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-06 18:57:22.000000 reddit_experiments-1.7.0/reddit_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-06 18:57:22.000000 reddit_experiments-1.7.0/reddit_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:57:22.000000 reddit_experiments-1.7.0/reddit_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 18:57:22.000000 reddit_experiments-1.7.0/reddit_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-06 18:57:22.000000 reddit_experiments-1.7.0/reddit_experiments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:57:22.000000 reddit_experiments-1.7.0/reddit_experiments.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/requirements-transitive.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-06 18:57:22.603658 reddit_experiments-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.587658 reddit_experiments-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    81420 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/tests/decider_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39287 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/tests/experiment_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.587658 reddit_experiments-1.7.0/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/tests/providers/feature_flag_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/tests/providers/forced_variant_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/tests/providers/r2_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/tests/providers/simple_experiment_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.587658 reddit_experiments-1.7.0/tests/providers/variant_sets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/tests/providers/variant_sets/multi_variant_set_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/tests/providers/variant_sets/range_variant_set_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/tests/providers/variant_sets/rollout_variant_set_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/tests/providers/variant_sets/single_variant_set_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.587658 reddit_experiments-1.7.0/tests/range_variant_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.603658 reddit_experiments-1.7.0/tests/range_variant_tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   154451 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/tests/range_variant_tests/data/original_zk_config.json
+-rw-r--r--   0 runner    (1001) docker     (123) 14213529 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/tests/range_variant_tests/data/output.json
+-rw-r--r--   0 runner    (1001) docker     (123)   163729 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/tests/range_variant_tests/data/range_variant_zk_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/tests/range_variant_tests/range_variant_parity_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:57:22.603658 reddit_experiments-1.7.0/tests/targeting/
+-rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-07-06 18:57:07.000000 reddit_experiments-1.7.0/tests/targeting/tree_targeting_tests.py
```

### Comparing `reddit_experiments-1.6.0/.github/workflows/python-package.yaml` & `reddit_experiments-1.7.0/.github/workflows/python-package.yaml`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/.github/workflows/python-publish.yaml` & `reddit_experiments-1.7.0/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/.readthedocs.yaml` & `reddit_experiments-1.7.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/LICENSE` & `reddit_experiments-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/Makefile` & `reddit_experiments-1.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/PKG-INFO` & `reddit_experiments-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit_experiments
-Version: 1.6.0
+Version: 1.7.0
 Summary: reddit's python experiments framework
 Home-page: https://github.com/reddit/experiments.py
 Author: reddit
 License: BSD
 Project-URL: Documentation, https://reddit-experiments.readthedocs.io/
 Description: # experiments.py
```

### Comparing `reddit_experiments-1.6.0/README.md` & `reddit_experiments-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/docs/conf.py` & `reddit_experiments-1.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/docs/images/ddg-logo.png` & `reddit_experiments-1.7.0/docs/images/ddg-logo.png`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/docs/images/favicon.png` & `reddit_experiments-1.7.0/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/docs/index.rst` & `reddit_experiments-1.7.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,17 @@
    ...
 
    # optional: a path to the file where experiment configuration is written
    # (default: /var/local/experiments.json)
    experiments.path = /var/local/foo.json
 
    # optional: how long to wait for the experiments file to exist before failing
-   # (default: do not wait. fail immediately if not available)
+   # default:
+   #    >= v1.7.0 wait 30 seconds
+   #    <  v1.7.0 do not wait, fail immediately if not available
    experiments.timeout = 60 seconds
 
    # optional: the base amount of time for exponential backoff while waiting
    # for the file to be available.
    # (default: no backoff time between tries)
    experiments.backoff = 1 second
 
@@ -58,15 +60,15 @@
 -----------------------------------------------------------
 
 Upgrade or integrate reddit-experiments package:
 
 .. code-block:: python
 
     # import latest reddit-experiments package in service requirements.txt
-    reddit-experiments>=1.4.0
+    reddit-experiments>=1.7.0
 
 Initialize :code:`decider` instance on Baseplate context
 --------------------------------------------------------
 
 In your service's initialization process, add a :code:`decider` instance to baseplate's context:
 
 .. code-block:: python
```

### Comparing `reddit_experiments-1.6.0/docs/legacy/index.rst` & `reddit_experiments-1.7.0/docs/legacy/index.rst`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/reddit_decider/__init__.py` & `reddit_experiments-1.7.0/reddit_decider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 
 from copy import deepcopy
 from dataclasses import dataclass
+from datetime import timedelta
 from enum import Enum
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import IO
 from typing import List
 from typing import Optional
@@ -685,64 +686,84 @@
         :param feature_name: Name of the dynamic config you want a value for.
 
         :param default: what is returned if dynamic config is not active
             (:code:`False` unless overriden).
 
         :return: the boolean value of the dyanimc config if it is active/exists, :code:`default` parameter otherwise.
         """
+        if self._internal is None:
+            logger.error("rs_decider is None--did not initialize.")
+            return default
+
         return self._get_dynamic_config_value(feature_name, default, bool, self._internal.get_bool)
 
     def get_int(self, feature_name: str, default: int = 0) -> int:
         """Fetch a Dynamic Configuration of int type.
 
         :param feature_name: Name of the dynamic config you want a value for.
 
         :param default: what is returned if dynamic config is not active
             (:code:`0` unless overriden).
 
         :return: the int value of the dyanimc config if it is active/exists, :code:`default` parameter otherwise.
         """
+        if self._internal is None:
+            logger.error("rs_decider is None--did not initialize.")
+            return default
+
         return self._get_dynamic_config_value(feature_name, default, int, self._internal.get_int)
 
     def get_float(self, feature_name: str, default: float = 0.0) -> float:
         """Fetch a Dynamic Configuration of float type.
 
         :param feature_name: Name of the dynamic config you want a value for.
 
         :param default: what is returned if dynamic config is not active
             (:code:`0.0` unless overriden).
 
         :return: the float value of the dyanimc config if it is active/exists, :code:`default` parameter otherwise.
         """
+        if self._internal is None:
+            logger.error("rs_decider is None--did not initialize.")
+            return default
+
         return self._get_dynamic_config_value(
             feature_name, default, float, self._internal.get_float
         )
 
     def get_string(self, feature_name: str, default: str = "") -> str:
         """Fetch a Dynamic Configuration of string type.
 
         :param feature_name: Name of the dynamic config you want a value for.
 
         :param default: what is returned if dynamic config is not active
             (:code:`""` unless overriden).
 
         :return: the string value of the dyanimc config if it is active/exists, :code:`default` parameter otherwise.
         """
+        if self._internal is None:
+            logger.error("rs_decider is None--did not initialize.")
+            return default
+
         return self._get_dynamic_config_value(feature_name, default, str, self._internal.get_string)
 
     def get_map(self, feature_name: str, default: Optional[dict] = None) -> Optional[dict]:
         """Fetch a Dynamic Configuration of map type.
 
         :param feature_name: Name of the dynamic config you want a value for.
 
         :param default: what is returned if dynamic config is not active
             (:code:`None` unless overriden).
 
         :return: the map value of the dyanimc config if it is active/exists, :code:`default` parameter otherwise.
         """
+        if self._internal is None:
+            logger.error("rs_decider is None--did not initialize.")
+            return default
+
         return self._get_dynamic_config_value(feature_name, default, dict, self._internal.get_map)
 
     def get_all_dynamic_configs(self) -> List[Dict[str, Any]]:
         """Return a list of dynamic configuration dicts in this format:
 
             .. code-block:: json
 
@@ -826,18 +847,14 @@
     def _get_dynamic_config_value(
         self,
         feature_name: str,
         default: Any,
         dc_type: Type[T],
         get_fn: Callable[..., Type[T]],
     ) -> T:
-        if self._internal is None:
-            logger.error("rs_decider is None--did not initialize.")
-            return default
-
         ctx = self._decider_context.to_dict()
 
         try:
             value = get_fn(feature_name=feature_name, context=ctx)
         except FeatureNotFoundException:
             return default
         except ValueTypeMismatchException as exc:
@@ -1189,17 +1206,18 @@
     ``experiments.path``, etc.
 
     Supported config keys:
 
         ``path`` (optional)
             The path to the experiment configuration file generated by the
             experiment configuration fetcher daemon.
+            Defaults to :code:`"/var/local/experiments.json"`.
         ``timeout`` (optional)
-            The time that we should wait for the file specified by ``path`` to
-            exist.  Defaults to `None` which is not blocking.
+            The time that we should wait for the file specified by ``path`` to exist.
+            Defaults to blocking for :code:`30` seconds.
         ``backoff`` (optional)
             The base amount of time for exponential backoff when trying to find the
             experiments config file. Defaults to no backoff between tries.
 
     :param app_config: The application configuration which should have
         settings for the decider client.
     :param event_logger: The EventLogger to be used to log bucketing events.
@@ -1211,15 +1229,15 @@
     config_prefix = prefix[:-1]
 
     cfg = config.parse_config(
         app_config,
         {
             config_prefix: {
                 "path": config.Optional(config.String, default="/var/local/experiments.json"),
-                "timeout": config.Optional(config.Timespan),
+                "timeout": config.Optional(config.Timespan, default=timedelta(seconds=30)),
                 "backoff": config.Optional(config.Timespan),
             }
         },
     )
     options = getattr(cfg, config_prefix)
 
     # pylint: disable=maybe-no-member
```

### Comparing `reddit_experiments-1.6.0/reddit_experiments/__init__.py` & `reddit_experiments-1.7.0/reddit_experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/reddit_experiments/providers/__init__.py` & `reddit_experiments-1.7.0/reddit_experiments/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/reddit_experiments/providers/base.py` & `reddit_experiments-1.7.0/reddit_experiments/providers/base.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/reddit_experiments/providers/feature_flag.py` & `reddit_experiments-1.7.0/reddit_experiments/providers/feature_flag.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/reddit_experiments/providers/forced_variant.py` & `reddit_experiments-1.7.0/reddit_experiments/providers/forced_variant.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/reddit_experiments/providers/r2.py` & `reddit_experiments-1.7.0/reddit_experiments/providers/r2.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/reddit_experiments/providers/simple_experiment.py` & `reddit_experiments-1.7.0/reddit_experiments/providers/simple_experiment.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/reddit_experiments/targeting/tree_targeting.py` & `reddit_experiments-1.7.0/reddit_experiments/targeting/tree_targeting.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/reddit_experiments/variant_sets/base.py` & `reddit_experiments-1.7.0/reddit_experiments/variant_sets/base.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/reddit_experiments/variant_sets/multi_variant_set.py` & `reddit_experiments-1.7.0/reddit_experiments/variant_sets/multi_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/reddit_experiments/variant_sets/range_variant_set.py` & `reddit_experiments-1.7.0/reddit_experiments/variant_sets/range_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/reddit_experiments/variant_sets/rollout_variant_set.py` & `reddit_experiments-1.7.0/reddit_experiments/variant_sets/rollout_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/reddit_experiments/variant_sets/single_variant_set.py` & `reddit_experiments-1.7.0/reddit_experiments/variant_sets/single_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/reddit_experiments.egg-info/PKG-INFO` & `reddit_experiments-1.7.0/reddit_experiments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-experiments
-Version: 1.6.0
+Version: 1.7.0
 Summary: reddit's python experiments framework
 Home-page: https://github.com/reddit/experiments.py
 Author: reddit
 License: BSD
 Project-URL: Documentation, https://reddit-experiments.readthedocs.io/
 Description: # experiments.py
```

### Comparing `reddit_experiments-1.6.0/reddit_experiments.egg-info/SOURCES.txt` & `reddit_experiments-1.7.0/reddit_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/requirements-transitive.txt` & `reddit_experiments-1.7.0/requirements-transitive.txt`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/setup.cfg` & `reddit_experiments-1.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/setup.py` & `reddit_experiments-1.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     use_scm_version=True,
     packages=find_packages(),
     python_requires=">=3.7",
     setup_requires=["setuptools_scm"],
     install_requires=[
         "baseplate>=2.0.0a1,<3.0",
         "reddit-edgecontext>=1.0.0a3,<2.0",
-        "reddit-decider~=1.3.1",
+        "reddit-decider~=1.4.1",
         "typing_extensions>=3.10.0.0,<5.0",
     ],
     package_data={"reddit_experiments": ["py.typed"], "reddit_decider": ["py.typed"]},
     zip_safe=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: BSD License",
```

### Comparing `reddit_experiments-1.6.0/tests/decider_tests.py` & `reddit_experiments-1.7.0/tests/decider_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,22 +84,22 @@
 class DeciderClientFromConfigTests(unittest.TestCase):
     def setUp(self):
         super().setUp()
         self.event_logger = mock.Mock(spec=DebugLogger)
         self.mock_span = mock.MagicMock(spec=ServerSpan)
         self.mock_span.context = None
 
-    def test_make_clients(self, file_watcher_mock):
+    def test_make_client_without_timeout_set(self, file_watcher_mock):
         with create_temp_config_file({}) as f:
             decider_ctx_factory = decider_client_from_config(
                 {"experiments.path": f.name}, self.event_logger
             )
         self.assertIsInstance(decider_ctx_factory, DeciderContextFactory)
         file_watcher_mock.assert_called_once_with(
-            path=f.name, parser=init_decider_parser, timeout=None, backoff=None
+            path=f.name, parser=init_decider_parser, timeout=30.0, backoff=None
         )
 
     def test_timeout(self, file_watcher_mock):
         with create_temp_config_file({}) as f:
             decider_ctx_factory = decider_client_from_config(
                 {"experiments.path": f.name, "experiments.timeout": "2 seconds"},
                 self.event_logger,
@@ -493,15 +493,15 @@
                 )
                 variant = decider.get_variant("test")
 
                 self.assertEqual(variant, None)
                 self.assertEqual(self.event_logger.log.call_count, 0)
 
                 assert any(
-                    "Partially loaded Decider: 1 features failed to load: {'test': 'invalid type: string \"1\", expected u32'}"
+                    "Partially loaded Decider: 1 features failed to load: {'test': 'Manifest parsing error: invalid type: string \"1\", expected u32'}"
                     in x.getMessage()
                     for x in captured.records
                 )
 
     def test_none_returned_on_get_variant_call_with_no_experiment_data(self):
         config = {
             "test": {
@@ -1477,14 +1477,67 @@
             event_fields = self.event_logger.log.call_args[1]
 
             # `variant == None` for child but event will fire with `variant == "control_1"` for analysis
             self.assert_exposure_event_fields(
                 experiment_name="hg", variant="control_1", event_fields=event_fields
             )
 
+    def test_get_variant_for_okta_groups(self):
+        identifier = "t2_test"
+        bucket_val = "user_id"
+        group_overrides = {"variant_2": {"EQ": {"field": "user_id", "values": ["$some_group_id"]}}}
+
+        self.exp_base_config["exp_1"]["experiment"].update({"overrides": [group_overrides]})
+        # reset variant for override to make sure it's not organically bucketed into it
+        self.exp_base_config["exp_1"]["experiment"].update(
+            {
+                "variants": [
+                    {"range_start": 0.0, "range_end": 0.0, "name": "variant_2"},
+                ]
+            }
+        )
+
+        og_cfg = {
+            "$override_groups": {
+                "id": 1337,
+                "value": {
+                    "$some_group_id": {
+                        "name": "some_group_id",
+                        "values": [identifier],
+                        "field": "user_id",
+                    }
+                },
+                "type": "dynamic_config",
+                "version": "1",
+                "enabled": False,
+                "owner": "test",
+                "name": "$override_group",
+                "value_type": "Map",
+                "experiment": {"experiment_version": 1},
+            },
+        }
+        self.exp_base_config.update(og_cfg)
+
+        with create_temp_config_file(self.exp_base_config) as f:
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
+
+            self.assertEqual(self.event_logger.log.call_count, 0)
+            variant = decider.get_variant_for_identifier_without_expose(
+                experiment_name="exp_1", identifier=identifier, identifier_type=bucket_val
+            )
+            self.assertEqual(variant, "variant_2")
+
+            self.dc._user_id = identifier
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
+            variant = decider.get_variant_without_expose(experiment_name="exp_1")
+            self.assertEqual(variant, "variant_2")
+
+            # no exposures should be triggered
+            self.assertEqual(self.event_logger.log.call_count, 0)
+
 
 class TestDeciderGetDynamicConfig(unittest.TestCase):
     def setUp(self):
         super().setUp()
         self.event_logger = mock.Mock(spec=DebugLogger)
         self.mock_span = mock.MagicMock(spec=ServerSpan)
         self.mock_span.context = None
@@ -1570,14 +1623,26 @@
             decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             res = decider.get_map("dc_1")
             self.assertEqual(res, dict({"key": "value", "another_key": "another_value"}))
             res = decider.get_string("dc_1")
             self.assertEqual(res, "")
 
+    def test_get_map_disabled(self):
+        self.dc_base_config["dc_1"].update(
+            {"value_type": "Map", "value": {"key": "value", "another_key": "another_value"}}
+        )
+        self.dc_base_config["dc_1"].update({"enabled": False})
+
+        with create_temp_config_file(self.dc_base_config) as f:
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
+
+            res = decider.get_map("dc_1")
+            self.assertEqual(res, None)
+
     def test_get_all_values(self):
         base_cfg = self.dc_base_config["dc_1"].copy()
 
         bool_val = True
         cfg_bool = {"dc_bool": base_cfg.copy()}
         cfg_bool["dc_bool"].update({"name": "dc_bool", "value": bool_val, "value_type": "Boolean"})
```

### Comparing `reddit_experiments-1.6.0/tests/experiment_tests.py` & `reddit_experiments-1.7.0/tests/experiment_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -670,14 +670,50 @@
             global_cache={},
             event_logger=self.event_logger,
         )
         self.assertEqual(self.event_logger.log.call_count, 0)
         variant = experiments.variant("test", user=self.user)
         self.assertEqual(variant, None)
 
+    def test_new_identifier_compatibility(self):
+        self.mock_filewatcher.get_data.return_value = {
+            "test": {
+                "id": 1,
+                "name": "test",
+                "enabled": True,
+                "owner": "test_owner",
+                "version": "1",
+                "emit_event": True,
+                "type": "range_variant",
+                "start_ts": time.time() - THIRTY_DAYS,
+                "stop_ts": time.time() + THIRTY_DAYS,
+                "experiment": {
+                    "variants": [
+                        {"name": "active", "size": 1, "range_end": 1.0, "range_start": 0},
+                    ],
+                    "experiment_version": 5,
+                    "shuffle_version": 91,
+                    "bucket_val": "ad_account_id",
+                    "log_bucketing": False,
+                },
+            }
+        }
+
+        experiments = Experiments(
+            config_watcher=self.mock_filewatcher,
+            server_span=self.mock_span,
+            context_name="test",
+            event_logger=self.event_logger,
+        )
+
+        self.assertEqual(self.event_logger.log.call_count, 0)
+        variant = experiments.variant("test", ad_account_id="a2_xxx")
+
+        self.assertEqual(variant, "active")
+
 
 @mock.patch("reddit_experiments.FileWatcher")
 class ExperimentsClientFromConfigTests(unittest.TestCase):
     def test_make_clients(self, file_watcher_mock):
         event_logger = mock.Mock(spec=DebugLogger)
         experiments = experiments_client_from_config(
             {"experiments.path": "/tmp/test"}, event_logger
```

### Comparing `reddit_experiments-1.6.0/tests/providers/feature_flag_tests.py` & `reddit_experiments-1.7.0/tests/providers/feature_flag_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/tests/providers/forced_variant_tests.py` & `reddit_experiments-1.7.0/tests/providers/forced_variant_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/tests/providers/r2_tests.py` & `reddit_experiments-1.7.0/tests/providers/r2_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/tests/providers/simple_experiment_tests.py` & `reddit_experiments-1.7.0/tests/providers/simple_experiment_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/tests/providers/variant_sets/multi_variant_set_tests.py` & `reddit_experiments-1.7.0/tests/providers/variant_sets/multi_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/tests/providers/variant_sets/range_variant_set_tests.py` & `reddit_experiments-1.7.0/tests/providers/variant_sets/range_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/tests/providers/variant_sets/rollout_variant_set_tests.py` & `reddit_experiments-1.7.0/tests/providers/variant_sets/rollout_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/tests/providers/variant_sets/single_variant_set_tests.py` & `reddit_experiments-1.7.0/tests/providers/variant_sets/single_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/tests/range_variant_tests/data/original_zk_config.json` & `reddit_experiments-1.7.0/tests/range_variant_tests/data/original_zk_config.json`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/tests/range_variant_tests/data/output.json` & `reddit_experiments-1.7.0/tests/range_variant_tests/data/output.json`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/tests/range_variant_tests/data/range_variant_zk_config.json` & `reddit_experiments-1.7.0/tests/range_variant_tests/data/range_variant_zk_config.json`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/tests/range_variant_tests/range_variant_parity_tests.py` & `reddit_experiments-1.7.0/tests/range_variant_tests/range_variant_parity_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.6.0/tests/targeting/tree_targeting_tests.py` & `reddit_experiments-1.7.0/tests/targeting/tree_targeting_tests.py`

 * *Files identical despite different names*

