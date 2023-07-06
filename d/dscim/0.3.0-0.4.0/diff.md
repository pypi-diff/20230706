# Comparing `tmp/dscim-0.3.0.tar.gz` & `tmp/dscim-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dscim-0.3.0.tar", last modified: Thu Sep 29 22:01:09 2022, max compression
+gzip compressed data, was "dscim-0.4.0.tar", last modified: Thu Jul  6 20:35:16 2023, max compression
```

## Comparing `dscim-0.3.0.tar` & `dscim-0.4.0.tar`

### file list

```diff
@@ -1,74 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 22:01:09.659402 dscim-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 22:01:09.651402 dscim-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 22:01:09.655402 dscim-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-09-29 22:00:50.000000 dscim-0.3.0/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-09-29 22:00:50.000000 dscim-0.3.0/.github/workflows/pythonpackage.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-09-29 22:00:50.000000 dscim-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2314 2022-09-29 22:00:50.000000 dscim-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-29 22:00:50.000000 dscim-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-29 22:00:50.000000 dscim-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5565 2022-09-29 22:01:09.659402 dscim-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4858 2022-09-29 22:00:50.000000 dscim-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-09-29 22:00:50.000000 dscim-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-09-29 22:00:50.000000 dscim-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-09-29 22:01:09.659402 dscim-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 22:01:09.651402 dscim-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 22:01:09.655402 dscim-0.3.0/src/dscim/
--rw-r--r--   0 runner    (1001) docker     (121)     8847 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3240 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/descriptors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 22:01:09.655402 dscim-0.3.0/src/dscim/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/diagnostics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6300 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/diagnostics/batch_maps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/diagnostics/compare_sccs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6363 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/diagnostics/crayola_plots.py
--rw-r--r--   0 runner    (1001) docker     (121)    10385 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/diagnostics/damage_function.py
--rw-r--r--   0 runner    (1001) docker     (121)     3376 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/diagnostics/damage_inc_share_boxplots.py
--rw-r--r--   0 runner    (1001) docker     (121)     4554 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/diagnostics/discount_rates.py
--rw-r--r--   0 runner    (1001) docker     (121)     5689 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/diagnostics/equity_risk_premiums.py
--rw-r--r--   0 runner    (1001) docker     (121)    12317 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/diagnostics/fair_step.py
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/diagnostics/global_consumption.py
--rw-r--r--   0 runner    (1001) docker     (121)     8179 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/diagnostics/maps.py
--rw-r--r--   0 runner    (1001) docker     (121)     3348 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/diagnostics/stacked_damage_function.py
--rw-r--r--   0 runner    (1001) docker     (121)    13559 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/diagnostics/var_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 22:01:09.655402 dscim-0.3.0/src/dscim/fair/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/fair/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 22:01:09.655402 dscim-0.3.0/src/dscim/menu/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/menu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/menu/baseline.py
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/menu/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     4508 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/menu/equity.py
--rw-r--r--   0 runner    (1001) docker     (121)    50268 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/menu/main_recipe.py
--rw-r--r--   0 runner    (1001) docker     (121)     2723 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/menu/risk_aversion.py
--rw-r--r--   0 runner    (1001) docker     (121)    14690 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/menu/simple_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 22:01:09.659402 dscim-0.3.0/src/dscim/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (121)     2531 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/preprocessing/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 22:01:09.659402 dscim-0.3.0/src/dscim/preprocessing/climate/
--rw-r--r--   0 runner    (1001) docker     (121)     2718 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/preprocessing/climate/all_masks_rff.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2500 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/preprocessing/climate/reformat.py
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/preprocessing/climate/ssp_clipped_rff.py
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/preprocessing/climate/stack_iterations.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/preprocessing/climate/stack_masks.py
--rw-r--r--   0 runner    (1001) docker     (121)    23433 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/preprocessing/input_damages.py
--rw-r--r--   0 runner    (1001) docker     (121)     2244 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/preprocessing/midprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 22:01:09.659402 dscim-0.3.0/src/dscim/preprocessing/misc/
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/preprocessing/misc/bottom_code_econ_zarr.py
--rw-r--r--   0 runner    (1001) docker     (121)     5786 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/preprocessing/misc/check_nans.py
--rw-r--r--   0 runner    (1001) docker     (121)     2960 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/preprocessing/misc/convert_float32.py
--rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/preprocessing/mortality_inputs_archived.py
--rw-r--r--   0 runner    (1001) docker     (121)    11386 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/preprocessing/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 22:01:09.659402 dscim-0.3.0/src/dscim/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (121)     7783 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2072 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/utils/generate_yaml.py
--rw-r--r--   0 runner    (1001) docker     (121)     5040 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/utils/menu_runs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2646 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/utils/plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8056 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/utils/rff.py
--rw-r--r--   0 runner    (1001) docker     (121)    23780 2022-09-29 22:00:50.000000 dscim-0.3.0/src/dscim/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 22:01:09.655402 dscim-0.3.0/src/dscim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5565 2022-09-29 22:01:07.000000 dscim-0.3.0/src/dscim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1979 2022-09-29 22:01:09.000000 dscim-0.3.0/src/dscim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-29 22:01:07.000000 dscim-0.3.0/src/dscim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-29 22:01:07.000000 dscim-0.3.0/src/dscim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:16.937011 dscim-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:16.929011 dscim-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:16.933011 dscim-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-06 20:34:53.000000 dscim-0.4.0/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-06 20:34:53.000000 dscim-0.4.0/.github/workflows/pythonpackage.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-06 20:34:53.000000 dscim-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-06 20:34:53.000000 dscim-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 20:34:53.000000 dscim-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 20:34:53.000000 dscim-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-06 20:35:16.937011 dscim-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-06 20:34:53.000000 dscim-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-06 20:34:53.000000 dscim-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-06 20:34:53.000000 dscim-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-06 20:35:16.937011 dscim-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:16.929011 dscim-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:16.933011 dscim-0.4.0/src/dscim/
+-rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/descriptors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:16.933011 dscim-0.4.0/src/dscim/menu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/menu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/menu/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/menu/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/menu/equity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50201 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/menu/main_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/menu/risk_aversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/menu/simple_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:16.933011 dscim-0.4.0/src/dscim/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/preprocessing/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:16.937011 dscim-0.4.0/src/dscim/preprocessing/climate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/preprocessing/climate/all_masks_rff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/preprocessing/climate/ssp_clipped_rff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/preprocessing/climate/stack_iterations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/preprocessing/climate/stack_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27405 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/preprocessing/input_damages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/preprocessing/midprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:16.937011 dscim-0.4.0/src/dscim/preprocessing/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/preprocessing/misc/bottom_code_econ_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/preprocessing/misc/check_nans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/preprocessing/misc/convert_float32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/preprocessing/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:16.937011 dscim-0.4.0/src/dscim/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/utils/generate_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/utils/menu_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/utils/plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16473 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/utils/rff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-07-06 20:34:53.000000 dscim-0.4.0/src/dscim/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:16.933011 dscim-0.4.0/src/dscim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-06 20:35:14.000000 dscim-0.4.0/src/dscim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-06 20:35:16.000000 dscim-0.4.0/src/dscim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:35:14.000000 dscim-0.4.0/src/dscim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 20:35:14.000000 dscim-0.4.0/src/dscim.egg-info/top_level.txt
```

### Comparing `dscim-0.3.0/.github/workflows/python-publish.yaml` & `dscim-0.4.0/.github/workflows/python-publish.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v3
         with:
-          python-version: '3.x'
+          python-version: '3.10'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install build
       - name: Build package
         run: python -m build
       - name: Publish package
```

### Comparing `dscim-0.3.0/.github/workflows/pythonpackage.yaml` & `dscim-0.4.0/.github/workflows/pythonpackage.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 jobs:
 
   codequality:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.x"]
+        python-version: ["3.10"]
     defaults:
       run:
         shell: bash
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v3
@@ -38,15 +38,15 @@
         run: |
           flake8
 
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.x"]
+        python-version: ["3.10"]
     defaults:
       run:
         shell: bash
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v3
@@ -60,7 +60,9 @@
           pip install -r requirements.txt
       - name: Install package
         run: |
           pip install .
       - name: Test with pytest
         run: |
           pytest -v --cov dscim --cov-report term-missing --cov-report xml
