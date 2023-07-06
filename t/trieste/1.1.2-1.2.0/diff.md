# Comparing `tmp/trieste-1.1.2.tar.gz` & `tmp/trieste-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trieste-1.1.2.tar", last modified: Thu Mar 23 14:11:59 2023, max compression
+gzip compressed data, was "trieste-1.2.0.tar", last modified: Wed Jul  5 11:14:21 2023, max compression
```

## Comparing `trieste-1.1.2.tar` & `trieste-1.2.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-23 14:11:59.771609 trieste-1.1.2/
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    11358 2022-07-01 06:54:15.000000 trieste-1.1.2/LICENSE
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     8361 2023-03-23 14:11:59.771609 trieste-1.1.2/PKG-INFO
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     7827 2023-03-10 09:13:45.000000 trieste-1.1.2/README.md
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     3043 2023-03-06 14:10:58.000000 trieste-1.1.2/pyproject.toml
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)       38 2023-03-23 14:11:59.771609 trieste-1.1.2/setup.cfg
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1793 2023-03-06 14:10:58.000000 trieste-1.1.2/setup.py
-drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-23 14:11:59.763609 trieste-1.1.2/trieste/
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)        6 2023-03-23 14:11:32.000000 trieste-1.1.2/trieste/VERSION
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1397 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/__init__.py
-drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-23 14:11:59.763609 trieste-1.1.2/trieste/acquisition/
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     3991 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/acquisition/__init__.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     5490 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/acquisition/combination.py
-drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-23 14:11:59.763609 trieste-1.1.2/trieste/acquisition/function/
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     2311 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/acquisition/function/__init__.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    20764 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/acquisition/function/active_learning.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    10279 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/acquisition/function/continuous_thompson_sampling.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    36326 2023-03-17 07:55:25.000000 trieste-1.1.2/trieste/acquisition/function/entropy.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    77739 2023-03-15 11:20:16.000000 trieste-1.1.2/trieste/acquisition/function/function.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    34562 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/acquisition/function/greedy_batch.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    33929 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/acquisition/function/multi_objective.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     7456 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/acquisition/function/utils.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    16951 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/acquisition/interface.py
-drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-23 14:11:59.763609 trieste-1.1.2/trieste/acquisition/multi_objective/
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)      890 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/acquisition/multi_objective/__init__.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     2789 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/acquisition/multi_objective/dominance.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    11521 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/acquisition/multi_objective/pareto.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    16741 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/acquisition/multi_objective/partition.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    30060 2023-03-14 13:21:58.000000 trieste-1.1.2/trieste/acquisition/optimizer.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    54551 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/acquisition/rule.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    11423 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/acquisition/sampler.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     4488 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/acquisition/utils.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    17113 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/ask_tell_optimization.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    42360 2023-03-17 07:55:25.000000 trieste-1.1.2/trieste/bayesian_optimizer.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     8597 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/data.py
-drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-23 14:11:59.763609 trieste-1.1.2/trieste/experimental/
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/experimental/__init__.py
-drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-23 14:11:59.767609 trieste-1.1.2/trieste/experimental/plotting/
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1444 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/experimental/plotting/__init__.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     6314 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/experimental/plotting/inequality_constraints.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    17735 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/experimental/plotting/plotting.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     8455 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/experimental/plotting/plotting_plotly.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     7102 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/logging.py
-drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-23 14:11:59.767609 trieste-1.1.2/trieste/models/
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1220 2023-03-17 07:55:25.000000 trieste-1.1.2/trieste/models/__init__.py
-drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-23 14:11:59.767609 trieste-1.1.2/trieste/models/gpflow/
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1858 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/gpflow/__init__.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    27128 2023-03-10 09:13:45.000000 trieste-1.1.2/trieste/models/gpflow/builders.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    18538 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/gpflow/inducing_point_selectors.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     7653 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/gpflow/interface.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    90589 2023-03-17 07:55:25.000000 trieste-1.1.2/trieste/models/gpflow/models.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     3374 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/gpflow/optimizer.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    38223 2023-03-23 10:52:43.000000 trieste-1.1.2/trieste/models/gpflow/sampler.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    14696 2023-03-17 07:55:25.000000 trieste-1.1.2/trieste/models/gpflow/utils.py
-drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-23 14:11:59.767609 trieste-1.1.2/trieste/models/gpflux/
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1158 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/gpflux/__init__.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     6191 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/gpflux/builders.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     3501 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/gpflux/interface.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    17909 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/gpflux/models.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    20007 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/gpflux/sampler.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    29397 2023-03-17 07:55:25.000000 trieste-1.1.2/trieste/models/interfaces.py
-drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-23 14:11:59.767609 trieste-1.1.2/trieste/models/keras/
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1334 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/keras/__init__.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    14523 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/keras/architectures.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     3471 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/keras/builders.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     4335 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/keras/interface.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    24710 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/keras/models.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     9679 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/keras/sampler.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     5241 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/keras/utils.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     7229 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/optimizer.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     4304 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/models/utils.py
-drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-23 14:11:59.767609 trieste-1.1.2/trieste/objectives/
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1319 2023-03-17 07:55:25.000000 trieste-1.1.2/trieste/objectives/__init__.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     8968 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/objectives/multi_objectives.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     3507 2023-03-17 07:55:25.000000 trieste-1.1.2/trieste/objectives/multifidelity_objectives.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    21437 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/objectives/single_objectives.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     2051 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/objectives/utils.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     3024 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/observer.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/py.typed
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    45403 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/space.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1272 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/types.py
-drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-23 14:11:59.771609 trieste-1.1.2/trieste/utils/
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)      833 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/utils/__init__.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     7433 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/utils/misc.py
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)      787 2023-03-06 14:10:58.000000 trieste-1.1.2/trieste/version.py
-drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-23 14:11:59.763609 trieste-1.1.2/trieste.egg-info/
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     8361 2023-03-23 14:11:59.000000 trieste-1.1.2/trieste.egg-info/PKG-INFO
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     2440 2023-03-23 14:11:59.000000 trieste-1.1.2/trieste.egg-info/SOURCES.txt
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)        1 2023-03-23 14:11:59.000000 trieste-1.1.2/trieste.egg-info/dependency_links.txt
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)      163 2023-03-23 14:11:59.000000 trieste-1.1.2/trieste.egg-info/requires.txt
--rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)        8 2023-03-23 14:11:59.000000 trieste-1.1.2/trieste.egg-info/top_level.txt
+drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-07-05 11:14:21.873660 trieste-1.2.0/
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    11358 2022-07-01 06:54:15.000000 trieste-1.2.0/LICENSE
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     8361 2023-07-05 11:14:21.873660 trieste-1.2.0/PKG-INFO
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     7827 2023-03-10 09:13:45.000000 trieste-1.2.0/README.md
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     3043 2023-06-29 10:19:49.000000 trieste-1.2.0/pyproject.toml
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)       38 2023-07-05 11:14:21.873660 trieste-1.2.0/setup.cfg
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1939 2023-07-04 13:39:17.000000 trieste-1.2.0/setup.py
+drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-07-05 11:14:21.869660 trieste-1.2.0/trieste/
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)        6 2023-07-05 11:13:33.000000 trieste-1.2.0/trieste/VERSION
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1351 2023-06-22 08:34:50.000000 trieste-1.2.0/trieste/__init__.py
+drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-07-05 11:14:21.869660 trieste-1.2.0/trieste/acquisition/
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     3991 2023-06-29 09:18:50.000000 trieste-1.2.0/trieste/acquisition/__init__.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     6417 2023-07-03 16:50:15.000000 trieste-1.2.0/trieste/acquisition/combination.py
+drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-07-05 11:14:21.869660 trieste-1.2.0/trieste/acquisition/function/
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     2311 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/acquisition/function/__init__.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    20764 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/acquisition/function/active_learning.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    10279 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/acquisition/function/continuous_thompson_sampling.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    36326 2023-03-17 07:55:25.000000 trieste-1.2.0/trieste/acquisition/function/entropy.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    77739 2023-07-04 10:50:47.000000 trieste-1.2.0/trieste/acquisition/function/function.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    34562 2023-05-17 06:43:21.000000 trieste-1.2.0/trieste/acquisition/function/greedy_batch.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    33929 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/acquisition/function/multi_objective.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     7456 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/acquisition/function/utils.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    16951 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/acquisition/interface.py
+drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-07-05 11:14:21.869660 trieste-1.2.0/trieste/acquisition/multi_objective/
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)      890 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/acquisition/multi_objective/__init__.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     2789 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/acquisition/multi_objective/dominance.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    11521 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/acquisition/multi_objective/pareto.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    16741 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/acquisition/multi_objective/partition.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    30061 2023-06-15 07:56:02.000000 trieste-1.2.0/trieste/acquisition/optimizer.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    64805 2023-07-03 06:38:32.000000 trieste-1.2.0/trieste/acquisition/rule.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    11521 2023-07-04 13:39:17.000000 trieste-1.2.0/trieste/acquisition/sampler.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     5297 2023-07-03 06:38:32.000000 trieste-1.2.0/trieste/acquisition/utils.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    17459 2023-07-04 14:45:52.000000 trieste-1.2.0/trieste/ask_tell_optimization.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    46324 2023-07-05 11:13:33.000000 trieste-1.2.0/trieste/bayesian_optimizer.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     8597 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/data.py
+drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-07-05 11:14:21.869660 trieste-1.2.0/trieste/experimental/
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/experimental/__init__.py
+drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-07-05 11:14:21.869660 trieste-1.2.0/trieste/experimental/plotting/
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1444 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/experimental/plotting/__init__.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     6314 2023-06-15 07:56:02.000000 trieste-1.2.0/trieste/experimental/plotting/inequality_constraints.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    17758 2023-07-04 13:39:17.000000 trieste-1.2.0/trieste/experimental/plotting/plotting.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     8489 2023-06-15 07:56:02.000000 trieste-1.2.0/trieste/experimental/plotting/plotting_plotly.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     7102 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/logging.py
+drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-07-05 11:14:21.869660 trieste-1.2.0/trieste/models/
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1220 2023-03-17 07:55:25.000000 trieste-1.2.0/trieste/models/__init__.py
+drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-07-05 11:14:21.873660 trieste-1.2.0/trieste/models/gpflow/
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1858 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/models/gpflow/__init__.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    27128 2023-03-10 09:13:45.000000 trieste-1.2.0/trieste/models/gpflow/builders.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    18538 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/models/gpflow/inducing_point_selectors.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     7905 2023-06-29 13:50:47.000000 trieste-1.2.0/trieste/models/gpflow/interface.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    90637 2023-06-26 09:48:21.000000 trieste-1.2.0/trieste/models/gpflow/models.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     3374 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/models/gpflow/optimizer.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    40450 2023-06-29 13:50:47.000000 trieste-1.2.0/trieste/models/gpflow/sampler.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    14696 2023-03-27 12:21:08.000000 trieste-1.2.0/trieste/models/gpflow/utils.py
+drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-07-05 11:14:21.873660 trieste-1.2.0/trieste/models/gpflux/
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1158 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/models/gpflux/__init__.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     6191 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/models/gpflux/builders.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     3501 2023-06-22 11:33:09.000000 trieste-1.2.0/trieste/models/gpflux/interface.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    18255 2023-06-22 08:34:50.000000 trieste-1.2.0/trieste/models/gpflux/models.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    20609 2023-06-15 07:56:02.000000 trieste-1.2.0/trieste/models/gpflux/sampler.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    30175 2023-07-03 06:38:32.000000 trieste-1.2.0/trieste/models/interfaces.py
+drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-07-05 11:14:21.873660 trieste-1.2.0/trieste/models/keras/
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1334 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/models/keras/__init__.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    14523 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/models/keras/architectures.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     3471 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/models/keras/builders.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     4335 2023-06-22 10:39:19.000000 trieste-1.2.0/trieste/models/keras/interface.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    25440 2023-06-22 08:34:50.000000 trieste-1.2.0/trieste/models/keras/models.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     9679 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/models/keras/sampler.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     5241 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/models/keras/utils.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     9230 2023-07-04 13:39:17.000000 trieste-1.2.0/trieste/models/optimizer.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     4316 2023-06-15 07:56:02.000000 trieste-1.2.0/trieste/models/utils.py
+drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-07-05 11:14:21.873660 trieste-1.2.0/trieste/objectives/
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1330 2023-06-22 08:34:50.000000 trieste-1.2.0/trieste/objectives/__init__.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     8968 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/objectives/multi_objectives.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     3507 2023-03-17 07:55:25.000000 trieste-1.2.0/trieste/objectives/multifidelity_objectives.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    23895 2023-06-22 08:34:50.000000 trieste-1.2.0/trieste/objectives/single_objectives.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     2051 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/objectives/utils.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     3024 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/observer.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)        0 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/py.typed
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    45403 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/space.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     1272 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/types.py
+drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-07-05 11:14:21.873660 trieste-1.2.0/trieste/utils/
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)      833 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/utils/__init__.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)    11630 2023-07-03 06:38:32.000000 trieste-1.2.0/trieste/utils/misc.py
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)      787 2023-03-06 14:10:58.000000 trieste-1.2.0/trieste/version.py
+drwxr-xr-x   0 uri.granta (1785601490) domain users (1785600513)        0 2023-07-05 11:14:21.869660 trieste-1.2.0/trieste.egg-info/
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     8361 2023-07-05 11:14:21.000000 trieste-1.2.0/trieste.egg-info/PKG-INFO
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)     2440 2023-07-05 11:14:21.000000 trieste-1.2.0/trieste.egg-info/SOURCES.txt
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)        1 2023-07-05 11:14:21.000000 trieste-1.2.0/trieste.egg-info/dependency_links.txt
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)      312 2023-07-05 11:14:21.000000 trieste-1.2.0/trieste.egg-info/requires.txt
+-rw-r--r--   0 uri.granta (1785601490) domain users (1785600513)        8 2023-07-05 11:14:21.000000 trieste-1.2.0/trieste.egg-info/top_level.txt
```

### Comparing `trieste-1.1.2/LICENSE` & `trieste-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/PKG-INFO` & `trieste-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trieste
-Version: 1.1.2
+Version: 1.2.0
 Summary: A Bayesian optimization research toolbox built on TensorFlow
 Home-page: https://github.com/secondmind-labs/trieste
 Author: The Trieste contributors
 Author-email: labs@secondmind.ai
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `trieste-1.1.2/README.md` & `trieste-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/pyproject.toml` & `trieste-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/setup.py` & `trieste-1.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,18 +36,19 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires="~=3.7",
     install_requires=[
         "absl-py",
         "dill!=0.3.6",
-        "gpflow>=2.7.0",
-        "gpflux>=0.3.1",
+        "gpflow>=2.8.1",
+        "gpflux>=0.4.2",
         "numpy",
-        "tensorflow>=2.5",
+        "tensorflow>=2.5; platform_system!='Darwin' or platform_machine!='arm64'",
+        "tensorflow-macos>=2.5; platform_system=='Darwin' and platform_machine=='arm64'",
         "tensorflow-probability>=0.13",
         "greenlet>=1.1.0",
     ],
     extras_require={
         "plotting": ["seaborn", "plotly"],
         "qhsri": ["pymoo", "cvxpy"],
     },
```

### Comparing `trieste-1.1.2/trieste/__init__.py` & `trieste-1.2.0/trieste/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,19 +15,14 @@
 The library root. See :mod:`~trieste.bayesian_optimizer` for the core optimizer, which requires
 models (see :mod:`~trieste.models`), and data sets (see :mod:`~trieste.data`). The
 :mod:`~trieste.acquisition` package provides a selection of acquisition algorithms and the
 functionality to define your own. The :mod:`~trieste.ask_tell_optimization` package provides API
 for Ask-Tell optimization and manual control of the optimization loop.
 The :mod:`~trieste.objectives` package contains several popular objective functions,
 useful for experimentation.
-
-Bibliography
-============
-
-.. bibliography::
 """
 from . import (
     acquisition,
     ask_tell_optimization,
     bayesian_optimizer,
     data,
     models,
```

### Comparing `trieste-1.1.2/trieste/acquisition/__init__.py` & `trieste-1.2.0/trieste/acquisition/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/acquisition/combination.py` & `trieste-1.2.0/trieste/acquisition/combination.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,49 +11,50 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 from abc import abstractmethod
 from collections.abc import Mapping, Sequence
-from typing import Optional
+from typing import Callable, Optional
 
 import tensorflow as tf
 
 from ..data import Dataset
-from ..models import ProbabilisticModel
+from ..models import ProbabilisticModelType
 from ..types import Tag, TensorType
 from .interface import AcquisitionFunction, AcquisitionFunctionBuilder
 
 
-class Reducer(AcquisitionFunctionBuilder[ProbabilisticModel]):
+class Reducer(AcquisitionFunctionBuilder[ProbabilisticModelType]):
     r"""
     A :class:`Reducer` builds an :const:`~trieste.acquisition.AcquisitionFunction` whose output is
     calculated from the outputs of a number of other
     :const:`~trieste.acquisition.AcquisitionFunction`\ s. How these outputs are composed is defined
     by the method :meth:`_reduce`.
     """
 
-    def __init__(self, *builders: AcquisitionFunctionBuilder[ProbabilisticModel]):
+    def __init__(self, *builders: AcquisitionFunctionBuilder[ProbabilisticModelType]):
         r"""
         :param \*builders: Acquisition function builders. At least one must be provided.
         :raise `~tf.errors.InvalidArgumentError`: If no builders are specified.
         """
         tf.debugging.assert_positive(
             len(builders), "At least one acquisition builder expected, got none."
         )
 
         self._acquisitions = builders
 
-    def _repr_builders(self) -> str:
-        return ", ".join(map(repr, self._acquisitions))
+    def __repr__(self) -> str:
+        """"""
+        return "{}({})".format(self.__class__.__name__, ", ".join(map(repr, self._acquisitions)))
 
     def prepare_acquisition_function(
         self,
-        models: Mapping[Tag, ProbabilisticModel],
+        models: Mapping[Tag, ProbabilisticModelType],
         datasets: Optional[Mapping[Tag, Dataset]] = None,
     ) -> AcquisitionFunction:
         r"""
         Return an acquisition function. This acquisition function is defined by first building
         acquisition functions from each of the
         :class:`~trieste.acquisition.AcquisitionFunctionBuilder`\ s specified at
         :meth:`__init__`, then reducing, with :meth:`_reduce`, the output of each of those
