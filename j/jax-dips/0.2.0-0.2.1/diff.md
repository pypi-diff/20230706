# Comparing `tmp/jax-dips-0.2.0.tar.gz` & `tmp/jax-dips-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-dips-0.2.0.tar", last modified: Thu Jul  6 01:16:30 2023, max compression
+gzip compressed data, was "jax-dips-0.2.1.tar", last modified: Thu Jul  6 02:24:39 2023, max compression
```

## Comparing `jax-dips-0.2.0.tar` & `jax-dips-0.2.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.500856 jax-dips-0.2.0/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    26588 2023-07-06 00:20:45.000000 jax-dips-0.2.0/LICENSE.md
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     8867 2023-07-06 01:16:30.500856 jax-dips-0.2.0/PKG-INFO
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     7682 2023-07-06 00:25:44.000000 jax-dips-0.2.0/README.md
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.496856 jax-dips-0.2.0/examples/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 00:18:52.000000 jax-dips-0.2.0/examples/__init__.py
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.496856 jax-dips-0.2.0/examples/stars/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 00:18:52.000000 jax-dips-0.2.0/examples/stars/__init__.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     7157 2023-07-06 00:22:40.000000 jax-dips-0.2.0/examples/stars/_solve_single_star.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     8780 2023-07-06 00:22:40.000000 jax-dips-0.2.0/examples/stars/_starbox.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    10881 2023-07-06 00:22:40.000000 jax-dips-0.2.0/examples/stars/solve_stars.py
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.496856 jax-dips-0.2.0/jax_dips/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)       22 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/__init__.py
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.496856 jax-dips-0.2.0/jax_dips/_experimental/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/_experimental/__init__.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     3244 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/_experimental/compositions.py
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.496856 jax-dips-0.2.0/jax_dips/_jaxmd_modules/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/_jaxmd_modules/__init__.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     2379 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/_jaxmd_modules/dataclasses.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     4620 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/_jaxmd_modules/energy.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    23628 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/_jaxmd_modules/partition.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     2571 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/_jaxmd_modules/quantity.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     7086 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/_jaxmd_modules/smap.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    13574 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/_jaxmd_modules/space.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     1863 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/_jaxmd_modules/util.py
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.496856 jax-dips-0.2.0/jax_dips/data/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/data/__init__.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    13349 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/data/data_management.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     3452 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/data/data_stream.py
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.496856 jax-dips-0.2.0/jax_dips/domain/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/domain/__init__.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    40392 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/domain/interpolate.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     5009 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/domain/mesh.py
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.500856 jax-dips-0.2.0/jax_dips/geometry/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/geometry/__init__.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    39302 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/geometry/geometric_integrations.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    37950 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/geometry/geometric_integrations_per_point.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     9824 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/geometry/level_set.py
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.500856 jax-dips-0.2.0/jax_dips/nn/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/nn/__init__.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     4493 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/nn/nn_solution_model.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     6619 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/nn/nn_solution_trainer.py
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.500856 jax-dips-0.2.0/jax_dips/solvers/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/solvers/__init__.py
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.500856 jax-dips-0.2.0/jax_dips/solvers/advection/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/solvers/advection/__init__.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    11932 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/solvers/advection/solver_advection.py
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.500856 jax-dips-0.2.0/jax_dips/solvers/free_boundary/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/solvers/free_boundary/__init__.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    29515 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/solvers/free_boundary/solver_poisson_advection.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    23584 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/solvers/free_boundary/trainer_poisson_advection.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     2479 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/solvers/optimizers.py
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.500856 jax-dips-0.2.0/jax_dips/solvers/poisson/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/solvers/poisson/__init__.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    23239 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/solvers/poisson/discretization.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     9023 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/solvers/poisson/nbm.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    24448 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/solvers/poisson/trainer.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     2544 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/solvers/simulation_states.py
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.500856 jax-dips-0.2.0/jax_dips/utils/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/utils/__init__.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     2663 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/utils/chunking.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     2293 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/utils/conversions.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     2309 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/utils/inspect.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     3870 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/utils/io.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     6960 2023-07-06 00:22:40.000000 jax-dips-0.2.0/jax_dips/utils/visualization.py
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.496856 jax-dips-0.2.0/jax_dips.egg-info/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     8867 2023-07-06 01:16:30.000000 jax-dips-0.2.0/jax_dips.egg-info/PKG-INFO
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     2022 2023-07-06 01:16:30.000000 jax-dips-0.2.0/jax_dips.egg-info/SOURCES.txt
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        1 2023-07-06 01:16:30.000000 jax-dips-0.2.0/jax_dips.egg-info/dependency_links.txt
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        1 2023-07-06 01:08:39.000000 jax-dips-0.2.0/jax_dips.egg-info/not-zip-safe
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)      385 2023-07-06 01:16:30.000000 jax-dips-0.2.0/jax_dips.egg-info/requires.txt
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)       24 2023-07-06 01:16:30.000000 jax-dips-0.2.0/jax_dips.egg-info/top_level.txt
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)       38 2023-07-06 01:16:30.500856 jax-dips-0.2.0/setup.cfg
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     1773 2023-07-06 01:16:12.000000 jax-dips-0.2.0/setup.py
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.500856 jax-dips-0.2.0/tests/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 00:18:52.000000 jax-dips-0.2.0/tests/__init__.py
-drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:16:30.500856 jax-dips-0.2.0/tests/confs/
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 00:22:40.000000 jax-dips-0.2.0/tests/confs/__init__.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    12910 2023-07-06 00:36:32.000000 jax-dips-0.2.0/tests/confs/experiment_configs.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     6430 2023-07-06 00:22:40.000000 jax-dips-0.2.0/tests/test_advection.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     1771 2023-07-06 00:22:40.000000 jax-dips-0.2.0/tests/test_amr.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     8608 2023-07-06 00:34:12.000000 jax-dips-0.2.0/tests/test_geometric_integrations.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     9955 2023-07-06 00:22:40.000000 jax-dips-0.2.0/tests/test_poisson.py
--rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     6397 2023-07-06 00:35:03.000000 jax-dips-0.2.0/tests/test_reinitialization.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    26588 2023-07-06 01:30:00.000000 jax-dips-0.2.1/LICENSE.md
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     9396 2023-07-06 02:24:39.618475 jax-dips-0.2.1/PKG-INFO
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     8211 2023-07-06 02:09:51.000000 jax-dips-0.2.1/README.md
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/examples/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:30:00.000000 jax-dips-0.2.1/examples/__init__.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/examples/stars/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:30:00.000000 jax-dips-0.2.1/examples/stars/__init__.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     7157 2023-07-06 01:30:00.000000 jax-dips-0.2.1/examples/stars/_solve_single_star.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     8780 2023-07-06 01:30:00.000000 jax-dips-0.2.1/examples/stars/_starbox.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    10881 2023-07-06 01:30:00.000000 jax-dips-0.2.1/examples/stars/solve_stars.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/jax_dips/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)       22 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/__init__.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/jax_dips/_experimental/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/_experimental/__init__.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     3244 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/_experimental/compositions.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/jax_dips/_jaxmd_modules/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/_jaxmd_modules/__init__.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     2379 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/_jaxmd_modules/dataclasses.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     4620 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/_jaxmd_modules/energy.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    23628 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/_jaxmd_modules/partition.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     2571 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/_jaxmd_modules/quantity.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     7086 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/_jaxmd_modules/smap.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    13574 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/_jaxmd_modules/space.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     1863 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/_jaxmd_modules/util.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/jax_dips/data/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/data/__init__.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    13349 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/data/data_management.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     3452 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/data/data_stream.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/jax_dips/domain/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/domain/__init__.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    40392 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/domain/interpolate.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     5009 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/domain/mesh.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/jax_dips/geometry/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/geometry/__init__.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    39302 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/geometry/geometric_integrations.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    37950 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/geometry/geometric_integrations_per_point.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     9824 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/geometry/level_set.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/jax_dips/nn/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/nn/__init__.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     4493 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/nn/nn_solution_model.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     6619 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/nn/nn_solution_trainer.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/jax_dips/solvers/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/solvers/__init__.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/jax_dips/solvers/advection/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/solvers/advection/__init__.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    11932 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/solvers/advection/solver_advection.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/jax_dips/solvers/free_boundary/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/solvers/free_boundary/__init__.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    29515 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/solvers/free_boundary/solver_poisson_advection.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    23584 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/solvers/free_boundary/trainer_poisson_advection.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     2479 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/solvers/optimizers.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/jax_dips/solvers/poisson/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/solvers/poisson/__init__.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    23239 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/solvers/poisson/discretization.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     9023 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/solvers/poisson/nbm.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    24448 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/solvers/poisson/trainer.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     2544 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/solvers/simulation_states.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/jax_dips/utils/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/utils/__init__.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     2663 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/utils/chunking.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     2293 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/utils/conversions.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     2309 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/utils/inspect.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     3870 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/utils/io.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     6960 2023-07-06 01:30:00.000000 jax-dips-0.2.1/jax_dips/utils/visualization.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/jax_dips.egg-info/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     9396 2023-07-06 02:24:39.000000 jax-dips-0.2.1/jax_dips.egg-info/PKG-INFO
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     2022 2023-07-06 02:24:39.000000 jax-dips-0.2.1/jax_dips.egg-info/SOURCES.txt
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        1 2023-07-06 02:24:39.000000 jax-dips-0.2.1/jax_dips.egg-info/dependency_links.txt
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        1 2023-07-06 02:21:14.000000 jax-dips-0.2.1/jax_dips.egg-info/not-zip-safe
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)      424 2023-07-06 02:24:39.000000 jax-dips-0.2.1/jax_dips.egg-info/requires.txt
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)       24 2023-07-06 02:24:39.000000 jax-dips-0.2.1/jax_dips.egg-info/top_level.txt
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)       38 2023-07-06 02:24:39.618475 jax-dips-0.2.1/setup.cfg
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     1863 2023-07-06 02:24:32.000000 jax-dips-0.2.1/setup.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/tests/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:30:00.000000 jax-dips-0.2.1/tests/__init__.py
+drwxrwxr-x   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 02:24:39.618475 jax-dips-0.2.1/tests/confs/
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)        0 2023-07-06 01:30:00.000000 jax-dips-0.2.1/tests/confs/__init__.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)    12910 2023-07-06 01:30:00.000000 jax-dips-0.2.1/tests/confs/experiment_configs.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     6430 2023-07-06 01:30:00.000000 jax-dips-0.2.1/tests/test_advection.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     1771 2023-07-06 01:30:00.000000 jax-dips-0.2.1/tests/test_amr.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     8608 2023-07-06 01:30:00.000000 jax-dips-0.2.1/tests/test_geometric_integrations.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     9955 2023-07-06 01:30:00.000000 jax-dips-0.2.1/tests/test_poisson.py
+-rw-rw-r--   0 pmistani  (1000) pmistani  (1000)     6397 2023-07-06 01:30:00.000000 jax-dips-0.2.1/tests/test_reinitialization.py
```

### Comparing `jax-dips-0.2.0/LICENSE.md` & `jax-dips-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/PKG-INFO` & `jax-dips-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-dips
-Version: 0.2.0
+Version: 0.2.1
 Summary: Differentiable 3D interfacial PDE solvers written in JAX using the Neural Bootstrapping Method.
 Home-page: https://github.com/JAX-DIPS/JAX-DIPS
 Author: Pouria Mistani & Samira Pakravan
 Author-email: p.a.mistani@gmail.com
 Maintainer: Pouria Mistani & Samira Pakravan
 Maintainer-email: p.a.mistani@gmail.com
 License: GNU LESSER GENERAL PUBLIC LICENSE v2.1