+      - name: Upload coverage to Codecov
+        uses: codecov/codecov-action@v3
```

### Comparing `dscim-0.3.0/.gitignore` & `dscim-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dscim-0.3.0/LICENSE` & `dscim-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dscim-0.3.0/PKG-INFO` & `dscim-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dscim
-Version: 0.3.0
+Version: 0.4.0
 Summary: Data-Driven Spatial Climate Impact Model core component code
 Project-URL: Homepage, https://github.com/ClimateImpactLab/dscim
 Project-URL: Documentation, https://github.com/ClimateImpactLab/dscim
 Project-URL: Source, https://github.com/ClimateImpactLab/dscim
 Project-URL: Bug Tracker, https://github.com/ClimateImpactLab/dscim/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `dscim-0.3.0/README.md` & `dscim-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dscim-0.3.0/pyproject.toml` & `dscim-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dscim-0.3.0/src/dscim/__init__.py` & `dscim-0.4.0/src/dscim/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,14 @@
         configuration file and for a desired sector
         """
 
         uncertainty = None
 
         # limit options for code release
         if self.ALLOWED_SECTORS != "any":
-
             assert any(
                 [sector in self.ALLOWED_SECTORS]
             ), f"Sector {sector} unavailable. Please pass one of {self.ALLOWED_SECTORS}."
         assert any(
             [kwargs["discounting_type"] in self.ALLOWED_DISCOUNTING_TYPES]
         ), f"Discounting_type {kwargs['discounting_type']} unavailable. Please pass one of {self.ALLOWED_DISCOUNTING_TYPES}."
         assert any(
```

### Comparing `dscim-0.3.0/src/dscim/descriptors.py` & `dscim-0.4.0/src/dscim/descriptors.py`

 * *Files identical despite different names*

### Comparing `dscim-0.3.0/src/dscim/diagnostics/fair_step.py` & `dscim-0.4.0/src/dscim/preprocessing/preprocessing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,416 +1,466 @@
+from math import ceil
+from pathlib import Path
 import os
+import sys
 
-username = os.getenv("USER")
-
+USER = os.getenv("USER")
+import dask
+import dask.array as da
+import dask.config
 import numpy as np
-import pandas as pd
 import xarray as xr
-from itertools import product
-import logging
-
-logger = logging.getLogger(__name__)
-import matplotlib.pyplot as plt
-import seaborn as sns
-from functools import reduce
-
-sns.set_style("darkgrid")
-sns.set_context("talk")
+from dask.distributed import Client, progress
+from dscim.utils.functions import ce_func, mean_func
+import yaml
+import time
+import argparse
 
 
-def marginal_damages(
-    sector,
-    sector_path,
-    discounting,
-    recipes=("risk_aversion", "equity"),
-    save_path=None,
+def ce_from_chunk(
+    chunk,
+    filepath,
+    reduction,
+    bottom_code,
+    histclim,
+    delta,
+    recipe,
+    eta,
+    zero,
+    socioec,
+    ce_batch_coords,
 ):
-
-    # get relevant files
-    marginal_damages = {}
-    for recipe in recipes:
-
-        marginal_damages[recipe] = (
-            xr.open_dataset(
-                f"{sector_path}/{recipe}_{discounting}_fair_marginal_damages_ce.nc4"
-            )
-            .to_dataframe()
-            .reset_index()
-        )
-
-        # sort for plotting consistency
-        marginal_damages[recipe]["ssp-model"] = (
-            marginal_damages[recipe].ssp + "-" + marginal_damages[recipe].model
+    year = chunk.year.values
+    ssp = chunk.ssp.values
+    model = chunk.model.values
+
+    gdppc = (
+        xr.open_zarr(socioec, chunks=None)
+        .sel(
+            year=year, ssp=ssp, model=model, region=ce_batch_coords["region"], drop=True
         )
-        marginal_damages[recipe] = marginal_damages[recipe].sort_values(["ssp-model"])
-
-        # to avoid errors when plotting by hue and style
-        if discounting == "wr":
-            marginal_damages[recipe]["ssp"], marginal_damages[recipe]["model"] = "", ""
-
-    fig, ax = plt.subplots(
-        2, len(recipes), figsize=(15, 10), sharex=True, sharey=True, squeeze=False
+        .gdppc
     )
 
-    plt.subplots_adjust(wspace=0, hspace=0, top=0.90)
-
-    for i, recipe in enumerate(recipes):
-
-        sns.lineplot(
-            data=marginal_damages[recipe].loc[marginal_damages[recipe].rcp == "rcp45"],
-            x="year",
-            y="temperature",
-            hue="ssp",
-            style="model",
-            ax=ax[0][i],
+    if reduction == "no_cc":
+        if zero:
+            chunk[histclim] = xr.where(chunk[histclim] == 0, 0, 0)
+        calculation = gdppc + chunk[histclim].mean("batch") - chunk[histclim]
+    elif reduction == "cc":
+        calculation = gdppc - chunk[delta]
+    else:
+        raise NotImplementedError("Pass 'cc' or 'no_cc' to reduction.")
+
+    if recipe == "adding_up":
+        result = mean_func(
+            np.maximum(
+                calculation,
+                bottom_code,
+            ),
+            "batch",
         )
-
-        ax[0][i].set_xlabel("Year")
-        ax[0][i].set_title(f"Recipe: {recipe}, rcp 4.5")
-
-        sns.lineplot(
-            data=marginal_damages[recipe].loc[marginal_damages[recipe].rcp == "rcp85"],
-            x="year",
-            y="temperature",
-            hue="ssp",
-            style="model",
-            ax=ax[1][i],
+    elif recipe == "risk_aversion":
+        result = ce_func(
+            np.maximum(
+                calculation,
+                bottom_code,
+            ),
+            "batch",
+            eta=eta,
         )
 
-        ax[1][i].set_xlabel("Year")
-        ax[1][i].set_title(f"Recipe: {recipe}, rcp 8.5")
-
-    fig.suptitle(
-        f"{sector}: {discounting} discounting \n Marginal damages from an additional pulse of C02"
-    )
-
-    ax[0][0].set_ylabel("Damages in 2019 USD")
-    ax[1][0].set_ylabel("Damages in 2019 USD")
-
-    if save_path is not None:
-        plt.savefig(
-            f"{save_path}/{sector}_{discounting}_marginal_damages.png",
-            dpi=300,
-            bbox_inches="tight",
-        )
+    return result
 
 
-def global_consumption(
+def reduce_damages(
+    recipe,
+    reduction,
+    eta,
     sector,
-    sector_path,
-    discounting,
-    recipes=("risk_aversion", "equity"),
-    save_path=None,
-    scale=10**12,
+    config,
+    socioec,
+    bottom_coding_gdppc=39.39265060424805,
+    zero=False,
 ):
+    if recipe == "adding_up":
+        assert (
+            eta is None
+        ), "Adding up does not take an eta argument. Please set to None."
+    # client = Client(n_workers=35, memory_limit="9G", threads_per_worker=1)
+
+    with open(config, "r") as stream:
+        c = yaml.safe_load(stream)
+        params = c["sectors"][sector]
+
+    damages = Path(params["sector_path"])
+    histclim = params["histclim"]
+    delta = params["delta"]
+    outpath = f"{c['paths']['reduced_damages_library']}/{sector}"
+
+    with xr.open_zarr(damages, chunks=None)[histclim] as ds:
+        with xr.open_zarr(socioec, chunks=None) as gdppc:
+            assert (
+                xr.open_zarr(damages).chunks["batch"][0] == 15
+            ), "'batch' dim on damages does not have chunksize of 15. Please rechunk."
+
+            if "coastal" not in sector:
+                chunkies = {
+                    "rcp": 1,
+                    "region": -1,
+                    "gcm": 1,
+                    "year": 10,
+                    "model": 1,
+                    "ssp": 1,
+                }
+            else:
+                chunkies = {
+                    "region": -1,
+                    "slr": 1,
+                    "year": 10,
+                    "model": 1,
+                    "ssp": 1,
+                }
 
-    gc = {}
-    for recipe in recipes:
-
-        gc[recipe] = (
-            xr.open_dataset(
-                f"{sector_path}/{recipe}_{discounting}_global_consumption.nc4"
-            )
-            .to_dataframe()
-            .reset_index()
-        )
-
-        gc[recipe]["global_cons_scaled"] = (
-            gc[recipe][f"global_cons_{discounting}"] / scale
-        )
-
-        if discounting == "wr":
-            gc[recipe]["ssp"], gc[recipe]["model"] = "", ""
+            ce_batch_dims = [i for i in gdppc.dims] + [
+                i for i in ds.dims if i not in gdppc.dims and i != "batch"
+            ]
+            ce_batch_coords = {c: ds[c].values for c in ce_batch_dims}
+            ce_batch_coords["region"] = [
+                i for i in gdppc.region.values if i in ce_batch_coords["region"]
+            ]
+            ce_shapes = [len(ce_batch_coords[c]) for c in ce_batch_dims]
 
-    fig, ax = plt.subplots(
-        1, len(recipes), figsize=(15, 10), squeeze=False, sharey=True, sharex=True
+    template = xr.DataArray(
+        da.empty(ce_shapes),
+        dims=ce_batch_dims,
+        coords=ce_batch_coords,
+    ).chunk(chunkies)
+
+    other = xr.open_zarr(damages).chunk(chunkies)
+
+    out = other.map_blocks(
+        ce_from_chunk,
+        kwargs=dict(
+            filepath=damages,
+            reduction=reduction,
+            bottom_code=bottom_coding_gdppc,
+            histclim=histclim,
+            delta=delta,
+            eta=eta,
+            recipe=recipe,
+            zero=zero,
+            socioec=socioec,
+            ce_batch_coords=ce_batch_coords,
+        ),
+        template=template,
     )
 
-    for i, recipe in enumerate(recipes):
+    out = out.astype(np.float32).rename(reduction).to_dataset()
 
-        sns.lineplot(
-            data=gc[recipe],
-            x="year",
-            y="global_cons_scaled",
-            hue="ssp",
-            style="model",
-            ax=ax[0][i],
+    out.attrs["bottom code"] = bottom_coding_gdppc
+    out.attrs["histclim=0"] = zero
+    out.attrs["filepath"] = str(damages)
+
+    if recipe == "adding_up":
+        out.to_zarr(
+            f"{outpath}/{recipe}_{reduction}.zarr",
+            consolidated=True,
+            mode="w",
+        )
+    elif recipe == "risk_aversion":
+        out.attrs["eta"] = eta
+        out.to_zarr(
+            f"{outpath}/{recipe}_{reduction}_eta{eta}.zarr",
+            consolidated=True,
+            mode="w",
         )
 
-        ax[0][i].set_title(f"RECIPE: {recipe}")
-
-    ax[0][0].set_ylabel(f'Global consumption in {"{:.0e}".format(scale)} 2019 USD')
 
-    fig.suptitle(
-        f"{sector}: {discounting} discounting \n Global consumption, no climate change"
+def reformat_climate_files():
+    from dscim.preprocessing.climate.reformat import (
+        convert_old_to_newformat_AR,
+        stack_gases,
     )
 
-    if save_path is not None:
-        plt.savefig(f"{save_path}/{sector}_{discounting}_global_consumption.pdf")
-
-
-def output_scc(
-    sector,
-    sector_path,
-    eta,
-    rho,
-    recipes=("adding_up", "risk_aversion", "equity", "local"),
-    discounting=("constant_model_collapsed", "constant", "euler_ramsey", "euler_gwr"),
-    save_path=None,
-    file=None,
-    subset_dict=None,
-    index=(
-        "discount_type",
-        "discrate",
-        "weitzman_parameter",
-        "model",
-        "ssp",
-        "rcp",
-        "gas",
-    ),
-):
-
-    final_dfs = []
-
-    for recipe in recipes:
+    # convert AR6 files
+    bd = "/shares/gcp/integration/float32/dscim_input_data/climate/AR6"
+    pathdt = {
+        "median": f"{bd}/ar6_fair162_medianparams_control_pulse_2020-2080_10yrincrements_conc_rf_temp_lambdaeff_emissions-driven_2naturalfix_v4.0_Jan212022.nc",
+        "sims": f"{bd}/ar6_fair162_control_pulse_2020-2030-2040-2050-2060-2070-2080_emis_conc_rf_temp_lambdaeff_emissions-driven_naturalfix_v4.0_Jan212022.nc",
+    }
 
-        dfs = []
+    newds = convert_old_to_newformat_AR(
+        pathdt,
+        gas="CO2_Fossil",
+        var="temperature",
+    )
 
-        for disc in discounting:
+    newds.to_netcdf(
+        f"{bd}/ar6_fair162_sim_and_medianparams_control_pulse_2030-2040-2050-2060-2070-2080_emis_conc_rf_temp_lambdaeff_emissions-driven_naturalfix_v4.0_Jan212022.nc"
+    )
 
-            ds = xr.open_dataset(
-                f"{sector_path}/{recipe}_{disc}_eta{eta}_rho{rho}_scc.nc4"
-            ).sel(subset_dict)
+    # convert RFF files
+    gases = {"CO2_Fossil": "Feb072022", "CH4": "Feb072022", "N2O": "Feb072022"}
+    stack_gases(gas_dict=gases)
 
-            if "runtype" in list(ds.coords):
-                ds = ds.drop("runtype")
-            else:
-                pass
 
-            if recipe == "local":
-                ds = ds.drop("year")
-                df = ds.to_dataframe().unstack(
-                    ["first_fair_aggregation", "fair_aggregation"]
+def sum_AMEL(
+    sectors,
+    config,
+    AMEL,
+):
+    # load config
+    with open(config, "r") as stream:
+        loaded_config = yaml.safe_load(stream)
+        params = loaded_config["sectors"]
+
+    output = params[AMEL]["sector_path"]
+
+    # save summed variables to zarr one by one
+    for i, var in enumerate(["delta", "histclim"]):
+        datasets = []
+
+        for sector in sectors:
+            print(f"Opening {sector},{params[sector]['sector_path']}")
+            ds = xr.open_zarr(params[sector]["sector_path"], consolidated=True)
+            ds = (
+                ds[params[sector][var]]
+                .rename(var)
+                .chunk(
+                    {
+                        "batch": 15,
+                        "ssp": 1,
+                        "model": 1,
+                        "rcp": 1,
+                        "gcm": 1,
+                        "year": 10,
+                        "region": -1,
+                    }
                 )
-            else:
-                df = ds.to_dataframe().unstack("fair_aggregation")
-
-            df = df.droplevel(0, axis=1)
-
-            if recipe == "local":
-                df.columns = [
-                    df.columns[i][0] + "-" + df.columns[i][1]
-                    for i in range(0, len(df.columns))
-                ]
-
-            df = df.rename(columns={col: f"{recipe}_{col}" for col in df.columns})
-
-            if disc not in ["constant", "constant_model_collapsed"]:
-
-                df["discrate"] = np.nan
-
-            df = df.reset_index().set_index(index)
+            )
+            ds = xr.where(np.isinf(ds), np.nan, ds)
+            datasets.append(ds)
 
-            dfs.append(df)
+        summed = (
+            xr.concat(datasets, dim="variable")
+            .sum("variable")
+            .rename(f"summed_{var}")
+            .astype(np.float32)
+            .chunk(
+                {
+                    "batch": 15,
+                    "ssp": 1,
+                    "model": 1,
+                    "rcp": 1,
+                    "gcm": 1,
+                    "year": 10,
+                    "region": 24378,
+                }
+            )
+            .to_dataset()
+        )
 
-        final_dfs.append(pd.concat(dfs))
+        summed.attrs["paths"] = str({s: params[s]["sector_path"] for s in sectors})
+        summed.attrs["delta"] = str({s: params[s]["delta"] for s in sectors})
+        summed.attrs["histclim"] = str({s: params[s]["histclim"] for s in sectors})
 
-    final_df = reduce(lambda left, right: left.join(right), final_dfs)
+        for v in summed.variables:
+            summed[v].encoding.clear()
 
-    if save_path is not None:
-        os.makedirs(save_path, exist_ok=True)
-        if file is not None:
-            final_df.to_csv(f"{save_path}/{file}")
+        if i == 0:
+            summed.to_zarr(output, consolidated=True, mode="w")
         else:
-            final_df.to_csv(f"{save_path}/{sector}_sccs.csv")
-
-    return final_df
+            summed.to_zarr(output, consolidated=True, mode="a")
 
 
-def plot_implicit_rates(
+def subset_USA_reduced_damages(
     sector,
-    path,
-    fair_aggregation="ce",
-    ssp=None,
-    model=None,
-    pulse_year=2020,
-    recipes=("risk_aversion", "equity"),
-    discounting=("ramsey", "gwr"),
-    save_path=None,
-    csv=True,
+    reduction,
+    recipe,
+    eta,
+    input_path,
 ):
-    if ssp is None:
-        ssp = ["SSP3"]
+    if recipe == "adding_up":
+        ds = xr.open_zarr(
+            f"{input_path}/{sector}/{recipe}_{reduction}.zarr",
+        )
+    elif recipe == "risk_aversion":
+        ds = xr.open_zarr(
+            f"{input_path}/{sector}/{recipe}_{reduction}_eta{eta}.zarr",
+        )
 
-    if model is None:
-        model = ["IIASA GDP"]
+    US_territories = [
+        "USA",
+        "XBK",
+        "GUM",
+        "XHO",
+        "XJV",
+        "XJA",
+        "XKR",
+        "XMW",
+        "XNV",
+        "MNP",
+        "XPL",
+        "PRI",
+        "VIR",
+        "XWK",
+    ]
+    subset = ds.sel(
+        region=[i for i in ds.region.values if any(j in i for j in US_territories)]
+    )
 
-    for recipe in recipes:
+    for var in subset.variables:
+        subset[var].encoding.clear()
 
-        for disc in discounting:
+    if recipe == "adding_up":
+        subset.to_zarr(
+            f"{input_path}/{sector}_USA/{recipe}_{reduction}.zarr",
+            consolidated=True,
+            mode="w",
+        )
+    elif recipe == "risk_aversion":
+        subset.to_zarr(
+            f"{input_path}/{sector}_USA/{recipe}_{reduction}_eta{eta}.zarr",
+            consolidated=True,
+            mode="w",
+        )
 
-            if "gwr" in disc:
-                ssp = ["['SSP3', 'SSP2', 'SSP4']"]
-                model = ["['IIASA GDP', 'OECD Env-Growth']"]
 
-            naive = xr.open_dataset(
-                f"{path}/{recipe}_naive_{disc}_discount_factors.nc4"
-            )
-            euler = xr.open_dataset(
-                f"{path}/{recipe}_euler_{disc}_discount_factors.nc4"
-            )
+def subset_USA_ssp_econ(
+    in_path,
+    out_path,
+):
+    zarr = xr.open_zarr(
+        in_path,
+        consolidated=True,
+    )
 
-            naive.coords["weitzman_parameter"] = euler.weitzman_parameter
-            naive.coords["rcp"] = "Naive Ramsey"
+    US_territories = [
+        "USA",
+        "XBK",
+        "GUM",
+        "XHO",
+        "XJV",
+        "XJA",
+        "XKR",
+        "XMW",
+        "XNV",
+        "MNP",
+        "XPL",
+        "PRI",
+        "VIR",
+        "XWK",
+    ]
+    zarr = zarr.sel(
+        region=[i for i in zarr.region.values if any(j in i for j in US_territories)]
+    )
 
-            if "gwr" in disc:
-                naive.coords["model"] = euler.model
-                naive.coords["ssp"] = euler.ssp
+    for var in zarr.variables:
+        zarr[var].encoding.clear()
 
-            subset = pd.concat(
-                [euler.to_dataframe().reset_index(), naive.to_dataframe().reset_index()]
-            )
+    zarr.to_zarr(
+        out_path,
+        consolidated=True,
+        mode="w",
+    )
 
-            subset["rate"] = (1 / subset.__xarray_dataarray_variable__) ** (
-                1 / (subset.year - pulse_year)
-            ) - 1
-
-            subset = subset.loc[
-                (subset.fair_aggregation == fair_aggregation)
-                & (subset.weitzman_parameter != "1")
-            ]
 
-            subset = subset.loc[(subset.ssp.isin(ssp)) & (subset.model.isin(model))]
+def clip_damages(
+    config,
+    sector,
+    econ_path="/shares/gcp/integration/float32/dscim_input_data/econvars/zarrs/integration-econ-bc39.zarr",
+):
+    """This function is no longer in use.
+    To operationalize, make sure to get a Dask client running with the following code:
 