@@ -71,15 +72,15 @@
             return self._reduce_acquisition_functions(at, self.functions)
 
         return evaluate_acquisition_function_fn
 
     def update_acquisition_function(
         self,
         function: AcquisitionFunction,
-        models: Mapping[Tag, ProbabilisticModel],
+        models: Mapping[Tag, ProbabilisticModelType],
         datasets: Optional[Mapping[Tag, Dataset]] = None,
     ) -> AcquisitionFunction:
         """
         :param function: The acquisition function to update.
         :param models: The model.
         :param datasets: Unused.
         """
@@ -90,15 +91,15 @@
 
         def evaluate_acquisition_function_fn(at: TensorType) -> TensorType:
             return self._reduce_acquisition_functions(at, self.functions)
 
         return evaluate_acquisition_function_fn
 
     @property
-    def acquisitions(self) -> Sequence[AcquisitionFunctionBuilder[ProbabilisticModel]]:
+    def acquisitions(self) -> Sequence[AcquisitionFunctionBuilder[ProbabilisticModelType]]:
         """The acquisition function builders specified at class initialisation."""
         return self._acquisitions
 
     def _reduce_acquisition_functions(
         self, at: TensorType, acquisition_functions: Sequence[AcquisitionFunction]
     ) -> TensorType:
         return self._reduce([fn(at) for fn in acquisition_functions])
@@ -108,41 +109,61 @@
         """
         :param inputs: The output of each constituent acquisition function.
         :return: The output of the reduced acquisition function.
         """
         raise NotImplementedError()
 
 
-class Sum(Reducer):
+class Sum(Reducer[ProbabilisticModelType]):
     """
     :class:`Reducer` whose resulting acquisition function returns the element-wise sum of the
     outputs of constituent acquisition functions.
     """
 
-    def __repr__(self) -> str:
-        """"""
-        return f"Sum({self._repr_builders()})"
-
     def _reduce(self, inputs: Sequence[TensorType]) -> TensorType:
         """
         :param inputs: The outputs of each acquisition function.
         :return: The element-wise sum of the ``inputs``.
         """
         return tf.add_n(inputs)
 
 
-class Product(Reducer):
+class Product(Reducer[ProbabilisticModelType]):
     """
     :class:`Reducer` whose resulting acquisition function returns the element-wise product of the
     outputs of constituent acquisition functions.
     """
 
-    def __repr__(self) -> str:
-        """"""
-        return f"Product({self._repr_builders()})"
-
     def _reduce(self, inputs: Sequence[TensorType]) -> TensorType:
         """
         :param inputs: The outputs of each acquisition function.
         :return: The element-wise product of the ``inputs``.
         """
         return tf.reduce_prod(inputs, axis=0)
+
+
+class Map(Reducer[ProbabilisticModelType]):
+    """
+    :class:`Reducer` that accepts just one acquisition function builder and applies a
+    given function to its output. For example ``Map(lambda x: -x, builder)`` would generate
+    an acquisition function that returns the negative of the output of ``builder``.
+    """
+
+    def __init__(
+        self,
+        map_fn: Callable[[TensorType], TensorType],
+        builder: AcquisitionFunctionBuilder[ProbabilisticModelType],
+    ):
+        """
+        :param map_fn: Function to apply.
+        :param builder: Acquisition function builder.
+        """
+        super().__init__(builder)
+        self._map_fn = map_fn
+
+    def _reduce(self, inputs: Sequence[TensorType]) -> TensorType:
+        """
+        :param inputs: The outputs of the acquisition function.
+        :return: The result of applying the map function to ``inputs``.
+        """
+        tf.debugging.assert_equal(len(inputs), 1)
+        return self._map_fn(inputs[0])
```

### Comparing `trieste-1.1.2/trieste/acquisition/function/__init__.py` & `trieste-1.2.0/trieste/acquisition/function/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/acquisition/function/active_learning.py` & `trieste-1.2.0/trieste/acquisition/function/active_learning.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/acquisition/function/continuous_thompson_sampling.py` & `trieste-1.2.0/trieste/acquisition/function/continuous_thompson_sampling.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/acquisition/function/entropy.py` & `trieste-1.2.0/trieste/acquisition/function/entropy.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/acquisition/function/function.py` & `trieste-1.2.0/trieste/acquisition/function/function.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/acquisition/function/greedy_batch.py` & `trieste-1.2.0/trieste/acquisition/function/greedy_batch.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/acquisition/function/multi_objective.py` & `trieste-1.2.0/trieste/acquisition/function/multi_objective.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/acquisition/function/utils.py` & `trieste-1.2.0/trieste/acquisition/function/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/acquisition/interface.py` & `trieste-1.2.0/trieste/acquisition/interface.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/acquisition/multi_objective/__init__.py` & `trieste-1.2.0/trieste/acquisition/multi_objective/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/acquisition/multi_objective/dominance.py` & `trieste-1.2.0/trieste/acquisition/multi_objective/dominance.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/acquisition/multi_objective/pareto.py` & `trieste-1.2.0/trieste/acquisition/multi_objective/pareto.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/acquisition/multi_objective/partition.py` & `trieste-1.2.0/trieste/acquisition/multi_objective/partition.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/acquisition/optimizer.py` & `trieste-1.2.0/trieste/acquisition/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,15 +346,15 @@
                     best_values = tf.math.reduce_max(fun_values, axis=0)
                     improve = best_values - tf.cast(best_initial_values, best_values.dtype)
                     return improve[0] if V == 1 else improve
 
                 if V == 1:
                     logging.scalar("spo_improvement_on_initial_samples", improvements)
                 else:
-                    logging.histogram("spo_improvement_on_initial_samples", improvements)
+                    logging.histogram("spo_improvements_on_initial_samples", improvements)
 
         best_run_ids = tf.math.argmax(fun_values, axis=0)  # [V]
         chosen_points = tf.gather(
             tf.transpose(chosen_x, [1, 0, 2]), best_run_ids, batch_dims=1
         )  # [V, D]
 
         return chosen_points
```

### Comparing `trieste-1.1.2/trieste/acquisition/rule.py` & `trieste-1.2.0/trieste/acquisition/rule.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 """
 This module contains acquisition rules, which choose the optimal point(s) to query on each step of
 the Bayesian optimization process.
 """
 from __future__ import annotations
 
 import copy
+import math
 from abc import ABC, abstractmethod
 from collections.abc import Mapping
 from dataclasses import dataclass
 from typing import Any, Callable, Generic, Optional, TypeVar, Union, cast, overload
 
 import numpy as np
 
@@ -35,15 +36,20 @@
     PymooProblem = object
 
 import tensorflow as tf
 
 from .. import logging, types
 from ..data import Dataset
 from ..models import ProbabilisticModel