@@ -47,35 +47,48 @@
 
 # Testing
 Do `pytest tests/test_*.py` of each of the available tests from the parent directory:
 - `test_advection`: a sphere is rotated 360 degrees around the box to replicate initial configuration. The L2 error in level-set function should be less than 1e-4 to pass. The advection is performed using semi-Lagrangian scheme with Sussman reinitialization.
 - `test_reinitialization`: starting from a sphere level-set function with -1 inside sphere and +1 outside, we repeatedly perform Sussman reinitialization until the signed-distance property of the level-set is achieved. Center of the box should have level-set value equal to radius of the sphere, and corner of the box should be at a pre-specified distance to pass.
 - `test_geometric_integrations`: integrating surface area of a sphere along with its volume. Small differences with associated theoretical values are expected to pass.
 - `test_poisson`: tests for both the pointwise and the grid-based Poisson solvers over a star and a sphere interfaces. Note that in the current implementation the grid-based solver does not support batching and is therefore faster. Fixing this issue will be done in the future versions.
-# Pre-requisites
 
-## Nvidia Driver
+# Installation
+To install the latest released version from PyPI do ```pip install jax-dips```.
 
-```
-apt install $(nvidia-detector)
-```
 
-## Docker Engine
-
-Please refer https://docs.docker.com/engine/install/ubuntu/
+# Development & Usage Environment
 