-            subset["weitzman_parameter"] = subset.weitzman_parameter.astype(
-                str
-            ).replace(
-                {
-                    "0.01": "1% of future GDP",
-                    "0.1": "10% of future GDP",
-                    "0.5": "50% of future GDP",
-                    "858795238461.09": "1% of current GDP",
-                    "1000000000000.0": "1 trillion USD",
-                    "1.0": "1 USD",
-                }
-            )
+    # set up dask
+    dask.config.set(
+        {
+            "distributed.worker.memory.target": 0.7,
+            "distributed.worker.memory.spill": 0.8,
+            "distributed.worker.memory.pause": 0.9,
+        }
+    )
 
-            # palette = ['blue', 'red', 'grey']
+    client = Client(n_workers=40, memory_limit="9G", threads_per_worker=1)
+    """
 
-            #             if recipe == 'equity':
-            #                 subset = subset.loc[subset.rcp != 'Naive Ramsey']
-            #                 palette = palette[0:2]
-
-            if len(ssp) <= 1:
-                g = sns.relplot(
-                    data=subset,
-                    x="year",
-                    y="rate",
-                    kind="line",
-                    col="weitzman_parameter",
-                    col_wrap=3,
-                    height=10,
-                    facet_kws={"sharey": True, "sharex": True, "legend_out": False},
-                    hue="rcp",
-                    style="model",
-                )  # palette=sns.color_palette(palette))
-            else:
-                g = sns.relplot(
-                    data=subset,
-                    x="year",
-                    y="rate",
-                    kind="line",
-                    col="weitzman_parameter",
-                    row="ssp",
-                    height=10,
-                    facet_kws={"sharey": True, "sharex": True, "legend_out": False},
-                    hue="rcp",
-                    style="model",
-                )  # palette=sns.color_palette(palette))
-
-            g.fig.suptitle(
-                f"""Implicit Discount Rates - Naive and Euler Discounting
-            Recipe: {recipe}, Sector: {sector}, Discounting = {disc}, SSP = {ssp}"""
-            )
-            plt.subplots_adjust(top=0.9, wspace=0)
+    # load config
+    with open(config, "r") as stream:
+        loaded_config = yaml.safe_load(stream)
+        params = loaded_config["sectors"][sector]
+
+    # get sector paths and variable names
+    sector_path = Path(params["sector_path"])
+    histclim = params["histclim"]
+    delta = params["delta"]
+
+    with xr.open_zarr(sector_path, chunks=None)[delta] as ds:
+        with xr.open_zarr(econ_path, chunks=None) as gdppc:
+            ce_batch_dims = [i for i in ds.dims]
+            ce_batch_coords = {c: ds[c].values for c in ce_batch_dims}
+            ce_batch_coords["region"] = [
+                i for i in ds.region.values if i in gdppc.region.values
+            ]
+            ce_shapes = [len(ce_batch_coords[c]) for c in ce_batch_dims]
+            ce_chunks = [xr.open_zarr(sector_path).chunks[c][0] for c in ce_batch_dims]
+            print(ce_chunks)
+
+    template = xr.DataArray(
+        da.empty(ce_shapes, chunks=ce_chunks),
+        dims=ce_batch_dims,
+        coords=ce_batch_coords,
+    )
 
-            if save_path:
-                os.makedirs(save_path, exist_ok=True)
-                plt.savefig(
-                    f"{save_path}/{recipe}_{disc}_{ssp}_{model}_implicit_discount_rates.png",
-                    dpi=300,
-                    bbox_inches="tight",
-                )
+    def chunk_func(
+        damages,
+    ):
+        year = damages.year.values
+        ssp = damages.ssp.values
+        model = damages.model.values
+        region = damages.region.values
+
+        gdppc = (
+            xr.open_zarr(econ_path, chunks=None)
+            .sel(year=year, ssp=ssp, model=model, region=region, drop=True)
+            .gdppc
+        )
 
-    #                 if csv:
-    #                     cols = ['fair_aggregation', 'weitzman_parameter', 'ssp', 'model', 'rcp']
-    #                     df = (subset.set_index(cols + ['year']).
-    #                            rate.
-    #                            sort_index(level=cols).
-    #                            unstack(cols)
-    #                           )
-
-    #                     df.to_csv(f"{save_path}/{recipe}_{disc}_implicit_discount_rates.csv")
-
-    return subset
-
-
-def statistics(df):
-    """Produces statistics about each SCC file.
-    Undocumented :/
+        # get damages as % of GDPpc
+        shares = damages / gdppc
 