-from ..models.interfaces import HasReparamSampler, ModelStack, ProbabilisticModelType
+from ..models.interfaces import (
+    HasReparamSampler,
+    ModelStack,
+    ProbabilisticModelType,
+    TrainableSupportsGetKernel,
+)
 from ..observer import OBJECTIVE
 from ..space import Box, SearchSpace
 from ..types import State, Tag, TensorType
 from .function import (
     BatchMonteCarloExpectedImprovement,
     ExpectedImprovement,
     ProbabilityOfImprovement,
@@ -61,15 +67,15 @@
 from .optimizer import (
     AcquisitionOptimizer,
     automatic_optimizer_selector,
     batchify_joint,
     batchify_vectorize,
 )
 from .sampler import ExactThompsonSampler, ThompsonSampler
-from .utils import select_nth_output
+from .utils import get_local_dataset, select_nth_output
 
 ResultType = TypeVar("ResultType", covariant=True)
 """ Unbound covariant type variable. """
 
 SearchSpaceType = TypeVar("SearchSpaceType", bound=SearchSpace, contravariant=True)
 """ Contravariant type variable bound to :class:`~trieste.space.SearchSpace`. """
 
@@ -298,15 +304,15 @@
                 values = self._acquisition_function(batched_points)[0]
                 if len(values) == 1:
                     logging.scalar(
                         "EGO.acquisition_function/maximum_found" + "[0]" * greedy, values[0]
                     )
                 else:  # vectorized acquisition function
                     logging.histogram(
-                        "EGO.acquisition_function/maximum_found" + "[0]" * greedy, values
+                        "EGO.acquisition_function/maximums_found" + "[0]" * greedy, values
                     )
 
         if isinstance(self._builder, GreedyAcquisitionFunctionBuilder):
             for i in range(
                 self._num_query_points - 1
             ):  # greedily allocate remaining batch elements
                 self._acquisition_function = self._builder.update_acquisition_function(
@@ -326,15 +332,15 @@
                         values = self._acquisition_function(batched_points)[0]
                         if len(values) == 1:
                             logging.scalar(
                                 f"EGO.acquisition_function/maximum_found[{i + 1}]", values[0]
                             )
                         else:  # vectorized acquisition function
                             logging.histogram(
-                                f"EGO.acquisition_function/maximum_found[{i+1}]", values
+                                f"EGO.acquisition_function/maximums_found[{i+1}]", values
                             )
 
         return points
 
 
 @dataclass(frozen=True)
 class AsynchronousRuleState:
@@ -1093,14 +1099,243 @@
             state_ = TrustRegion.State(acquisition_space, eps, y_min, is_global)
 
             return state_, points
 
         return state_func
 
 
+class TURBO(
+    AcquisitionRule[
+        types.State[Optional["TURBO.State"], TensorType], Box, TrainableSupportsGetKernel
+    ]
+):
+    """Implements the TURBO algorithm as detailed in :cite:`eriksson2019scalable`."""
+
+    @dataclass(frozen=True)
+    class State:
+        """The acquisition state for the :class:`TURBO` acquisition rule."""
+
+        acquisition_space: Box
+        """ The search space. """
+
+        L: float
+        """ Length of the trust region (before standardizing by model lengthscales) """
+
+        failure_counter: int
+        """ Number of consecutive failures (reset if we see a success). """
+
+        success_counter: int
+        """ Number of consecutive successes (reset if we see a failure).  """
+
+        y_min: TensorType
+        """ The minimum observed value. """
+
+        def __deepcopy__(self, memo: dict[int, object]) -> TURBO.State:
+            box_copy = copy.deepcopy(self.acquisition_space, memo)
+            return TURBO.State(
+                box_copy, self.L, self.failure_counter, self.success_counter, self.y_min
+            )
+
+    def __init__(
+        self,
+        search_space: SearchSpace,
+        num_trust_regions: int = 1,
+        rule: Optional[AcquisitionRule[ResultType, Box, TrainableSupportsGetKernel]] = None,
+        L_min: Optional[float] = None,
+        L_init: Optional[float] = None,
+        L_max: Optional[float] = None,
+        success_tolerance: int = 3,
+        failure_tolerance: Optional[int] = None,
+        local_models: Optional[Mapping[Tag, TrainableSupportsGetKernel]] = None,
+    ):
+        """
+        Note that the optional parameters are set by a heuristic if not given by the user.
+
+        :param search_space: The search space.
+        :param num_trust_regions: Number of trust regions controlled by TURBO
+        :param rule: rule used to select points from within the trust region, using the local model.
+        :param L_min: Minimum allowed length of the trust region.
+        :param L_init: Initial length of the trust region.
+        :param L_max: Maximum allowed length of the trust region.
+        :param success_tolerance: Number of consecutive successes before changing region size.
+        :param failure tolerance: Number of consecutive failures before changing region size.
+        :param local_models: Optional model to act as the local model. This will be refit using
+            the data from each trust region. If no local_models are provided then we just
+            copy the global model.
+        """
+
+        if not num_trust_regions > 0:
+            raise ValueError(f"Num trust regions must be greater than 0, got {num_trust_regions}")
+
+        if num_trust_regions > 1:
+            raise NotImplementedError(
+                f"TURBO does not yet support multiple trust regions, but got {num_trust_regions}"
+            )
+
+        # implement heuristic defaults for TURBO if not specified by user
+        if rule is None:  # default to Thompson sampling with batches of size 1
+            rule = DiscreteThompsonSampling(tf.minimum(100 * search_space.dimension, 5_000), 1)
+
+        if failure_tolerance is None:
+            if isinstance(
+                rule,
+                (
+                    EfficientGlobalOptimization,
+                    DiscreteThompsonSampling,
+                    RandomSampling,
+                    AsynchronousOptimization,
+                ),
+            ):
+                failure_tolerance = math.ceil(search_space.dimension / rule._num_query_points)
+            else:
+                failure_tolerance == search_space.dimension
+            assert isinstance(failure_tolerance, int)
+        search_space_max_width = tf.reduce_max(search_space.upper - search_space.lower)
+        if L_min is None:
+            L_min = (0.5**7) * search_space_max_width
+        if L_init is None:
+            L_init = 0.8 * search_space_max_width
+        if L_max is None:
+            L_max = 1.6 * search_space_max_width
+
+        if not success_tolerance > 0:
+            raise ValueError(
+                f"success tolerance must be an integer greater than 0, got {success_tolerance}"
+            )
+        if not failure_tolerance > 0:
+            raise ValueError(
+                f"success tolerance must be an integer greater than 0, got {failure_tolerance}"
+            )
+
+        if L_min <= 0:
+            raise ValueError(f"L_min must be postive, got {L_min}")
+        if L_init <= 0:
+            raise ValueError(f"L_min must be postive, got {L_init}")
+        if L_max <= 0:
+            raise ValueError(f"L_min must be postive, got {L_max}")
+
+        self._num_trust_regions = num_trust_regions
+        self._L_min = L_min
+        self._L_init = L_init
+        self._L_max = L_max
+        self._success_tolerance = success_tolerance
+        self._failure_tolerance = failure_tolerance
+        self._rule = rule
+        self._local_models = local_models
+
+    def __repr__(self) -> str:
+        """"""
+        return f"TURBO({self._num_trust_regions!r}, {self._rule})"
+
+    def acquire(
+        self,
+        search_space: Box,
+        models: Mapping[Tag, TrainableSupportsGetKernel],
+        datasets: Optional[Mapping[Tag, Dataset]] = None,
+    ) -> types.State[State | None, TensorType]:
+        """
+        Construct a local search space from ``search_space`` according the TURBO algorithm,
+        and use that with the ``rule`` specified at :meth:`~TURBO.__init__` to find new
+        query points. Return a function that constructs these points given a previous trust region
+        state.
+
+        If no ``state`` is specified (it is `None`), then we build the initial trust region.
+
+        If a ``state`` is specified, and the new optimum improves over the previous optimum,
+        the previous acquisition is considered successful.
+
+        If ``success_tolerance`` previous consecutive acquisitions were successful then the search
+        space is made larger. If  ``failure_tolerance`` consecutive acquisitions were unsuccessful
+        then the search space is shrunk. If neither condition is triggered then the search space
+        remains the same.
+
+        **Note:** The acquisition search space will never extend beyond the boundary of the
+        ``search_space``. For a local search, the actual search space will be the
+        intersection of the trust region and ``search_space``.
+
+        :param search_space: The local acquisition search space for *this step*.
+        :param models: The model for each tag.
+        :param datasets: The known observer query points and observations. Uses the data for key
+            `OBJECTIVE` to calculate the new trust region.
+        :return: A function that constructs the next acquisition state and the recommended query
+            points from the previous acquisition state.
+        :raise KeyError: If ``datasets`` does not contain the key `OBJECTIVE`.
+        """
+        if self._local_models is None:  # if user doesnt specifiy a local model
+            self._local_models = copy.copy(models)  # copy global model (will be fit locally later)
+
+        if self._local_models.keys() != {OBJECTIVE}:
+            raise ValueError(
+                f"dict of models must contain the single key {OBJECTIVE}, got keys {models.keys()}"
+            )
+
+        if datasets is None or datasets.keys() != {OBJECTIVE}:
+            raise ValueError(
+                f"""datasets must be provided and contain the single key {OBJECTIVE}"""
+            )
+
+        dataset = datasets[OBJECTIVE]
+        local_model = self._local_models[OBJECTIVE]
+        global_lower = search_space.lower
+        global_upper = search_space.upper
+
+        y_min = tf.reduce_min(dataset.observations, axis=0)
+
+        def state_func(
+            state: TURBO.State | None,
+        ) -> tuple[TURBO.State | None, TensorType]:
+            if state is None:  # initialise first TR
+                L, failure_counter, success_counter = self._L_init, 0, 0
+            else:  # update TR
+                step_is_success = y_min < state.y_min - 1e-10  # maybe make this stronger?
+                failure_counter = (
+                    0 if step_is_success else state.failure_counter + 1
+                )  # update or reset counter
+                success_counter = (
+                    state.success_counter + 1 if step_is_success else 0
+                )  # update or reset counter
+                L = state.L
+                if success_counter == self._success_tolerance:
+                    L *= 2.0  # make region bigger
+                    success_counter = 0
+                elif failure_counter == self._failure_tolerance:
+                    L *= 0.5  # make region smaller
+                    failure_counter = 0
+
+                L = tf.minimum(L, self._L_max)
+                if L < self._L_min:  # if gets too small then start again
+                    L, failure_counter, success_counter = self._L_init, 0, 0
+
+            # build region with volume according to length L but stretched according to lengthscales
+            xmin = dataset.query_points[tf.argmin(dataset.observations)[0], :]  # centre of region
+            lengthscales = (
+                local_model.get_kernel().lengthscales
+            )  # stretch region according to model lengthscales
+            tr_width = (
+                lengthscales * L / tf.reduce_prod(lengthscales) ** (1.0 / global_lower.shape[-1])
+            )  # keep volume fixed
+            acquisition_space = Box(
+                tf.reduce_max([global_lower, xmin - tr_width / 2.0], axis=0),
+                tf.reduce_min([global_upper, xmin + tr_width / 2.0], axis=0),
+            )
+
+            # fit the local model using just data from the trust region
+            local_dataset = get_local_dataset(acquisition_space, dataset)
+            local_model.update(local_dataset)
+            local_model.optimize(local_dataset)
+
+            # use local model and local dataset to choose next query point(s)
+            points = self._rule.acquire_single(acquisition_space, local_model, local_dataset)
+            state_ = TURBO.State(acquisition_space, L, failure_counter, success_counter, y_min)
+
+            return state_, points
+
+        return state_func
+
+
 class BatchHypervolumeSharpeRatioIndicator(
     AcquisitionRule[TensorType, SearchSpace, ProbabilisticModel]
 ):
     """Implements the Batch Hypervolume Sharpe-ratio indicator acquisition
     rule, designed for large batches, introduced by Binois et al, 2021.
     See :cite:`binois2021portfolio` for details.
     """
```

### Comparing `trieste-1.1.2/trieste/acquisition/sampler.py` & `trieste-1.2.0/trieste/acquisition/sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         model: ProbabilisticModel,
         sample_size: int,
         at: TensorType,
         select_output: Callable[[TensorType], TensorType] = select_nth_output,
     ) -> TensorType:
         """
         Return exact samples from either the objective function's minimiser or its minimal value
-        over the candidate set `at`.
+        over the candidate set `at`. Note that minimiser ties aren't broken randomly.
 
         :param model: The model to sample from.
         :param sample_size: The desired number of samples.
         :param at: Where to sample the predictive distribution, with shape `[N, D]`, for points
             of dimension `D`.
         :param select_output: A method that returns the desired output from the model sampler, with
             shape `[S, N]` where `S` is the number of samples and `N` is the number of locations.
@@ -221,15 +221,15 @@
         model: ProbabilisticModel,
         sample_size: int,
         at: TensorType,
         select_output: Callable[[TensorType], TensorType] = select_nth_output,
     ) -> TensorType:
         """
         Return approximate samples from either the objective function's minimser or its minimal
-        value over the candidate set `at`.
+        value over the candidate set `at`. Note that minimiser ties aren't broken randomly.
 
         :param model: The model to sample from.
         :param sample_size: The desired number of samples.
         :param at: Where to sample the predictive distribution, with shape `[N, D]`, for points
             of dimension `D`.
         :param select_output: A method that returns the desired output from the model sampler, with
             shape `[S, N]` where `S` is the number of samples and `N` is the number of locations.
```

### Comparing `trieste-1.1.2/trieste/acquisition/utils.py` & `trieste-1.2.0/trieste/acquisition/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import functools
 from typing import Tuple, Union
 
 import tensorflow as tf
 
+from ..data import Dataset
 from ..space import SearchSpaceType
 from ..types import TensorType
 from .interface import AcquisitionFunction
 from .optimizer import AcquisitionOptimizer
 
 
 def split_acquisition_function(
@@ -110,7 +111,27 @@
 
     :param x: Input with shape [..., B, L], where L is the number of outputs of the model.
     :param output_dim: Dimension of the output to be selected. Defaults to the first output.
     :return: TensorType with shape [..., B], where the output_dim dimension has been selected to
         reduce the input.
     """
     return x[..., output_dim]
+
+
+def get_local_dataset(local_space: SearchSpaceType, dataset: Dataset) -> Dataset:
+    """
+    A utility function that takes in a dataset and returns the entries lying
+    within a given search space.
+
+    :param local_space: A search space.
+    :param dataset: A Dataset.
+    :return: A Dataset containing entries only in the local_space.
+    """
+    if tf.shape(dataset.query_points)[1] != local_space.dimension:
+        raise ValueError("Dataset and search space must have equal dimensions")
+
+    is_in_region_mask = local_space.contains(dataset.query_points)
+    local_dataset = Dataset(
+        query_points=tf.boolean_mask(dataset.query_points, is_in_region_mask),
+        observations=tf.boolean_mask(dataset.observations, is_in_region_mask),
+    )
+    return local_dataset
```

### Comparing `trieste-1.1.2/trieste/ask_tell_optimization.py` & `trieste-1.2.0/trieste/ask_tell_optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,18 @@
 from typing import Dict, Generic, Mapping, TypeVar, cast, overload
 
 try:
     import pandas as pd
 except ModuleNotFoundError:
     pd = None
 
+import warnings
+
 from . import logging
-from .acquisition.rule import AcquisitionRule, EfficientGlobalOptimization
+from .acquisition.rule import TURBO, AcquisitionRule, EfficientGlobalOptimization
 from .bayesian_optimizer import (
     FrozenRecord,
     OptimizationResult,
     Record,
     observation_plot_init,
     write_summary_initial_model_fit,
     write_summary_observations,
@@ -214,14 +216,22 @@
             self._acquisition_rule = cast(
                 AcquisitionRule[TensorType, SearchSpaceType, TrainableProbabilisticModelType],
                 EfficientGlobalOptimization(),
             )
         else:
             self._acquisition_rule = acquisition_rule
 
+        if (fit_model) and isinstance(acquisition_rule, TURBO):
+            warnings.warn(
+                """
+                Are you sure you want to keep fitting the global model even though you
+                are using TURBO which uses local models? This is a waste of computation.
+                """
+            )
+
         if fit_model:
             with Timer() as initial_model_fitting_timer:
                 for tag, model in self._models.items():
                     dataset = datasets[tag]
                     model.update(dataset)
                     model.optimize(dataset)
```

### Comparing `trieste-1.1.2/trieste/bayesian_optimizer.py` & `trieste-1.2.0/trieste/bayesian_optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 This module contains the :class:`BayesianOptimizer` class, used to perform Bayesian optimization.
 """
 
 from __future__ import annotations
 
 import copy
 import traceback
+import warnings
 from collections import Counter
 from dataclasses import dataclass
 from pathlib import Path
 from typing import (
+    Any,
     Callable,
     ClassVar,
     Dict,
     Generic,
     Mapping,
     MutableMapping,
     Optional,
@@ -48,15 +50,15 @@
     import pandas as pd
     import seaborn as sns
 except ModuleNotFoundError:
     pd = None
     sns = None
 
 from . import logging
-from .acquisition.rule import AcquisitionRule, EfficientGlobalOptimization
+from .acquisition.rule import TURBO, AcquisitionRule, EfficientGlobalOptimization
 from .data import Dataset
 from .models import SupportsCovarianceWithTopFidelity, TrainableProbabilisticModel
 from .observer import OBJECTIVE, Observer
 from .space import SearchSpace
 from .types import State, Tag, TensorType
 from .utils import Err, Ok, Result, Timer
 
@@ -192,14 +194,24 @@
         **Note:** In contrast to the standard library function :func:`dataclasses.astuple`, this
         method does *not* deepcopy instance attributes.
 
         :return: The :attr:`final_result` and :attr:`history` as a 2-tuple.
         """
         return self.final_result, self.history
 
+    @property
+    def is_ok(self) -> bool:
+        """`True` if the final result contains a :class:`Record`."""
+        return self.final_result.is_ok
+
+    @property
+    def is_err(self) -> bool:
+        """`True` if the final result contains an exception."""
+        return self.final_result.is_err
+
     def try_get_final_datasets(self) -> Mapping[Tag, Dataset]:
         """
         Convenience method to attempt to get the final data.
 
         :return: The final data, if the optimization completed successfully.
         :raise Exception: If an exception occurred during optimization.
         """
@@ -322,18 +334,20 @@
         self,
         num_steps: int,
         datasets: Mapping[Tag, Dataset],
         models: Mapping[Tag, TrainableProbabilisticModel],
         *,
         track_state: bool = True,
         track_path: Optional[Path | str] = None,
+        fit_model: bool = True,
         fit_initial_model: bool = True,
         early_stop_callback: Optional[
             EarlyStopCallback[TrainableProbabilisticModel, object]
         ] = None,
+        start_step: int = 0,
     ) -> OptimizationResult[None]:
         ...
 
     @overload
     def optimize(
         self,
         num_steps: int,
@@ -341,18 +355,20 @@
         models: Mapping[Tag, TrainableProbabilisticModelType],
         acquisition_rule: AcquisitionRule[
             TensorType, SearchSpaceType, TrainableProbabilisticModelType
         ],
         *,
         track_state: bool = True,
         track_path: Optional[Path | str] = None,
+        fit_model: bool = True,
         fit_initial_model: bool = True,
         early_stop_callback: Optional[
             EarlyStopCallback[TrainableProbabilisticModelType, object]
         ] = None,
+        start_step: int = 0,
         # this should really be OptimizationResult[None], but tf.Tensor is untyped so the type
         # checker can't differentiate between TensorType and State[S | None, TensorType], and
         # the return types clash. object is close enough to None that object will do.
     ) -> OptimizationResult[object]:
         ...
 
     @overload
@@ -363,18 +379,20 @@
         models: Mapping[Tag, TrainableProbabilisticModelType],
         acquisition_rule: AcquisitionRule[
             TensorType, SearchSpaceType, TrainableProbabilisticModelType
         ],
         *,
         track_state: bool = True,
         track_path: Optional[Path | str] = None,
+        fit_model: bool = True,
         fit_initial_model: bool = True,
         early_stop_callback: Optional[
             EarlyStopCallback[TrainableProbabilisticModelType, object]
         ] = None,
+        start_step: int = 0,
     ) -> OptimizationResult[object]:
         ...
 
     @overload
     def optimize(
         self,
         num_steps: int,
@@ -383,18 +401,20 @@
         acquisition_rule: AcquisitionRule[
             State[StateType | None, TensorType], SearchSpaceType, TrainableProbabilisticModelType
         ],
         acquisition_state: StateType | None = None,
         *,
         track_state: bool = True,
         track_path: Optional[Path | str] = None,
+        fit_model: bool = True,
         fit_initial_model: bool = True,
         early_stop_callback: Optional[
             EarlyStopCallback[TrainableProbabilisticModelType, StateType]
         ] = None,
+        start_step: int = 0,
     ) -> OptimizationResult[StateType]:
         ...
 
     @overload
     def optimize(
         self,
         num_steps: int,
@@ -403,34 +423,38 @@
         acquisition_rule: AcquisitionRule[
             State[StateType | None, TensorType], SearchSpaceType, TrainableProbabilisticModelType
         ],
         acquisition_state: StateType | None = None,
         *,
         track_state: bool = True,
         track_path: Optional[Path | str] = None,
+        fit_model: bool = True,
         fit_initial_model: bool = True,
         early_stop_callback: Optional[
             EarlyStopCallback[TrainableProbabilisticModelType, StateType]
         ] = None,
+        start_step: int = 0,
     ) -> OptimizationResult[StateType]:
         ...
 
     @overload
     def optimize(
         self,
         num_steps: int,
         datasets: Dataset,
         models: TrainableProbabilisticModel,
         *,
         track_state: bool = True,
         track_path: Optional[Path | str] = None,
+        fit_model: bool = True,
         fit_initial_model: bool = True,
         early_stop_callback: Optional[
             EarlyStopCallback[TrainableProbabilisticModel, object]
         ] = None,
+        start_step: int = 0,
     ) -> OptimizationResult[None]:
         ...
 
     @overload
     def optimize(
         self,
         num_steps: int,
@@ -438,18 +462,20 @@
         models: TrainableProbabilisticModelType,
         acquisition_rule: AcquisitionRule[
             TensorType, SearchSpaceType, TrainableProbabilisticModelType
         ],
         *,
         track_state: bool = True,
         track_path: Optional[Path | str] = None,
+        fit_model: bool = True,
         fit_initial_model: bool = True,
         early_stop_callback: Optional[
             EarlyStopCallback[TrainableProbabilisticModelType, object]
         ] = None,
+        start_step: int = 0,
     ) -> OptimizationResult[object]:
         ...
 
     @overload
     def optimize(
         self,
         num_steps: int,
@@ -457,18 +483,20 @@
         models: TrainableProbabilisticModelType,
         acquisition_rule: AcquisitionRule[
             TensorType, SearchSpaceType, TrainableProbabilisticModelType
         ],
         *,
         track_state: bool = True,
         track_path: Optional[Path | str] = None,
+        fit_model: bool = True,
         fit_initial_model: bool = True,
         early_stop_callback: Optional[
             EarlyStopCallback[TrainableProbabilisticModelType, object]
         ] = None,
+        start_step: int = 0,
     ) -> OptimizationResult[object]:
         ...
 
     @overload
     def optimize(
         self,
         num_steps: int,
@@ -477,18 +505,20 @@
         acquisition_rule: AcquisitionRule[
             State[StateType | None, TensorType], SearchSpaceType, TrainableProbabilisticModelType
         ],
         acquisition_state: StateType | None = None,
         *,
         track_state: bool = True,
         track_path: Optional[Path | str] = None,
+        fit_model: bool = True,
         fit_initial_model: bool = True,
         early_stop_callback: Optional[
             EarlyStopCallback[TrainableProbabilisticModelType, StateType]
         ] = None,
+        start_step: int = 0,
     ) -> OptimizationResult[StateType]:
         ...
 
     @overload
     def optimize(
         self,
         num_steps: int,
@@ -497,18 +527,20 @@
         acquisition_rule: AcquisitionRule[
             State[StateType | None, TensorType], SearchSpaceType, TrainableProbabilisticModelType
         ],
         acquisition_state: StateType | None = None,
         *,
         track_state: bool = True,
         track_path: Optional[Path | str] = None,
+        fit_model: bool = True,
         fit_initial_model: bool = True,
         early_stop_callback: Optional[
             EarlyStopCallback[TrainableProbabilisticModelType, StateType]
         ] = None,
+        start_step: int = 0,
     ) -> OptimizationResult[StateType]:
         ...
 
     def optimize(
         self,
         num_steps: int,
         datasets: Mapping[Tag, Dataset] | Dataset,
@@ -519,18 +551,20 @@
             TrainableProbabilisticModelType,
         ]
         | None = None,
         acquisition_state: StateType | None = None,
         *,
         track_state: bool = True,
         track_path: Optional[Path | str] = None,
+        fit_model: bool = True,
         fit_initial_model: bool = True,
         early_stop_callback: Optional[
             EarlyStopCallback[TrainableProbabilisticModelType, StateType]
         ] = None,
+        start_step: int = 0,
     ) -> OptimizationResult[StateType] | OptimizationResult[None]:
         """
         Attempt to find the minimizer of the ``observer`` in the ``search_space`` (both specified at
         :meth:`__init__`). This is the central implementation of the Bayesian optimization loop.
 
         For each step in ``num_steps``, this method:
             - Finds the next points with which to query the ``observer`` using the
@@ -564,20 +598,24 @@
         :param acquisition_state: The acquisition state to use on the first optimization step.
             This argument allows the caller to restore the optimization process from an existing
             :class:`Record`.
         :param track_state: If `True`, this method saves the optimization state at the start of each
             step. Models and acquisition state are copied using `copy.deepcopy`.
         :param track_path: If set, the optimization state is saved to disk at this path,
             rather than being copied in memory.
-        :param fit_initial_model: If `False`, this method assumes that the initial models have
-            already been optimized on the datasets and so do not require optimization before the
-            first optimization step.
+        :param fit_model: If `False` then we never fit the model during BO (e.g. if we
+            are using a rule that doesn't rely on the models and don't want to waste computation).
+        :param fit_initial_model: If `False` then we assume that the initial models have
+            already been optimized on the datasets and so do not require optimization before
+            the first optimization step.
         :param early_stop_callback: An optional callback that is evaluated with the current
             datasets, models and optimization state before every optimization step. If this
             returns `True` then the optimization loop is terminated early.
+        :param start_step: The step number to start with. This number is removed from ``num_steps``
+            and is useful for restarting previous computations.
         :return: An :class:`OptimizationResult`. The :attr:`final_result` element contains either
             the final optimization data, models and acquisition state, or, if an exception was
             raised while executing the optimization loop, it contains the exception raised. In
             either case, the :attr:`history` element is the history of the data, models and
             acquisition state at the *start* of each optimization step (up to and including any step
             that fails to complete). The history will never include the final optimization result.
         :raise ValueError: If any of the following are true:
@@ -603,14 +641,23 @@
                 f"datasets and models should contain the same keys. Got {datasets.keys()} and"
                 f" {models.keys()} respectively."
             )
 
         if not datasets:
             raise ValueError("dicts of datasets and models must be populated.")
 
+        if fit_model and isinstance(acquisition_rule, TURBO):
+            warnings.warn(
+                """
+                Are you sure you want to keep fitting the global model even though you
+                are using TURBO which has only local models? This is a waste of computation.
+                Consider setting 'fit_model'='False'.
+                """
+            )
+
         if acquisition_rule is None:
             if datasets.keys() != {OBJECTIVE}:
                 raise ValueError(
                     f"Default acquisition rule EfficientGlobalOptimization requires tag"
                     f" {OBJECTIVE!r}, got keys {datasets.keys()}"
                 )
 
@@ -630,15 +677,15 @@
                     self._search_space,
                     acquisition_rule,
                     datasets,
                     models,
                     num_steps,
                 )
 
-        for step in range(1, num_steps + 1):
+        for step in range(start_step + 1, num_steps + 1):
             logging.set_step_number(step)
 
             if early_stop_callback and early_stop_callback(datasets, models, acquisition_state):
                 tf.print("Optimization terminated early", output_stream=absl.logging.INFO)
                 break
 
             try:
@@ -663,15 +710,15 @@
                             "some of the model wrappers accept a model closure as a workaround.) "
                             "For these models, the `track_state`` argument of the "
                             ":meth:`~trieste.bayesian_optimizer.BayesianOptimizer.optimize` method "
                             "should be set to `False`. This means that only the final model "
                             "will be available."
                         ) from e
 
-                if step == 1 and fit_initial_model:
+                if step == 1 and fit_model and fit_initial_model:
                     with Timer() as initial_model_fitting_timer:
                         for tag, model in models.items():
                             dataset = datasets[tag]
                             model.update(dataset)
                             model.optimize(dataset)
                     if summary_writer:
                         logging.set_step_number(0)