-## nvidia-docker2
+## 1. Virtual Environment
+Create a virtual environment by running the following command
+```
+./create_virtualenv.sh
+```
+and the ```env_jax_dips``` virtual environment will be created. Then you can launch into this environment by 
+```source env_jax_dips/bin/activate```. After you are done, ```deactivate```.
 
-Please refer https://nvidia.github.io/nvidia-docker/ to setup apt repo
+## 2. Docker
 
-apt-get install nvidia-docker2
+### Prerequisites
+First you will need to install the nvidia driver and docker engines:
+- Nvidia Driver
+  ```
+  apt install $(nvidia-detector)
+  ```
 
+- Docker Engine
+  Please refer https://docs.docker.com/engine/install/ubuntu/
 
-# Development & Usage Environment
+- nvidia-docker2
+  Please refer https://nvidia.github.io/nvidia-docker/ to setup apt repo
+  ```
+  apt-get install nvidia-docker2
+  ```
 
+### Instructions
 Docker images provide an isolated and consistent runtime environment, ensuring that the application behaves the same regardless of the host system. We recommend using the docker image provided here as it is fully loaded with libraries for datacenter scale simulatiopns and optimized for NVIDIA GPUs. For a full list of the supported software and specific versions that come packaged with this container image see the Frameworks Support Matrix https://docs.nvidia.com/deeplearning/frameworks/support-matrix/index.html
 
 
 To personalize your development environment you need to set up a `.env` file that contains
 ```
 IMAGE_NAME=docker.io/pourion/jax_dips:latest       # default docker image available for download! Change this if you want to build new docker images and push to your preferred docker registry
 DATA_PATH=/data/                                   # default data path inside your docker container, will mirror your DATA_MOUNT_PATH directory
@@ -85,30 +98,30 @@
 REGISTRY=<your-preferred-registry-name>            # (optional) choices are docker.io (default), nvcr.io, ghcr.io, etc.
 REGISTRY_USER=<your-registry-username>             # (optional) your username to connect to docker registry
 REGISTRY_ACCESS_TOKEN=<your-registry-access-token> # (optional) your access token to connect to docker registry
 WANDB_API_KEY=NotSpecified                         # (optional) your API key to connect to Weights and Biases service
 JUPYTER_PORT=8888                                  # (optional) port to connect to jupyter server
 ```
 