-    """
+        # find the 1st/99th percentile of damage share
+        # across batches and regions
+        quantile = shares.quantile([0.01, 0.99], ["batch", "region"])
+
+        # find the equivalent damages
+        # if damage share is capped to 1st/99th percentile
+        quantdams = quantile * gdppc
+
+        # keep damages that are within cutoff,
+        # otherwise replace with capped damages
+        damages = xr.where(
+            (shares <= quantile.sel(quantile=0.99, drop=True)),
+            damages,
+            quantdams.sel(quantile=0.99, drop=True),
+        )
 
-    rcp_grouped = df.reset_index().pivot(
-        index=["discount_type", "discrate", "ssp", "model", "weitzman_parameter"],
-        columns=["rcp"],
-    )
-
-    for i, j in list([("rcp45", "rcp85"), ("ssp245", "ssp460"), ("ssp460", "ssp370")]):
-
-        print(f"\n {i} > {j} \n")
-
-        for col in rcp_grouped.columns.get_level_values("fair_aggregation").unique():
-            sketch = rcp_grouped.loc[rcp_grouped[col][i] > rcp_grouped[col][j]]
-            print(f"\t {col}: {round(len(sketch)/len(rcp_grouped[col])*100,2)} %")
-
-    comparators = [
-        ("risk_aversion_ce", "risk_aversion_mean"),
-        ("equity_ce", "equity_mean"),
-        ("equity_ce", "risk_aversion_ce"),
-        ("equity_mean", "risk_aversion_mean"),
-        ("risk_aversion_median", "adding_up_median"),
-        ("equity_median", "risk_aversion_median"),
-    ]
+        damages = xr.where(
+            (shares >= quantile.sel(quantile=0.01, drop=True)),
+            damages,
+            quantdams.sel(quantile=0.01, drop=True),
+        )
 
-    df["ra_diff"] = (
-        (df.risk_aversion_ce - df.risk_aversion_uncollapsed) / df.risk_aversion_ce * 100
-    )
-    df["eq_diff"] = (df.equity_ce - df.equity_uncollapsed) / df.equity_ce * 100
+        return damages
 
-    describers = {
-        "ra_diff": "(risk aversion CE - risk aversion mean(SCCs)) / risk aversion CE * 100",
-        "eq_diff": "(equity CE - equity mean(SCCs)) / equity CE * 100",
-    }
+    data = xr.open_zarr(sector_path)
 
-    group_disc = df.groupby("discount_type")
+    for var in [delta, histclim]:
+        out = (
+            data[var].map_blocks(chunk_func, template=template).rename(var).to_dataset()
+        )
 
-    for i, j in comparators:
+        parent, name = sector_path.parent, sector_path.name
+        clipped_name = name.replace(".zarr", "_clipped.zarr")
+        outpath = Path(parent).joinpath(clipped_name)
 
-        print(f"\n {i} < {j} \n")
-        for name, disc in group_disc:
-            share = round(len(disc.loc[disc[i] < disc[j]]) / len(disc) * 100, 2)
-            print(f"\t {name}: {share} %")
-            if share > 0:
-                wp = disc.groupby("weitzman_parameter")
-                for wp_name, wp_df in wp:
-                    wp_share = round(
-                        len(wp_df.loc[wp_df[i] < wp_df[j]]) / len(disc) * 100, 2
-                    )
-                    print(f"\t \t {wp_name}: {wp_share} %")
-
-    for var, label in describers.items():
-        print(f"\n {label} \n")
-        for name, disc in group_disc:
-            print(f"\t {name}: ")
-            for stat in ["mean", "min", "max"]:
-                print(f"\t \t {stat}: {round(disc[var].describe()[stat], 2)}")
+        out.to_zarr(outpath, mode="a", consolidated=True)
```

### Comparing `dscim-0.3.0/src/dscim/menu/baseline.py` & `dscim-0.4.0/src/dscim/menu/baseline.py`

 * *Files identical despite different names*

### Comparing `dscim-0.3.0/src/dscim/menu/decorators.py` & `dscim-0.4.0/src/dscim/menu/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,23 +23,21 @@
     def decorator_save(func):
         @functools.wraps(func)
         def save_wrap(self, *args, **kwargs):
             out = func(self, *args, **kwargs)
             save = out
 
             if (self.save_path is not None) and (name in self.save_files):
-
                 if not os.path.exists(self.save_path):
                     os.makedirs(self.save_path)
 
                 filename = f"{self.NAME}_{self.discounting_type}_eta{self.eta}_rho{self.rho}_{name}{self.filename_suffix}"
                 filename_path = os.path.join(self.save_path, filename)
 
                 if isinstance(save, xr.DataArray):
-
                     save = save.rename(name).to_dataset()
                     save.attrs = self.output_attrs
 
                     # change `None` object to str(None)
                     for att in save.attrs:
                         if save.attrs[att] is None:
                             save.attrs.update({att: "None"})
```

### Comparing `dscim-0.3.0/src/dscim/menu/equity.py` & `dscim-0.4.0/src/dscim/menu/equity.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,24 +61,22 @@
         return self.ce_no_cc - self.ce_cc
 
     def global_damages_calculation(self) -> pd.DataFrame:
         dams_collapse = self.calculated_damages * self.collapsed_pop.sum(dim="region")
         df = dams_collapse.to_dataframe("damages").reset_index()
 
         if "gwr" in self.discounting_type:
-
             df = df.assign(
                 ssp=str(list(self.gdp.ssp.values)),
                 model=str(list(self.gdp.model.values)),
             )
 
         return df
 
     def global_consumption_calculation(self, disc_type):
-
         # get global consumption certainty equivalent across regions
         ce_cons = c_equivalence(
             self.gdppc,
             dims="region",
             weights=self.pop,
             eta=self.eta,
         )
```

### Comparing `dscim-0.3.0/src/dscim/menu/main_recipe.py` & `dscim-0.4.0/src/dscim/menu/main_recipe.py`

 * *Files 6% similar despite different names*

```diff
@@ -522,34 +522,30 @@
 
         yrs = range(self.climate.pulse_year, self.ext_subset_end_year + 1)
 
         params_list, preds_list = [], []
 
         if self.discounting_type == "constant_model_collapsed":
             for ssp in damage_function_points["ssp"].unique():
-
                 # Subset dataframe to specific SSP
                 fit_subset = damage_function_points[
                     damage_function_points["ssp"] == ssp
                 ]
 
                 global_c_subset = global_consumption.sel({"ssp": ssp})
                 # Fit damage function curves using the data subset
                 damage_function = model_outputs(
                     damage_function=fit_subset,
                     formula=self.formula,
-                    extrap_formula=self.extrap_formula,
                     type_estimation=self.fit_type,
                     global_c=global_c_subset,
                     extrapolation_type=self.ext_method,
                     quantiles=self.quantreg_quantiles,
                     year_range=yrs,
-                    extrap_year=self.ext_subset_start_year,
                     year_start_pred=self.ext_subset_end_year + 1,
-                    year_end_pred=self.ext_end_year,
                 )
 
                 # Add variables
                 params = damage_function["parameters"].expand_dims(
                     dict(
                         discount_type=[self.discounting_type],
                         ssp=[ssp],
@@ -573,36 +569,32 @@
         ):
             for ssp, model in list(
                 product(
                     damage_function_points.ssp.unique(),
                     damage_function_points.model.unique(),
                 )
             ):
-
                 # Subset dataframe to specific SSP-IAM combination.
                 fit_subset = damage_function_points[
                     (damage_function_points["ssp"] == ssp)
                     & (damage_function_points["model"] == model)
                 ]
 
                 global_c_subset = global_consumption.sel({"ssp": ssp, "model": model})
 
                 # Fit damage function curves using the data subset
                 damage_function = model_outputs(
                     damage_function=fit_subset,
                     formula=self.formula,
-                    extrap_formula=self.extrap_formula,
                     type_estimation=self.fit_type,
                     global_c=global_c_subset,
                     extrapolation_type=self.ext_method,
                     quantiles=self.quantreg_quantiles,
                     year_range=yrs,
-                    extrap_year=self.ext_subset_start_year,
                     year_start_pred=self.ext_subset_end_year + 1,
-                    year_end_pred=self.ext_end_year,
                 )
 
                 # Add variables
                 params = damage_function["parameters"].expand_dims(
                     dict(
                         discount_type=[self.discounting_type], ssp=[ssp], model=[model]
                     )
@@ -623,22 +615,19 @@
             fit_subset = damage_function_points
 
             # Fit damage function curves using the data subset
             damage_function = model_outputs(
                 damage_function=fit_subset,
                 type_estimation=self.fit_type,
                 formula=self.formula,
-                extrap_formula=self.extrap_formula,
                 global_c=global_consumption,
                 extrapolation_type=self.ext_method,
                 quantiles=self.quantreg_quantiles,
                 year_range=yrs,
-                extrap_year=self.ext_subset_start_year,
                 year_start_pred=self.ext_subset_end_year + 1,
-                year_end_pred=self.ext_end_year,
             )
 
             # Add variables
             params = damage_function["parameters"].expand_dims(
                 dict(
                     discount_type=[self.discounting_type],
                     ssp=[str(list(self.gdp.ssp.values))],
@@ -676,29 +665,27 @@
         -------
         dict
             dict['params'] is a dataframe of betas for each year
             dict['preds'] is a dataframe of predicted y hat for each
                 year and anomaly
         """
         if self.scenario_dimensions is None:
-
             # this only occurs for global discounting
             # with a single scenario passed
             damage_function = self.damage_function_calculation(
                 damage_function_points=self.damage_function_points,
                 global_consumption=self.global_consumption,
             )
 
         else:
             # cycle through the different combinations of the scenario dims
             subset = self.damage_function_points.groupby(self.scenario_dimensions)
             damage_function, dict_list = {}, []
 
             for name, dt in subset:
-
                 # turn single-dim into a tuple to make indexing easier later
                 if len(self.scenario_dimensions) == 1:
                     name = tuple([name])
 
                 df = self.damage_function_calculation(
                     damage_function_points=dt,
                     global_consumption=self.global_consumption,
@@ -812,15 +799,14 @@
 
         # Calculate global consumption per capita
         array_pc = self.global_consumption_calculation(
             disc_type
         ) / self.collapsed_pop.sum("region")
 
         if self.NAME == "equity":
-
             # equity recipe's growth is capped to
             # risk aversion recipe's growth rates
             extrapolated = extrapolate(
                 xr_array=array_pc,
                 start_year=self.ext_subset_start_year,
                 end_year=self.ext_subset_end_year,
                 interp_year=self.ext_end_year,
@@ -844,19 +830,17 @@
     @cachedproperty
     @save(name="global_consumption")
     def global_consumption(self):
         """Global consumption without climate change"""
 
         # rff simulation means that GDP already exists out to 2300
         if 2300 in self.gdp.year:
-
             self.logger.debug("Global consumption found up to 2300.")
             global_cons = self.gdp.sum("region").rename("global_consumption")
         else:
-
             self.logger.info("Extrapolating global consumption.")
 
             # holding population constant
             # from 2100 to 2300 with 2099 values
             pop = self.collapsed_pop.sum("region")
             pop = pop.reindex(
                 year=range(pop.year.min().values, self.ext_end_year + 1),
@@ -903,23 +887,34 @@
 
         """
         # if parameter is share of consumption,
         # multiply by no-climate-change consumption
         if parameter <= 1:
             parameter = parameter * no_cc_consumption
 
-        w_utility = parameter ** (1 - self.eta) / (1 - self.eta)
-        bottom_utility = parameter ** (-self.eta) * (parameter - cc_consumption)
-        bottom_coded_cons = power(
-            ((1 - self.eta) * (w_utility - bottom_utility)), (1 / (1 - self.eta))
-        )
+        if self.eta == 1:
+            w_utility = np.log(parameter)
+            bottom_utility = np.power(parameter, -1) * (parameter - cc_consumption)
+            bottom_coded_cons = np.exp((w_utility - bottom_utility))
 
-        clipped_cons = xr.where(
-            cc_consumption > parameter, cc_consumption, bottom_coded_cons
-        )
+            clipped_cons = xr.where(
+                cc_consumption > parameter, cc_consumption, bottom_coded_cons
+            )
+        else:
+            w_utility = np.power(parameter, (1 - self.eta)) / (1 - self.eta)
+            bottom_utility = np.power(parameter, -self.eta) * (
+                parameter - cc_consumption
+            )
+            bottom_coded_cons = power(
+                ((1 - self.eta) * (w_utility - bottom_utility)), (1 / (1 - self.eta))
+            )
+
+            clipped_cons = xr.where(
+                cc_consumption > parameter, cc_consumption, bottom_coded_cons
+            )
 
         return clipped_cons
 
     @property
     def gmsl_max(self):
         """
         This function finds the GMSL value at which the damage function
@@ -932,15 +927,14 @@
             years, ssps, models, and if applicable, values of GMST
         """
 
         if self.formula in [
             "damages ~ -1 + anomaly + np.power(anomaly, 2) + gmsl + np.power(gmsl, 2)",
             "damages ~ -1 + gmsl + np.power(gmsl, 2)",
         ]:
-
             gmsl_max = -self.damage_function_coefficients["gmsl"] / (
                 2 * self.damage_function_coefficients["np.power(gmsl, 2)"]
             )
 
             # if the damage function curves up, there is no local max.
             # Thus there will be no linearization.
             gmsl_max = xr.where(
@@ -976,15 +970,14 @@
             formula=self.formula,
         )
 
         cc_cons = self.global_consumption - damages
 
         gc_no_pulse = []
         for wp in self.weitzman_parameter:
-
             gc = self.weitzman_min(
                 no_cc_consumption=self.global_consumption,
                 cc_consumption=cc_cons,
                 parameter=wp,
             )
             gc = gc.assign_coords({"weitzman_parameter": str(wp)})
 
@@ -1041,15 +1034,14 @@
     @save(name="marginal_damages")
     def marginal_damages(self):
         """Marginal damages due to additional pulse"""
 
         marginal_damages = []
 
         for agg in [i for i in self.fair_aggregation if i != "median"]:
-
             if agg == "ce":
                 md = self.ce_fair_no_pulse - self.ce_fair_pulse
             elif agg in ["mean", "gwr_mean"]:
                 md = self.global_consumption_no_pulse.mean(
                     self.fair_dims
                 ) - self.global_consumption_pulse.mean(self.fair_dims)
             elif agg == "median_params":
@@ -1273,15 +1265,14 @@
 
             # expand dims to match Euler
             discount_factors = self.calculate_discount_factors(array).expand_dims(
                 {"fair_aggregation": fair_aggregation}
             )
 
         elif "euler" in discounting_type:
-
             discount_factors = []
             for agg in [i for i in fair_aggregation if i != "median"]:
                 if agg == "ce":
                     factors = self.calculate_discount_factors(
                         self.ce_fair_no_pulse / pop
                     )
                 elif agg == "mean":
@@ -1289,15 +1280,14 @@
                         self.global_consumption_no_pulse.mean(self.fair_dims) / pop
                     )
                 elif agg == "gwr_mean":
                     factors = self.calculate_discount_factors(
                         self.global_consumption_no_pulse / full_pop
                     ).mean(self.fair_dims)
                 elif agg == "median_params":
-
                     median_params_damages = compute_damages(
                         self.climate.fair_median_params_control,
                         betas=self.damage_function_coefficients,
                         formula=self.formula,
                     )
 
                     median_params_consumption = (
@@ -1357,15 +1347,14 @@
             f[var].encoding.clear()
 
         return f
 
     @cachedproperty
     @save("uncollapsed_marginal_damages")
     def uncollapsed_marginal_damages(self):
-
         md = (
             (
                 (self.global_consumption_no_pulse - self.global_consumption_pulse)
                 * self.climate.conversion
             )
             .rename("marginal_damages")
             .to_dataset()
```

### Comparing `dscim-0.3.0/src/dscim/menu/risk_aversion.py` & `dscim-0.4.0/src/dscim/menu/risk_aversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
             pd.DataFrame
         """
 
         dams_collapse = (self.calculated_damages * self.collapsed_pop).sum(dim="region")
         df = dams_collapse.to_dataframe("damages").reset_index()
 
         if "gwr" in self.discounting_type:
-
             df = df.assign(
                 ssp=str(list(self.gdp.ssp.values)),
                 model=str(list(self.gdp.model.values)),
             )
 
         return df
```

### Comparing `dscim-0.3.0/src/dscim/menu/simple_storage.py` & `dscim-0.4.0/src/dscim/menu/simple_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,14 @@
         eta,
         gdppc_bottom_code,
         delta=None,
         histclim=None,
         ce_path=None,
         subset_dict=None,
     ):
-
         self.sector_path = sector_path
         self.save_path = save_path
         self.gdppc_bottom_code = gdppc_bottom_code
         self.subset_dict = subset_dict
         self.econ_vars = econ_vars
         self.climate = climate_vars
         self.delta = delta
```

### Comparing `dscim-0.3.0/src/dscim/preprocessing/README.md` & `dscim-0.4.0/src/dscim/preprocessing/README.md`

 * *Files identical despite different names*

### Comparing `dscim-0.3.0/src/dscim/preprocessing/climate/all_masks_rff.py` & `dscim-0.4.0/src/dscim/preprocessing/climate/all_masks_rff.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 ]
 
 # set list of masks to generate ('gdppc', 'emissions', 'climate')
 mask_types = ["gdppc", "emissions", "climate"]
 
 
 def get_mask(mask_set, quantiles, dim="rff_sp"):
-
     # quantiles of variable
     quants = mask_set.quantile(quantiles, dim)
 
     # assign False to values outside quantile bounds, else True
     mask = (
         xr.where(
             (mask_set >= quants.sel(quantile=quantiles[0]))
@@ -40,15 +39,14 @@
         .to_dataset()
     )
 
     return mask
 
 
 for mask_type in mask_types:
-
     if mask_type == "emissions":
         # mask on cumulative emissions in 2300
         mask_set = (
             xr.open_dataset(
                 "/shares/gcp/integration/rff/climate/rff-sp_emissions_all_gases.nc"
             )
             .emissions.sel(gas="C", drop=True)
```

### Comparing `dscim-0.3.0/src/dscim/preprocessing/climate/ssp_clipped_rff.py` & `dscim-0.4.0/src/dscim/preprocessing/climate/ssp_clipped_rff.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     (0.01, 0.99),
 ]
 
 years = range(2020, 2081, 10)
 
 
 def mask_year(args):
-
     year, q = args
 
     ssp_climate = "/shares/gcp/integration/float32/dscim_input_data/climate/AR6/ar6_fair162_sim_and_medianparams_control_pulse_2020-2030-2040-2050-2060-2070-2080_emis_conc_rf_temp_lambdaeff_emissions-driven_naturalfix_v4.0_Jan212022.nc"
     rff_folder = "/shares/gcp/integration/rff/climate/CO2_Fossil/"
     rff_file = "ar6_rff_iter0-19_fair162_CO2_Fossil_control_pulse_{}_temp_v5.02_newformat_Jan72022.nc"
     out_folder = "/shares/gcp/integration/rff/climate/CO2_Fossil/sspclipped/"
 
@@ -39,15 +38,14 @@
         xr.open_dataset(ssp_climate)
         .sel(pulse_year=year)
         .quantile(q[1], ["simulation"])
         .max("rcp")
     )
 
     for var in rff.keys():
-
         # index of sim-rff_sps which are out of bounds
         index = (
             rff[var]
             .where(((rff[var] > ssp_max[var]) | (rff[var] < ssp_min[var])), drop=True)
             .to_dataframe()
             .reset_index()
         )
```

### Comparing `dscim-0.3.0/src/dscim/preprocessing/climate/stack_iterations.py` & `dscim-0.4.0/src/dscim/preprocessing/climate/stack_iterations.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import sys
 
 USER = os.getenv("USER")
 from p_tqdm import p_map
 
 
 def stack(file, itr):
-
     ds = xr.open_dataset(file)
     ds = ds.rename({"simulation": "rff_sp"}).expand_dims({"simulation": [itr]})
 
     return ds
 
 
 print("Stacking climate iterations...")
```

### Comparing `dscim-0.3.0/src/dscim/preprocessing/climate/stack_masks.py` & `dscim-0.4.0/src/dscim/preprocessing/climate/stack_masks.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 # parameters
 dir = "/shares/gcp/integration/rff/climate/masks/CO2_Fossil"
 
 stack_list = [["gdppc", "emissions"], ["gdppc", "emissions", "climate"]]
 
 for stack in stack_list:
-
     # open all the relevant masks
     masks = p_map(xr.open_dataset, [f"{dir}/{s}_based_masks.nc4" for s in stack])
 
     # find the union of the first two
     union_mask = xr.ufuncs.logical_and(*masks[:2])
     if len(masks) > 2:
         # for each further mask, cumulatively find union with preceding masks
```

### Comparing `dscim-0.3.0/src/dscim/preprocessing/input_damages.py` & `dscim-0.4.0/src/dscim/preprocessing/input_damages.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Calculate damages from the projection system using VSL
 """
 
 import os
-import glob
 import re
 import logging
 import warnings
 import multiprocessing
 import numpy as np
 import pandas as pd
 import xarray as xr
@@ -91,14 +90,58 @@
     )
     df["exists"] = df.path.apply(lambda x: Path(x).exists())
     df["iam"] = df["model"].replace(moddict)
 
     return df.query(query)
 
 
+def concatenate_damage_output(damage_dir, basename, save_path):
+    """Concatenate labor/energy damage output across batches.
+
+    Parameters
+    ----------
+    damage_dir str
+        Directory containing separate labor/energy damage output files by batches.
+    basename str
+        Prefix of the damage output filenames (ex. {basename}_batch0.zarr)
+    save_path str
+        Path to save concatenated file in .zarr format
+    """
+    paths = [
+        f"{damage_dir}/{basename}_{b}.zarr"
+        for b in ["batch" + str(i) for i in range(0, 15)]
+    ]
+    data = xr.open_mfdataset(paths=paths, engine="zarr")
+
+    for v in data:
+        del data[v].encoding["chunks"]
+
+    chunkies = {
+        "batch": 15,
+        "rcp": 1,
+        "gcm": 1,
+        "model": 1,
+        "ssp": 1,
+        "region": -1,
+        "year": 10,
+    }
+
+    data = data.chunk(chunkies)
+
+    for v in list(data.coords.keys()):
+        if data.coords[v].dtype == object:
+            data.coords[v] = data.coords[v].astype("unicode")
+    data.coords["batch"] = data.coords["batch"].astype("unicode")
+    for v in list(data.variables.keys()):
+        if data[v].dtype == object:
+            data[v] = data[v].astype("unicode")
+
+    data.to_zarr(save_path, mode="w")
+
+
 def calculate_labor_impacts(input_path, file_prefix, variable, val_type):
     """Calculate impacts for labor results.
 
     Paramemters
     ----------
     input_path str
         Path to model/gcm/iam/rcp/ folder, usually from the
@@ -204,15 +247,17 @@
                 logger.error(f"Error in batch{i}: {e}")
                 pass
 
         # Concatenate file within batch
         conversion_value = 1.273526
         concat_ds = xr.combine_by_coords(list_damages_batch)
         for v in [f"histclim_{variable}", f"delta_{variable}"]:
-            concat_ds[v] = (concat_ds[v] / ec_cls.econ_vars.pop) * -1 * conversion_value
+            concat_ds[v] = (
+                (concat_ds[v] / ec_cls.econ_vars.pop.load()) * -1 * conversion_value
+            )
 
         # Save file
         file_name = f"{variable}_{val_type}_{i}"
         path_to_file = os.path.join(save_path, file_name)
 
         # convert to float32
         concat_ds = concat_ds.astype(np.float32)
@@ -320,15 +365,14 @@
         ds.coords["model"] = ds.model.str.replace("high", "OECD Env-Growth")
         ds.coords["model"] = ds.model.str.replace("low", "IIASA GDP")
         return ds
 
     def process_batch(g):
         i = g.batch.values[0]
         if i in [f"batch{j}" for j in batches]:
-
             print(f"Processing damages in {i}")
             ds = xr.open_mfdataset(g.path, preprocess=prep, parallel=True)[vars]
             attrs = ds.attrs
             ds = ds.sel({"year": slice(min_year, max_year)})
             # ag has missing 2099 damages so we fill these in with the 2098 damages
             ds = ds.reindex(year=range(min_year, max_year + 1), method="ffill")
 
@@ -340,21 +384,20 @@
                 for var in [
                     "continent",
                     "iam",
                     "Es_Ed",
                     "market_level",
                     "demand_topcode",
                 ]:
-
                     if var in ds.coords:
                         attrs[var] = ds[var].values
                         ds = ds.drop(var)
 
             # get in per capita 2019 PPP-adjusted USD damages
-            ds = (ds / pop) * -1 * 1.273526
+            ds = (ds / pop.load()) * -1 * 1.273526
 
             # replace infinite values with missings
             for var in ds.keys():
                 ds[var] = xr.where(np.isinf(ds[var]), np.nan, ds[var])
 
             if scalar is not None:
                 print("Scaling for reallocation.")
@@ -364,33 +407,35 @@
             return ds
         else:
             print(f"Skipped {i}.")
 
     batches = p_map(
         process_batch, [g for i, g in paths.groupby("batch")], num_cpus=num_cpus
     )
+    batches = [ds for ds in batches if ds is not None]
     chunkies = {
         "rcp": 1,
-        "region": 24378,
+        "region": -1,
         "gcm": 1,
         "year": 10,
         "model": 1,
         "ssp": 1,
         "batch": 15,
     }
     batches = (
         xr.concat(batches, "batch", combine_attrs="override")
         .chunk(chunkies)
         .drop("variable")
         .squeeze()
     )
     batches = xr.where(np.isinf(batches), np.nan, batches)
+    batches = batches.astype(np.float32)
 
-    batches.rename({"wc_reallocation": varname})[varname].to_zarr(
-        save_path, mode="a", consolidated=True
+    batches.rename({"wc_reallocation": varname})[varname].to_dataset().to_zarr(
+        store=save_path, mode="a", consolidated=True
     )
 
 
 def read_energy_files(df, seed="TINV_clim_price014_total_energy_fulladapt-histclim"):
     """Read energy CSV files and trasnform them to Xarray objects
 
     This function reads a dataframe with the filesystem metadata (from
@@ -434,15 +479,15 @@
             pass
 
         damages_arr.to_netcdf(os.path.join(row.path, f"{seed}.nc4"))
 
     return None
 
 
-def read_energy_files_parallel(input_path, save_path, ec_cls, **kwargs):
+def read_energy_files_parallel(input_path, **kwargs):
     """Concatenate energy results from CSV to NetCDF by batches using
     multiprocessing
 
     This function takes all CSV files per batch and maps the
     ``read_energy_files`` function to all the files within a batch. The files
     will be saved in the same path as the CSV files but in NetCDF format.
 
@@ -452,17 +497,14 @@
     with a ``EconVars`` class and then calculate 2019 USD damages
 
     Parameters
     ----------
     input_path : str
         Path to root folder organized by batch containing all projection system
         files
-    save_path : str
-        Path to saved damages by batch files
-    ec_cls : ``dscim.menu.simple_storage.EconVars``
     **kwargs
         Other elements too the ``read_energy_files`` damages
 
     Returns
     ------
         None
     """
@@ -585,15 +627,17 @@
                 logger.error(f"Error in batch{i}: {e}")
                 pass
 
         # Concatenate file within batch
         conversion_value = 1.273526
         concat_ds = xr.combine_by_coords(list_damages_batch)
         for v in [f"histclim_{variable}", f"delta_{variable}"]:
-            concat_ds[v] = (concat_ds[v] / ec_cls.econ_vars.pop) * conversion_value
+            concat_ds[v] = (
+                concat_ds[v] / ec_cls.econ_vars.pop.load()
+            ) * conversion_value
 
         # Save file
         file_name = f"{variable}_{i}"
         path_to_file = os.path.join(save_path, file_name)
 
         # convert to float32
         concat_ds = concat_ds.astype(np.float32)
@@ -632,22 +676,18 @@
     save_path="/shares/gcp/integration/float32/input_data_histclim/energy_data/replication_2022aug/",
 ):
     ec = EconVars(path_econ)
 
     if re_calculate:
         read_energy_files_parallel(
             input_path=input_path,
-            save_path=save_path,
-            ec_cls=ec,
             seed="TINV_clim_integration_total_energy_delta",
         )
         read_energy_files_parallel(
             input_path=input_path,
-            save_path=save_path,
-            ec_cls=ec,
             seed="TINV_clim_integration_total_energy_histclim",
         )
 
     # process in 3 rounds to limit memory usage
     for i in range(0, 3):
         partial_func = partial(
             calculate_energy_batch_damages,
@@ -661,87 +701,168 @@
 
 
 def prep_mortality_damages(
     gcms,
     paths,
     vars,
     outpath,
-    path_econ="/shares/gcp/integration/float32/dscim_input_data/econvars/zarrs/integration-econ-bc39.zarr",
+    mortality_version,
+    path_econ,
 ):
-
-    print(
-        "This function only works on mortality_v4 and mortality_v5 damages from the mortality repo's valuation. Earlier versions of mortality contain different variable definitions (per capita, not per capita, with or without histclim subtracted off."
-    )
-
     ec = EconVars(path_econ=path_econ)
 
     # longest-string gcm has to be processed first so the coordinate is the right str length
     gcms = sorted(gcms, key=len, reverse=True)
 
-    for i, gcm in enumerate(gcms):
-        print(gcm, i, "/", len(gcms))
+    if mortality_version == 0:
+        scaling_deaths = "epa_scaled"
+        scaling_costs = "epa_scaled"
+        valuation = "vly"
+    elif mortality_version == 1:
+        scaling_deaths = "epa_iso_scaled"
+        scaling_costs = "epa_scaled"
+        valuation = "vsl"
+    elif mortality_version == 4:
+        scaling_deaths = "epa_popavg"
+        scaling_costs = "epa_scaled"
+        valuation = "vsl"
+    elif mortality_version == 5:
+        scaling_deaths = "epa_row"
+        scaling_costs = "epa_scaled"
+        valuation = "vsl"
+    else:
+        raise ValueError("Mortality version not valid: ", str(mortality_version))
+
+    # We set 0 population to infinity so that per capita damages are 0 in locations with 0 population
+    pop = ec.econ_vars.pop.load()
+    pop = xr.where(pop == 0, np.Inf, pop)
 
-        def prep(ds, gcm=gcm):
-            return ds.sel(gcm=gcm).drop("gcm")
+    for i, gcm in enumerate(gcms):
+        print(gcm, i + 1, "/", len(gcms))
 
         data = {}
-        for var, name in vars.items():
-            data[var] = xr.open_mfdataset(paths[var], preprocess=prep, parallel=True)[
-                name
-            ]
+
+        def prep(
+            ds,
+            gcm=gcm,
+            scaling_deaths=scaling_deaths,
+            scaling_costs=scaling_costs,
+            valuation=valuation,
+        ):
+            if scaling_deaths == scaling_costs:
+                return ds.sel(
+                    gcm=gcm,
+                    scaling=[scaling_deaths],
+                    valuation=valuation,
+                ).drop(["gcm", "valuation"])
+            else:
+                return ds.sel(
+                    gcm=gcm,
+                    scaling=[scaling_deaths, scaling_costs],
+                    valuation=valuation,
+                ).drop(["gcm", "valuation"])
+
+        data = xr.open_mfdataset(paths, preprocess=prep, parallel=True, engine="zarr")
 
         damages = xr.Dataset(
             {
                 "delta": (
-                    data["delta_deaths"] - data["histclim_deaths"] + data["delta_costs"]
+                    data[vars["delta_deaths"]].sel(scaling=scaling_deaths, drop=True)
+                    - data[vars["histclim_deaths"]].sel(
+                        scaling=scaling_deaths, drop=True
+                    )
+                    + data[vars["delta_costs"]].sel(scaling=scaling_costs, drop=True)
+                )
+                / pop,
+                "histclim": data[vars["histclim_deaths"]].sel(
+                    scaling=scaling_deaths, drop=True
                 )
-                / ec.econ_vars.pop.load(),
-                "histclim": data["histclim_deaths"] / ec.econ_vars.pop.load(),
+                / pop,
             }
         ).expand_dims({"gcm": [gcm]})
 
         damages = damages.chunk(
-            {"batch": 15, "ssp": 1, "model": 1, "rcp": 1, "gcm": 1, "year": 10}
+            {
+                "batch": 15,
+                "ssp": 1,
+                "model": 1,
+                "rcp": 1,
+                "gcm": 1,
+                "year": 10,
+                "region": -1,
+            }
         )
         damages.coords.update({"batch": [f"batch{i}" for i in damages.batch.values]})
 
         # convert to EPA VSL
         damages = damages * 0.90681089
+        damages = damages.astype(np.float32)
+
+        for v in list(damages.coords.keys()):
+            if damages.coords[v].dtype == object:
+                damages.coords[v] = damages.coords[v].astype("unicode")
+
+        for v in list(damages.variables.keys()):
+            if damages[v].dtype == object:
+                damages[v] = damages[v].astype("unicode")
 
         if i == 0:
             damages.to_zarr(
-                outpath,
+                f"{outpath}/impacts-darwin-montecarlo-damages-v{mortality_version}.zarr",
                 consolidated=True,
                 mode="w",
             )
         else:
             damages.to_zarr(
-                outpath,
+                f"{outpath}/impacts-darwin-montecarlo-damages-v{mortality_version}.zarr",
                 consolidated=True,
                 append_dim="gcm",
             )
 
         for v in data.values():
             v.close()
         damages.close()
 
 
 def coastal_inputs(
     version,
-    adapt_type,
-    vsl_valuation,
     path,
+    adapt_type,
+    vsl_valuation=None,
 ):
-
     try:
         d = xr.open_zarr(f"{path}/coastal_damages_{version}.zarr")
     except GroupNotFoundError:
         print(f"Zarr not found: {path}/coastal_damages_{version}.zarr")
         exit()
 
-    d = d.sel(adapt_type=adapt_type, vsl_valuation=vsl_valuation, drop=True)
-
-    d.to_zarr(
-        f"{path}/coastal_damages_{version}-{adapt_type}-{vsl_valuation}.zarr",
-        consolidated=True,
-        mode="w",
-    )
+    if "vsl_valuation" in d.coords:
+        if vsl_valuation is None:
+            raise ValueError(
+                "vsl_valuation is a coordinate in the input dataset but is set to None. Please provide a value for vsl_valuation by which to subset the input dataset."
+            )
+        else:
+            d = d.sel(adapt_type=adapt_type, vsl_valuation=vsl_valuation, drop=True)
+            chunkies = {
+                "batch": 15,
+                "ssp": 1,
+                "model": 1,
+                "slr": 1,
+                "year": 10,
+                "region": -1,
+            }
+            d = d.chunk(chunkies)
+            d.to_zarr(
+                f"{path}/coastal_damages_{version}-{adapt_type}-{vsl_valuation}.zarr",
+                consolidated=True,
+                mode="w",
+            )
+    else:
+        print(
+            "vsl_valuation is not a dimension of the input dataset, subset adapt_type only"
+        )
+        d = d.sel(adapt_type=adapt_type, drop=True)
+        d.to_zarr(
+            f"{path}/coastal_damages_{version}-{adapt_type}.zarr",
+            consolidated=True,
+            mode="w",
+        )
```

### Comparing `dscim-0.3.0/src/dscim/preprocessing/midprocessing.py` & `dscim-0.4.0/src/dscim/preprocessing/midprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     output,
     recipe,
     disc,
     eta,
     rho,
     fit=True,
 ):
-
     os.makedirs(output, exist_ok=True)
     shutil.copy2(
         f"{input}/{recipe}_{disc}_eta{eta}_rho{rho}_damage_function_coefficients.nc4",
         output,
     )
 
     if fit:
@@ -37,15 +36,14 @@
     coastal,
     AMEL,
     input_dir,
     mask="unmasked",
     pulse_year=2020,
     fit=True,
 ):
-
     print(f"Creating {recipe} {disc} for {CAMEL}...")
     os.makedirs(f"{input_dir}/{CAMEL}/{pulse_year}/{mask}", exist_ok=True)
 
     coefs, fit = {}, {}
 
     for sector in [coastal, AMEL]:
         coefs[
@@ -69,15 +67,14 @@
     }
 
     coefs["combined"].to_netcdf(
         f"{input_dir}/{CAMEL}/{pulse_year}/{mask}/{recipe}_{disc}_eta{eta}_rho{rho}_damage_function_coefficients.nc4"
     )
 
     if fit:
-
         for sector in [coastal, AMEL]:
             fit[
                 sector
             ] = f"{input_dir}/{sector}/{pulse_year}/{mask}/{recipe}_{disc}_eta{eta}_rho{rho}_damage_function_fit.nc4"
 
         fit["combined"] = xr.open_dataset(fit[coastal]) + xr.open_dataset(fit[AMEL])
```

### Comparing `dscim-0.3.0/src/dscim/preprocessing/misc/bottom_code_econ_zarr.py` & `dscim-0.4.0/src/dscim/preprocessing/misc/bottom_code_econ_zarr.py`

 * *Files identical despite different names*

### Comparing `dscim-0.3.0/src/dscim/preprocessing/misc/check_nans.py` & `dscim-0.4.0/src/dscim/preprocessing/misc/check_nans.py`

 * *Files identical despite different names*

### Comparing `dscim-0.3.0/src/dscim/preprocessing/misc/convert_float32.py` & `dscim-0.4.0/src/dscim/preprocessing/misc/convert_float32.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,27 +81,24 @@
 
 def process_csv(f):
     shutil.copyfile(f, f.replace(input_root, output_root))
     return f"copied: {f}"
 
 
 if convert_csv:
-
     i_csv = p_uimap(process_csv, files_csv)
     with open(f"{output_root}/log_csv.csv", "w", newline="") as write_file:
         write = csv.writer(write_file)
         write.writerows([r] for r in i_csv)
 
 
 if convert_zarr:
-
     i_zarr = p_uimap(process_zarr, files_zarr)
     with open(f"{output_root}/log_zarr.csv", "w", newline="") as write_file:
         write = csv.writer(write_file)
         write.writerows([r] for r in i_zarr)
 
 if convert_nc4:
-
     i_nc4 = p_uimap(process_nc4, files_nc4, num_cpus=8)
     with open(f"{output_root}/log_nc4.csv", "w", newline="") as write_file:
         write = csv.writer(write_file)
         write.writerows([r] for r in i_nc4)
```

### Comparing `dscim-0.3.0/src/dscim/utils/functions.py` & `dscim-0.4.0/src/dscim/utils/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dscim.utils.utils import power
 
 
 def ce_func(consumption, dims, eta):
     """Calculate CRRA function"""
     # use log utility when eta is 1
     if eta == 1:
-        return xr.ufuncs.exp(xr.ufuncs.log(consumption).mean(dims))
+        return np.exp(np.log(consumption).mean(dims))
     # CRRA utility otherwise
     else:
         return power(
             (power(consumption, (1 - eta)) / (1 - eta)).mean(dims) * (1 - eta),
             (1 / (1 - eta)),
         )
 
@@ -139,15 +139,14 @@
         input_core_dims=[[], ["year"]],
         vectorize=True,
     )
     return constant_discount_rates
 
 
 def get_model_weights(rcp):
-
     # clean weights
     WEIGHT_FILE = (
         f"/shares/gcp/climate/SMME-weights/{rcp}_2090_SMME_edited_for_April_2016.tsv"
     )
     weights = pd.read_csv(
         WEIGHT_FILE, sep="\t", usecols=["quantile", "model", "weight"]
     )
```

### Comparing `dscim-0.3.0/src/dscim/utils/generate_yaml.py` & `dscim-0.4.0/src/dscim/utils/generate_yaml.py`

 * *Files identical despite different names*

### Comparing `dscim-0.3.0/src/dscim/utils/menu_runs.py` & `dscim-0.4.0/src/dscim/utils/menu_runs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dscim.menu.simple_storage import Climate, EconVars
 import dscim.menu.baseline
 import dscim.menu.risk_aversion
 import dscim.menu.equity
+from pathlib import Path
 
 import os
 import gc
 import time
 import yaml
 
 USER = os.getenv("USER")
@@ -32,35 +33,45 @@
     eta_rhos,
     config,
     USA,
     AR,
     masks=None,
     fair_dims_list=None,
     order="damage_function",
+    regenerate_sccs=True,
 ):
     if masks is None:
         masks = [None]
     if fair_dims_list is None:
         fair_dims_list = [["simulation"]]
 
     with open(config, "r") as stream:
         conf = yaml.safe_load(stream)
 
     for sector, pulse_year, menu_disc, eta_rho, mask, fair_dims in product(
-        sectors, pulse_years, menu_discs, eta_rhos.items(), masks, fair_dims_list
+        sectors, pulse_years, menu_discs, eta_rhos, masks, fair_dims_list
     ):
-
         menu_option, discount_type = menu_disc
         save_path = f"{conf['paths'][f'AR{AR}_ssp_results']}/{sector}/{pulse_year}/"
 
         if mask is not None:
             save_path = save_path + "/" + mask
         else:
             save_path = save_path + "/" + "unmasked"
 
+        if not regenerate_sccs:
+            scc_path = (
+                Path(save_path)
+                / "unmasked"
+                / f"{menu_option}_{discount_type}_eta{eta_rho[0]}_rho{eta_rho[1]}_sccs.nc4"
+            )
+            if scc_path.is_file():
+                print("sccs found")
+                continue
+
         if fair_dims != ["simulation"]:
             save_path = (
                 save_path
                 + "/"
                 + f"fair_collapsed_{'_'.join([i for i in fair_dims if i!='simulation'])}"
             )
 
@@ -115,26 +126,35 @@
     sectors,
     pulse_years,
     menu_discs,
     eta_rhos,
     config,
     USA,
     order="scc",
+    regenerate_sccs=True,
 ):
-
     with open(config, "r") as stream:
         conf = yaml.safe_load(stream)
 
     for sector, pulse_year, menu_disc, eta_rho in product(
-        sectors, pulse_years, menu_discs, eta_rhos.items()
+        sectors, pulse_years, menu_discs, eta_rhos
     ):
-
         menu_option, discount_type = menu_disc
         save_path = f"{conf['paths']['rff_results']}/{sector}/{pulse_year}/unmasked"
 
+        if not regenerate_sccs:
+            scc_path = (
+                Path(save_path)
+                / "unmasked"
+                / f"{menu_option}_{discount_type}_eta{eta_rho[0]}_rho{eta_rho[1]}_sccs.nc4"
+            )
+            if scc_path.is_file():
+                print("sccs found")
+                continue
+
         if USA:
             econ = EconVars(
                 path_econ=f"{conf['rffdata']['socioec_output']}/rff_USA_socioeconomics.nc4"
             )
         else:
             econ = EconVars(
                 path_econ=f"{conf['rffdata']['socioec_output']}/rff_global_socioeconomics.nc4"
```

### Comparing `dscim-0.3.0/src/dscim/utils/plotting_utils.py` & `dscim-0.4.0/src/dscim/utils/plotting_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,25 @@
     """
 
     def __init__(self):
         super().__init__(base=10.0, linthresh=1.0)
 
     @staticmethod
     def orders_magnitude(vmin, vmax):
-
         max_size = np.log10(max(abs(vmax), 1))
         min_size = np.log10(max(abs(vmin), 1))
 
         if vmax > 1 and vmin > 1:
             return max_size - min_size
         elif vmax < -1 and vmin < -1:
             return min_size - max_size
         else:
             return max(min_size, max_size)
 
     def tick_values(self, vmin, vmax):
-
         if vmax < vmin:
             vmin, vmax = vmax, vmin
 
         orders_magnitude = self.orders_magnitude(vmin, vmax)
 
         if orders_magnitude <= 1:
             spread = vmax - vmin
@@ -58,15 +56,14 @@
                 10 ** np.linspace(neg_b, neg_a, int(neg_a - neg_b) + 1)[::-1]
             )
             negative = np.ravel(np.outer(negative_powers, [1.0, 5.0]))
 
             return np.concatenate([negative, linear, positive])
 
         else:
-
             pos_a, pos_b = np.floor(np.log10(max(vmin, 1))), np.ceil(
                 np.log10(max(vmax, 1))
             )
             positive = 10 ** np.linspace(pos_a, pos_b, int(pos_b - pos_a) + 1)
 
             linear = np.array([0.0]) if vmin < 1 and vmax > -1 else np.array([])
```

### Comparing `dscim-0.3.0/src/dscim/utils/utils.py` & `dscim-0.4.0/src/dscim/utils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -295,45 +295,47 @@
 
     if negative_values != 0:
         raise ValueError(
             "Negative values were passed to the certainty equivalence function"
         )
 
     if func is None:
-        exp = 1 / (1 - eta)
-        utility = np.true_divide(array ** (1 - eta), (1 - eta))
+        if eta == 1:
+            utility = np.log(array)
+        else:
+            exp = 1 / (1 - eta)
+            utility = np.true_divide(array ** (1 - eta), (1 - eta))
 
         if weights is None:
             exp_utility = utility.mean(dim=dims)
         else:
             exp_utility = utility.weighted(weights).mean(dim=dims)
 
-        ce_array = (exp_utility * (1 - eta)) ** exp
+        if eta == 1:
+            ce_array = np.exp(exp_utility)
+        else:
+            ce_array = (exp_utility * (1 - eta)) ** exp
 
     else:
         try:
             ce_array = array.map_partitions(func, **func_args)
         except Exception as exception:
             raise ValueError(f"Custom function not conforming with array: {exception}")
 
     return ce_array
 
 
 def model_outputs(
     damage_function,
     extrapolation_type,
     formula,
-    extrap_formula,
     year_range,
-    extrap_year,
     year_start_pred,
-    year_end_pred,
     quantiles,
     global_c=None,
-    base_year=2010,
     min_anomaly=0,
     max_anomaly=20,
     step_anomaly=0.2,
     min_gmsl=0,
     max_gmsl=300,
     step_gmsl=3,
     type_estimation="ols",
@@ -349,32 +351,20 @@
     Parameters
     ----------
     damage_function: pandas.DataFrame
         A global damage function.
     type_estimation: str
         Type of model use for damage function fitting: `ols`, `quantreg`
     extrapolation_type : str
-        Type of extrapolation: `global_c_ratio`, `time_trends`
+        Type of extrapolation: `global_c_ratio`
     global_c : xr.DataArray
         Array with global consumption extrapolated to 2300. This is only used
         when ``extrapolation_type`` is ``global_c_ratio``.
-    fix_global_c : int
-        Year to fix damages and use as base to the ``global_c_ratio``
-        extrapolation. Default value is 2099.
-    base_year: int
-        Base year for `time_trends` rebasing.
-    interp_year: int
-        Year pre-2100 to fit damages used for linear extrapolation.
-        i.e. If `interp_year=2085`, data from years 2085 to 2099 will be
-        used to extrapolate data to years post-2100. 2085 is the default.
-        Only used in `time_trends` rebasing.
     year_start_pred: int
         Start of extrapolation
-    year_end_pred: int
-        End of extrapolation
     year_range: sequence, lst, tuple, range
         Range of years to estimate over. Default is 2010 to 2100
 
     Returns
     ------
 
     dict
@@ -385,40 +375,22 @@
 
     # set year of prediction for global C extrapolation
     fix_global_c = year_start_pred - 1
 
     # set exogenous variables for predictions
     gmsl = np.arange(min_gmsl, max_gmsl, step_gmsl)
     temps = np.arange(min_anomaly, max_anomaly, step_anomaly)
-    extrap_years = range(year_start_pred, year_end_pred + 1)
 
     if ("anomaly" in damage_function.columns) and ("gmsl" in damage_function.columns):
         exog_X = pd.DataFrame(product(temps, gmsl))
         exog = dict(anomaly=exog_X.values[:, 0], gmsl=exog_X.values[:, 1])
-
-        extrap_X = pd.DataFrame(product(temps, extrap_years, gmsl))
-        extrap_exog = dict(
-            anomaly=extrap_X.values[:, 0],
-            year_rebase=extrap_X.values[:, 1] - base_year,
-            gmsl=extrap_X.values[:, 2],
-        )
     elif "anomaly" in damage_function.columns:
         exog = dict(anomaly=temps)
-
-        extrap_X = pd.DataFrame(product(temps, extrap_years))
-        extrap_exog = dict(
-            anomaly=extrap_X.values[:, 0], year_rebase=extrap_X.values[:, 1] - base_year
-        )
     elif "gmsl" in damage_function.columns:
         exog = dict(gmsl=gmsl)
-
-        extrap_X = pd.DataFrame(product(gmsl, extrap_years))
-        extrap_exog = dict(
-            gmsl=extrap_X.values[:, 0], year_rebase=extrap_X.values[:, 1] - base_year
-        )
     else:
         print("Independent variables not found.")
 
     # Rolling window estimation (5-yr)
     list_params, list_y_hats = [], []
 
     for year in year_range:
@@ -436,58 +408,15 @@
         list_params.append(params)
         list_y_hats.append(y_hat)
 
     # Concatenate results
     param_df = pd.concat(list_params)
     y_hat_df = pd.concat(list_y_hats)
 
-    if extrapolation_type == "time_trends":
-
-        raise NotImplementedError(
-            "This has not been tested since adding quantregs option."
-        )
-
-        # Linear-extrapolation for post-2100 years
-        df_extrap = damage_function[damage_function.year >= extrap_year]
-        df_extrap = df_extrap.assign(year_rebase=df_extrap.year - base_year)
-
-        extrap_params, extrap_y_hat = modeler(
-            df=df_extrap,
-            formula=extrap_formula,
-            type_estimation=type_estimation,
-            exog=extrap_exog,
-        )
-        extrap_y_hat = extrap_y_hat.drop(columns="year_rebase")
-        extrap_y_hat["year"] = extrap_X.values[:, 1]
-
-        # Reformulating parameters
-        extrapolation_year = []
-        for year in extrap_years:
-
-            params_df = extrap_params.copy(deep=True)
-            unint_terms = int(len(params_df.columns) / 2)
-
-            # sum uninteracted terms with matching (interacted term * rebased year)
-            for i in range(0, unint_terms):
-                params_df.iloc[:, i] = params_df.iloc[:, i] + params_df.iloc[
-                    :, (unint_terms + i)
-                ] * (year - base_year)
-
-            params_df = params_df.iloc[:, range(0, unint_terms)]
-
-            params_df = params_df.assign(year=year)
-            extrapolation_year.append(params_df)
-
-        extrapolation_results = pd.concat(extrapolation_year)
-
-        parameters = pd.concat([param_df, extrapolation_results]).to_xarray()
-        preds = pd.concat([y_hat_df, extrap_y_hat]).to_xarray()
-
-    elif extrapolation_type == "global_c_ratio":
-
+    if extrapolation_type == "global_c_ratio":
         # convert to xarray immediately
         index = ["year", "q"] if type_estimation == "quantreg" else ["year"]
         y_hat_df = y_hat_df.set_index(
             [i for i in y_hat_df.columns if "y_hat" not in i]
         ).to_xarray()
         param_df = param_df.set_index(index).to_xarray()
 
@@ -590,66 +519,58 @@
         ] * anomaly.gmsl * np.power(
             anomaly.temperature, 2
         )
     elif (
         formula
         == "damages ~ -1 + anomaly + np.power(anomaly, 2) + gmsl + np.power(gmsl, 2)"
     ):
-
         damages_fair = (
             betas["anomaly"] * anomaly.temperature
             + betas["np.power(anomaly, 2)"] * np.power(anomaly.temperature, 2)
             + betas["gmsl"] * anomaly.gmsl
             + betas["np.power(gmsl, 2)"] * np.power(anomaly.gmsl, 2)
         )
     elif (
         formula == "damages ~ anomaly + np.power(anomaly, 2) + gmsl + np.power(gmsl, 2)"
     ):
-
         damages_fair = (
             betas["Intercept"]
             + betas["anomaly"] * anomaly.temperature
             + betas["np.power(anomaly, 2)"] * np.power(anomaly.temperature, 2)
             + betas["gmsl"] * anomaly.gmsl
             + betas["np.power(gmsl, 2)"] * np.power(anomaly.gmsl, 2)
         )
     elif formula == "damages ~ -1 + gmsl + anomaly + np.power(anomaly, 2)":
-
         damages_fair = (
             betas["anomaly"] * anomaly.temperature
             + betas["np.power(anomaly, 2)"] * np.power(anomaly.temperature, 2)
             + betas["gmsl"] * anomaly.gmsl
         )
 
     elif formula == "damages ~ -1 + anomaly + np.power(anomaly, 2)":
-
         damages_fair = betas["anomaly"] * anomaly.temperature + betas[
             "np.power(anomaly, 2)"
         ] * np.power(anomaly.temperature, 2)
 
     elif formula == "damages ~ anomaly + np.power(anomaly, 2)":
-
         damages_fair = (
             betas["Intercept"]
             + betas["anomaly"] * anomaly.temperature
             + betas["np.power(anomaly, 2)"] * np.power(anomaly.temperature, 2)
         )
     elif formula == "damages ~ gmsl + np.power(gmsl, 2)":
-
         damages_fair = (
             betas["Intercept"]
             + betas["gmsl"] * anomaly.gmsl
             + betas["np.power(gmsl, 2)"] * np.power(anomaly.gmsl, 2)
         )
     elif formula == "damages ~ -1 + gmsl + np.power(gmsl, 2)":
-
         damages_fair = betas["gmsl"] * anomaly.gmsl + betas[
             "np.power(gmsl, 2)"
         ] * np.power(anomaly.gmsl, 2)
     elif formula == "damages ~ -1 + gmsl":
-
         damages_fair = betas["gmsl"] * anomaly.gmsl
 
     elif formula == "damages ~ -1 + np.power(anomaly, 2)":
         damages_fair = betas["np.power(anomaly, 2)"] * np.power(anomaly.temperature, 2)
 
     return damages_fair
```

### Comparing `dscim-0.3.0/src/dscim.egg-info/PKG-INFO` & `dscim-0.4.0/src/dscim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dscim
-Version: 0.3.0
+Version: 0.4.0
 Summary: Data-Driven Spatial Climate Impact Model core component code
 Project-URL: Homepage, https://github.com/ClimateImpactLab/dscim
 Project-URL: Documentation, https://github.com/ClimateImpactLab/dscim
 Project-URL: Source, https://github.com/ClimateImpactLab/dscim
 Project-URL: Bug Tracker, https://github.com/ClimateImpactLab/dscim/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `dscim-0.3.0/src/dscim.egg-info/SOURCES.txt` & `dscim-0.4.0/src/dscim.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,56 +5,38 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 .github/workflows/python-publish.yaml
 .github/workflows/pythonpackage.yaml
 src/dscim/__init__.py
-src/dscim/cli.py
 src/dscim/descriptors.py
 src/dscim.egg-info/PKG-INFO
 src/dscim.egg-info/SOURCES.txt
 src/dscim.egg-info/dependency_links.txt
 src/dscim.egg-info/top_level.txt
-src/dscim/diagnostics/__init__.py
-src/dscim/diagnostics/batch_maps.py
-src/dscim/diagnostics/compare_sccs.py
-src/dscim/diagnostics/crayola_plots.py
-src/dscim/diagnostics/damage_function.py
-src/dscim/diagnostics/damage_inc_share_boxplots.py
-src/dscim/diagnostics/discount_rates.py
-src/dscim/diagnostics/equity_risk_premiums.py
-src/dscim/diagnostics/fair_step.py
-src/dscim/diagnostics/global_consumption.py
-src/dscim/diagnostics/maps.py
-src/dscim/diagnostics/stacked_damage_function.py
-src/dscim/diagnostics/var_timeseries.py
-src/dscim/fair/__init__.py
 src/dscim/menu/__init__.py
 src/dscim/menu/baseline.py
 src/dscim/menu/decorators.py
 src/dscim/menu/equity.py
 src/dscim/menu/main_recipe.py
 src/dscim/menu/risk_aversion.py
 src/dscim/menu/simple_storage.py
 src/dscim/preprocessing/README.md
 src/dscim/preprocessing/__init__.py
 src/dscim/preprocessing/input_damages.py
 src/dscim/preprocessing/midprocessing.py
-src/dscim/preprocessing/mortality_inputs_archived.py
 src/dscim/preprocessing/preprocessing.py
 src/dscim/preprocessing/climate/all_masks_rff.py
-src/dscim/preprocessing/climate/reformat.py
 src/dscim/preprocessing/climate/ssp_clipped_rff.py
 src/dscim/preprocessing/climate/stack_iterations.py
 src/dscim/preprocessing/climate/stack_masks.py
 src/dscim/preprocessing/misc/bottom_code_econ_zarr.py
 src/dscim/preprocessing/misc/check_nans.py
 src/dscim/preprocessing/misc/convert_float32.py
 src/dscim/utils/__init__.py
-src/dscim/utils/dicts.py
 src/dscim/utils/functions.py
 src/dscim/utils/generate_yaml.py
 src/dscim/utils/menu_runs.py
 src/dscim/utils/plotting_utils.py
 src/dscim/utils/rff.py
 src/dscim/utils/utils.py
```