@@ -696,20 +743,20 @@
                     tagged_output = (
                         observer_output
                         if isinstance(observer_output, Mapping)
                         else {OBJECTIVE: observer_output}
                     )
 
                     datasets = {tag: datasets[tag] + tagged_output[tag] for tag in tagged_output}
-
                     with Timer() as model_fitting_timer:
-                        for tag, model in models.items():
-                            dataset = datasets[tag]
-                            model.update(dataset)
-                            model.optimize(dataset)
+                        if fit_model:
+                            for tag, model in models.items():
+                                dataset = datasets[tag]
+                                model.update(dataset)
+                                model.optimize(dataset)
 
                 if summary_writer:
                     with summary_writer.as_default(step=step):
                         write_summary_observations(
                             datasets,
                             models,
                             tagged_output,
@@ -752,14 +799,56 @@
 
         record = Record(datasets, models, acquisition_state)
         result = OptimizationResult(Ok(record), history)
         if track_state and track_path is not None:
             result.save_result(Path(track_path) / OptimizationResult.RESULTS_FILENAME)
         return result
 
+    def continue_optimization(
+        self,
+        num_steps: int,
+        optimization_result: OptimizationResult[StateType],
+        *args: Any,
+        **kwargs: Any,
+    ) -> OptimizationResult[StateType]:
+        """
+        Continue a previous optimization that either failed, was terminated early, or which
+        you simply wish to run for more steps.
+
+        :param num_steps: The total number of optimization steps, including any that have already
+            been run.
+        :param optimization_result: The optimization result from which to extract the datasets,
+            models and acquisition state. If the result was successful then the final result is
+            used; otherwise the last record in the history is used. The size of the history
+            is used to determine how many more steps are required.
+        :param args: Any more positional arguments to pass on to optimize.
+        :param kwargs: Any more keyword arguments to pass on to optimize.
+        :return: An :class:`OptimizationResult`. The history will contain both the history from
+            `optimization_result` (including the `final_result` if that was successful) and
+            any new records.
+        """
+        history: list[Record[StateType] | FrozenRecord[StateType]] = []
+        history.extend(optimization_result.history)
+        if optimization_result.final_result.is_ok:
+            history.append(optimization_result.final_result.unwrap())
+        if not history:
+            raise ValueError("Cannot continue from empty optimization result")
+
+        result = self.optimize(  # type: ignore[call-overload]
+            num_steps,
+            history[-1].datasets,
+            history[-1].models,
+            *args,
+            acquisition_state=history[-1].acquisition_state,
+            **kwargs,
+            start_step=len(history) - 1,
+        )
+        result.history[:1] = history
+        return result
+
 
 def write_summary_init(
     observer: Observer,
     search_space: SearchSpace,
     acquisition_rule: AcquisitionRule[
         TensorType | State[StateType | None, TensorType],
         SearchSpaceType,
@@ -937,15 +1026,15 @@
     query_plot_dfs: MutableMapping[int, pd.DataFrame],
 ) -> None:
     """Write TensorBoard summary for the current step query points."""
 
     if tf.rank(query_points) == 2:
         for i in tf.range(tf.shape(query_points)[1]):
             if len(query_points) == 1:
-                logging.scalar(f"query_points/[{i}]", float(query_points[0, i]))
+                logging.scalar(f"query_point/[{i}]", float(query_points[0, i]))
             else:
                 logging.histogram(f"query_points/[{i}]", query_points[:, i])
         logging.histogram("query_points/euclidean_distances", lambda: pdist(query_points))
 
     if pd and sns and logging.include_summary("query_points/_pairplot"):
         columns = [f"x{i}" for i in range(tf.shape(query_points)[1])]
         qp_preds = query_points
@@ -983,35 +1072,39 @@
     minimum: Optional[tf.Tensor] = None,
     minimizers: Optional[tf.Tensor] = None,
     minimum_atol: float = 0,
     minimum_rtol: float = 0.05,
     minimizers_atol: float = 0,
     minimizers_rtol: float = 0.05,
     objective_tag: Tag = OBJECTIVE,
+    minimum_step_number: Optional[int] = None,
 ) -> EarlyStopCallback[TrainableProbabilisticModel, object]:
     """
     Generate an early stop function that terminates a BO loop when it gets close enough to the
     given objective minimum and/or minimizer points.
 
     :param minimum: Optional minimum to stop at, with shape [1].
     :param minimizers: Optional minimizer points to stop at, with shape [N, D].
     :param minimum_atol: Absolute tolerance for minimum.
     :param minimum_rtol: Relative tolerance for minimum.
     :param minimizers_atol: Absolute tolerance for minimizer point.
     :param minimizers_rtol: Relative tolerance for minimizer point.
     :param objective_tag: The tag for the objective data.
+    :param minimum_step_number: Minimum step number to stop at.
     :return: An early stop function that terminates if we get close enough to both the minimum
         and any of the minimizer points.
     """
 
     def early_stop_callback(
         datasets: Mapping[Tag, Dataset],
         _models: Mapping[Tag, TrainableProbabilisticModel],
         _acquisition_state: object,
     ) -> bool:
+        if minimum_step_number is not None and logging.get_step_number() < minimum_step_number:
+            return False
         dataset = datasets[objective_tag]
         arg_min_idx = tf.squeeze(tf.argmin(dataset.observations, axis=0))
         if minimum is not None:
             best_y = dataset.observations[arg_min_idx]
             close_y = np.isclose(best_y, minimum, atol=minimum_atol, rtol=minimum_rtol)
             if not tf.reduce_all(close_y):
                 return False
```

### Comparing `trieste-1.1.2/trieste/data.py` & `trieste-1.2.0/trieste/data.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/experimental/plotting/__init__.py` & `trieste-1.2.0/trieste/experimental/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/experimental/plotting/inequality_constraints.py` & `trieste-1.2.0/trieste/experimental/plotting/inequality_constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,18 +54,18 @@
     :return: figure
     """
     objective_fn = simulation.objective
     constraint_fn = simulation.constraint
     lower_bound = search_space.lower
     upper_bound = search_space.upper
 
-    grid, xx, yy = create_grid(lower_bound, upper_bound, grid_density=80)
+    grid, xx, yy = create_grid(lower_bound, upper_bound, grid_density=30)
     objective = objective_fn(grid).numpy()
     constraint = constraint_fn(grid).numpy()
-    fig, (axes1, axes2) = plt.subplots(2, 2, sharex="all", sharey="all", figsize=(6, 6))
+    fig, (axes1, axes2) = plt.subplots(2, 2, sharex="all", sharey="all", figsize=(8, 8))
 
     levels = 30
 
     axes1[0].contourf(xx, yy, objective.reshape(*xx.shape), levels, alpha=0.9)
     axes1[1].contourf(xx, yy, constraint.reshape(*xx.shape), levels, alpha=0.9)
     axes1[0].set_title("Objective")
     axes1[1].set_title("Constraint")
@@ -109,18 +109,18 @@
     constraint_fn = simulation.constraint
     lower_bound = search_space.lower
     upper_bound = search_space.upper
     levels = 30
     psize = 15
     cw, cb, co = "white", "tab:blue", "tab:orange"
 
-    grid, xx, yy = create_grid(lower_bound, upper_bound, grid_density=80)
+    grid, xx, yy = create_grid(lower_bound, upper_bound, grid_density=30)
     objective = objective_fn(grid).numpy()
     constraint = constraint_fn(grid).numpy()
-    fig, ax = plt.subplots(1, 1, figsize=(3, 3))
+    fig, ax = plt.subplots(1, 1, figsize=(8, 6))
     constraint_points = constraint_data[-1].numpy()
     x = objective_data[0].numpy()
 
     mask_ids = constraint[:, 0] > simulation.threshold
     mask = np.zeros_like(objective, dtype=bool)
     mask[mask_ids, :] = True
     objective_masked = np.ma.array(objective, mask=mask)
```

### Comparing `trieste-1.1.2/trieste/experimental/plotting/plotting.py` & `trieste-1.2.0/trieste/experimental/plotting/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from trieste.acquisition import AcquisitionFunction
 from trieste.acquisition.multi_objective.dominance import non_dominated
 from trieste.types import TensorType
 from trieste.utils import to_numpy
 
 
 def create_grid(
-    mins: TensorType, maxs: TensorType, grid_density: int = 20
+    mins: TensorType, maxs: TensorType, grid_density: int = 30
 ) -> tuple[TensorType, TensorType, TensorType]:
     """
     Creates a regular 2D grid of size `grid_density^2` between mins and maxs.
 
     :param mins: list of 2 lower bounds
     :param maxs: list of 2 upper bounds
     :param grid_density: scalar
@@ -93,21 +93,21 @@
         )
 
 
 def plot_function_2d(
     obj_func: Callable[[TensorType], TensorType],
     mins: TensorType,
     maxs: TensorType,
-    grid_density: int = 20,
+    grid_density: int = 100,
     contour: bool = False,
     log: bool = False,
     title: Optional[Sequence[str]] = None,
     xlabel: Optional[str] = None,
     ylabel: Optional[str] = None,
-    figsize: Optional[tuple[float, float]] = None,
+    figsize: Optional[tuple[float, float]] = (8, 6),
     colorbar: bool = False,
     alpha: float = 1.0,
     fill: bool = False,
 ) -> tuple[Figure, Axes]:
     """
     2D/3D plot of an obj_func for a grid of size grid_density**2 between mins and maxs
 
@@ -171,21 +171,21 @@
     return fig, ax
 
 
 def plot_acq_function_2d(
     acq_func: AcquisitionFunction,
     mins: TensorType,
     maxs: TensorType,
-    grid_density: int = 20,
+    grid_density: int = 100,
     contour: bool = False,
     log: bool = False,
     title: Optional[Sequence[str]] = None,
     xlabel: Optional[str] = None,
     ylabel: Optional[str] = None,
-    figsize: Optional[tuple[float, float]] = None,
+    figsize: Optional[tuple[float, float]] = (8, 6),
     colorbar: bool = False,
     alpha: float = 1.0,
     fill: bool = False,
 ) -> tuple[Figure, Axes]:
     """
     Wrapper to produce a 2D/3D plot of an acq_func for a grid of size grid_density**2 between
     mins and maxs.
@@ -225,28 +225,28 @@
         fill,
     )
 
 
 def format_point_markers(
     num_pts: int,
     num_init: Optional[int] = None,
-    idx_best: Optional[int] = None,
+    idx_best: Optional[TensorType] = None,
     mask_fail: Optional[TensorType] = None,
     m_init: str = "x",
     m_add: str = "o",
     c_pass: str = "tab:green",
     c_fail: str = "tab:red",
     c_best: str = "tab:purple",
 ) -> tuple[TensorType, TensorType]:
     """
     Prepares point marker styles according to some BO factors.
 
     :param num_pts: total number of BO points
     :param num_init: initial number of BO points
-    :param idx_best: index of the best BO point
+    :param idx_best: index of the best BO point(s)
     :param mask_fail: Bool vector, True if the corresponding observation violates the constraint(s)
     :param m_init: marker for the initial BO points
     :param m_add: marker for the other BO points
     :param c_pass: color for the regular BO points
     :param c_fail: color for the failed BO points
     :param c_best: color for the best BO points
     :return: 2 string vectors col_pts, mark_pts containing marker styles and colors
@@ -309,15 +309,15 @@
             ax.scatter(pts[i, 0], pts[i, 1], obs_values[i], c=col_pts[i], marker=mark_pts[i])
 
 
 def plot_mobo_points_in_obj_space(
     obs_values: TensorType,
     num_init: Optional[int] = None,
     mask_fail: Optional[TensorType] = None,
-    figsize: Optional[tuple[float, float]] = None,
+    figsize: Optional[tuple[float, float]] = (8, 6),
     xlabel: str = "Obj 1",
     ylabel: str = "Obj 2",
     zlabel: str = "Obj 3",
     title: Optional[str] = None,
     m_init: str = "x",
     m_add: str = "o",
     c_pass: str = "tab:green",
@@ -382,15 +382,15 @@
 
 
 def plot_mobo_history(
     obs_values: TensorType,
     metric_func: Callable[[TensorType], TensorType],
     num_init: int,
     mask_fail: Optional[TensorType] = None,
-    figsize: Optional[tuple[float, float]] = None,
+    figsize: Optional[tuple[float, float]] = (8, 6),
 ) -> tuple[Figure, Axes]:
     """
     Draw the performance measure for multi-objective optimization.
 
     :param obs_values: TF Tensor or numpy array of objective values
     :param metric_func: a callable function calculate metric score
     :param num_init: initial number of BO points
@@ -457,19 +457,19 @@
     ax.axvline(x=num_init - 0.5, color="tab:blue")
 
 
 def plot_gp_2d(
     model: GPModel,
     mins: TensorType,
     maxs: TensorType,
-    grid_density: int = 20,
+    grid_density: int = 100,
     contour: bool = False,
     xlabel: Optional[str] = None,
     ylabel: Optional[str] = None,
-    figsize: Optional[tuple[float, float]] = None,
+    figsize: Optional[tuple[float, float]] = (8, 6),
     predict_y: bool = False,
 ) -> tuple[Figure, Axes]:
     """
     2D/3D plot of a gp model for a grid of size grid_density**2 between mins and maxs
 
     :param model: a gpflow model
     :param mins: 2 lower bounds
```

### Comparing `trieste-1.1.2/trieste/experimental/plotting/plotting_plotly.py` & `trieste-1.2.0/trieste/experimental/plotting/plotting_plotly.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 from typing import Callable, Optional
 
 import numpy as np
-import pandas as pd
 import plotly.graph_objects as go
 import tensorflow as tf
 from plotly.subplots import make_subplots
 
 from trieste.models.interfaces import ProbabilisticModel
 from trieste.types import TensorType
 from trieste.utils import to_numpy
@@ -84,18 +83,18 @@
     :param fig: the current plotly figure
     :param alpha: transparency
     :param figrow: row index of the subfigure
     :param figcol: column index of the subfigure
     :return: updated plotly figure
     """
 
-    d = pd.DataFrame(f.reshape([xx.shape[0], yy.shape[1]]), index=xx, columns=yy)
+    z = f.reshape([xx.shape[0], yy.shape[1]])
 
     fig.add_trace(
-        go.Surface(z=d, x=xx, y=yy, showscale=False, opacity=alpha, colorscale="viridis"),
+        go.Surface(z=z, x=xx, y=yy, showscale=False, opacity=alpha, colorscale="viridis"),
         row=figrow,
         col=figcol,
     )
     return fig
 
 
 def add_bo_points_plotly(
@@ -142,15 +141,15 @@
     return fig
 
 
 def plot_model_predictions_plotly(
     model: ProbabilisticModel,
     mins: TensorType,
     maxs: TensorType,
-    grid_density: int = 100,
+    grid_density: int = 20,
     num_samples: Optional[int] = None,
     alpha: float = 0.85,
 ) -> go.Figure:
     """
     Plots 2-dimensional plot of model's predictions. We first create a regular grid of points
     and evaluate the model on these points. We then plot the mean and 2 standard deviations to
     show epistemic uncertainty.
@@ -198,22 +197,24 @@
         lcb = fmean - 2 * np.sqrt(fvar)
         ucb = fmean + 2 * np.sqrt(fvar)
 
         fig = add_surface_plotly(xx, yy, fmean, fig, alpha=alpha, figrow=1, figcol=k + 1)
         fig = add_surface_plotly(xx, yy, lcb, fig, alpha=alpha - 0.35, figrow=1, figcol=k + 1)
         fig = add_surface_plotly(xx, yy, ucb, fig, alpha=alpha - 0.35, figrow=1, figcol=k + 1)
 
+    fig.update_layout(height=600, width=600)
+
     return fig
 
 
 def plot_function_plotly(
     obj_func: Callable[[TensorType], TensorType],
     mins: TensorType,
     maxs: TensorType,
-    grid_density: int = 100,
+    grid_density: int = 20,
     title: Optional[str] = None,
     xlabel: Optional[str] = None,
     ylabel: Optional[str] = None,
     alpha: float = 1.0,
 ) -> go.Figure:
     """
     Plots 2-dimensional plot of an objective function. To illustrate the function we create a
@@ -249,8 +250,10 @@
 
     for k in range(n_output):
         f = F[:, k]
         fig = add_surface_plotly(xx, yy, f, fig, alpha=alpha, figrow=1, figcol=k + 1)
         fig.update_xaxes(title_text=xlabel, row=1, col=k + 1)
         fig.update_yaxes(title_text=ylabel, row=1, col=k + 1)
 
+    fig.update_layout(height=600, width=600)
+
     return fig
```

### Comparing `trieste-1.1.2/trieste/logging.py` & `trieste-1.2.0/trieste/logging.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/models/__init__.py` & `trieste-1.2.0/trieste/models/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/models/gpflow/__init__.py` & `trieste-1.2.0/trieste/models/gpflow/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/models/gpflow/builders.py` & `trieste-1.2.0/trieste/models/gpflow/builders.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/models/gpflow/inducing_point_selectors.py` & `trieste-1.2.0/trieste/models/gpflow/inducing_point_selectors.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/models/gpflow/interface.py` & `trieste-1.2.0/trieste/models/gpflow/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,17 +67,22 @@
         """
         Create a posterior cache for fast sequential predictions.  Note that this must happen
         at initialisation and *after* we ensure the model data is variable. Furthermore,
         the cache must be updated whenever the underlying model is changed.
         """
         self._posterior = self.model.posterior(PrecomputeCacheType.VARIABLE)
 
+    def _ensure_variable_model_data(self) -> None:
+        """Ensure GPflow data, which is normally stored in Tensors, is instead stored in
+        dynamically shaped Variables. Override this as required."""
+
     def __setstate__(self, state: dict[str, Any]) -> None:
         # when unpickling we may need to regenerate the posterior cache
         self.__dict__.update(state)
+        self._ensure_variable_model_data()
         if self._posterior is not None:
             self.create_posterior_cache()
 
     def update_posterior_cache(self) -> None:
         """Update the posterior cache. This needs to be called whenever the underlying model
         is changed."""
         if self._posterior is not None:
```

### Comparing `trieste-1.1.2/trieste/models/gpflow/models.py` & `trieste-1.2.0/trieste/models/gpflow/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1083,28 +1083,16 @@
         )
 
     def trajectory_sampler(self) -> TrajectorySampler[SparseVariational]:
         """
         Return a trajectory sampler. For :class:`SparseVariational`, we build
         trajectories using a decoupled random Fourier feature approximation.
 
-        At the moment only models with single latent GP are supported.
-
         :return: The trajectory sampler.
-        :raise NotImplementedError: If we try to use the
-            sampler with a model that has more than one latent GP.
         """