-## Pull development container
+#### Pull development container
 Currently the latest docker image available on Docker Hub is available at `docker.io/pourion/jax_dips`. Instead of building the container, you can only pull the latest docker image by running 
 
 ```
 ./launch.sh pull
 ```
 which pulls from docker hub; i.e., equivalent to ```$ docker pull pourion/jax_dips:latest```.
-## Build development container
+#### Build development container
 Alternatively you can build the container by running the following command
 ```
 ./launch.sh build
 ```
 In case you want to add additional libraries to your container this is the recommended way.
 
 
-## Start developement container
+#### Start developement container
 This will create a container and places the user in the container with source code mounted. 
 
 ```
 ./launch.sh dev
 ```
 Additionally, you can run the container in background without having your terminal jump into the container. This can be done by passing the `-d` flag for daemon:
 ```
@@ -117,15 +130,15 @@
 
 You can always attach your teminal to the running `jax_dips` container by
 
 ```
 ./launch.sh attach
 ```
 
-### Development in VS Code 
+#### Development in VS Code 
 Once the container is created and is running on your machine, user can attach to this container from VS code; i.e., you need to install Microsoft's `Dev Containers` extension in your VS Code, then `Ctrl+Shift+P` and choose `Dev Containers: Attach to Running Container...`, then choose the `jax_dips` container from the list of running containers on your machine.
 
 ## Cite JAX-DIPS
 If you use JAX-DIPS in your research please use the following citations:
 
 ```bibtex
 @article{mistani2022jax,
```

### Comparing `jax-dips-0.2.0/README.md` & `jax-dips-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,35 +21,48 @@
 
 # Testing
 Do `pytest tests/test_*.py` of each of the available tests from the parent directory:
 - `test_advection`: a sphere is rotated 360 degrees around the box to replicate initial configuration. The L2 error in level-set function should be less than 1e-4 to pass. The advection is performed using semi-Lagrangian scheme with Sussman reinitialization.
 - `test_reinitialization`: starting from a sphere level-set function with -1 inside sphere and +1 outside, we repeatedly perform Sussman reinitialization until the signed-distance property of the level-set is achieved. Center of the box should have level-set value equal to radius of the sphere, and corner of the box should be at a pre-specified distance to pass.
 - `test_geometric_integrations`: integrating surface area of a sphere along with its volume. Small differences with associated theoretical values are expected to pass.
 - `test_poisson`: tests for both the pointwise and the grid-based Poisson solvers over a star and a sphere interfaces. Note that in the current implementation the grid-based solver does not support batching and is therefore faster. Fixing this issue will be done in the future versions.
-# Pre-requisites
 
-## Nvidia Driver
+# Installation
+To install the latest released version from PyPI do ```pip install jax-dips```.
 
-```
-apt install $(nvidia-detector)
-```
 
-## Docker Engine
-
-Please refer https://docs.docker.com/engine/install/ubuntu/
+# Development & Usage Environment
 
-## nvidia-docker2
+## 1. Virtual Environment
+Create a virtual environment by running the following command
+```
+./create_virtualenv.sh
+```
+and the ```env_jax_dips``` virtual environment will be created. Then you can launch into this environment by 
+```source env_jax_dips/bin/activate```. After you are done, ```deactivate```.
 
-Please refer https://nvidia.github.io/nvidia-docker/ to setup apt repo
+## 2. Docker
 
-apt-get install nvidia-docker2
+### Prerequisites
+First you will need to install the nvidia driver and docker engines:
+- Nvidia Driver
+  ```
+  apt install $(nvidia-detector)
+  ```
 
+- Docker Engine
+  Please refer https://docs.docker.com/engine/install/ubuntu/
 
-# Development & Usage Environment
+- nvidia-docker2
+  Please refer https://nvidia.github.io/nvidia-docker/ to setup apt repo
+  ```
+  apt-get install nvidia-docker2
+  ```
 
+### Instructions
 Docker images provide an isolated and consistent runtime environment, ensuring that the application behaves the same regardless of the host system. We recommend using the docker image provided here as it is fully loaded with libraries for datacenter scale simulatiopns and optimized for NVIDIA GPUs. For a full list of the supported software and specific versions that come packaged with this container image see the Frameworks Support Matrix https://docs.nvidia.com/deeplearning/frameworks/support-matrix/index.html
 
 
 To personalize your development environment you need to set up a `.env` file that contains
 ```
 IMAGE_NAME=docker.io/pourion/jax_dips:latest       # default docker image available for download! Change this if you want to build new docker images and push to your preferred docker registry
 DATA_PATH=/data/                                   # default data path inside your docker container, will mirror your DATA_MOUNT_PATH directory
@@ -59,30 +72,30 @@
 REGISTRY=<your-preferred-registry-name>            # (optional) choices are docker.io (default), nvcr.io, ghcr.io, etc.
 REGISTRY_USER=<your-registry-username>             # (optional) your username to connect to docker registry
 REGISTRY_ACCESS_TOKEN=<your-registry-access-token> # (optional) your access token to connect to docker registry
 WANDB_API_KEY=NotSpecified                         # (optional) your API key to connect to Weights and Biases service
 JUPYTER_PORT=8888                                  # (optional) port to connect to jupyter server
 ```
 
-## Pull development container
+#### Pull development container
 Currently the latest docker image available on Docker Hub is available at `docker.io/pourion/jax_dips`. Instead of building the container, you can only pull the latest docker image by running 
 
 ```
 ./launch.sh pull
 ```
 which pulls from docker hub; i.e., equivalent to ```$ docker pull pourion/jax_dips:latest```.
-## Build development container
+#### Build development container
 Alternatively you can build the container by running the following command
 ```
 ./launch.sh build
 ```
 In case you want to add additional libraries to your container this is the recommended way.
 
 
-## Start developement container
+#### Start developement container
 This will create a container and places the user in the container with source code mounted. 
 
 ```
 ./launch.sh dev
 ```
 Additionally, you can run the container in background without having your terminal jump into the container. This can be done by passing the `-d` flag for daemon:
 ```
@@ -91,15 +104,15 @@
 
 You can always attach your teminal to the running `jax_dips` container by
 
 ```
 ./launch.sh attach
 ```
 
-### Development in VS Code 
+#### Development in VS Code 
 Once the container is created and is running on your machine, user can attach to this container from VS code; i.e., you need to install Microsoft's `Dev Containers` extension in your VS Code, then `Ctrl+Shift+P` and choose `Dev Containers: Attach to Running Container...`, then choose the `jax_dips` container from the list of running containers on your machine.
 
 ## Cite JAX-DIPS
 If you use JAX-DIPS in your research please use the following citations:
 
 ```bibtex
 @article{mistani2022jax,
```

### Comparing `jax-dips-0.2.0/examples/stars/_solve_single_star.py` & `jax-dips-0.2.1/examples/stars/_solve_single_star.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/examples/stars/_starbox.py` & `jax-dips-0.2.1/examples/stars/_starbox.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/examples/stars/solve_stars.py` & `jax-dips-0.2.1/examples/stars/solve_stars.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/_experimental/compositions.py` & `jax-dips-0.2.1/jax_dips/_experimental/compositions.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/_jaxmd_modules/dataclasses.py` & `jax-dips-0.2.1/jax_dips/_jaxmd_modules/dataclasses.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/_jaxmd_modules/energy.py` & `jax-dips-0.2.1/jax_dips/_jaxmd_modules/energy.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/_jaxmd_modules/partition.py` & `jax-dips-0.2.1/jax_dips/_jaxmd_modules/partition.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/_jaxmd_modules/quantity.py` & `jax-dips-0.2.1/jax_dips/_jaxmd_modules/quantity.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/_jaxmd_modules/smap.py` & `jax-dips-0.2.1/jax_dips/_jaxmd_modules/smap.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/_jaxmd_modules/space.py` & `jax-dips-0.2.1/jax_dips/_jaxmd_modules/space.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/_jaxmd_modules/util.py` & `jax-dips-0.2.1/jax_dips/_jaxmd_modules/util.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/data/data_management.py` & `jax-dips-0.2.1/jax_dips/data/data_management.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/data/data_stream.py` & `jax-dips-0.2.1/jax_dips/data/data_stream.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/domain/interpolate.py` & `jax-dips-0.2.1/jax_dips/domain/interpolate.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/domain/mesh.py` & `jax-dips-0.2.1/jax_dips/domain/mesh.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/geometry/geometric_integrations.py` & `jax-dips-0.2.1/jax_dips/geometry/geometric_integrations.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/geometry/geometric_integrations_per_point.py` & `jax-dips-0.2.1/jax_dips/geometry/geometric_integrations_per_point.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/geometry/level_set.py` & `jax-dips-0.2.1/jax_dips/geometry/level_set.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/nn/nn_solution_model.py` & `jax-dips-0.2.1/jax_dips/nn/nn_solution_model.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/nn/nn_solution_trainer.py` & `jax-dips-0.2.1/jax_dips/nn/nn_solution_trainer.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/solvers/advection/solver_advection.py` & `jax-dips-0.2.1/jax_dips/solvers/advection/solver_advection.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/solvers/free_boundary/solver_poisson_advection.py` & `jax-dips-0.2.1/jax_dips/solvers/free_boundary/solver_poisson_advection.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/solvers/free_boundary/trainer_poisson_advection.py` & `jax-dips-0.2.1/jax_dips/solvers/free_boundary/trainer_poisson_advection.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/solvers/optimizers.py` & `jax-dips-0.2.1/jax_dips/solvers/optimizers.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/solvers/poisson/discretization.py` & `jax-dips-0.2.1/jax_dips/solvers/poisson/discretization.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/solvers/poisson/nbm.py` & `jax-dips-0.2.1/jax_dips/solvers/poisson/nbm.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/solvers/poisson/trainer.py` & `jax-dips-0.2.1/jax_dips/solvers/poisson/trainer.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/solvers/simulation_states.py` & `jax-dips-0.2.1/jax_dips/solvers/simulation_states.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/utils/chunking.py` & `jax-dips-0.2.1/jax_dips/utils/chunking.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/utils/conversions.py` & `jax-dips-0.2.1/jax_dips/utils/conversions.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/utils/inspect.py` & `jax-dips-0.2.1/jax_dips/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/utils/io.py` & `jax-dips-0.2.1/jax_dips/utils/io.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips/utils/visualization.py` & `jax-dips-0.2.1/jax_dips/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/jax_dips.egg-info/PKG-INFO` & `jax-dips-0.2.1/jax_dips.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-dips
-Version: 0.2.0
+Version: 0.2.1
 Summary: Differentiable 3D interfacial PDE solvers written in JAX using the Neural Bootstrapping Method.
 Home-page: https://github.com/JAX-DIPS/JAX-DIPS
 Author: Pouria Mistani & Samira Pakravan
 Author-email: p.a.mistani@gmail.com
 Maintainer: Pouria Mistani & Samira Pakravan
 Maintainer-email: p.a.mistani@gmail.com
 License: GNU LESSER GENERAL PUBLIC LICENSE v2.1
@@ -47,35 +47,48 @@
 
 # Testing
 Do `pytest tests/test_*.py` of each of the available tests from the parent directory:
 - `test_advection`: a sphere is rotated 360 degrees around the box to replicate initial configuration. The L2 error in level-set function should be less than 1e-4 to pass. The advection is performed using semi-Lagrangian scheme with Sussman reinitialization.
 - `test_reinitialization`: starting from a sphere level-set function with -1 inside sphere and +1 outside, we repeatedly perform Sussman reinitialization until the signed-distance property of the level-set is achieved. Center of the box should have level-set value equal to radius of the sphere, and corner of the box should be at a pre-specified distance to pass.
 - `test_geometric_integrations`: integrating surface area of a sphere along with its volume. Small differences with associated theoretical values are expected to pass.
 - `test_poisson`: tests for both the pointwise and the grid-based Poisson solvers over a star and a sphere interfaces. Note that in the current implementation the grid-based solver does not support batching and is therefore faster. Fixing this issue will be done in the future versions.
-# Pre-requisites
 
-## Nvidia Driver
+# Installation
+To install the latest released version from PyPI do ```pip install jax-dips```.
 
-```
-apt install $(nvidia-detector)
-```
 
-## Docker Engine
-
-Please refer https://docs.docker.com/engine/install/ubuntu/
+# Development & Usage Environment
 
-## nvidia-docker2
+## 1. Virtual Environment
+Create a virtual environment by running the following command
+```
+./create_virtualenv.sh
+```
+and the ```env_jax_dips``` virtual environment will be created. Then you can launch into this environment by 
+```source env_jax_dips/bin/activate```. After you are done, ```deactivate```.
 
-Please refer https://nvidia.github.io/nvidia-docker/ to setup apt repo
+## 2. Docker
 
-apt-get install nvidia-docker2
+### Prerequisites
+First you will need to install the nvidia driver and docker engines:
+- Nvidia Driver
+  ```
+  apt install $(nvidia-detector)
+  ```
 
+- Docker Engine
+  Please refer https://docs.docker.com/engine/install/ubuntu/
 
-# Development & Usage Environment
+- nvidia-docker2
+  Please refer https://nvidia.github.io/nvidia-docker/ to setup apt repo
+  ```
+  apt-get install nvidia-docker2
+  ```
 
+### Instructions
 Docker images provide an isolated and consistent runtime environment, ensuring that the application behaves the same regardless of the host system. We recommend using the docker image provided here as it is fully loaded with libraries for datacenter scale simulatiopns and optimized for NVIDIA GPUs. For a full list of the supported software and specific versions that come packaged with this container image see the Frameworks Support Matrix https://docs.nvidia.com/deeplearning/frameworks/support-matrix/index.html
 
 
 To personalize your development environment you need to set up a `.env` file that contains
 ```
 IMAGE_NAME=docker.io/pourion/jax_dips:latest       # default docker image available for download! Change this if you want to build new docker images and push to your preferred docker registry
 DATA_PATH=/data/                                   # default data path inside your docker container, will mirror your DATA_MOUNT_PATH directory
@@ -85,30 +98,30 @@
 REGISTRY=<your-preferred-registry-name>            # (optional) choices are docker.io (default), nvcr.io, ghcr.io, etc.
 REGISTRY_USER=<your-registry-username>             # (optional) your username to connect to docker registry
 REGISTRY_ACCESS_TOKEN=<your-registry-access-token> # (optional) your access token to connect to docker registry
 WANDB_API_KEY=NotSpecified                         # (optional) your API key to connect to Weights and Biases service
 JUPYTER_PORT=8888                                  # (optional) port to connect to jupyter server
 ```
 
-## Pull development container
+#### Pull development container
 Currently the latest docker image available on Docker Hub is available at `docker.io/pourion/jax_dips`. Instead of building the container, you can only pull the latest docker image by running 
 
 ```
 ./launch.sh pull
 ```
 which pulls from docker hub; i.e., equivalent to ```$ docker pull pourion/jax_dips:latest```.
-## Build development container
+#### Build development container
 Alternatively you can build the container by running the following command
 ```
 ./launch.sh build
 ```
 In case you want to add additional libraries to your container this is the recommended way.
 
 
-## Start developement container
+#### Start developement container
 This will create a container and places the user in the container with source code mounted. 
 
 ```
 ./launch.sh dev
 ```
 Additionally, you can run the container in background without having your terminal jump into the container. This can be done by passing the `-d` flag for daemon:
 ```
@@ -117,15 +130,15 @@
 
 You can always attach your teminal to the running `jax_dips` container by
 
 ```
 ./launch.sh attach
 ```
 
-### Development in VS Code 
+#### Development in VS Code 
 Once the container is created and is running on your machine, user can attach to this container from VS code; i.e., you need to install Microsoft's `Dev Containers` extension in your VS Code, then `Ctrl+Shift+P` and choose `Dev Containers: Attach to Running Container...`, then choose the `jax_dips` container from the list of running containers on your machine.
 
 ## Cite JAX-DIPS
 If you use JAX-DIPS in your research please use the following citations:
 
 ```bibtex
 @article{mistani2022jax,
```

### Comparing `jax-dips-0.2.0/jax_dips.egg-info/SOURCES.txt` & `jax-dips-0.2.1/jax_dips.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/setup.py` & `jax-dips-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 
 _here = pathlib.Path(__file__).resolve().parent
 
 name = "jax-dips"
 
-version = "0.2.0"
+version = "0.2.1"
 
 author = "Pouria Mistani & Samira Pakravan"
 
 author_email = "p.a.mistani@gmail.com"
 
 description = "Differentiable 3D interfacial PDE solvers written in JAX using the Neural Bootstrapping Method."
 
@@ -37,16 +37,19 @@
 ]
 
 python_requires = "~=3.8"
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 requirements.append("pyevtk")
+
 requirements.pop(0)
 requirements.pop(0)
+requirements.insert(0, "jax")
+requirements.insert(1, 'jaxlib ; extra == "cuda12_local"')
 
 
 setuptools.setup(
     name=name,
     version=version,
     author=author,
     author_email=author_email,
```

### Comparing `jax-dips-0.2.0/tests/confs/experiment_configs.py` & `jax-dips-0.2.1/tests/confs/experiment_configs.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/tests/test_advection.py` & `jax-dips-0.2.1/tests/test_advection.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/tests/test_amr.py` & `jax-dips-0.2.1/tests/test_amr.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/tests/test_geometric_integrations.py` & `jax-dips-0.2.1/tests/test_geometric_integrations.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/tests/test_poisson.py` & `jax-dips-0.2.1/tests/test_poisson.py`

 * *Files identical despite different names*

### Comparing `jax-dips-0.2.0/tests/test_reinitialization.py` & `jax-dips-0.2.1/tests/test_reinitialization.py`

 * *Files identical despite different names*