-        if self.model.num_latent_gps > 1:
-            raise NotImplementedError(
-                f"""
-                Trajectory sampler does not currently support models with multiple latent
-                GPs, however received a model with {self.model.num_latent_gps} latent GPs.
-                """
-            )
-
         return DecoupledTrajectorySampler(self, self._num_rff_features)
 
 
 class VariationalGaussianProcess(
     GPflowPredictor,
     TrainableProbabilisticModel,
     SupportsCovarianceBetweenPoints,
@@ -1224,21 +1212,27 @@
                 tf.Variable(
                     model.data[1],
                     trainable=False,
                     shape=[None, *model.data[1].shape[1:]],
                 ),
             )
 
+            # reinitialise the model so that the underlying Parameters have the right shape
+            # and then reassign the original values
+            old_q_mu = model.q_mu
+            old_q_sqrt = model.q_sqrt
             model.__init__(  # type: ignore[misc]
                 variable_data,
                 model.kernel,
                 model.likelihood,
                 model.mean_function,
                 model.num_latent_gps,
             )
+            model.q_mu.assign(old_q_mu)
+            model.q_sqrt.assign(old_q_sqrt)
 
     def __repr__(self) -> str:
         """"""
         return (
             f"VariationalGaussianProcess({self.model!r}, {self.optimizer!r})"
             f"{self._use_natgrads!r}, {self._natgrad_gamma!r}, {self._num_rff_features!r})"
         )
@@ -1521,15 +1515,15 @@
             )
 
             new_fidelity_signal_sample = (
                 self.rho[fidelity] * signal_sample + fidelity_residual_sample
             )  # [S, N, P]
 
             mask = query_points_fidelity_col >= fidelity  # [N, P]
-            mask = tf.repeat(mask[..., None, :, :], num_samples, axis=-3)
+            mask = tf.broadcast_to(mask[..., None, :, :], new_fidelity_signal_sample.shape)
 
             signal_sample = tf.where(mask, new_fidelity_signal_sample, signal_sample)
 
         return signal_sample
 
     def predict_y(self, query_points: TensorType) -> tuple[TensorType, TensorType]:
         """
@@ -1708,26 +1702,28 @@
         """
         (
             query_points_wo_fidelity,
             query_points_fidelity_col,
         ) = check_and_extract_fidelity_query_points(
             query_points, max_fidelity=self.num_fidelities - 1
         )  # [..., N, D], [..., N, 1]
-        # Repeat query_points to get same shape as signal sample
-        query_points_fidelity_col = tf.repeat(
-            query_points_fidelity_col[..., None, :, :], num_samples, axis=-3
-        )  # [..., S, N, 1]
 
         signal_sample = self.fidelity_models[0].sample(
             query_points_wo_fidelity, num_samples
         )  # [..., S, N, 1]
 
+        # Repeat query_points to get same shape as signal sample
+        query_points_fidelity_col = tf.broadcast_to(
+            query_points_fidelity_col[..., None, :, :], signal_sample.shape
+        )  # [..., S, N, 1]
+
         for fidelity in range(1, self.num_fidelities):
-            qp_repeated = tf.repeat(
-                query_points_wo_fidelity[..., None, :, :], num_samples, axis=-3
+            qp_repeated = tf.broadcast_to(
+                query_points_wo_fidelity[..., None, :, :],
+                signal_sample.shape[:-1] + query_points_wo_fidelity.shape[-1],
             )  # [..., S, N, D]
             qp_augmented = tf.concat([qp_repeated, signal_sample], axis=-1)  # [..., S, N, D + 1]
             new_signal_sample = self.fidelity_models[fidelity].sample(
                 qp_augmented, 1
             )  # [..., S, 1, N, 1]
             # Remove second dimension caused by getting a single sample
             new_signal_sample = new_signal_sample[..., :, 0, :, :]
@@ -1810,24 +1806,29 @@
         sample_mean, sample_var = self.fidelity_models[0].predict(
             query_points_wo_fidelity
         )  # [..., N, 1], [..., N, 1]
 
         # Create new dimension to store samples for each query point
         # Repeat the inital sample mean and variance S times and add a dimension in the
         # middle (so that sample mean and query points can be concatenated sensibly)
-        sample_mean = tf.repeat(sample_mean, self.monte_carlo_random_numbers.shape[0], axis=-1)[
+        sample_mean = tf.broadcast_to(
+            sample_mean, sample_mean.shape[:-1] + self.monte_carlo_random_numbers.shape[0]
+        )[
             ..., :, None, :
         ]  # [..., N, 1, S]
-        sample_var = tf.repeat(sample_var, self.monte_carlo_random_numbers.shape[0], axis=-1)[
+        sample_var = tf.broadcast_to(
+            sample_var, sample_var.shape[:-1] + self.monte_carlo_random_numbers.shape[0]
+        )[
             ..., :, None, :
         ]  # [..., N, 1, S]
 
         # Repeat fidelity points for each sample to match shapes for masking
-        query_points_fidelity_col = tf.repeat(
-            query_points_fidelity_col, self.monte_carlo_random_numbers.shape[0], axis=-1
+        query_points_fidelity_col = tf.broadcast_to(
+            query_points_fidelity_col,
+            query_points_fidelity_col.shape[:-1] + self.monte_carlo_random_numbers.shape[0],
         )[
             ..., :, None, :
         ]  # [..., N, 1, S]
 
         # Predict for all fidelities but stop updating once we have
         # reached desired fidelity for each query point
         for fidelity in range(1, self.num_fidelities):
@@ -1872,25 +1873,24 @@
             and sample_var: Samples of the posterior variance at the given fidelity,
             of shape [..., N, 1, S]
         """
         # Repeat random numbers for each query point and add middle dimension
         # for concatentation with query points This also means that it has the same
         # shape as sample_var and sample_mean, so there's no broadcasting required
         # Note: at the moment we use the same monte carlo values for every value in the batch dim
-        reshaped_random_numbers = tf.repeat(
-            tf.transpose(self.monte_carlo_random_numbers), query_point.shape[-2], axis=-2
-        )[
-            ..., None, :
-        ]  # [..., N, 1, S]
+
+        reshaped_random_numbers = tf.broadcast_to(
+            tf.transpose(self.monte_carlo_random_numbers)[..., None, :],
+            sample_mean.shape,
+        )  # [..., N, 1, S]
         samples = reshaped_random_numbers * tf.sqrt(sample_var) + sample_mean  # [..., N, 1, S]
         # Add an extra unit dim to query_point and repeat for each of the samples
-        qp_repeated = tf.repeat(
+        qp_repeated = tf.broadcast_to(
             query_point[..., :, :, None],  # [..., N, D, 1]
-            self.monte_carlo_random_numbers.shape[0],
-            axis=-1,
+            query_point.shape + samples.shape[-1],
         )  # [..., N, D, S]
         qp_augmented = tf.concat([qp_repeated, samples], axis=-2)  # [..., N, D+1, S]
 
         # Flatten sample dimension to n_qp dimension to pass through predictor
         # Switch dims to make reshape match up correct dimensions for query points
         # Use Einsum to switch last two dimensions
         qp_augmented = tf.linalg.matrix_transpose(qp_augmented)  # [..., N, S, D+1]
@@ -1980,29 +1980,31 @@
         num_samples = 100
         (
             query_points_wo_fidelity,
             query_points_fidelity_col,
         ) = check_and_extract_fidelity_query_points(
             query_points, max_fidelity=self.num_fidelities - 1
         )  # [N, D], [N, 1]
-        # Repeat query_points to get same shape as signal sample
-        query_points_fidelity_col = tf.repeat(
-            query_points_fidelity_col[None, :, :], num_samples, axis=0
-        )
 
         # Signal sample stops updating once fidelity is reached for that query point
         signal_sample = self.fidelity_models[0].model.predict_f_samples(
             query_points_wo_fidelity, num_samples, full_cov=False
         )
+
+        # Repeat query_points to get same shape as signal sample
+        query_points_fidelity_col = tf.broadcast_to(
+            query_points_fidelity_col[None, :, :], signal_sample.shape
+        )
         # Max fidelity sample keeps updating to the max fidelity
         max_fidelity_sample = tf.identity(signal_sample)
 
         for fidelity in range(1, self.num_fidelities):
-            qp_repeated = tf.repeat(
-                query_points_wo_fidelity[None, :, :], num_samples, axis=0
+            qp_repeated = tf.broadcast_to(
+                query_points_wo_fidelity[None, :, :],
+                tf.TensorShape(num_samples) + query_points_wo_fidelity.shape,
             )  # [S, N, D]
             # We use max fidelity sample here, which is okay because anything
             # with a lower fidelity will not be updated
             qp_augmented = tf.concat([qp_repeated, max_fidelity_sample], axis=-1)  # [S, N, D + 1]
             new_signal_sample = self.fidelity_models[fidelity].model.predict_f_samples(
                 qp_augmented, 1, full_cov=False
             )
```

### Comparing `trieste-1.1.2/trieste/models/gpflow/optimizer.py` & `trieste-1.2.0/trieste/models/gpflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/models/gpflow/sampler.py` & `trieste-1.2.0/trieste/models/gpflow/sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Callable, Optional, Tuple, TypeVar, Union, cast
 
 import tensorflow as tf
 import tensorflow_probability as tfp
+from gpflow.kernels import Kernel, MultioutputKernel
 from gpflux.layers.basis_functions.fourier_features import RandomFourierFeaturesCosine
 from gpflux.math import compute_A_inv_b
-from typing_extensions import Protocol, runtime_checkable
+from typing_extensions import Protocol, TypeGuard, runtime_checkable
 
 from ...types import TensorType
 from ...utils import DEFAULTS, flatten_leading_dims
 from ..interfaces import (
     ProbabilisticModel,
     ReparametrizationSampler,
     SupportsGetInducingVariables,
@@ -39,33 +40,40 @@
     SupportsGetObservationNoise,
     SupportsPredictJoint,
     TrajectoryFunction,
     TrajectoryFunctionClass,
     TrajectorySampler,
 )
 
+_IntTensorType = Union[tf.Tensor, int]
 
-def qmc_normal_samples(num_samples: int, n_sample_dim: int, skip: int = 0) -> tf.Tensor:
+
+def qmc_normal_samples(
+    num_samples: _IntTensorType, n_sample_dim: _IntTensorType, skip: _IntTensorType = 0
+) -> tf.Tensor:
     """
     Generates `num_samples` sobol samples, skipping the first `skip`, where each
     sample has dimension `n_sample_dim`.
     """
+
+    if num_samples == 0 or n_sample_dim == 0:
+        return tf.zeros(shape=(num_samples, n_sample_dim), dtype=tf.float64)
+
     sobol_samples = tf.math.sobol_sample(
         dim=n_sample_dim,
         num_results=num_samples,
         dtype=tf.float64,
         skip=skip,
     )
 
     dist = tfp.distributions.Normal(
         loc=tf.constant(0.0, dtype=tf.float64),
         scale=tf.constant(1.0, dtype=tf.float64),
     )
     normal_samples = dist.quantile(sobol_samples)
-    tf.debugging.assert_shapes([(normal_samples, (num_samples, n_sample_dim))])
     return normal_samples
 
 
 class IndependentReparametrizationSampler(ReparametrizationSampler[ProbabilisticModel]):
     r"""
     This sampler employs the *reparameterization trick* to approximate samples from a
     :class:`ProbabilisticModel`\ 's predictive distribution as
@@ -88,17 +96,15 @@
         :param qmc: Whether to use QMC sobol sampling instead of random normal sampling. QMC
             sampling more accurately approximates a normal distribution than truly random samples.
         :param qmc_skip: Whether to use the skip parameter to ensure the QMC sampler gives different
             samples whenever it is reset. This is not supported with XLA.
         :raise ValueError (or InvalidArgumentError): If ``sample_size`` is not positive.
         """
         super().__init__(sample_size, model)
-        self._eps = tf.Variable(
-            tf.ones([sample_size, 0], dtype=tf.float64), shape=[sample_size, None]
-        )  # [S, 0]
+        self._eps: Optional[tf.Variable] = None
         self._qmc = qmc
         self._qmc_skip = qmc_skip
 
     def sample(self, at: TensorType, *, jitter: float = DEFAULTS.JITTER) -> TensorType:
         """
         Return approximate samples from the `model` specified at :meth:`__init__`. Multiple calls to
         :meth:`sample`, for any given :class:`IndependentReparametrizationSampler` and ``at``, will
@@ -131,14 +137,17 @@
                 normal_samples = qmc_normal_samples(self._sample_size, mean.shape[-1], skip)
             else:
                 normal_samples = tf.random.normal(
                     [self._sample_size, tf.shape(mean)[-1]], dtype=tf.float64
                 )
             return normal_samples  # [S, L]
 
+        if self._eps is None:
+            self._eps = tf.Variable(sample_eps())
+
         tf.cond(
             self._initialized,
             lambda: self._eps,
             lambda: self._eps.assign(sample_eps()),
         )
 
         return mean + tf.sqrt(var) * tf.cast(self._eps[:, None, :], var.dtype)  # [..., S, 1, L]
@@ -177,17 +186,15 @@
         """
         super().__init__(sample_size, model)
         if not isinstance(model, SupportsPredictJoint):
             raise NotImplementedError(
                 f"BatchReparametrizationSampler only works with models that support "
                 f"predict_joint; received {model.__repr__()}"
             )
-        self._eps = tf.Variable(
-            tf.ones([0, 0, sample_size], dtype=tf.float64), shape=[None, None, sample_size]
-        )  # [0, 0, S]
+        self._eps: Optional[tf.Variable] = None
         self._qmc = qmc
         self._qmc_skip = qmc_skip
 
     def sample(self, at: TensorType, *, jitter: float = DEFAULTS.JITTER) -> TensorType:
         """
         Return approximate samples from the `model` specified at :meth:`__init__`. Multiple calls to
         :meth:`sample`, for any given :class:`BatchReparametrizationSampler` and ``at``, will
@@ -212,22 +219,14 @@
         tf.debugging.assert_rank_at_least(at, 2)
         tf.debugging.assert_greater_equal(jitter, 0.0)
 
         batch_size = at.shape[-2]
 
         tf.debugging.assert_positive(batch_size)
 
-        if self._initialized:
-            tf.debugging.assert_equal(
-                batch_size,
-                tf.shape(self._eps)[-2],
-                f"{type(self).__name__} requires a fixed batch size. Got batch size {batch_size}"
-                f" but previous batch size was {tf.shape(self._eps)[-2]}.",
-            )
-
         mean, cov = self._model.predict_joint(at)  # [..., B, L], [..., L, B, B]
 
         def sample_eps() -> tf.Tensor:
             self._initialized.assign(True)
             if self._qmc:
                 if self._qmc_skip:
                     skip = IndependentReparametrizationSampler.skip
@@ -243,20 +242,32 @@
                 normal_samples = tf.transpose(normal_samples, perm=[0, 2, 1])  # [L, B, S]
             else:
                 normal_samples = tf.random.normal(
                     [tf.shape(mean)[-1], batch_size, self._sample_size], dtype=tf.float64
                 )  # [L, B, S]
             return normal_samples
 
+        if self._eps is None:
+            # dynamically shaped as the same sampler may be called with different sized batches
+            self._eps = tf.Variable(sample_eps(), shape=[None, None, self._sample_size])
+
         tf.cond(
             self._initialized,
             lambda: self._eps,
             lambda: self._eps.assign(sample_eps()),
         )
 
+        if self._initialized:
+            tf.debugging.assert_equal(
+                batch_size,
+                tf.shape(self._eps)[-2],
+                f"{type(self).__name__} requires a fixed batch size. Got batch size {batch_size}"
+                f" but previous batch size was {tf.shape(self._eps)[-2]}.",
+            )
+
         identity = tf.eye(batch_size, dtype=cov.dtype)  # [B, B]
         cov_cholesky = tf.linalg.cholesky(cov + jitter * identity)  # [..., L, B, B]
 
         variance_contribution = cov_cholesky @ tf.cast(self._eps, cov.dtype)  # [..., L, B, S]
 
         leading_indices = tf.range(tf.rank(variance_contribution) - 3)
         absolute_trailing_indices = [-1, -2, -3] + tf.rank(variance_contribution)
@@ -301,14 +312,29 @@
 FeatureDecompositionTrajectorySamplerModelType = TypeVar(
     "FeatureDecompositionTrajectorySamplerModelType",
     bound=FeatureDecompositionTrajectorySamplerModel,
     contravariant=True,
 )
 
 
+def _is_multioutput_kernel(kernel: Kernel) -> TypeGuard[MultioutputKernel]:
+    return isinstance(kernel, MultioutputKernel)
+
+
+def _get_kernel_function(kernel: Kernel) -> Callable[[TensorType, TensorType], tf.Tensor]:
+    # Select between a multioutput kernel and a single-output kernel.
+    def K(X: TensorType, X2: Optional[TensorType] = None) -> tf.Tensor:
+        if _is_multioutput_kernel(kernel):
+            return kernel.K(X, X2, full_output_cov=False)  # [L, M, M]
+        else:
+            return tf.expand_dims(kernel.K(X, X2), axis=0)  # [1, M, M]
+
+    return K
+
+
 class FeatureDecompositionTrajectorySampler(
     TrajectorySampler[FeatureDecompositionTrajectorySamplerModelType],
     ABC,
 ):
     r"""
 
     This is a general class to build functions that approximate a trajectory sampled from an
@@ -352,15 +378,16 @@
 
     def get_trajectory(self) -> TrajectoryFunction:
         """
         Generate an approximate function draw (trajectory) by sampling weights
         and evaluating the feature functions.
 
         :return: A trajectory function representing an approximate trajectory from the Gaussian
-            process, taking an input of shape `[N, D]` and returning shape `[N, 1]`
+            process, taking an input of shape `[N, B, D]` and returning shape `[N, B, L]`
+            where `L` is the number of outputs of the model.
         """
 
         weight_sampler = self._prepare_weight_sampler()  # prep feature weight distribution
 
         return feature_decomposition_trajectory(
             feature_functions=self._feature_functions,
             weight_sampler=weight_sampler,
@@ -401,19 +428,19 @@
         tf.debugging.Assert(
             isinstance(trajectory, feature_decomposition_trajectory), [tf.constant([])]
         )
         cast(feature_decomposition_trajectory, trajectory).resample()
         return trajectory  # return trajectory with resampled weights
 
     @abstractmethod
-    def _prepare_weight_sampler(self) -> Callable[[int], TensorType]:  # [B] -> [L, B]
+    def _prepare_weight_sampler(self) -> Callable[[int], TensorType]:  # [B] -> [B, F, L]
         """
         Calculate the posterior of the feature weights for the specified feature functions,
         returning a function that takes in a batch size `B` and returns `B` samples for
-        the weights of each of the `L` features.
+        the weights of each of the `F` features for `L` outputs.
         """
         raise NotImplementedError
 
 
 class RandomFourierFeatureTrajectorySampler(
     FeatureDecompositionTrajectorySampler[FeatureDecompositionInternalDataModel]
 ):
@@ -466,51 +493,48 @@
                 f"RandomFourierFeatureTrajectorySampler only works with models with "
                 f"get_kernel, get_observation_noise and get_internal_data methods; "
                 f"but received {model.__repr__()}."
             )
 
         tf.debugging.assert_positive(num_features)
         self._num_features = num_features
-        self._model = model
-        feature_functions = ResampleableRandomFourierFeatureFunctions(
-            self._model, self._num_features
-        )
-        super().__init__(self._model, feature_functions)
+        feature_functions = ResampleableRandomFourierFeatureFunctions(model, self._num_features)
+        super().__init__(model, feature_functions)
 
-    def _prepare_weight_sampler(self) -> Callable[[int], TensorType]:  # [B] -> [L, B]
+    def _prepare_weight_sampler(self) -> Callable[[int], TensorType]:  # [B] -> [B, F, 1]
         """
         Calculate the posterior of theta (the feature weights) for the RFFs, returning
         a function that takes in a batch size `B` and returns `B` samples for
-        the weights of each of the RFF `L` features.
+        the weights of each of the RFF `F` features for one output.
         """
 
         dataset = self._model.get_internal_data()
         num_data = tf.shape(dataset.query_points)[0]  # n
         if (
             self._num_features < num_data
         ):  # if m < n  then calculate posterior in design space (an m*m matrix inversion)
             theta_posterior = self._prepare_theta_posterior_in_design_space()
         else:  # if n <= m  then calculate posterior in gram space (an n*n matrix inversion)
             theta_posterior = self._prepare_theta_posterior_in_gram_space()
 
-        return lambda b: theta_posterior.sample(b)
+        return lambda b: tf.expand_dims(theta_posterior.sample(b), axis=-1)
 
     def _prepare_theta_posterior_in_design_space(self) -> tfp.distributions.MultivariateNormalTriL:
         r"""
         Calculate the posterior of theta (the feature weights) in the design space. This
         distribution is a Gaussian
 
         .. math:: \theta \sim N(D^{-1}\Phi^Ty,D^{-1}\sigma^2)
 
         where the [m,m] design matrix :math:`D=(\Phi^T\Phi + \sigma^2I_m)` is defined for
         the [n,m] matrix of feature evaluations across the training data :math:`\Phi`
         and observation noise variance :math:`\sigma^2`.
         """
         dataset = self._model.get_internal_data()
-        phi = self._feature_functions(dataset.query_points)  # [n, m]
+        phi = self._feature_functions(tf.convert_to_tensor(dataset.query_points))  # [n, m]
         D = tf.matmul(phi, phi, transpose_a=True)  # [m, m]
         s = self._model.get_observation_noise() * tf.eye(self._num_features, dtype=phi.dtype)
         L = tf.linalg.cholesky(D + s)
         D_inv = tf.linalg.cholesky_solve(L, tf.eye(self._num_features, dtype=phi.dtype))
 
         residuals = dataset.observations - self._model.get_mean_function()(dataset.query_points)
         theta_posterior_mean = tf.matmul(D_inv, tf.matmul(phi, residuals, transpose_a=True))[
@@ -532,15 +556,15 @@
 
         where the [n,n] gram matrix :math:`G=(\Phi\Phi^T + \sigma^2I_n)` is defined for the [n,m]
         matrix of feature evaluations across the training data :math:`\Phi` and
         observation noise variance :math:`\sigma^2`.
         """
         dataset = self._model.get_internal_data()
         num_data = tf.shape(dataset.query_points)[0]  # n
-        phi = self._feature_functions(dataset.query_points)  # [n, m]
+        phi = self._feature_functions(tf.convert_to_tensor(dataset.query_points))  # [n, m]
         G = tf.matmul(phi, phi, transpose_b=True)  # [n, n]
         s = self._model.get_observation_noise() * tf.eye(num_data, dtype=phi.dtype)
         L = tf.linalg.cholesky(G + s)
         L_inv_phi = tf.linalg.triangular_solve(L, phi)  # [n, m]
         residuals = dataset.observations - self._model.get_mean_function()(
             dataset.query_points
         )  # [n, 1]
@@ -567,29 +591,28 @@
         ]
     ]
 ):
     r"""
 
     This class builds functions that approximate a trajectory sampled from an underlying Gaussian
     process model using decoupled sampling. See :cite:`wilson2020efficiently` for an introduction
-    to decoupled sampling. Currently we do not support models with multiple latent Gaussian
-    processes.
+    to decoupled sampling.
 
     Unlike our :class:`RandomFourierFeatureTrajectorySampler` which uses a RFF decomposition to
     aprroximate the Gaussian process posterior, a :class:`DecoupledTrajectorySampler` only
     uses an RFF decomposition to approximate the Gausian process prior and instead using
-    a cannonical decomposition to discretize the effect of updating the prior on the given data.
+    a canonical decomposition to discretize the effect of updating the prior on the given data.
 
     In particular, we approximate the Gaussian processes' posterior samples as the finite feature
     approximation
 
     .. math:: \hat{f}(.) = \sum_{i=1}^L w_i\phi_i(.) + \sum_{j=1}^m v_jk(.,z_j)
 
     where :math:`\phi_i(.)` and :math:`w_i` are the Fourier features and their weights that
-    discretize the prior. In contrast, `k(.,z_j)` and :math:`v_i` are the cannonical features and
+    discretize the prior. In contrast, `k(.,z_j)` and :math:`v_i` are the canonical features and
     their weights that discretize the data update.
 
     The expression for :math:`v_i` depends on if we are using an exact Gaussian process or a sparse
     approximations. See  eq. (13) in :cite:`wilson2020efficiently` for details.
 
     Note that if a model is both of :class:`FeatureDecompositionInducingPointModel` type and
     :class:`FeatureDecompositionInternalDataModel` type,
@@ -619,99 +642,105 @@
                 f"DecoupledTrajectorySampler only works with models that either support "
                 f"get_kernel, get_observation_noise and get_internal_data or support get_kernel "
                 f"and get_inducing_variables; but received {model.__repr__()}."
             )
 
         tf.debugging.assert_positive(num_features)
         self._num_features = num_features
-        self._model = model
-        feature_functions = ResampleableDecoupledFeatureFunctions(self._model, self._num_features)
+        feature_functions = ResampleableDecoupledFeatureFunctions(model, self._num_features)
 
-        super().__init__(self._model, feature_functions)
+        super().__init__(model, feature_functions)
 
-    def _prepare_weight_sampler(self) -> Callable[[int], TensorType]:
+    def _prepare_weight_sampler(self) -> Callable[[int], TensorType]:  # [B] -> [B, F + M, L]
         """
         Prepare the sampler function that provides samples of the feature weights
-        for both the RFF and cannonical feature functions, i.e. we return a function
+        for both the RFF and canonical feature functions, i.e. we return a function
         that takes in a batch size `B` and returns `B` samples for the weights of each of
-        the `L`  RFF features and `N` cannonical features.
+        the `F`  RFF features and `M` canonical features for `L` outputs.
         """
 
+        kernel_K = _get_kernel_function(self._model.get_kernel())
         if isinstance(self._model, FeatureDecompositionInducingPointModel):
             (  # extract variational parameters
                 inducing_points,
                 q_mu,
                 q_sqrt,
                 whiten,
-            ) = self._model.get_inducing_variables()  # [M, d], [M, 1], [1, M, 1]
-            q_sqrt = q_sqrt[0, :, :]  # [M, M]
-            Kmm = self._model.get_kernel().K(inducing_points, inducing_points)  # [M, M]
+            ) = self._model.get_inducing_variables()  # [M, D], [M, L], [L, M, M], []
+            Kmm = kernel_K(inducing_points, inducing_points)  # [L, M, M]
             Kmm += tf.eye(tf.shape(inducing_points)[0], dtype=Kmm.dtype) * DEFAULTS.JITTER
         else:  # massage quantities from GP to look like variational parameters
             internal_data = self._model.get_internal_data()
-            inducing_points = internal_data.query_points  # [M, d]
-            q_mu = self._model.get_internal_data().observations  # [M, 1]
+            inducing_points = internal_data.query_points  # [M, D]
+            q_mu = self._model.get_internal_data().observations  # [M, L]
             q_mu = q_mu - self._model.get_mean_function()(
                 inducing_points
             )  # account for mean function
             q_sqrt = tf.eye(tf.shape(inducing_points)[0], dtype=tf.float64)  # [M, M]
+            q_sqrt = tf.expand_dims(q_sqrt, axis=0)  # [1, M, M]
             q_sqrt = tf.math.sqrt(self._model.get_observation_noise()) * q_sqrt
             whiten = False
-            Kmm = (
-                self._model.get_kernel().K(inducing_points, inducing_points) + q_sqrt**2
-            )  # [M, M]
+            Kmm = kernel_K(inducing_points, inducing_points) + q_sqrt**2  # [L, M, M]
 
+        M, L = tf.shape(q_mu)
         tf.debugging.assert_shapes(
             [
-                (inducing_points, ["M", "d"]),
-                (q_mu, ["M", "1"]),
-                (q_sqrt, ["M", "M"]),
-                (Kmm, ["M", "M"]),
+                (inducing_points, ["M", "D"]),
+                (q_mu, ["M", "L"]),
+                (q_sqrt, ["L", "M", "M"]),
+                (Kmm, ["L", "M", "M"]),
             ]
         )
 
         def weight_sampler(batch_size: int) -> Tuple[TensorType, TensorType]:
             prior_weights = tf.random.normal(  # Non-RFF features will require scaling here
-                [self._num_features, batch_size], dtype=tf.float64
-            )  # [L, B]
+                [L, self._num_features, batch_size], dtype=tf.float64
+            )  # [L, F, B]
 
             u_noise_sample = tf.matmul(
-                q_sqrt,  # [M, M]
-                tf.random.normal(
-                    (tf.shape(inducing_points)[0], batch_size), dtype=tf.float64
-                ),  # [ M, B]
-            )  # [M, B]
+                q_sqrt,  # [L, M, M]
+                tf.random.normal((L, M, batch_size), dtype=tf.float64),  # [L, M, B]
+            )  # [L, M, B]
 
-            u_sample = q_mu + u_noise_sample  # [M, B]
+            u_sample = tf.linalg.matrix_transpose(q_mu)[..., None] + u_noise_sample  # [L, M, B]
 
             if whiten:
-                Luu = tf.linalg.cholesky(Kmm)  # [M, M]
-                u_sample = tf.matmul(Luu, u_sample)  # [M, B]
+                Luu = tf.linalg.cholesky(Kmm)  # [L, M, M]
+                u_sample = tf.matmul(Luu, u_sample)  # [L, M, B]
 
-            phi_Z = self._feature_functions(inducing_points)[:, : self._num_features]  # [M, B]
-            weight_space_prior_Z = phi_Z @ prior_weights  # [M, B]
-
-            diff = u_sample - weight_space_prior_Z  # [M, B]
-
-            v = compute_A_inv_b(Kmm, diff)  # [M, B]
-
-            tf.debugging.assert_shapes([(v, ["M", "B"]), (prior_weights, ["L", "B"])])
-
-            return tf.transpose(tf.concat([prior_weights, v], axis=0))  # [B, L + M]
+            # It is important that the feature-function is called with a tensor, instead of a
+            # parameter (which inducing points can be). This is to ensure pickling works correctly.
+            # First time a Keras layer (i.e. feature-functions) is built, the shape of the input is
+            # used to set the input-spec. If the input is a parameter, the input-spec will not be
+            # for an ordinary tensor and pickling will fail.
+            phi_Z = self._feature_functions(tf.convert_to_tensor(inducing_points))[
+                ..., : self._num_features
+            ]  # [M, F] or [L, M, F]
+            weight_space_prior_Z = phi_Z @ prior_weights  # [L, M, B]
+
+            diff = u_sample - weight_space_prior_Z  # [L, M, B]
+
+            v = compute_A_inv_b(Kmm, diff)  # [L, M, B]
+
+            tf.debugging.assert_shapes([(v, ["L", "M", "B"]), (prior_weights, ["L", "F", "B"])])
+
+            return tf.transpose(
+                tf.concat([prior_weights, v], axis=1), perm=[2, 1, 0]
+            )  # [B, F + M, L]
 
         return weight_sampler
 
 
 class ResampleableRandomFourierFeatureFunctions(RandomFourierFeaturesCosine):
     """
     A wrapper around GPFlux's random Fourier feature function that allows for
     efficient in-place updating when generating new decompositions.
 
-    In particular, we store the bias and weights as variables, which can then be
-    updated without triggering expensive graph retracing.
+    In particular, the bias and weights are stored as variables, which can then be
+    updated by calling :meth:`resample` without triggering expensive graph retracing.
 
     Note that if a model is both of :class:`FeatureDecompositionInducingPointModel` type and
     :class:`FeatureDecompositionInternalDataModel` type,
     :class:`FeatureDecompositionInducingPointModel` will take a priority and inducing points
     will be used for computations rather than data.
     """
 
@@ -738,40 +767,38 @@
             raise NotImplementedError(
                 f"ResampleableRandomFourierFeatureFunctions only work with models that either"
                 f"support get_kernel, get_observation_noise and get_internal_data or support "
                 f"get_kernel and get_inducing_variables;"
                 f"but received {model.__repr__()}."
             )
 
-        self._kernel = model.get_kernel()
-        self._n_components = n_components
-        super().__init__(self._kernel, self._n_components, dtype=tf.float64)
+        super().__init__(model.get_kernel(), n_components, dtype=tf.float64)
 
         if isinstance(model, SupportsGetInducingVariables):
             dummy_X = model.get_inducing_variables()[0][0:1, :]
         else:
             dummy_X = model.get_internal_data().query_points[0:1, :]
 
-        self.__call__(dummy_X)  # dummy call to force init of weights
-        self.b: TensorType = tf.Variable(self.b)
-        self.W: TensorType = tf.Variable(self.W)  # allow updateable weights
+        # Always build the weights and biases. This is important for saving the trajectory (using
+        # tf.saved_model.save) before it has been used.
+        self.build(dummy_X.shape)
 
     def resample(self) -> None:
         """
         Resample weights and biases
         """
         self.b.assign(self._bias_init(tf.shape(self.b), dtype=self._dtype))
         self.W.assign(self._weights_init(tf.shape(self.W), dtype=self._dtype))
 
 
 class ResampleableDecoupledFeatureFunctions(ResampleableRandomFourierFeatureFunctions):
     """
     A wrapper around our :class:`ResampleableRandomFourierFeatureFunctions` which rather
-    than evaluates just `L` RFF functions instead evaluates the concatenation of
-    `L` RFF functions with evaluations of the cannonical basis functions.
+    than evaluates just `F` RFF functions instead evaluates the concatenation of
+    `F` RFF functions with evaluations of the canonical basis functions.
 
     Note that if a model is both of :class:`FeatureDecompositionInducingPointModel` type and
     :class:`FeatureDecompositionInternalDataModel` type,
     :class:`FeatureDecompositionInducingPointModel` will take a priority and inducing points
     will be used for computations rather than data.
     """
 
@@ -784,32 +811,36 @@
         n_components: int,
     ):
         """
         :param model: The model that will be approximed by these feature functions.
         :param n_components: The desired number of features.
         """
 
+        super().__init__(model, n_components)
+
         if isinstance(model, SupportsGetInducingVariables):
-            inducing_points = model.get_inducing_variables()[0]  # [M, D]
+            self._inducing_points = model.get_inducing_variables()[0]  # [M, D]
         else:
-            inducing_points = model.get_internal_data().query_points  # [M, D]
+            self._inducing_points = model.get_internal_data().query_points  # [M, D]
 
-        self._cannonical_feature_functions = lambda x: tf.linalg.matrix_transpose(
-            model.get_kernel().K(inducing_points, x)
+        kernel_K = _get_kernel_function(self.kernel)
+        self._canonical_feature_functions = lambda x: tf.linalg.matrix_transpose(
+            kernel_K(self._inducing_points, x)
         )
 
-        super().__init__(model, n_components)
-
-    def __call__(self, x: TensorType) -> TensorType:  # [N,D] -> [N, L + M]
+    def call(self, x: TensorType) -> TensorType:  # [N, D] -> [N, F + M] or [L, N, F + M]
         """
-        combine prior basis functions with cannonical basis functions
+        combine prior basis functions with canonical basis functions
         """
-        fourier_feature_eval = super().__call__(x)  # [N, L]
-        cannonical_feature_eval = self._cannonical_feature_functions(x)  # [N, M]
-        return tf.concat([fourier_feature_eval, cannonical_feature_eval], axis=-1)  # [N, L + M]
+        fourier_feature_eval = super().call(x)  # [N, F] or [L, N, F]
+        canonical_feature_eval = self._canonical_feature_functions(x)  # [1, N, M] or [L, N, M]
+        # ensure matching rank between features, i.e. drop the leading 1 dimension
+        matched_shape = tf.shape(canonical_feature_eval)[-tf.rank(fourier_feature_eval) :]
+        canonical_feature_eval = tf.reshape(canonical_feature_eval, matched_shape)
+        return tf.concat([fourier_feature_eval, canonical_feature_eval], axis=-1)
 
 
 class feature_decomposition_trajectory(TrajectoryFunctionClass):
     r"""
     An approximate sample from a Gaussian processes' posterior samples represented as a
     finite weighted sum of features.
 
@@ -837,23 +868,23 @@
         """
         self._feature_functions = feature_functions
         self._mean_function = mean_function
         self._weight_sampler = weight_sampler
         self._initialized = tf.Variable(False)
 
         self._weights_sample = tf.Variable(  # dummy init to be updated before trajectory evaluation
-            tf.ones([0, 0], dtype=tf.float64), shape=[None, None]
+            tf.ones([0, 0, 0], dtype=tf.float64), shape=[None, None, None]
         )
 
         self._batch_size = tf.Variable(
             0, dtype=tf.int32
         )  # dummy init to be updated before trajectory evaluation
 
     @tf.function
-    def __call__(self, x: TensorType) -> TensorType:  # [N, B, d] -> [N, B, 1]
+    def __call__(self, x: TensorType) -> TensorType:  # [N, B, D] -> [N, B, L]
         """Call trajectory function."""
 
         if not self._initialized:  # work out desired batch size from input
             self._batch_size.assign(tf.shape(x)[-2])  # B
             self.resample()  # sample B feature weights
             self._initialized.assign(True)
 
@@ -863,27 +894,34 @@
             message=f"""
             This trajectory only supports batch sizes of {self._batch_size}.
             If you wish to change the batch size you must get a new trajectory
             by calling the get_trajectory method of the trajectory sampler.
             """,
         )
 
-        flat_x, unflatten = flatten_leading_dims(x)  # [N*B, d]
-        flattened_feature_evaluations = self._feature_functions(flat_x)  # [N*B, m]
-        feature_evaluations = unflatten(flattened_feature_evaluations)  # [N, B, m]
+        flat_x, unflatten = flatten_leading_dims(x)  # [N*B, D]
+        flattened_feature_evaluations = self._feature_functions(
+            flat_x
+        )  # [N*B, F + M] or [L, N*B, F + M]
+        # ensure tensor is always rank 3
+        rank3_shape = tf.concat([[1], tf.shape(flattened_feature_evaluations)], axis=0)[-3:]
+        flattened_feature_evaluations = tf.reshape(flattened_feature_evaluations, rank3_shape)
+        flattened_feature_evaluations = tf.transpose(
+            flattened_feature_evaluations, perm=[1, 2, 0]
+        )  # [N*B, F + M, L]
+        feature_evaluations = unflatten(flattened_feature_evaluations)  # [N, B, F + M, L]
+
         mean = self._mean_function(x)  # account for the model's mean function
-        return (
-            tf.reduce_sum(feature_evaluations * self._weights_sample, -1, keepdims=True) + mean
-        )  # [N, B, 1]
+        return tf.reduce_sum(feature_evaluations * self._weights_sample, -2) + mean  # [N, B, L]
 
     def resample(self) -> None:
         """
         Efficiently resample in-place without retracing.
         """
-        self._weights_sample.assign(  # [B, m]
+        self._weights_sample.assign(  # [B, F + M, L]
             self._weight_sampler(self._batch_size)
         )  # resample weights
 
     def update(self, weight_sampler: Callable[[int], TensorType]) -> None:
         """
         Efficiently update the trajectory with a new weight distribution and resample its weights.
```

### Comparing `trieste-1.1.2/trieste/models/gpflow/utils.py` & `trieste-1.2.0/trieste/models/gpflow/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/models/gpflux/__init__.py` & `trieste-1.2.0/trieste/models/gpflux/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/models/gpflux/builders.py` & `trieste-1.2.0/trieste/models/gpflux/builders.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/models/gpflux/interface.py` & `trieste-1.2.0/trieste/models/gpflux/interface.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/models/gpflux/models.py` & `trieste-1.2.0/trieste/models/gpflux/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,18 @@
         if not isinstance(self.optimizer.optimizer, tf.optimizers.Optimizer):
             raise ValueError(
                 f"Optimizer for `DeepGaussianProcess` must be an instance of a "
                 f"`tf.optimizers.Optimizer` or `tf.keras.optimizers.Optimizer`, "
                 f"received {type(self.optimizer.optimizer)} instead."
             )
 
-        self.original_lr = self.optimizer.optimizer.lr.numpy()
+        if not isinstance(
+            self.optimizer.optimizer.lr, tf.keras.optimizers.schedules.LearningRateSchedule
+        ):
+            self.original_lr = self.optimizer.optimizer.lr.numpy()
 
         epochs = 400
 
         def scheduler(epoch: int, lr: float) -> float:
             if epoch == epochs // 2:
                 return lr * 0.1
             else:
@@ -354,18 +357,22 @@
             **fit_args,
             initial_epoch=self._absolute_epochs,
         )
 
         if self._continuous_optimisation:
             self._absolute_epochs = self._absolute_epochs + len(hist.history["loss"])
 
-        # Reset lr in case there was an lr schedule: a schedule will have change the learning rate,
-        # so that the next time we call `optimize` the starting learning rate would be different.
-        # Therefore we make sure the learning rate is set back to its initial value.
-        self.optimizer.optimizer.lr.assign(self.original_lr)
+        # Reset lr in case there was an lr schedule: a schedule will have changed the learning
+        # rate, so that the next time we call `optimize` the starting learning rate would be
+        # different. Therefore, we make sure the learning rate is set back to its initial value.
+        # However, this is not needed for `LearningRateSchedule` instances.
+        if not isinstance(
+            self.optimizer.optimizer.lr, tf.keras.optimizers.schedules.LearningRateSchedule
+        ):
+            self.optimizer.optimizer.lr.assign(self.original_lr)
 
     def log(self, dataset: Optional[Dataset] = None) -> None:
         """
         Log model training information at a given optimization step to the Tensorboard.
         We log a few summary statistics of losses, layer KL divergences and metrics (as provided in
         ``optimizer``): ``final`` value at the end of the training, ``diff`` value as a difference
         between inital and final epoch. We also log epoch statistics, but as histograms, rather
```

### Comparing `trieste-1.1.2/trieste/models/gpflux/sampler.py` & `trieste-1.2.0/trieste/models/gpflux/sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -233,28 +233,26 @@
 
         if not isinstance(layer, GPLayer):
             raise ValueError(
                 f"Layers other than gpflux.layers.GPLayer are not currently supported, received"
                 f"{type(layer)}"
             )
 
+        if isinstance(
+            layer.inducing_variable, gpflow.inducing_variables.SeparateIndependentInducingVariables
+        ):
+            raise ValueError(
+                "SeparateIndependentInducingVariables are not currently supported for decoupled "
+                "sampling."
+            )
+
         tf.debugging.assert_positive(num_features)
         self._num_features = num_features
 
-        if isinstance(layer.kernel, gpflow.kernels.MultioutputKernel):
-            if not isinstance(layer.kernel, gpflow.kernels.SharedIndependent):
-                raise ValueError(
-                    f"Multioutput kernels other than gpflow.kernels.SharedIndependent are not"
-                    f"currently supported, received {type(layer.kernel)}"
-                )
-            self._kernel = layer.kernel.kernel
-        else:
-            # GPLayers are supposed to only use multioutput kernels but we also use them with
-            # simple kernels
-            self._kernel = layer.kernel  # type: ignore[unreachable]
+        self._kernel = layer.kernel
 
         self._feature_functions = ResampleableDecoupledDeepGaussianProcessFeatureFunctions(
             layer, num_features
         )
 
         self._weight_sampler = self._prepare_weight_sampler()
 
@@ -293,18 +291,26 @@
             This trajectory only supports batch sizes of {self._batch_size}.
             If you wish to change the batch size you must get a new trajectory
             by calling the get_trajectory method of the trajectory sampler.
             """,
         )
 
         flat_x, unflatten = flatten_leading_dims(x)
-        flattened_feature_evaluations = self._feature_functions(flat_x)
-        feature_evaluations = unflatten(flattened_feature_evaluations)[
-            ..., None
-        ]  # [N, B, L + M, 1]
+        flattened_feature_evaluations = self._feature_functions(
+            flat_x
+        )  # [P, N, L + M] or [N, L + M]
+        if self._feature_functions.is_multioutput:
+            flattened_feature_evaluations = tf.transpose(
+                flattened_feature_evaluations, perm=[1, 2, 0]
+            )
+            feature_evaluations = unflatten(flattened_feature_evaluations)  # [N, B, L + M, P]
+        else:
+            feature_evaluations = unflatten(flattened_feature_evaluations)[
+                ..., None
+            ]  # [N, B, L + M, 1]
 
         return tf.reduce_sum(
             feature_evaluations * self._weights_sample, -2
         ) + self._layer.mean_function(
             x
         )  # [N, B, P]
 
@@ -333,48 +339,58 @@
         if isinstance(self._layer.inducing_variable, InducingPoints):
             inducing_points = self._layer.inducing_variable.Z  # [M, D]
         else:
             inducing_points = self._layer.inducing_variable.inducing_variable.Z  # [M, D]
 
         q_mu = self._layer.q_mu  # [M, P]
         q_sqrt = self._layer.q_sqrt  # [P, M, M]
-        Kmm = self._kernel.K(inducing_points, inducing_points)  # [M, M]
+        if self._feature_functions.is_multioutput:
+            Kmm = self._kernel.K(
+                inducing_points, inducing_points, full_output_cov=False
+            )  # [P, M, M]
+        else:
+            Kmm = self._kernel.K(inducing_points, inducing_points)  # [M, M]
         Kmm += tf.eye(tf.shape(inducing_points)[0], dtype=Kmm.dtype) * DEFAULTS.JITTER
         whiten = self._layer.whiten
         M, P = tf.shape(q_mu)[0], tf.shape(q_mu)[1]
 
         tf.debugging.assert_shapes(
             [
                 (inducing_points, ["M", "D"]),
                 (q_mu, ["M", "P"]),
                 (q_sqrt, ["P", "M", "M"]),
-                (Kmm, ["M", "M"]),
             ]
         )
 
         def weight_sampler(batch_size: int) -> TensorType:
-            prior_weights = tf.random.normal([batch_size, self._num_features, P], dtype=tf.float64)
+            prior_weights = tf.random.normal(
+                [batch_size, P, self._num_features, 1], dtype=tf.float64
+            )  # [B, P, L, 1]
 
             u_noise_sample = tf.matmul(
                 q_sqrt,  # [P, M, M]
                 tf.random.normal([batch_size, P, M, 1], dtype=tf.float64),  # [B, P, M, 1]
             )  # [B, P, M, 1]
-            u_sample = q_mu + tf.linalg.matrix_transpose(u_noise_sample[..., 0])  # [B, M, P]
+            u_sample = tf.linalg.matrix_transpose(q_mu)[..., None] + u_noise_sample  # [B, P, M, 1]
 
             if whiten:
-                Luu = tf.linalg.cholesky(Kmm)  # [M, M]
-                u_sample = tf.matmul(Luu, u_sample)
-
-            phi_Z = self._feature_functions(inducing_points)[:, : self._num_features]
-            weight_space_prior_Z = phi_Z @ prior_weights  # [B, M, P]
+                Luu = tf.linalg.cholesky(Kmm)  # [M, M] or [P, M, M]
+                u_sample = tf.matmul(Luu, u_sample)  # [B, P, M, 1]
 
-            diff = u_sample - weight_space_prior_Z  # [B, M, P]
-            v = compute_A_inv_b(Kmm, diff)  # [B, M, P]
-
-            return tf.concat([prior_weights, v], axis=1)  # [B, L + M, P]
+            phi_Z = self._feature_functions(inducing_points)[
+                ..., : self._num_features
+            ]  # [M, L] or [P, M, L]
+            weight_space_prior_Z = phi_Z @ prior_weights  # [B, P, M, 1]
+
+            diff = u_sample - weight_space_prior_Z  # [B, P, M, 1]
+            v = compute_A_inv_b(Kmm, diff)  # [B, P, M, 1]
+
+            return tf.transpose(
+                tf.concat([prior_weights, v], axis=2)[..., 0], perm=[0, 2, 1]
+            )  # [B, L + M, P]
 
         return weight_sampler
 
 
 class ResampleableDecoupledDeepGaussianProcessFeatureFunctions(RandomFourierFeaturesCosine):
     """
     A wrapper around GPflux's random Fourier feature function that allows for efficient in-place
@@ -391,29 +407,32 @@
         """
         if not isinstance(layer, GPLayer):
             raise ValueError(
                 f"ResampleableDecoupledDeepGaussianProcessFeatureFunctions currently only work with"
                 f"gpflux.layers.GPLayer layers, received {type(layer)} instead"
             )
 
-        if isinstance(layer.kernel, gpflow.kernels.SharedIndependent):
-            self._kernel = layer.kernel.kernel
-        else:
-            self._kernel = layer.kernel
+        self._kernel = layer.kernel
+
         self._n_components = n_components
         super().__init__(self._kernel, self._n_components, dtype=tf.float64)
 
         if isinstance(layer.inducing_variable, InducingPoints):
             inducing_points = layer.inducing_variable.Z
         else:
             inducing_points = layer.inducing_variable.inducing_variable.Z
 
-        self._canonical_feature_functions = lambda x: tf.linalg.matrix_transpose(
-            self._kernel.K(inducing_points, x)
-        )
+        if self.is_multioutput:
+            self._canonical_feature_functions = lambda x: tf.linalg.matrix_transpose(
+                self._kernel.K(inducing_points, x, full_output_cov=False)
+            )
+        else:
+            self._canonical_feature_functions = lambda x: tf.linalg.matrix_transpose(
+                self._kernel.K(inducing_points, x)
+            )
 
         dummy_X = inducing_points[0:1, :]
 
         self.__call__(dummy_X)
         self.b: TensorType = tf.Variable(self.b)
         self.W: TensorType = tf.Variable(self.W)
 
@@ -424,21 +443,21 @@
         if not hasattr(self, "_bias_init"):
             self.b.assign(self._sample_bias(tf.shape(self.b), dtype=self._dtype))
             self.W.assign(self._sample_weights(tf.shape(self.W), dtype=self._dtype))
         else:
             self.b.assign(self._bias_init(tf.shape(self.b), dtype=self._dtype))
             self.W.assign(self._weights_init(tf.shape(self.W), dtype=self._dtype))
 
-    def __call__(self, x: TensorType) -> TensorType:  # [N, D] -> [N, L + M]
+    def __call__(self, x: TensorType) -> TensorType:  # [N, D] -> [N, L + M] or [P, N, L + M]
         """
         Evaluate and combine prior basis functions and canonical basic functions at the input.
         """
-        fourier_feature_eval = super().__call__(x)  # [N, L]
-        canonical_feature_eval = self._canonical_feature_functions(x)  # [N, M]
-        return tf.concat([fourier_feature_eval, canonical_feature_eval], axis=-1)  # [N, L + M]
+        fourier_feature_eval = super().__call__(x)  # [N, L] or [P, N, L]
+        canonical_feature_eval = self._canonical_feature_functions(x)  # [P, N, M] or [N, M]
+        return tf.concat([fourier_feature_eval, canonical_feature_eval], axis=-1)  # [P, N, L + M]
 
 
 class dgp_feature_decomposition_trajectory(TrajectoryFunctionClass):
     r"""
     An approximate sample from a deep Gaussian process's posterior, where the samples are
     represented as a finite weighted sum of features. This class essentially takes a list of
     :class:`DeepGaussianProcessDecoupledLayer`\s and iterates through them to sample, update and
```

### Comparing `trieste-1.1.2/trieste/models/interfaces.py` & `trieste-1.2.0/trieste/models/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Callable, Generic, Optional, TypeVar
+from typing import Any, Callable, Generic, Optional, TypeVar
 
 import gpflow
 import tensorflow as tf
 from typing_extensions import Protocol, runtime_checkable
 
 from ..data import Dataset
 from ..types import TensorType
 from ..utils import DEFAULTS
+from ..utils.misc import get_variables
 
 ProbabilisticModelType = TypeVar(
     "ProbabilisticModelType", bound="ProbabilisticModel", contravariant=True
 )
 """ Contravariant type variable bound to :class:`~trieste.models.ProbabilisticModel`.
 This is used to specify classes such as samplers and acquisition function builders that
 take models as input parameters and might ony support models with certain features. """
@@ -95,14 +96,27 @@
         """
         Log model-specific information at a given optimization step.
 
         :param dataset: Optional data that can be used to log additional data-based model summaries.
         """
         return
 
+    def get_module_with_variables(self, *dependencies: Any) -> tf.Module:
+        """
+        Return a fresh module with the model's variables attached, which can then be extended
+        with methods and saved using tf.saved_model.
+
+        :param dependencies: Dependent objects whose variables should also be included.
+        """
+        module = tf.Module()
+        module.saved_variables = get_variables(self)
+        for dependency in dependencies:
+            module.saved_variables += get_variables(dependency)
+        return module
+
 
 @runtime_checkable
 class TrainableProbabilisticModel(ProbabilisticModel, Protocol):
     """A trainable probabilistic model."""
 
     @abstractmethod
     def update(self, dataset: Dataset) -> None:
@@ -149,14 +163,21 @@
         Return the kernel of the model.
         :return: The kernel.
         """
         raise NotImplementedError
 
 
 @runtime_checkable
+class TrainableSupportsGetKernel(TrainableProbabilisticModel, SupportsGetKernel, Protocol):
+    """A trainable probabilistic model that supports get_kernel."""
+
+    pass
+
+
+@runtime_checkable
 class SupportsGetObservationNoise(ProbabilisticModel, Protocol):
     """A probabilistic model that supports get_observation_noise."""
 
     @abstractmethod
     def get_observation_noise(self) -> TensorType:
         """
         Return the variance of observation noise.
```

### Comparing `trieste-1.1.2/trieste/models/keras/__init__.py` & `trieste-1.2.0/trieste/models/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/models/keras/architectures.py` & `trieste-1.2.0/trieste/models/keras/architectures.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/models/keras/builders.py` & `trieste-1.2.0/trieste/models/keras/builders.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/models/keras/interface.py` & `trieste-1.2.0/trieste/models/keras/interface.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/models/keras/models.py` & `trieste-1.2.0/trieste/models/keras/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import tensorflow_probability as tfp
 import tensorflow_probability.python.distributions as tfd
 from tensorflow.python.keras.callbacks import Callback
 
 from ... import logging
 from ...data import Dataset
 from ...types import TensorType
+from ...utils import flatten_leading_dims
 from ..interfaces import HasTrajectorySampler, TrainableProbabilisticModel, TrajectorySampler
 from ..optimizer import KerasOptimizer
 from ..utils import write_summary_data_based_metrics
 from .architectures import KerasEnsemble, MultivariateNormalTriL
 from .interface import DeepEnsembleModel, KerasPredictor
 from .sampler import DeepEnsembleTrajectorySampler
 from .utils import negative_log_likelihood, sample_model_index, sample_with_replacement
@@ -131,15 +132,19 @@
             self.optimizer.metrics = ["mse"]
 
         model.model.compile(
             self.optimizer.optimizer,
             loss=[self.optimizer.loss] * model.ensemble_size,
             metrics=[self.optimizer.metrics] * model.ensemble_size,
         )
-        self.original_lr = self.optimizer.optimizer.lr.numpy()
+
+        if not isinstance(
+            self.optimizer.optimizer.lr, tf.keras.optimizers.schedules.LearningRateSchedule
+        ):
+            self.original_lr = self.optimizer.optimizer.lr.numpy()
         self._absolute_epochs = 0
         self._continuous_optimisation = continuous_optimisation
 
         self._model = model
         self._bootstrap = bootstrap
         self._diversify = diversify
 
@@ -245,26 +250,30 @@
         the nature of the approximations stated above the final layer should be a Gaussian
         distribution with `mean` and `variance` methods.
 
         :param query_points: The points at which to make predictions.
         :return: The predicted mean and variance of the observations at the specified
             ``query_points``.
         """
-        ensemble_distributions = self.ensemble_distributions(query_points)
+        # handle leading batch dimensions, while still allowing `Functional` to
+        # "allow (None,) and (None, 1) Tensors to be passed interchangeably"
+        input_dims = min(len(query_points.shape), len(self.model.input_shape[0]))
+        flat_x, unflatten = flatten_leading_dims(query_points, output_dims=input_dims)
+        ensemble_distributions = self.ensemble_distributions(flat_x)
         predicted_means = tf.math.reduce_mean(
             [dist.mean() for dist in ensemble_distributions], axis=0
         )
         predicted_vars = (
             tf.math.reduce_mean(
                 [dist.variance() + dist.mean() ** 2 for dist in ensemble_distributions], axis=0
             )
             - predicted_means**2
         )
 
-        return predicted_means, predicted_vars
+        return unflatten(predicted_means), unflatten(predicted_vars)
 
     def predict_ensemble(self, query_points: TensorType) -> tuple[TensorType, TensorType]:
         """
         Returns mean and variance at ``query_points`` for each member of the ensemble. First tensor
         is the mean and second is the variance, where each has shape [..., M, N, 1], where M is
         the ``ensemble_size``.
 
@@ -371,18 +380,22 @@
             y=y,
             **fit_args,
             initial_epoch=self._absolute_epochs,
         )
         if self._continuous_optimisation:
             self._absolute_epochs = self._absolute_epochs + len(history.history["loss"])
 
-        # Reset lr in case there was an lr schedule: a schedule will have change the learning rate,
-        # so that the next time we call `optimize` the starting learning rate would be different.
-        # Therefore, we make sure the learning rate is set back to its initial value.
-        self.optimizer.optimizer.lr.assign(self.original_lr)
+        # Reset lr in case there was an lr schedule: a schedule will have changed the learning
+        # rate, so that the next time we call `optimize` the starting learning rate would be
+        # different. Therefore, we make sure the learning rate is set back to its initial value.
+        # However, this is not needed for `LearningRateSchedule` instances.
+        if not isinstance(
+            self.optimizer.optimizer.lr, tf.keras.optimizers.schedules.LearningRateSchedule
+        ):
+            self.optimizer.optimizer.lr.assign(self.original_lr)
 
     def log(self, dataset: Optional[Dataset] = None) -> None:
         """
         Log model training information at a given optimization step to the Tensorboard.
         We log several summary statistics of losses and metrics given in ``fit_args`` to
         ``optimizer`` (final, difference between inital and final loss, min and max). We also log
         epoch statistics, but as histograms, rather than time series. We also log several training
```

### Comparing `trieste-1.1.2/trieste/models/keras/sampler.py` & `trieste-1.2.0/trieste/models/keras/sampler.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/models/keras/utils.py` & `trieste-1.2.0/trieste/models/keras/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/models/optimizer.py` & `trieste-1.2.0/trieste/models/optimizer.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 This module contains common optimizers based on :class:`~tf.optimizers.Optimizer` that can be used
 with models. Specific models can also sub-class these optimizers or implement their own, and should
 register their loss functions using a :func:`create_loss_function`.
 """
 
 from __future__ import annotations
 
+import copy
 from dataclasses import dataclass, field
 from functools import singledispatch
 from typing import Any, Callable, Iterable, Optional, Tuple, Union
 
 import scipy
 import tensorflow as tf
 import tensorflow_probability as tfp
@@ -146,14 +147,38 @@
         @jit(apply=self.compile)
         def train_fn() -> None:
             self.optimizer.minimize(loss_fn, variables, **self.minimize_args)
 
         for _ in range(self.max_iter):
             train_fn()
 
+    def __deepcopy__(self, memo: dict[int, object]) -> BatchOptimizer:
+        # workaround for https://github.com/tensorflow/tensorflow/issues/58973
+        # (keras optimizers not being deepcopyable in TF 2.11 and 2.12)
+        cls = self.__class__
+        result = cls.__new__(cls)
+        memo[id(self)] = result
+        for k, v in self.__dict__.items():
+            if (
+                k == "optimizer"
+                and isinstance(v, tf.keras.optimizers.Optimizer)
+                and hasattr(v, "_distribution_strategy")
+            ):
+                # avoid copying distribution strategy: reuse it instead
+                strategy = v._distribution_strategy
+                v._distribution_strategy = None
+                try:
+                    setattr(result, k, copy.deepcopy(v, memo))
+                finally:
+                    v._distribution_strategy = strategy
+                result.optimizer._distribution_strategy = strategy
+            else:
+                setattr(result, k, copy.deepcopy(v, memo))
+        return result
+
 
 @dataclass
 class KerasOptimizer:
     """Optimizer wrapper for training models implemented with Keras."""
 
     optimizer: tf.keras.optimizers.Optimizer
     """ The underlying optimizer to use for training the model. """
@@ -171,14 +196,34 @@
         ]
     ] = None
     """ Optional loss function for training the model. """
 
     metrics: Optional[list[tf.keras.metrics.Metric]] = None
     """ Optional metrics for monitoring the performance of the network. """
 
+    def __deepcopy__(self, memo: dict[int, object]) -> KerasOptimizer:
+        # workaround for https://github.com/tensorflow/tensorflow/issues/58973
+        # (keras optimizers not being deepcopyable in TF 2.11 and 2.12)
+        cls = self.__class__
+        result = cls.__new__(cls)
+        memo[id(self)] = result
+        for k, v in self.__dict__.items():
+            if k == "optimizer" and hasattr(v, "_distribution_strategy"):
+                # avoid copying distribution strategy: reuse it instead
+                strategy = v._distribution_strategy
+                v._distribution_strategy = None
+                try:
+                    setattr(result, k, copy.deepcopy(v, memo))
+                finally:
+                    v._distribution_strategy = strategy
+                result.optimizer._distribution_strategy = strategy
+            else:
+                setattr(result, k, copy.deepcopy(v, memo))
+        return result
+
 
 @singledispatch
 def create_loss_function(model: Any, dataset: TrainingData, compile: bool = False) -> LossClosure:
     """
     Generic function for building a loss function for a specified `model` and `dataset`.
     The implementations depends on the type of the model, which should use this function as a
     decorator together with its register method to make a model-specific loss function available.
```

### Comparing `trieste-1.1.2/trieste/models/utils.py` & `trieste-1.2.0/trieste/models/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
     :param prefix: The prefix to add to "accuracy" category of model summaries.
     """
     name = prefix + "accuracy"
     predict = model.predict(dataset.query_points)
 
     # basics
     logging.histogram(f"{name}/predict_mean", predict[0])
-    logging.scalar(f"{name}/predict_mean", tf.reduce_mean(predict[0]))
+    logging.scalar(f"{name}/predict_mean__mean", tf.reduce_mean(predict[0]))
     logging.histogram(f"{name}/predict_variance", predict[1])
-    logging.scalar(f"{name}/predict_variance", tf.reduce_mean(predict[1]))
+    logging.scalar(f"{name}/predict_variance__mean", tf.reduce_mean(predict[1]))
     logging.histogram(f"{name}/observations", dataset.observations)
     logging.scalar(f"{name}/observations_mean", tf.reduce_mean(dataset.observations))
     logging.scalar(f"{name}/observations_variance", tf.math.reduce_variance(dataset.observations))
 
     # accuracy metrics
     diffs = tf.cast(dataset.observations, predict[0].dtype) - predict[0]
     z_residuals = diffs / tf.math.sqrt(predict[1])
```

### Comparing `trieste-1.1.2/trieste/objectives/__init__.py` & `trieste-1.2.0/trieste/objectives/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from .single_objectives import (
     Ackley5,
     Branin,
     ConstrainedScaledBranin,
     GramacyLee,
     Hartmann3,
     Hartmann6,
+    Levy8,
     LogarithmicGoldsteinPrice,
     Michalewicz2,
     Michalewicz5,
     Michalewicz10,
     ObjectiveTestProblem,
     Rosenbrock4,
     ScaledBranin,
```

### Comparing `trieste-1.1.2/trieste/objectives/multi_objectives.py` & `trieste-1.2.0/trieste/objectives/multi_objectives.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/objectives/multifidelity_objectives.py` & `trieste-1.2.0/trieste/objectives/multifidelity_objectives.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/objectives/single_objectives.py` & `trieste-1.2.0/trieste/objectives/single_objectives.py`

 * *Files 7% similar despite different names*

```diff
@@ -326,39 +326,101 @@
 )
 """The Shekel test function over :math:`[0, 1]^4`. This function has ten local
 minima and a single global minimum. See https://www.sfu.ca/~ssurjano/shekel.html for details.
 Note that we rescale the original problem, which is typically defined
 over `[0, 10]^4`."""
 
 
-def rosenbrock_4(x: TensorType) -> TensorType:
+def levy(x: TensorType, d: int) -> TensorType:
     """
-    The Rosenbrock function, rescaled to have zero mean and unit variance over :math:`[0, 1]^4. See
-    :cite:`Picheny2013` for details.
-    This function (also known as the Banana function) is unimodal, however the minima
-    lies in a narrow valley.
+    The Levy test function over :math:`[0, 1]^d`. This function has many local
+    minima and a single global minimum. See https://www.sfu.ca/~ssurjano/levy.html for details.
+    Note that we rescale the original problem, which is typically defined
+    over `[-10, 10]^d`, to be defined over a unit hypercube :math:`[0, 1]^d`.
 
-    :param x: The points at which to evaluate the function, with shape [..., 4].
+    :param x: The points at which to evaluate the function, with shape [..., d].
+    :param d: The dimension of the function.
+    :return: The function values at ``x``, with shape [..., 1].
+    :raise ValueError (or InvalidArgumentError): If ``x`` has an invalid shape.
+    """
+    tf.debugging.assert_greater_equal(d, 1)
+    tf.debugging.assert_shapes([(x, (..., d))])
+
+    w: TensorType = 1 + ((x * 20.0 - 10) - 1) / 4
+    term1 = tf.pow(tf.sin(pi * w[..., 0:1]), 2)
+    term3 = (w[..., -1:] - 1) ** 2 * (1 + tf.pow(tf.sin(2 * pi * w[..., -1:]), 2))
+    wi = w[..., 0:-1]
+    wi_sum = tf.reduce_sum(
+        (wi - 1) ** 2 * (1 + 10 * tf.pow(tf.sin(pi * wi + 1), 2)), axis=-1, keepdims=True
+    )
+    return term1 + wi_sum + term3
+
+
+def levy_8(x: TensorType) -> TensorType:
+    """
+    Convenience function for the 8-dimensional :func:`levy` function, with output
+    normalised to unit interval
+
+    :param x: The points at which to evaluate the function, with shape [..., 8].
+    :return: The function values at ``x``, with shape [..., 1].
+    """
+    return levy(x, d=8) / 450.0
+
+
+Levy8 = SingleObjectiveTestProblem(
+    name="Levy 8",
+    objective=levy_8,
+    search_space=Box([0.0], [1.0]) ** 8,
+    minimizers=tf.constant([[11 / 20] * 8], tf.float64),
+    minimum=tf.constant([0], tf.float64),
+)
+"""Convenience function for the 8-dimensional :func:`levy` function.
+Taken from https://www.sfu.ca/~ssurjano/levy.html"""
+
+
+def rosenbrock(x: TensorType, d: int) -> TensorType:
+    """
+    The Rosenbrock function, also known as the Banana function, is a unimodal function,
+    however the minima lies in a narrow valley. Even though this valley is
+    easy to find, convergence to the minimum is difficult. See
+    https://www.sfu.ca/~ssurjano/rosen.html for details. Inputs are rescaled to
+    be defined over a unit hypercube :math:`[0, 1]^d`.
+
+    :param x: The points at which to evaluate the function, with shape [..., d].
+    :param d: The dimension of the function.
     :return: The function values at ``x``, with shape [..., 1].
     :raise ValueError (or InvalidArgumentError): If ``x`` has an invalid shape.
     """
-    tf.debugging.assert_shapes([(x, (..., 4))])
+    tf.debugging.assert_greater_equal(d, 1)
+    tf.debugging.assert_shapes([(x, (..., d))])
 
     y: TensorType = x * 15.0 - 5
     unscaled_function = tf.reduce_sum(
         (100.0 * (y[..., 1:] - y[..., :-1]) ** 2 + (1 - y[..., :-1]) ** 2), axis=-1, keepdims=True
     )
-    return (unscaled_function - 3.827 * 1e5) / (3.755 * 1e5)
+    return unscaled_function
+
+
+def rosenbrock_4(x: TensorType) -> TensorType:
+    """
+    Convenience function for the 4-dimensional :func:`rosenbrock` function with steepness 10.
+    It is rescaled to have zero mean and unit variance over :math:`[0, 1]^4. See
+    :cite:`Picheny2013` for details.
+
+    :param x: The points at which to evaluate the function, with shape [..., 4].
+    :return: The function values at ``x``, with shape [..., 1].
+    """
+    return (rosenbrock(x, d=4) - 3.827 * 1e5) / (3.755 * 1e5)
 
 
 Rosenbrock4 = SingleObjectiveTestProblem(
     name="Rosenbrock 4",
     objective=rosenbrock_4,
     search_space=Box([0.0], [1.0]) ** 4,
-    minimizers=tf.constant([[0.4, 0.4, 0.4, 0.4]], tf.float64),
+    minimizers=tf.constant([[0.4] * 4], tf.float64),
     minimum=tf.constant([-1.01917], tf.float64),
 )
 """The Rosenbrock function, rescaled to have zero mean and unit variance over :math:`[0, 1]^4. See
 :cite:`Picheny2013` for details.
 This function (also known as the Banana function) is unimodal, however the minima
 lies in a narrow valley."""
 
@@ -451,14 +513,15 @@
 def michalewicz(x: TensorType, d: int = 2, m: int = 10) -> TensorType:
     """
     The Michalewicz function over :math:`[0, \\pi]` for all i=1,...,d. Dimensionality is determined
     by the parameter ``d`` and it features steep ridges and drops. It has :math:`d!` local minima,
     and it is multimodal. The parameter ``m`` defines the steepness of they valleys and ridges; a
     larger ``m`` leads to a more difficult search. The recommended value of ``m`` is 10. See
     https://www.sfu.ca/~ssurjano/egg.html for details.
+
     :param x: The points at which to evaluate the function, with shape [..., d].
     :param d: The dimension of the function.
     :param m: The steepness of the valleys/ridges.
     :return: The function values at ``x``, with shape [..., 1].
     :raise ValueError (or InvalidArgumentError): If ``x`` has an invalid shape.
     """
     tf.debugging.assert_greater_equal(d, 1)
```

### Comparing `trieste-1.1.2/trieste/objectives/utils.py` & `trieste-1.2.0/trieste/objectives/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/observer.py` & `trieste-1.2.0/trieste/observer.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/space.py` & `trieste-1.2.0/trieste/space.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/types.py` & `trieste-1.2.0/trieste/types.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/utils/__init__.py` & `trieste-1.2.0/trieste/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste/version.py` & `trieste-1.2.0/trieste/version.py`

 * *Files identical despite different names*

### Comparing `trieste-1.1.2/trieste.egg-info/PKG-INFO` & `trieste-1.2.0/trieste.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trieste
-Version: 1.1.2
+Version: 1.2.0
 Summary: A Bayesian optimization research toolbox built on TensorFlow
 Home-page: https://github.com/secondmind-labs/trieste
 Author: The Trieste contributors
 Author-email: labs@secondmind.ai
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `trieste-1.1.2/trieste.egg-info/SOURCES.txt` & `trieste-1.2.0/trieste.egg-info/SOURCES.txt`

 * *Files identical despite different names*

