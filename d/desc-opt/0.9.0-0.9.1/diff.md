# Comparing `tmp/desc-opt-0.9.0.tar.gz` & `tmp/desc-opt-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desc-opt-0.9.0.tar", last modified: Fri Jun 16 20:49:51 2023, max compression
+gzip compressed data, was "desc-opt-0.9.1.tar", last modified: Thu Jul  6 02:02:57 2023, max compression
```

## Comparing `desc-opt-0.9.0.tar` & `desc-opt-0.9.1.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:49:51.587927 desc-opt-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-16 20:48:40.000000 desc-opt-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-16 20:48:40.000000 desc-opt-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-16 20:49:51.587927 desc-opt-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-16 20:48:40.000000 desc-opt-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:49:51.587927 desc-opt-0.9.0/desc/
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-16 20:49:51.587927 desc-opt-0.9.0/desc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    45395 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/basis.py
--rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/coils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:49:51.539926 desc-opt-0.9.0/desc/compute/
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/compute/_basis_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/compute/_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    47023 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/compute/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/compute/_equil.py
--rw-r--r--   0 runner    (1001) docker     (123)    81999 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/compute/_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/compute/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    45531 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/compute/_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    30037 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/compute/_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/compute/_qs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/compute/_stability.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/compute/data_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    27215 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/compute/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/continuation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/derivatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:49:51.543926 desc-opt-0.9.0/desc/equilibrium/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/equilibrium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46604 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/equilibrium/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/equilibrium/coords.py
--rw-r--r--   0 runner    (1001) docker     (123)    38755 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/equilibrium/equilibrium.py
--rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/equilibrium/initial_guess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/equilibrium/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:49:51.571926 desc-opt-0.9.0/desc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)  2781266 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/examples/ARIES-CS_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)  1854489 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/examples/ATF_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)   974880 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/examples/DSHAPE_CURRENT_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)   974880 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/examples/DSHAPE_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)  1515598 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/examples/ESTELL_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)  1003793 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/examples/HELIOTRON_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)  3109450 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/examples/NCSX_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)  3059745 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/examples/QAS_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)   650984 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/examples/SOLOVEV_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)  3500803 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/examples/W7-X_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)  1942753 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/examples/WISTELL-A_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/examples/precise_QA.py
--rw-r--r--   0 runner    (1001) docker     (123)  4020724 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/examples/precise_QA_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/examples/precise_QH.py
--rw-r--r--   0 runner    (1001) docker     (123)  4017915 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/examples/precise_QH_output.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:49:51.579927 desc-opt-0.9.0/desc/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/geometry/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    40845 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/geometry/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    35258 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/geometry/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/geometry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    44783 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:49:51.579927 desc-opt-0.9.0/desc/io/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/io/ascii_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/io/core_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/io/equilibrium_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/io/hdf5_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    58768 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/io/input_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/io/pickle_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    24850 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/magnetic_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:49:51.579927 desc-opt-0.9.0/desc/objectives/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/objectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/objectives/_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    30125 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/objectives/_equilibrium.py
--rw-r--r--   0 runner    (1001) docker     (123)    20944 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/objectives/_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    33678 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/objectives/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    21629 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/objectives/_qs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13318 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/objectives/_stability.py
--rw-r--r--   0 runner    (1001) docker     (123)    83665 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/objectives/linear_objectives.py
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/objectives/nae_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/objectives/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    34300 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/objectives/objective_funs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/objectives/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:49:51.583927 desc-opt-0.9.0/desc/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25793 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/optimize/_constraint_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/optimize/_desc_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28726 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/optimize/_scipy_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/optimize/aug_lagrangian.py
--rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/optimize/aug_lagrangian_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/optimize/bound_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15020 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/optimize/fmin_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/optimize/least_squares.py
--rw-r--r--   0 runner    (1001) docker     (123)    18916 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/optimize/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/optimize/stochastic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/optimize/tr_subproblems.py
--rw-r--r--   0 runner    (1001) docker     (123)    15629 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/optimize/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (123)   120469 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    43879 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    29582 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    59913 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/vmec.py
--rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-06-16 20:48:40.000000 desc-opt-0.9.0/desc/vmec_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:49:51.583927 desc-opt-0.9.0/desc_opt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-16 20:49:51.000000 desc-opt-0.9.0/desc_opt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-16 20:49:51.000000 desc-opt-0.9.0/desc_opt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:49:51.000000 desc-opt-0.9.0/desc_opt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 20:49:51.000000 desc-opt-0.9.0/desc_opt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-16 20:49:51.000000 desc-opt-0.9.0/desc_opt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 20:49:51.000000 desc-opt-0.9.0/desc_opt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-16 20:48:40.000000 desc-opt-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-16 20:49:51.587927 desc-opt-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-16 20:48:40.000000 desc-opt-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:49:51.587927 desc-opt-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_axis_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)    57032 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_coils.py
--rw-r--r--   0 runner    (1001) docker     (123)    37458 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_compute_funs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_compute_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_constrain_current.py
--rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_equilibrium.py
--rw-r--r--   0 runner    (1001) docker     (123)    27156 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    33693 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_input_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    24525 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_linear_objectives.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_magnetic_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    26361 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_objective_funs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25635 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_perturbations.py
--rw-r--r--   0 runner    (1001) docker     (123)    27108 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_stability_funs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    21693 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-06-16 20:48:40.000000 desc-opt-0.9.0/tests/test_vmec.py
--rw-r--r--   0 runner    (1001) docker     (123)    68590 2023-06-16 20:48:40.000000 desc-opt-0.9.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:02:57.807091 desc-opt-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-06 02:00:57.000000 desc-opt-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-06 02:00:57.000000 desc-opt-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-07-06 02:02:57.807091 desc-opt-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-06 02:00:57.000000 desc-opt-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:02:57.811092 desc-opt-0.9.1/desc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-06 02:02:57.811092 desc-opt-0.9.1/desc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46420 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/coils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:02:57.763091 desc-opt-0.9.1/desc/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19023 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/compute/_basis_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/compute/_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47078 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/compute/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/compute/_equil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81919 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/compute/_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/compute/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45531 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/compute/_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30037 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/compute/_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/compute/_qs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/compute/_stability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/compute/data_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45044 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/compute/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24629 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/continuation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21571 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/derivatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:02:57.763091 desc-opt-0.9.1/desc/equilibrium/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/equilibrium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47058 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/equilibrium/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16371 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/equilibrium/coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38761 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/equilibrium/equilibrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/equilibrium/initial_guess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/equilibrium/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:02:57.791091 desc-opt-0.9.1/desc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)  2781266 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/examples/ARIES-CS_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)  1854489 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/examples/ATF_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)   974880 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/examples/DSHAPE_CURRENT_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)   974880 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/examples/DSHAPE_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)  1515598 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/examples/ESTELL_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)  1003793 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/examples/HELIOTRON_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)  3109450 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/examples/NCSX_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)  3059745 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/examples/QAS_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)   650984 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/examples/SOLOVEV_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)  3500803 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/examples/W7-X_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)  1942753 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/examples/WISTELL-A_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/examples/precise_QA.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4020724 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/examples/precise_QA_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/examples/precise_QH.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4017915 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/examples/precise_QH_output.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:02:57.799091 desc-opt-0.9.1/desc/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/geometry/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41130 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/geometry/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35918 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/geometry/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/geometry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44794 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44842 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:02:57.799091 desc-opt-0.9.1/desc/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/io/ascii_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/io/core_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/io/equilibrium_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/io/hdf5_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58768 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/io/input_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/io/pickle_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24850 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/magnetic_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:02:57.799091 desc-opt-0.9.1/desc/objectives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/objectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/objectives/_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30290 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/objectives/_equilibrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/objectives/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33909 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/objectives/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21761 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/objectives/_qs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/objectives/_stability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84358 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/objectives/linear_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/objectives/nae_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/objectives/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35732 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/objectives/objective_funs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/objectives/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:02:57.803091 desc-opt-0.9.1/desc/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27500 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/optimize/_constraint_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17501 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/optimize/_desc_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28726 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/optimize/_scipy_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/optimize/aug_lagrangian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/optimize/aug_lagrangian_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/optimize/bound_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/optimize/fmin_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/optimize/least_squares.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18967 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/optimize/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/optimize/stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/optimize/tr_subproblems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16139 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/optimize/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27407 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121457 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43879 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29582 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59935 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/vmec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-07-06 02:00:57.000000 desc-opt-0.9.1/desc/vmec_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:02:57.803091 desc-opt-0.9.1/desc_opt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-07-06 02:02:57.000000 desc-opt-0.9.1/desc_opt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-06 02:02:57.000000 desc-opt-0.9.1/desc_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 02:02:57.000000 desc-opt-0.9.1/desc_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 02:02:57.000000 desc-opt-0.9.1/desc_opt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-06 02:02:57.000000 desc-opt-0.9.1/desc_opt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 02:02:57.000000 desc-opt-0.9.1/desc_opt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-06 02:00:58.000000 desc-opt-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-06 02:02:57.811092 desc-opt-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-06 02:00:58.000000 desc-opt-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:02:57.807091 desc-opt-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_axis_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57530 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_coils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37458 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_compute_funs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_compute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_constrain_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_equilibrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27398 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32876 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_input_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25138 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_linear_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_magnetic_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28247 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_objective_funs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26703 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27120 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_stability_funs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9108 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21693 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28804 2023-07-06 02:00:58.000000 desc-opt-0.9.1/tests/test_vmec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68590 2023-07-06 02:00:58.000000 desc-opt-0.9.1/versioneer.py
```

### Comparing `desc-opt-0.9.0/LICENSE` & `desc-opt-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/PKG-INFO` & `desc-opt-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desc-opt
-Version: 0.9.0
+Version: 0.9.1
 Summary: Computes, analyzes and optimizes 3D MHD equilibria for stellarators and tokamaks
 Home-page: https://github.com/PlasmaControl/DESC/
 Author: Daniel Dudt, Rory Conlin, Dario Panici, Egemen Kolemen
 Author-email: PlasmaControl@princeton.edu
 License: MIT
 Project-URL: Issues Tracker, https://github.com/PlasmaControl/DESC/issues
 Project-URL: Contributing, https://github.com/PlasmaControl/DESC/blob/master/CONTRIBUTING.rst
```

### Comparing `desc-opt-0.9.0/README.rst` & `desc-opt-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/__init__.py` & `desc-opt-0.9.1/desc/__init__.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/__main__.py` & `desc-opt-0.9.1/desc/__main__.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/backend.py` & `desc-opt-0.9.1/desc/backend.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 
 if use_jax:  # noqa: C901 - FIXME: simplify this, define globally and then assign?
     jit = jax.jit
     fori_loop = jax.lax.fori_loop
     cond = jax.lax.cond
     switch = jax.lax.switch
     while_loop = jax.lax.while_loop
+    vmap = jax.vmap
     from jax.experimental.ode import odeint
     from jax.scipy.linalg import block_diag, cho_factor, cho_solve, qr, solve_triangular
     from jax.scipy.special import gammaln
 
     def put(arr, inds, vals):
         """Functional interface for array "fancy indexing".
 
@@ -266,7 +267,33 @@
             The output from the final iteration of body_fun, of type a.
 
         """
         val = init_val
         while cond_fun(val):
             val = body_fun(val)
         return val
+
+    def vmap(fun, out_axes=0):
+        """A numpy implementation of jax.lax.map whose API is a subset of jax.vmap.
+
+        Like Python's builtin map,
+        except inputs and outputs are in the form of stacked arrays,
+        and the returned object is a vectorized version of the input function.
+
+        Parameters
+        ----------
+        fun: callable
+            Function (A -> B)
+        out_axes: int
+            An integer indicating where the mapped axis should appear in the output.
+
+        Returns
+        -------
+        fun_vmap: callable
+            Vectorized version of fun.
+
+        """
+
+        def fun_vmap(fun_inputs):
+            return np.stack([fun(fun_input) for fun_input in fun_inputs], axis=out_axes)
+
+        return fun_vmap
```

### Comparing `desc-opt-0.9.0/desc/basis.py` & `desc-opt-0.9.1/desc/basis.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         "_NFP",
         "_modes",
         "_sym",
         "_spectral_indexing",
     ]
 
     def __init__(self):
-
         self._enforce_symmetry()
         self._sort_modes()
         self._create_idx()
 
     def _set_up(self):
         """Do things after loading or changing resolution."""
         self._enforce_symmetry()
@@ -146,24 +145,39 @@
         """Change resolution of the basis to the given resolutions."""
 
     @property
     def L(self):
         """int: Maximum radial resolution."""
         return self.__dict__.setdefault("_L", 0)
 
+    @L.setter
+    def L(self, L):
+        assert int(L) == L, "Basis Resolution must be an integer!"
+        self._L = int(L)
+
     @property
     def M(self):
         """int:  Maximum poloidal resolution."""
         return self.__dict__.setdefault("_M", 0)
 
+    @M.setter
+    def M(self, M):
+        assert int(M) == M, "Basis Resolution must be an integer!"
+        self._M = int(M)
+
     @property
     def N(self):
         """int: Maximum toroidal resolution."""
         return self.__dict__.setdefault("_N", 0)
 
+    @N.setter
+    def N(self, N):
+        assert int(N) == N, "Basis Resolution must be an integer!"
+        self._N = int(N)
+
     @property
     def NFP(self):
         """int: Number of field periods."""
         return self.__dict__.setdefault("_NFP", 1)
 
     @property
     def sym(self):
@@ -213,18 +227,17 @@
     sym : {"even", False}
         Type of symmetry. "even" has only even powers of rho, for an analytic profile
         on the disc. False uses the full (odd + even) powers.
 
     """
 
     def __init__(self, L, sym="even"):
-
-        self._L = L
-        self._M = 0
-        self._N = 0
+        self.L = L
+        self.M = 0
+        self.N = 0
         self._NFP = 1
         self._sym = sym
         self._spectral_indexing = "linear"
 
         self._modes = self._get_modes(L=self.L)
 
         super().__init__()
@@ -302,15 +315,15 @@
         Parameters
         ----------
         L : int
             Maximum radial resolution.
 
         """
         if L != self.L:
-            self._L = L
+            self.L = L
             self._modes = self._get_modes(self.L)
             self._set_up()
 
 
 class FourierSeries(Basis):
     """1D basis set for use with the magnetic axis.
 
@@ -326,18 +339,17 @@
         * ``'cos'`` for cos(m*t-n*z) symmetry
         * ``'sin'`` for sin(m*t-n*z) symmetry
         * ``False`` for no symmetry (Default)
 
     """
 
     def __init__(self, N, NFP=1, sym=False):
-
-        self._L = 0
-        self._M = 0
-        self._N = N
+        self.L = 0
+        self.M = 0
+        self.N = N
         self._NFP = NFP
         self._sym = sym
         self._spectral_indexing = "linear"
 
         self._modes = self._get_modes(N=self.N)
 
         super().__init__()
@@ -389,15 +401,15 @@
             modes = self.modes
         if (derivatives[0] != 0) or (derivatives[1] != 0):
             return jnp.zeros((nodes.shape[0], modes.shape[0]))
         if not len(modes):
             return np.array([]).reshape((len(nodes), 0))
 
         r, t, z = nodes.T
-        n = modes[:, 2]
+        l, m, n = modes.T
         if unique:
             _, zidx, zoutidx = np.unique(
                 z, return_index=True, return_inverse=True, axis=0
             )
             _, nidx, noutidx = np.unique(
                 n, return_index=True, return_inverse=True, axis=0
             )
@@ -405,28 +417,31 @@
             n = n[nidx]
 
         toroidal = fourier(z[:, np.newaxis], n, self.NFP, derivatives[2])
         if unique:
             toroidal = toroidal[zoutidx][:, noutidx]
         return toroidal
 
-    def change_resolution(self, N, NFP=None):
+    def change_resolution(self, N, NFP=None, sym=None):
         """Change resolution of the basis to the given resolutions.
 
         Parameters
         ----------
         N : int
             Maximum toroidal resolution.
         NFP : int
             Number of field periods.
+        sym : bool
+            Whether to enforce stellarator symmetry.
 
         """
         self._NFP = NFP if NFP is not None else self.NFP
         if N != self.N:
-            self._N = N
+            self.N = N
+            self._sym = sym if sym is not None else self.sym
             self._modes = self._get_modes(self.N)
             self._set_up()
 
 
 class DoubleFourierSeries(Basis):
     """2D basis set for use on a single flux surface.
 
@@ -444,18 +459,17 @@
         * ``'cos'`` for cos(m*t-n*z) symmetry
         * ``'sin'`` for sin(m*t-n*z) symmetry
         * ``False`` for no symmetry (Default)
 
     """
 
     def __init__(self, M, N, NFP=1, sym=False):
-
-        self._L = 0
-        self._M = M
-        self._N = N
+        self.L = 0
+        self.M = M
+        self.N = N
         self._NFP = NFP
         self._sym = sym
         self._spectral_indexing = "linear"
 
         self._modes = self._get_modes(M=self.M, N=self.N)
 
         super().__init__()
@@ -515,16 +529,15 @@
             modes = self.modes
         if derivatives[0] != 0:
             return jnp.zeros((nodes.shape[0], modes.shape[0]))
         if not len(modes):
             return np.array([]).reshape((len(nodes), 0))
 
         r, t, z = nodes.T
-        m = modes[:, 1]
-        n = modes[:, 2]
+        l, m, n = modes.T
         if unique:
             _, tidx, toutidx = np.unique(
                 t, return_index=True, return_inverse=True, axis=0
             )
             _, zidx, zoutidx = np.unique(
                 z, return_index=True, return_inverse=True, axis=0
             )
@@ -542,35 +555,38 @@
         poloidal = fourier(t[:, np.newaxis], m, 1, derivatives[1])
         toroidal = fourier(z[:, np.newaxis], n, self.NFP, derivatives[2])
         if unique:
             poloidal = poloidal[toutidx][:, moutidx]
             toroidal = toroidal[zoutidx][:, noutidx]
         return poloidal * toroidal
 
-    def change_resolution(self, M, N, NFP=None):
+    def change_resolution(self, M, N, NFP=None, sym=None):
         """Change resolution of the basis to the given resolutions.
 
         Parameters
         ----------
         M : int
             Maximum poloidal resolution.
         N : int
             Maximum toroidal resolution.
         NFP : int
             Number of field periods.
+        sym : bool
+            Whether to enforce stellarator symmetry.
 
         Returns
         -------
         None
 
         """
         self._NFP = NFP if NFP is not None else self.NFP
-        if M != self.M or N != self.N:
-            self._M = M
-            self._N = N
+        if M != self.M or N != self.N or sym != self.sym:
+            self.M = M
+            self.N = N
+            self._sym = sym if sym is not None else self.sym
             self._modes = self._get_modes(self.M, self.N)
             self._set_up()
 
 
 class ZernikePolynomial(Basis):
     """2D basis set for analytic functions in a unit disc.
 
@@ -601,18 +617,17 @@
         decreasing size, ending in a diamond shape for L=2*M where
         the traditional fringe/U of Arizona indexing is recovered.
         For L > 2*M, adds chevrons to the bottom, making a hexagonal diamond.
 
     """
 
     def __init__(self, L, M, sym=False, spectral_indexing="ansi"):
-
-        self._L = L
-        self._M = M
-        self._N = 0
+        self.L = L
+        self.M = M
+        self.N = 0
         self._NFP = 1
         self._sym = sym
         self._spectral_indexing = spectral_indexing
 
         self._modes = self._get_modes(
             L=self.L, M=self.M, spectral_indexing=self.spectral_indexing
         )
@@ -655,15 +670,15 @@
         """
         assert spectral_indexing in [
             "ansi",
             "fringe",
         ], "Unknown spectral_indexing: {}".format(spectral_indexing)
         default_L = {"ansi": M, "fringe": 2 * M}
         L = L if L >= 0 else default_L.get(spectral_indexing, M)
-        self._L = L
+        self.L = L
 
         if spectral_indexing == "ansi":
             pol_posm = [
                 [(m + d, m) for m in range(0, M + 1) if m + d < M + 1]
                 for d in range(0, L + 1, 2)
             ]
             if L > M:
@@ -721,16 +736,16 @@
             modes = self.modes
         if derivatives[2] != 0:
             return jnp.zeros((nodes.shape[0], modes.shape[0]))
         if not len(modes):
             return np.array([]).reshape((len(nodes), 0))
 
         r, t, z = nodes.T
+        l, m, n = modes.T
         lm = modes[:, :2]
-        m = modes[:, 1]
         if unique:
             _, ridx, routidx = np.unique(
                 r, return_index=True, return_inverse=True, axis=0
             )
             _, tidx, toutidx = np.unique(
                 t, return_index=True, return_inverse=True, axis=0
             )
@@ -756,28 +771,35 @@
         poloidal = fourier(t[:, np.newaxis], m, 1, derivatives[1])
 
         if unique:
             radial = radial[routidx][:, lmoutidx]
             poloidal = poloidal[toutidx][:, moutidx]
         return radial * poloidal
 
-    def change_resolution(self, L, M):
+    def change_resolution(self, L, M, sym=None):
         """Change resolution of the basis to the given resolutions.
 
         Parameters
         ----------
         L : int
             Maximum radial resolution.
         M : int
             Maximum poloidal resolution.
+        sym : bool
+            Whether to enforce stellarator symmetry.
+
+        Returns
+        -------
+        None
 
         """
-        if L != self.L or M != self.M:
-            self._L = L
-            self._M = M
+        if L != self.L or M != self.M or sym != self.sym:
+            self.L = L
+            self.M = M
+            self._sym = sym if sym is not None else self.sym
             self._modes = self._get_modes(
                 self.L, self.M, spectral_indexing=self.spectral_indexing
             )
             self._set_up()
 
 
 class FourierZernikeBasis(Basis):
@@ -817,18 +839,17 @@
         decreasing size, ending in a diamond shape for L=2*M where
         the traditional fringe/U of Arizona indexing is recovered.
         For L > 2*M, adds chevrons to the bottom, making a hexagonal diamond.
 
     """
 
     def __init__(self, L, M, N, NFP=1, sym=False, spectral_indexing="ansi"):
-
-        self._L = L
-        self._M = M
-        self._N = N
+        self.L = L
+        self.M = M
+        self.N = N
         self._NFP = NFP
         self._sym = sym
         self._spectral_indexing = spectral_indexing
 
         self._modes = self._get_modes(
             L=self.L, M=self.M, N=self.N, spectral_indexing=self.spectral_indexing
         )
@@ -873,15 +894,15 @@
         """
         assert spectral_indexing in [
             "ansi",
             "fringe",
         ], "Unknown spectral_indexing: {}".format(spectral_indexing)
         default_L = {"ansi": M, "fringe": 2 * M}
         L = L if L >= 0 else default_L.get(spectral_indexing, M)
-        self._L = L
+        self.L = L
 
         if spectral_indexing == "ansi":
             pol_posm = [
                 [(m + d, m) for m in range(0, M + 1) if m + d < M + 1]
                 for d in range(0, L + 1, 2)
             ]
             if L > M:
@@ -938,19 +959,19 @@
             Basis functions evaluated at nodes.
 
         """
         if modes is None:
             modes = self.modes
         if not len(modes):
             return np.array([]).reshape((len(nodes), 0))
+
         # TODO: avoid duplicate calculations when mixing derivatives
         r, t, z = nodes.T
+        l, m, n = modes.T
         lm = modes[:, :2]
-        m = modes[:, 1]
-        n = modes[:, 2]
         if unique:
             _, ridx, routidx = np.unique(
                 r, return_index=True, return_inverse=True, axis=0
             )
             _, tidx, toutidx = np.unique(
                 t, return_index=True, return_inverse=True, axis=0
             )
@@ -985,34 +1006,41 @@
         toroidal = fourier(z[:, np.newaxis], n, NFP=self.NFP, dt=derivatives[2])
         if unique:
             radial = radial[routidx][:, lmoutidx]
             poloidal = poloidal[toutidx][:, moutidx]
             toroidal = toroidal[zoutidx][:, noutidx]
         return radial * poloidal * toroidal
 
-    def change_resolution(self, L, M, N, NFP=None):
+    def change_resolution(self, L, M, N, NFP=None, sym=None):
         """Change resolution of the basis to the given resolutions.
 
         Parameters
         ----------
         L : int
             Maximum radial resolution.
         M : int
             Maximum poloidal resolution.
         N : int
             Maximum toroidal resolution.
         NFP : int
             Number of field periods.
+        sym : bool
+            Whether to enforce stellarator symmetry.
+
+        Returns
+        -------
+        None
 
         """
         self._NFP = NFP if NFP is not None else self.NFP
-        if L != self.L or M != self.M or N != self.N:
-            self._L = L
-            self._M = M
-            self._N = N
+        if L != self.L or M != self.M or N != self.N or sym != self.sym:
+            self.L = L
+            self.M = M
+            self.N = N
+            self._sym = sym if sym is not None else self.sym
             self._modes = self._get_modes(
                 self.L, self.M, self.N, spectral_indexing=self.spectral_indexing
             )
             self._set_up()
 
 
 def polyder_vec(p, m):
@@ -1156,26 +1184,26 @@
             c = c.astype(int)
         except OverflowError:
             c = c.astype(float)
     c = c[idx]
     return c
 
 
-def zernike_radial_poly(rho, l, m, dr=0):
+def zernike_radial_poly(r, l, m, dr=0):
     """Radial part of zernike polynomials.
 
     Evaluates basis functions using numpy to
     exactly compute the polynomial coefficients
     and Horner's method for low resolution,
     or extended precision arithmetic for high resolution.
     Faster for low resolution, but not differentiable.
 
     Parameters
     ----------
-    rho : ndarray, shape(N,)
+    r : ndarray, shape(N,)
         radial coordinates to evaluate basis
     l : ndarray of int, shape(K,)
         radial mode number(s)
     m : ndarray of int, shape(K,)
         azimuthal mode number(s)
     dr : int
         order of derivative (Default = 0)
@@ -1187,15 +1215,15 @@
 
     """
     coeffs = zernike_radial_coeffs(l, m)
     lmax = np.max(l)
     coeffs = polyder_vec(coeffs, dr)
     # this should give accuracy of ~1e-10 in the eval'd polynomials
     prec = int(0.4 * lmax + 8.4)
-    return polyval_vec(coeffs, rho, prec=prec).T
+    return polyval_vec(coeffs, r, prec=prec).T
 
 
 def zernike_radial(r, l, m, dr=0):
     """Radial part of zernike polynomials.
 
     Evaluates basis functions using JAX and a stable
     evaluation scheme based on jacobi polynomials and
```

### Comparing `desc-opt-0.9.0/desc/coils.py` & `desc-opt-0.9.1/desc/coils.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/compat.py` & `desc-opt-0.9.1/desc/compat.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 import numpy as np
 
 from desc.grid import Grid
 
 
 def ensure_positive_jacobian(eq):
-    """Convert an Equilibrium to have a positive coordinate jacobian.
+    """Convert an Equilibrium to have a positive coordinate Jacobian.
 
     Parameters
     ----------
     eq : Equilibrium or iterable of Equilibrium
-        Equilibria to convert to right handed coordinate system.
+        Equilibria to convert to right-handed coordinate system.
 
     Returns
     -------
     eq : Equilibrium or iterable of Equilibrium
-        Same as input, but with coefficients adjusted to give right handed coordinates.
+        Same as input, but with coefficients adjusted to give right-handed coordinates.
     """
-    # maybe its iterable:
+    # maybe it's iterable:
     if hasattr(eq, "__len__"):
         for e in eq:
             ensure_positive_jacobian(e)
         return eq
 
     signgs = np.sign(eq.compute("sqrt(g)", grid=Grid(np.array([[1, 0, 0]])))["sqrt(g)"])
     if signgs < 0:
@@ -36,12 +36,14 @@
 
         lone = np.ones_like(eq.L_lmn)
         lone[eq.L_basis.modes[:, 1] >= 0] *= -1
         eq.L_lmn *= lone
 
         if eq.iota is not None:
             eq.i_l *= -1
+        else:
+            eq.c_l *= -1
         eq.surface = eq.get_surface_at(rho=1)
 
     signgs = np.sign(eq.compute("sqrt(g)", grid=Grid(np.array([[1, 0, 0]])))["sqrt(g)"])
     assert signgs == 1
     return eq
```

### Comparing `desc-opt-0.9.0/desc/compute/__init__.py` & `desc-opt-0.9.1/desc/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/compute/_basis_vectors.py` & `desc-opt-0.9.1/desc/compute/_basis_vectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -651,28 +651,28 @@
 )
 def _b(params, transforms, profiles, data, **kwargs):
     data["b"] = (data["B"].T / jnp.linalg.norm(data["B"], axis=-1)).T
     return data
 
 
 @register_compute_fun(
-    name="n",
-    label="\\hat{n}",
+    name="n_rho",
+    label="\\hat{\\mathbf{n}}_{\\rho}",
     units="~",
     units_long="None",
-    description="Unit vector normal to flux surface",
+    description="Unit vector normal to constant rho surface (direction of e^rho)",
     dim=3,
     params=[],
     transforms={},
     profiles=[],
     coordinates="rtz",
     data=["e^rho"],
 )
-def _n(params, transforms, profiles, data, **kwargs):
-    data["n"] = (data["e^rho"].T / jnp.linalg.norm(data["e^rho"], axis=-1)).T
+def _n_rho(params, transforms, profiles, data, **kwargs):
+    data["n_rho"] = (data["e^rho"].T / jnp.linalg.norm(data["e^rho"], axis=-1)).T
     return data
 
 
 @register_compute_fun(
     name="grad(alpha)",
     label="\\nabla \\alpha",
     units="m^{-1}",
```

### Comparing `desc-opt-0.9.0/desc/compute/_bootstrap.py` & `desc-opt-0.9.1/desc/compute/_bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Compute functions for bootstrap current."""
 
 from scipy.constants import elementary_charge
 from scipy.special import roots_legendre
 
 from ..backend import fori_loop, jnp
 from .data_index import register_compute_fun
-from .utils import compress, expand, surface_averages
+from .utils import compress, expand, surface_averages_map
 
 
 @register_compute_fun(
     name="trapped fraction",
     label="1 - \\frac{3}{4} \\langle B^2 \\rangle \\int_0^{1/Bmax} "
     "\\frac{\\lambda\\; d\\lambda}{\\langle \\sqrt{1 - \\lambda B} \\rangle}",
     units="~",
@@ -45,25 +45,26 @@
     lambda_weights = jnp.asarray(base_weights * 0.5)
 
     grid = transforms["grid"]
     Bmax = data["max_tz |B|"]
     modB_over_Bmax = data["|B|"] / Bmax
     sqrt_g = data["sqrt(g)"]
     Bmax_squared = compress(grid, Bmax * Bmax)
+    V_r = compress(grid, data["V_r(r)"])
+    compute_surface_averages = surface_averages_map(grid, expand_out=False)
 
     # Sum over the lambda grid points, using fori_loop for efficiency.
     def body_fun(jlambda, lambda_integral):
-        flux_surf_avg_term = surface_averages(
-            grid,
+        flux_surf_avg_term = compute_surface_averages(
             jnp.sqrt(1 - lambd[jlambda] * modB_over_Bmax),
             sqrt_g,
-            denominator=data["V_r(r)"],
+            denominator=V_r,
         )
         return lambda_integral + lambda_weights[jlambda] * lambd[jlambda] / (
-            Bmax_squared * compress(grid, flux_surf_avg_term)
+            Bmax_squared * flux_surf_avg_term
         )
 
     lambda_integral = fori_loop(0, n_gauss, body_fun, jnp.zeros(grid.num_rho))
 
     trapped_fraction = 1 - 0.75 * compress(grid, data["<B^2>"]) * lambda_integral
     data["trapped fraction"] = expand(grid, trapped_fraction)
     return data
```

### Comparing `desc-opt-0.9.0/desc/compute/_core.py` & `desc-opt-0.9.1/desc/compute/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
     params=[],
     transforms={},
     profiles=[],
     coordinates="rtz",
     data=["theta", "lambda"],
 )
 def _theta_sfl(params, transforms, profiles, data, **kwargs):
-    data["theta_sfl"] = data["theta"] + data["lambda"]
+    data["theta_sfl"] = (data["theta"] + data["lambda"]) % (2 * jnp.pi)
     return data
 
 
 @register_compute_fun(
     name="theta_sfl_r",
     label="\\partial_{\\rho} \\vartheta",
     units="rad",
@@ -322,24 +322,24 @@
 
 
 @register_compute_fun(
     name="alpha",
     label="\\alpha",
     units="~",
     units_long="None",
-    description="Field line label",
+    description="Field line label, defined on [0, 2pi)",
     dim=1,
     params=[],
     transforms={},
     profiles=[],
     coordinates="rtz",
     data=["theta_sfl", "zeta", "iota"],
 )
 def _alpha(params, transforms, profiles, data, **kwargs):
-    data["alpha"] = data["theta_sfl"] - data["iota"] * data["zeta"]
+    data["alpha"] = (data["theta_sfl"] - data["iota"] * data["zeta"]) % (2 * jnp.pi)
     return data
 
 
 @register_compute_fun(
     name="alpha_r",
     label="\\partial_\\rho \\alpha",
     units="~",
```

### Comparing `desc-opt-0.9.0/desc/compute/_equil.py` & `desc-opt-0.9.1/desc/compute/_equil.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/compute/_field.py` & `desc-opt-0.9.1/desc/compute/_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from desc.backend import jnp, put
 
 from .data_index import register_compute_fun
 from .utils import (
     cross,
     dot,
-    expand,
     surface_averages,
     surface_integrals,
     surface_max,
     surface_min,
 )
 
 
@@ -2896,17 +2895,15 @@
     params=[],
     transforms={"grid": []},
     profiles=[],
     coordinates="r",
     data=["|B|"],
 )
 def _max_tz_modB(params, transforms, profiles, data, **kwargs):
-    data["max_tz |B|"] = expand(
-        transforms["grid"], surface_max(transforms["grid"], data["|B|"])
-    )
+    data["max_tz |B|"] = surface_max(transforms["grid"], data["|B|"])
     return data
 
 
 @register_compute_fun(
     name="min_tz |B|",
     label="\\min_{\\theta \\zeta} |B|",
     units="T",
@@ -2916,17 +2913,15 @@
     params=[],
     transforms={"grid": []},
     profiles=[],
     coordinates="r",
     data=["|B|"],
 )
 def _min_tz_modB(params, transforms, profiles, data, **kwargs):
-    data["min_tz |B|"] = expand(
-        transforms["grid"], surface_min(transforms["grid"], data["|B|"])
-    )
+    data["min_tz |B|"] = surface_min(transforms["grid"], data["|B|"])
     return data
 
 
 @register_compute_fun(
     name="effective r/R0",
     label="(r / R_0)_{effective}",
     units="~",
@@ -2986,36 +2981,36 @@
     units_long="Inverse meters",
     description="Normal curvature vector of magnetic field lines",
     dim=1,
     params=[],
     transforms={},
     profiles=[],
     coordinates="rtz",
-    data=["kappa", "n"],
+    data=["kappa", "n_rho"],
 )
 def _kappa_n(params, transforms, profiles, data, **kwargs):
-    data["kappa_n"] = dot(data["kappa"], data["n"])
+    data["kappa_n"] = dot(data["kappa"], data["n_rho"])
     return data
 
 
 @register_compute_fun(
     name="kappa_g",
     label="\\kappa_g",
     units="m^{-1}",
     units_long="Inverse meters",
     description="Geodesic curvature vector of magnetic field lines",
     dim=1,
     params=[],
     transforms={},
     profiles=[],
     coordinates="rtz",
-    data=["kappa", "n", "b"],
+    data=["kappa", "n_rho", "b"],
 )
 def _kappa_g(params, transforms, profiles, data, **kwargs):
-    data["kappa_g"] = dot(data["kappa"], cross(data["n"], data["b"]))
+    data["kappa_g"] = dot(data["kappa"], cross(data["n_rho"], data["b"]))
     return data
 
 
 @register_compute_fun(
     name="grad(B)",
     label="\\nabla \\mathbf{B}",
     units="T \\cdot m^{-1}",
```

### Comparing `desc-opt-0.9.0/desc/compute/_geometry.py` & `desc-opt-0.9.1/desc/compute/_geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from desc.backend import jnp
 
 from .data_index import register_compute_fun
-from .utils import compress, cross, dot, surface_integrals
+from .utils import cross, dot, line_integrals, surface_integrals
 
 
 @register_compute_fun(
     name="V",
     label="V",
     units="m^{3}",
     units_long="cubic meters",
@@ -101,14 +101,15 @@
 )
 def _A(params, transforms, profiles, data, **kwargs):
     data["A"] = jnp.mean(
         surface_integrals(
             transforms["grid"],
             jnp.abs(data["sqrt(g)"] / data["R"]),
             surface_label="zeta",
+            expand_out=False,
         )
     )
     return data
 
 
 @register_compute_fun(
     name="S(r)",
@@ -192,32 +193,31 @@
     params=[],
     transforms={"grid": []},
     profiles=[],
     coordinates="",
     data=["sqrt(g)", "g_tt"],
 )
 def _a_major_over_a_minor(params, transforms, profiles, data, **kwargs):
-    P = compress(  # perimeter
-        transforms["grid"],
-        surface_integrals(
+    max_rho = transforms["grid"].nodes[transforms["grid"].unique_rho_idx[-1], 0]
+    P = (  # perimeter
+        line_integrals(
             transforms["grid"],
             jnp.sqrt(data["g_tt"]),
-            surface_label="zeta",
-            max_surface=True,
-        ),
-        surface_label="zeta",
+            line_label="theta",
+            fix_surface=("rho", max_rho),
+            expand_out=False,
+        )
+        / max_rho
     )
-    A = compress(  # surface area
+    # surface area
+    A = surface_integrals(
         transforms["grid"],
-        surface_integrals(
-            transforms["grid"],
-            jnp.abs(data["sqrt(g)"] / data["R"]),
-            surface_label="zeta",
-        ),
+        jnp.abs(data["sqrt(g)"] / data["R"]),
         surface_label="zeta",
+        expand_out=False,
     )
     # derived from Ramanujan approximation for the perimeter of an ellipse
     a = (  # semi-major radius
         jnp.sqrt(3)
         * (
             jnp.sqrt(8 * jnp.pi * A + P**2)
             + jnp.sqrt(
@@ -230,32 +230,14 @@
     ) / (12 * jnp.pi)
     b = A / (jnp.pi * a)  # semi-minor radius
     data["a_major/a_minor"] = jnp.max(a / b)
     return data
 
 
 @register_compute_fun(
-    name="n_rho",
-    label="\\hat{\\mathbf{n}}_{\\rho}",
-    units="~",
-    units_long="None",
-    description="Unit normal vector to constant rho surface",
-    dim=3,
-    params=[],
-    transforms={},
-    profiles=[],
-    coordinates="rtz",
-    data=["e^rho"],
-)
-def _n_rho(params, transforms, profiles, data, **kwargs):
-    data["n_rho"] = (data["e^rho"].T / jnp.linalg.norm(data["e^rho"])).T
-    return data
-
-
-@register_compute_fun(
     name="L_sff",
     label="L_{sff}",
     units="m",
     units_long="meters",
     description="L coefficient of second fundamental form",
     dim=1,
     params=[],
```

### Comparing `desc-opt-0.9.0/desc/compute/_metric.py` & `desc-opt-0.9.1/desc/compute/_metric.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/compute/_profiles.py` & `desc-opt-0.9.1/desc/compute/_profiles.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/compute/_qs.py` & `desc-opt-0.9.1/desc/compute/_qs.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/compute/_stability.py` & `desc-opt-0.9.1/desc/compute/_stability.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/compute/data_index.py` & `desc-opt-0.9.1/desc/compute/data_index.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/continuation.py` & `desc-opt-0.9.1/desc/continuation.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,18 +72,19 @@
         sym=eq.sym,
         spectral_indexing=spectral_indexing,
     )
 
     if not isinstance(optimizer, Optimizer):
         optimizer = Optimizer(optimizer)
     constraints_i = get_fixed_boundary_constraints(
+        eq=eqi,
         iota=objective != "vacuum" and eq.iota is not None,
         kinetic=eq.electron_temperature is not None,
     )
-    objective_i = get_equilibrium_objective(objective)
+    objective_i = get_equilibrium_objective(eq=eqi, mode=objective)
 
     eqfam = EquilibriaFamily()
 
     ii = 0
     stop = False
     while ii < mres_steps and not stop:
         timer.start("Iteration {} total".format(ii + 1))
@@ -114,18 +115,19 @@
                 1,
                 pert_order,
                 objective_i,
                 optimizer,
             )
 
         constraints_i = get_fixed_boundary_constraints(
+            eq=eqi,
             iota=objective != "vacuum" and eq.iota is not None,
             kinetic=eq.electron_temperature is not None,
         )
-        objective_i = get_equilibrium_objective(objective)
+        objective_i = get_equilibrium_objective(eq=eqi, mode=objective)
         if len(deltas) > 0:
             if verbose > 0:
                 print("Perturbing equilibrium")
             eqi.perturb(
                 objective=objective_i,
                 constraints=constraints_i,
                 deltas=deltas,
@@ -210,18 +212,19 @@
 
     eqi = eqfam[-1].copy()
     eqfam_temp = eqfam.copy()
     # make sure its at full radial/poloidal resolution
     eqi.change_resolution(L=eq.L, M=eq.M, L_grid=eq.L_grid, M_grid=eq.M_grid)
 
     constraints_i = get_fixed_boundary_constraints(
+        eq=eqi,
         iota=objective != "vacuum" and eq.iota is not None,
         kinetic=eq.electron_temperature is not None,
     )
-    objective_i = get_equilibrium_objective(objective)
+    objective_i = get_equilibrium_objective(eq=eqi, mode=objective)
 
     pres_steps = (
         0
         if (abs(eq.pressure(np.linspace(0, 1, 20))) < 1e-14).all() or pres_step == 0
         else int(np.ceil(1 / pres_step))
     )
     pres_ratio = 0 if pres_steps else 1
@@ -340,18 +343,19 @@
 
     eqi = eqfam[-1].copy()
     eqfam_temp = eqfam.copy()
     # make sure its at full resolution
     eqi.change_resolution(eq.L, eq.M, eq.N, eq.L_grid, eq.M_grid, eq.N_grid)
 
     constraints_i = get_fixed_boundary_constraints(
+        eq=eqi,
         iota=objective != "vacuum" and eq.iota is not None,
         kinetic=eq.electron_temperature is not None,
     )
-    objective_i = get_equilibrium_objective(objective)
+    objective_i = get_equilibrium_objective(eq=eqi, mode=objective)
 
     bdry_steps = 0 if eq.N == 0 or bdry_step == 0 else int(np.ceil(1 / bdry_step))
     bdry_ratio = 0 if eq.N else 1
 
     surf_axisym = eq.surface.copy()
     surf_axisym.change_resolution(eq.L, eq.M, 0)
     surf_axisym.change_resolution(eq.L, eq.M, eq.N)
@@ -649,16 +653,17 @@
         pert_order, ftol, xtol, gtol, maxiter, eqfam
     )
     if isinstance(eqfam, (list, tuple)):
         eqfam = EquilibriaFamily(*eqfam)
 
     if not isinstance(optimizer, Optimizer):
         optimizer = Optimizer(optimizer)
-    objective_i = get_equilibrium_objective(objective)
+    objective_i = get_equilibrium_objective(eq=eqfam[-1], mode=objective)
     constraints_i = get_fixed_boundary_constraints(
+        eq=eqfam[-1],
         iota=objective != "vacuum" and eqfam[0].iota is not None,
         kinetic=eqfam[0].electron_temperature is not None,
     )
 
     ii = 0
     nn = len(eqfam)
     stop = False
@@ -696,16 +701,17 @@
                 "pressure": eqi.pressure,
                 "Psi": eqi.Psi,
             }
             deltas = get_deltas(things1, things2)
 
             # maybe rebuild objective if resolution changed.
             if eqfam[ii - 1].resolution != eqi.resolution:
-                objective_i = get_equilibrium_objective(objective)
+                objective_i = get_equilibrium_objective(eq=eqfam[ii], mode=objective)
                 constraints_i = get_fixed_boundary_constraints(
+                    eq=eqfam[ii],
                     iota=objective != "vacuum" and eqfam[ii].iota is not None,
                     kinetic=eqfam[ii].electron_temperature is not None,
                 )
 
         if len(deltas) > 0:
             if verbose > 0:
                 print("Perturbing equilibrium")
```

### Comparing `desc-opt-0.9.0/desc/derivatives.py` & `desc-opt-0.9.1/desc/derivatives.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Wrapper classes for JAX automatic differentiation and finite differences."""
 
 from abc import ABC, abstractmethod
 
 import numpy as np
 from termcolor import colored
 
-from desc.backend import jnp, put, use_jax
+from desc.backend import fori_loop, jnp, put, use_jax
 
 if use_jax:
     import jax
 
 
 class _Derivative(ABC):
     """_Derivative is an abstract base class for derivative matrix calculations.
@@ -146,61 +146,97 @@
             fun and x is the input argument at position argnum. Exact shape and meaning
             will depend on "mode"
 
         """
         return self._compute(*args)
 
     @classmethod
-    def compute_jvp(cls, fun, argnum, v, *args):
+    def compute_vjp(cls, fun, argnum, v, *args, **kwargs):
+        """Compute v.T * df/dx.
+
+        Parameters
+        ----------
+        fun : callable
+            function to differentiate
+        argnum : int or tuple
+            arguments to differentiate with respect to
+        v : array-like or tuple of array-like
+            tangent vectors. Should be one for each output of fun.
+        args : tuple
+            arguments passed to fun
+        kwargs : dict
+            keyword arguments passed to fun
+
+        Returns
+        -------
+        vjp : array-like
+            Vector v times Jacobian, summed over different argnums
+
+        """
+        assert jnp.isscalar(argnum), "vjp for multiple args not currently supported"
+        _ = kwargs.pop("rel_step", None)  # unused by autodiff
+
+        def _fun(*args):
+            return v.T @ fun(*args, **kwargs)
+
+        return jax.grad(_fun, argnum)(*args)
+
+    @classmethod
+    def compute_jvp(cls, fun, argnum, v, *args, **kwargs):
         """Compute df/dx*v.
 
         Parameters
         ----------
         fun : callable
             function to differentiate
         argnum : int or tuple
             arguments to differentiate with respect to
         v : array-like or tuple of array-like
             tangent vectors. Should be one for each argnum
         args : tuple
-            arguments passed to f
+            arguments passed to fun
+        kwargs : dict
+            keyword arguments passed to fun
 
         Returns
         -------
         jvp : array-like
             Jacobian times vectors v, summed over different argnums
 
         """
-        tangents = list(nested_zeros_like(args))
-        if jnp.isscalar(argnum):
-            argnum = (argnum,)
-        else:
-            argnum = tuple(argnum)
+        _ = kwargs.pop("rel_step", None)  # unused by autodiff
+        argnum = (argnum,) if jnp.isscalar(argnum) else tuple(argnum)
         v = (v,) if not isinstance(v, tuple) else v
 
-        for i, vi in enumerate(v):
-            tangents[argnum[i]] = vi
-        y, u = jax.jvp(fun, args, tuple(tangents))
+        def _fun(*x):
+            _args = list(args)
+            for i, xi in zip(argnum, x):
+                _args[i] = xi
+            return fun(*_args, **kwargs)
+
+        y, u = jax.jvp(_fun, tuple(args[i] for i in argnum), v)
         return u
 
     @classmethod
-    def compute_jvp2(cls, fun, argnum1, argnum2, v1, v2, *args):
+    def compute_jvp2(cls, fun, argnum1, argnum2, v1, v2, *args, **kwargs):
         """Compute d^2f/dx^2*v1*v2.
 
         Parameters
         ----------
         fun : callable
             function to differentiate
         argnum1, argnum2 : int or tuple of int
             arguments to differentiate with respect to. First entry corresponds to v1,
             second to v2
         v1,v2 : array-like or tuple of array-like
             tangent vectors. Should be one for each argnum
         args : tuple
-            arguments passed to f
+            arguments passed to fun
+        kwargs : dict
+            keyword arguments passed to fun
 
         Returns
         -------
         jvp2 : array-like
             second derivative times vectors v1, v2, summed over different argnums
 
         """
@@ -213,33 +249,37 @@
         if np.isscalar(argnum2):
             argnum2 = (argnum2 + 1,)
             v2 = (v2,) if not isinstance(v2, tuple) else v2
         else:
             argnum2 = tuple([i + 1 for i in argnum2])
             v2 = tuple(v2)
 
-        dfdx = lambda dx1, *args: cls.compute_jvp(fun, argnum1, dx1, *args)
-        d2fdx2 = lambda dx1, dx2: cls.compute_jvp(dfdx, argnum2, dx2, dx1, *args)
+        dfdx = lambda dx1, *args: cls.compute_jvp(fun, argnum1, dx1, *args, **kwargs)
+        d2fdx2 = lambda dx1, dx2: cls.compute_jvp(
+            dfdx, argnum2, dx2, dx1, *args, **kwargs
+        )
         return d2fdx2(v1, v2)
 
     @classmethod
-    def compute_jvp3(cls, fun, argnum1, argnum2, argnum3, v1, v2, v3, *args):
+    def compute_jvp3(cls, fun, argnum1, argnum2, argnum3, v1, v2, v3, *args, **kwargs):
         """Compute d^3f/dx^3*v1*v2*v3.
 
         Parameters
         ----------
         fun : callable
             function to differentiate
         argnum1, argnum2, argnum3 : int or tuple of int
             arguments to differentiate with respect to. First entry corresponds to v1,
             second to v2 etc
         v1,v2,v3 : array-like or tuple of array-like
             tangent vectors. Should be one for each argnum
         args : tuple
-            arguments passed to f
+            arguments passed to fun
+        kwargs : dict
+            keyword arguments passed to fun
 
         Returns
         -------
         jvp3 : array-like
             third derivative times vectors v2, v3, v3, summed over different argnums
 
         """
@@ -259,26 +299,43 @@
         if np.isscalar(argnum3):
             argnum3 = (argnum3 + 2,)
             v3 = (v3,) if not isinstance(v3, tuple) else v3
         else:
             argnum3 = tuple([i + 2 for i in argnum3])
             v3 = tuple(v3)
 
-        dfdx = lambda dx1, *args: cls.compute_jvp(fun, argnum1, dx1, *args)
-        d2fdx2 = lambda dx1, dx2, *args: cls.compute_jvp(dfdx, argnum2, dx2, dx1, *args)
+        dfdx = lambda dx1, *args: cls.compute_jvp(fun, argnum1, dx1, *args, **kwargs)
+        d2fdx2 = lambda dx1, dx2, *args: cls.compute_jvp(
+            dfdx, argnum2, dx2, dx1, *args, **kwargs
+        )
         d3fdx3 = lambda dx1, dx2, dx3: cls.compute_jvp(
-            d2fdx2, argnum3, dx3, dx2, dx1, *args
+            d2fdx2, argnum3, dx3, dx2, dx1, *args, **kwargs
         )
         return d3fdx3(v1, v2, v3)
 
-    def _compute_jvp(self, v, *args):
-        return self.compute_jvp(self._fun, self.argnum, v, *args)
+    def _compute_jvp(self, v, *args, **kwargs):
+        return self.compute_jvp(self._fun, self.argnum, v, *args, **kwargs)
+
+    def _jac_looped(self, *args, **kwargs):
+
+        n = args[self._argnum].size
+        shp = jax.eval_shape(self._fun, *args).shape
+        I = jnp.eye(n)
+        J = jnp.zeros((*shp, n)).T
+
+        def body(i, J):
+            tangents = I[i]
+            Ji = self._compute_jvp(tangents, *args, **kwargs)
+            J = put(J, i, Ji.T)
+            return J
+
+        return fori_loop(0, n, body, J).T
 
     def _set_mode(self, mode) -> None:
-        if mode not in ["fwd", "rev", "grad", "hess", "jvp"]:
+        if mode not in ["fwd", "rev", "grad", "hess", "jvp", "looped"]:
             raise ValueError(
                 colored("invalid mode option for automatic differentiation", "red")
             )
 
         self._mode = mode
         if self._mode == "fwd":
             self._compute = jax.jacfwd(self._fun, self._argnum)
@@ -286,14 +343,16 @@
             self._compute = jax.jacrev(self._fun, self._argnum)
         elif self._mode == "grad":
             self._compute = jax.grad(self._fun, self._argnum)
         elif self._mode == "hess":
             self._compute = jax.hessian(self._fun, self._argnum)
         elif self._mode == "jvp":
             self._compute = self._compute_jvp
+        elif self._mode == "looped":
+            self._compute = self._jac_looped
 
 
 class FiniteDiffDerivative(_Derivative):
     """Computes derivatives using 2nd order centered finite differences.
 
     Parameters
     ----------
@@ -322,17 +381,19 @@
         self._set_mode(mode)
 
     def _compute_hessian(self, *args):
         """Compute the Hessian matrix using 2nd order centered finite differences.
 
         Parameters
         ----------
-        *args : list
+        args : tuple
             Arguments of the objective function where the derivative is to be
             evaluated at.
+        kwargs : dict
+            keyword arguments passed to fun
 
         Returns
         -------
         H : ndarray of float, shape(len(x),len(x))
             d^2f/dx^2, where f is the output of the function fun and x is the input
             argument at position argnum.
 
@@ -365,17 +426,20 @@
         return hess
 
     def _compute_grad_or_jac(self, *args):
         """Compute the gradient or Jacobian matrix (ie, first derivative).
 
         Parameters
         ----------
-        *args : list
+        args : tuple
             Arguments of the objective function where the derivative is to be
             evaluated at.
+        kwargs : dict
+            keyword arguments passed to fun
+
 
         Returns
         -------
         J : ndarray of float, shape(len(f),len(x))
             df/dx, where f is the output of the function fun and x is the input
             argument at position argnum.
 
@@ -402,66 +466,103 @@
             dfdx = df / dx
             J = put(J.T, i, dfdx.flatten()).T
         if m == 1:
             J = np.ravel(J)
         return J
 
     @classmethod
+    def compute_vjp(cls, fun, argnum, v, *args, **kwargs):
+        """Compute v.T * df/dx.
+
+        Parameters
+        ----------
+        fun : callable
+            function to differentiate
+        argnum : int or tuple
+            arguments to differentiate with respect to
+        v : array-like or tuple of array-like
+            tangent vectors. Should be one for each output of fun
+        args : tuple
+            arguments passed to fun
+        kwargs : dict
+            keyword arguments passed to fun
+
+        Returns
+        -------
+        vjp : array-like
+            Vector v times Jacobian, summed over different argnums
+
+        """
+        assert np.isscalar(argnum), "vjp for multiple args not currently supported"
+        rel_step = kwargs.pop("rel_step", 1e-3)
+
+        def _fun(*args):
+            return v.T @ fun(*args, **kwargs)
+
+        return FiniteDiffDerivative(_fun, argnum, "grad", rel_step)(*args)
+
+    @classmethod
     def compute_jvp(cls, fun, argnum, v, *args, **kwargs):
         """Compute df/dx*v.
 
         Parameters
         ----------
         fun : callable
             function to differentiate
         argnum : int or tuple
             arguments to differentiate with respect to
         v : array-like or tuple of array-like
             tangent vectors. Should be one for each argnum
         args : tuple
-            arguments passed to f
+            arguments passed to fun
+        kwargs : dict
+            keyword arguments passed to fun
 
         Returns
         -------
         jvp : array-like
             Jacobian times vectors v, summed over different argnums
 
         """
-        rel_step = kwargs.get("rel_step", 1e-3)
+        rel_step = kwargs.pop("rel_step", 1e-3)
 
         if np.isscalar(argnum):
             nargs = 1
             argnum = (argnum,)
         else:
             nargs = len(argnum)
         v = (v,) if not isinstance(v, tuple) else v
 
         f = np.array(
             [
-                cls._compute_jvp_1arg(fun, argnum[i], v[i], *args, rel_step=rel_step)
+                cls._compute_jvp_1arg(
+                    fun, argnum[i], v[i], *args, rel_step=rel_step, **kwargs
+                )
                 for i in range(nargs)
             ]
         )
         return np.sum(f, axis=0)
 
     @classmethod
-    def compute_jvp2(cls, fun, argnum1, argnum2, v1, v2, *args):
+    def compute_jvp2(cls, fun, argnum1, argnum2, v1, v2, *args, **kwargs):
         """Compute d^2f/dx^2*v1*v2.
 
         Parameters
         ----------
         fun : callable
             function to differentiate
         argnum1, argnum2 : int or tuple of int
             arguments to differentiate with respect to. First entry corresponds to v1,
             second to v2
         v1,v2 : array-like or tuple of array-like
             tangent vectors. Should be one for each argnum
         args : tuple
-            arguments passed to f
+            arguments passed to fun
+        kwargs : dict
+            keyword arguments passed to fun
 
         Returns
         -------
         jvp2 : array-like
             second derivative times vectors v1, v2, summed over different argnums
 
         """
@@ -474,33 +575,37 @@
         if np.isscalar(argnum2):
             argnum2 = (argnum2 + 1,)
             v2 = (v2,) if not isinstance(v2, tuple) else v2
         else:
             argnum2 = tuple([i + 1 for i in argnum2])
             v2 = tuple(v2)
 
-        dfdx = lambda dx1, *args: cls.compute_jvp(fun, argnum1, dx1, *args)
-        d2fdx2 = lambda dx1, dx2: cls.compute_jvp(dfdx, argnum2, dx2, dx1, *args)
+        dfdx = lambda dx1, *args: cls.compute_jvp(fun, argnum1, dx1, *args, **kwargs)
+        d2fdx2 = lambda dx1, dx2: cls.compute_jvp(
+            dfdx, argnum2, dx2, dx1, *args, **kwargs
+        )
         return d2fdx2(v1, v2)
 
     @classmethod
-    def compute_jvp3(cls, fun, argnum1, argnum2, argnum3, v1, v2, v3, *args):
+    def compute_jvp3(cls, fun, argnum1, argnum2, argnum3, v1, v2, v3, *args, **kwargs):
         """Compute d^3f/dx^3*v1*v2*v3.
 
         Parameters
         ----------
         fun : callable
             function to differentiate
         argnum1, argnum2, argnum3 : int or tuple of int
             arguments to differentiate with respect to. First entry corresponds to v1,
             second to v2 etc
         v1,v2,v3 : array-like or tuple of array-like
             tangent vectors. Should be one for each argnum
         args : tuple
-            arguments passed to f
+            arguments passed to fun
+        kwargs : dict
+            keyword arguments passed to fun
 
         Returns
         -------
         jvp3 : array-like
             third derivative times vectors v2, v3, v3, summed over different argnums
 
         """
@@ -520,40 +625,42 @@
         if np.isscalar(argnum3):
             argnum3 = (argnum3 + 2,)
             v3 = (v3,) if not isinstance(v3, tuple) else v3
         else:
             argnum3 = tuple([i + 2 for i in argnum3])
             v3 = tuple(v3)
 
-        dfdx = lambda dx1, *args: cls.compute_jvp(fun, argnum1, dx1, *args)
-        d2fdx2 = lambda dx1, dx2, *args: cls.compute_jvp(dfdx, argnum2, dx2, dx1, *args)
+        dfdx = lambda dx1, *args: cls.compute_jvp(fun, argnum1, dx1, *args, **kwargs)
+        d2fdx2 = lambda dx1, dx2, *args: cls.compute_jvp(
+            dfdx, argnum2, dx2, dx1, *args, **kwargs
+        )
         d3fdx3 = lambda dx1, dx2, dx3: cls.compute_jvp(
-            d2fdx2, argnum3, dx3, dx2, dx1, *args
+            d2fdx2, argnum3, dx3, dx2, dx1, *args, **kwargs
         )
         return d3fdx3(v1, v2, v3)
 
-    def _compute_jvp(self, v, *args):
+    def _compute_jvp(self, v, *args, **kwargs):
         return self.compute_jvp(
-            self._fun, self._argnum, v, *args, rel_step=self.rel_step
+            self._fun, self._argnum, v, *args, rel_step=self.rel_step, **kwargs
         )
 
     @classmethod
     def _compute_jvp_1arg(cls, fun, argnum, v, *args, **kwargs):
         """Compute a jvp wrt a single argument."""
-        rel_step = kwargs.get("rel_step", 1e-3)
+        rel_step = kwargs.pop("rel_step", 1e-3)
         normv = np.linalg.norm(v)
         if normv != 0:
             vh = v / normv
         else:
             vh = v
         x = args[argnum]
 
         def f(x):
             tempargs = args[0:argnum] + (x,) + args[argnum + 1 :]
-            return fun(*tempargs)
+            return fun(*tempargs, **kwargs)
 
         h = rel_step
         df = (f(x + h * vh) - f(x - h * vh)) / (2 * h)
         return df * normv
 
     def _set_mode(self, mode):
         if mode not in ["fwd", "rev", "grad", "hess", "jvp"]:
@@ -591,24 +698,11 @@
             fun and x is the input argument at position argnum. Exact shape and meaning
             will depend on "mode"
 
         """
         return self._compute(*args)
 
 
-def nested_zeros_like(x):
-    """Get a nested pytree of zeros like a given pytree."""
-    if x is None:
-        return None
-    if jnp.isscalar(x):
-        return 0.0
-    if isinstance(x, tuple):
-        return tuple([nested_zeros_like(a) for a in x])
-    if isinstance(x, list):
-        return list([nested_zeros_like(a) for a in x])
-    return jnp.zeros_like(x)
-
-
 if use_jax:
     Derivative = AutoDiffDerivative
 else:
     Derivative = FiniteDiffDerivative
```

### Comparing `desc-opt-0.9.0/desc/equilibrium/configuration.py` & `desc-opt-0.9.1/desc/equilibrium/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,14 @@
         atomic_number=None,
         surface=None,
         axis=None,
         sym=None,
         spectral_indexing=None,
         **kwargs,
     ):
-
         assert spectral_indexing in [None, "ansi", "fringe",], (
             "spectral_indexing should be one of 'ansi', 'fringe', None, got "
             + f"{spectral_indexing}"
         )
         if spectral_indexing is None and hasattr(surface, "spectral_indexing"):
             self._spectral_indexing = surface.spectral_indexing
         elif spectral_indexing is None:
@@ -504,68 +503,83 @@
         """Return a (deep)copy of this equilibrium."""
         if deepcopy:
             new = copy.deepcopy(self)
         else:
             new = copy.copy(self)
         return new
 
-    def change_resolution(self, L=None, M=None, N=None, NFP=None, *args, **kwargs):
+    def change_resolution(
+        self, L=None, M=None, N=None, NFP=None, sym=None, *args, **kwargs
+    ):
         """Set the spectral resolution.
 
         Parameters
         ----------
         L : int
-            maximum radial zernike mode number
+            Maximum radial Zernike mode number.
         M : int
-            maximum poloidal fourier mode number
+            Maximum poloidal Fourier mode number.
         N : int
-            maximum toroidal fourier mode number
+            Maximum toroidal Fourier mode number.
         NFP : int
             Number of field periods.
+        sym : bool
+            Whether to enforce stellarator symmetry.
 
         """
-        L_change = M_change = N_change = NFP_change = False
+        L_change = M_change = N_change = NFP_change = sym_change = False
         if L is not None and L != self.L:
             L_change = True
             self._L = L
         if M is not None and M != self.M:
             M_change = True
             self._M = M
         if N is not None and N != self.N:
             N_change = True
             self._N = N
         if NFP is not None and NFP != self.NFP:
             NFP_change = True
             self._NFP = NFP
+        if sym is not None and sym != self.sym:
+            sym_change = True
+            self._sym = sym
 
-        if not np.any([L_change, M_change, N_change, NFP_change]):
+        if not np.any([L_change, M_change, N_change, NFP_change, sym_change]):
             return
 
         old_modes_R = self.R_basis.modes
         old_modes_Z = self.Z_basis.modes
         old_modes_L = self.L_basis.modes
 
-        self.R_basis.change_resolution(self.L, self.M, self.N, self.NFP)
-        self.Z_basis.change_resolution(self.L, self.M, self.N, self.NFP)
-        self.L_basis.change_resolution(self.L, self.M, self.N, self.NFP)
+        self.R_basis.change_resolution(
+            self.L, self.M, self.N, NFP=self.NFP, sym="cos" if self.sym else self.sym
+        )
+        self.Z_basis.change_resolution(
+            self.L, self.M, self.N, NFP=self.NFP, sym="sin" if self.sym else self.sym
+        )
+        self.L_basis.change_resolution(
+            self.L, self.M, self.N, NFP=self.NFP, sym="sin" if self.sym else self.sym
+        )
 
         for profile in [
             "pressure",
             "iota",
             "current",
             "electron_temperature",
             "electron_density",
             "ion_temperature",
             "atomic_number",
         ]:
             p = getattr(self, profile)
             if hasattr(p, "change_resolution") and L_change:
                 p.change_resolution(max(p.basis.L, self.L))
 
-        self.surface.change_resolution(self.L, self.M, self.N, NFP=self.NFP)
+        self.surface.change_resolution(
+            self.L, self.M, self.N, NFP=self.NFP, sym=self.sym
+        )
 
         self._R_lmn = copy_coeffs(self.R_lmn, old_modes_R, self.R_basis.modes)
         self._Z_lmn = copy_coeffs(self.Z_lmn, old_modes_Z, self.Z_basis.modes)
         self._L_lmn = copy_coeffs(self.L_lmn, old_modes_L, self.L_basis.modes)
 
     def get_surface_at(self, rho=None, theta=None, zeta=None):
         """Return a representation for a given coordinate surface.
```

### Comparing `desc-opt-0.9.0/desc/equilibrium/coords.py` & `desc-opt-0.9.1/desc/equilibrium/coords.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,15 +422,15 @@
     L_grid : int, optional
         radial spatial resolution to use for fit to new basis. Default = 2*L
     M_grid : int, optional
         poloidal spatial resolution to use for fit to new basis. Default = 2*M
     N_grid : int, optional
         toroidal spatial resolution to use for fit to new basis. Default = 2*N
     rcond : float, optional
-        cutoff for small singular values in least squares fit.
+        cutoff for small singular values in the least squares fit.
     copy : bool, optional
         Whether to update the existing equilibrium or make a copy (Default).
 
     Returns
     -------
     eq_sfl : Equilibrium
         Equilibrium transformed to a straight field line coordinate representation.
```

### Comparing `desc-opt-0.9.0/desc/equilibrium/equilibrium.py` & `desc-opt-0.9.1/desc/equilibrium/equilibrium.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,15 +88,14 @@
     sym : bool (optional)
         Whether to enforce stellarator symmetry. Default surface.sym or False.
     spectral_indexing : str (optional)
         Type of Zernike indexing scheme to use. Default ``'ansi'``
     """
 
     _io_attrs_ = _Configuration._io_attrs_ + [
-        "_solved",
         "_L_grid",
         "_M_grid",
         "_N_grid",
         "_node_pattern",
     ]
 
     def __init__(
@@ -119,15 +118,14 @@
         atomic_number=None,
         surface=None,
         axis=None,
         sym=None,
         spectral_indexing=None,
         **kwargs,
     ):
-
         super().__init__(
             Psi,
             NFP,
             L,
             M,
             N,
             pressure,
@@ -159,15 +157,14 @@
             and (N_grid == int(N_grid))
             and (N_grid >= 0)
         ), "N_grid should be a non-negative integer or None, got {N_grid}"
         self._L_grid = L_grid if L_grid is not None else 2 * self.L
         self._M_grid = M_grid if M_grid is not None else 2 * self.M
         self._N_grid = N_grid if N_grid is not None else 2 * self.N
         self._node_pattern = node_pattern if node_pattern is not None else "jacobi"
-        self._solved = False
         self.optimizer_results = {}
 
     def __repr__(self):
         """String form of the object."""
         return (
             type(self).__name__
             + " at "
@@ -219,23 +216,14 @@
     def node_pattern(self):
         """str: Pattern for placement of nodes in curvilinear coordinates."""
         if not hasattr(self, "_node_pattern"):
             self._node_pattern = None
         return self._node_pattern
 
     @property
-    def solved(self):
-        """bool: Whether the equilibrium has been solved."""
-        return self._solved
-
-    @solved.setter
-    def solved(self, solved):
-        self._solved = solved
-
-    @property
     def resolution(self):
         """dict: Spectral and real space resolution parameters of the Equilibrium."""
         return {
             "L": self.L,
             "M": self.M,
             "N": self.N,
             "L_grid": self.L_grid,
@@ -251,48 +239,60 @@
         print(
             "Node resolution (L,M,N)=({},{},{})".format(
                 self.L_grid, self.M_grid, self.N_grid
             )
         )
 
     def change_resolution(
-        self, L=None, M=None, N=None, L_grid=None, M_grid=None, N_grid=None, NFP=None
+        self,
+        L=None,
+        M=None,
+        N=None,
+        L_grid=None,
+        M_grid=None,
+        N_grid=None,
+        NFP=None,
+        sym=None,
     ):
         """Set the spectral resolution and real space grid resolution.
 
         Parameters
         ----------
         L : int
-            maximum radial zernike mode number.
+            Maximum radial Zernike mode number.
         M : int
-            maximum poloidal fourier mode number.
+            Maximum poloidal Fourier mode number.
         N : int
-            maximum toroidal fourier mode number.
+            Maximum toroidal Fourier mode number.
         L_grid : int
-            radial real space grid resolution.
+            Radial real space grid resolution.
         M_grid : int
-            poloidal real space grid resolution.
+            Poloidal real space grid resolution.
         N_grid : int
-            toroidal real space grid resolution.
+            Toroidal real space grid resolution.
         NFP : int
-            number of field periods.
+            Number of field periods.
+        sym : bool
+            Whether to enforce stellarator symmetry.
 
         """
-        L_change = M_change = N_change = NFP_change = False
+        L_change = M_change = N_change = NFP_change = sym_change = False
         if L is not None and L != self.L:
             L_change = True
         if M is not None and M != self.M:
             M_change = True
         if N is not None and N != self.N:
             N_change = True
         if NFP is not None and NFP != self.NFP:
             NFP_change = True
+        if sym is not None and sym != self.sym:
+            sym_change = True
 
-        if any([L_change, M_change, N_change, NFP_change]):
-            super().change_resolution(L, M, N, NFP)
+        if any([L_change, M_change, N_change, NFP_change, sym_change]):
+            super().change_resolution(L, M, N, NFP, sym)
 
         if L_grid is not None and L_grid != self.L_grid:
             self._L_grid = L_grid
         if M_grid is not None and M_grid != self.M_grid:
             self._M_grid = M_grid
         if N_grid is not None and N_grid != self.N_grid:
             self._N_grid = N_grid
@@ -478,19 +478,20 @@
             ``message`` which describes the cause of the termination. See
             `OptimizeResult` for a description of other attributes.
 
 
         """
         if constraints is None:
             constraints = get_fixed_boundary_constraints(
+                eq=self,
                 iota=objective != "vacuum" and self.iota is not None,
                 kinetic=self.electron_temperature is not None,
             )
         if not isinstance(objective, ObjectiveFunction):
-            objective = get_equilibrium_objective(objective)
+            objective = get_equilibrium_objective(eq=self, mode=objective)
         if not isinstance(optimizer, Optimizer):
             optimizer = Optimizer(optimizer)
 
         if copy:
             eq = self.copy()
         else:
             eq = self
@@ -533,15 +534,14 @@
             if value[-1].size:
                 setattr(eq, key, value[-1])
 
         if verbose > 0:
             print("End of solver")
             objective.print_value(objective.x(eq))
 
-        eq.solved = result["success"]
         return eq, result
 
     def optimize(
         self,
         objective=None,
         constraints=None,
         optimizer="proximal-lsq-exact",
@@ -598,18 +598,19 @@
             `OptimizeResult` for a description of other attributes.
 
         """
         if not isinstance(optimizer, Optimizer):
             optimizer = Optimizer(optimizer)
         if constraints is None:
             constraints = get_fixed_boundary_constraints(
+                eq=self,
                 iota=self.iota is not None,
                 kinetic=self.electron_temperature is not None,
             )
-            constraints = (ForceBalance(), *constraints)
+            constraints = (ForceBalance(eq=self), *constraints)
 
         if copy:
             eq = self.copy()
         else:
             eq = self
 
         result = optimizer.optimize(
@@ -637,15 +638,14 @@
                 setattr(eq, key, value[-1])
         if verbose > 0:
             print("End of solver")
             objective.print_value(objective.x(eq))
             for con in constraints:
                 con.print_value(*con.xs(eq))
 
-        eq.solved = result["success"]
         return eq, result
 
     def _optimize(  # noqa: C901
         self,
         objective,
         constraint=None,
         ftol=1e-6,
@@ -692,15 +692,15 @@
         from desc.optimize.utils import check_termination
         from desc.perturbations import optimal_perturb
 
         solve_options = {} if solve_options is None else solve_options
         perturb_options = {} if perturb_options is None else perturb_options
 
         if constraint is None:
-            constraint = get_equilibrium_objective()
+            constraint = get_equilibrium_objective(eq=self)
 
         timer = Timer()
         timer.start("Total time")
 
         eq = self
         if not objective.built:
             objective.build(eq)
@@ -716,15 +716,14 @@
 
         if verbose > 0:
             objective.print_value(objective.x(eq))
 
         iteration = 1
         success = None
         while success is None:
-
             timer.start("Step {} time".format(iteration))
             if verbose > 0:
                 print("====================")
                 print("Optimization Step {}".format(iteration))
                 print("====================")
                 print("Trust-Region ratio = {:9.3e}".format(tr_ratio[0]))
 
@@ -858,17 +857,18 @@
         Returns
         -------
         eq_new : Equilibrium
             Perturbed equilibrium.
 
         """
         if objective is None:
-            objective = get_equilibrium_objective()
+            objective = get_equilibrium_objective(eq=self)
         if constraints is None:
             constraints = get_fixed_boundary_constraints(
+                eq=self,
                 iota=self.iota is not None,
                 kinetic=self.electron_temperature is not None,
             )
 
         eq = perturb(
             self,
             objective,
@@ -877,15 +877,14 @@
             order=order,
             tr_ratio=tr_ratio,
             weight=weight,
             include_f=include_f,
             verbose=verbose,
             copy=copy,
         )
-        eq.solved = False
 
         return eq
 
 
 class EquilibriaFamily(IOAble, MutableSequence):
     """EquilibriaFamily stores a list of Equilibria.
 
@@ -903,15 +902,14 @@
 
         For more information see inputs required by ``'Equilibrium'``.
     """
 
     _io_attrs_ = ["_equilibria"]
 
     def __init__(self, *args):
-
         self.equilibria = []
         if len(args) == 1 and isinstance(args[0], list):
             for inp in args[0]:
                 self.equilibria.append(Equilibrium(**inp))
         else:
             for arg in args:
                 if isinstance(arg, Equilibrium):
```

### Comparing `desc-opt-0.9.0/desc/equilibrium/initial_guess.py` & `desc-opt-0.9.1/desc/equilibrium/initial_guess.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/equilibrium/utils.py` & `desc-opt-0.9.1/desc/equilibrium/utils.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/examples/ARIES-CS_output.h5` & `desc-opt-0.9.1/desc/examples/ARIES-CS_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/examples/ATF_output.h5` & `desc-opt-0.9.1/desc/examples/ATF_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/examples/DSHAPE_CURRENT_output.h5` & `desc-opt-0.9.1/desc/examples/DSHAPE_CURRENT_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/examples/DSHAPE_output.h5` & `desc-opt-0.9.1/desc/examples/DSHAPE_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/examples/ESTELL_output.h5` & `desc-opt-0.9.1/desc/examples/ESTELL_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/examples/HELIOTRON_output.h5` & `desc-opt-0.9.1/desc/examples/HELIOTRON_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/examples/NCSX_output.h5` & `desc-opt-0.9.1/desc/examples/NCSX_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/examples/QAS_output.h5` & `desc-opt-0.9.1/desc/examples/QAS_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/examples/SOLOVEV_output.h5` & `desc-opt-0.9.1/desc/examples/SOLOVEV_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/examples/W7-X_output.h5` & `desc-opt-0.9.1/desc/examples/W7-X_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/examples/WISTELL-A_output.h5` & `desc-opt-0.9.1/desc/examples/WISTELL-A_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/examples/__init__.py` & `desc-opt-0.9.1/desc/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/examples/precise_QA.py` & `desc-opt-0.9.1/desc/examples/precise_QA.py`

 * *Files 15% similar despite different names*

```diff
@@ -49,19 +49,21 @@
 for k in range(1, eq.M + 1):
     print("\n==================================")
     print("Optimizing boundary modes M,N <= {}".format(k))
     print("====================================")
     objective = ObjectiveFunction(
         (
             # pass in the grid we defined, and don't forget the target helicity!
-            QuasisymmetryTwoTerm(helicity=(1, 0), grid=grid, normalize=False),
-            AspectRatio(target=6, weight=1e1, normalize=False),
+            QuasisymmetryTwoTerm(
+                eq=eqfam[-1], helicity=(1, 0), grid=grid, normalize=False
+            ),
+            AspectRatio(eq=eqfam[-1], target=6, weight=1e1, normalize=False),
             # this targets a profile pointwise, which is ok because we expect it to be
             # fairly flat
-            RotationalTransform(target=0.42, weight=10, normalize=False),
+            RotationalTransform(eq=eqfam[-1], target=0.42, weight=10, normalize=False),
             # we could optionally set normalize=True which would compute things in
             # normalized/dimensionless units, effectively changing the weights
         ),
         verbose=0,
     )
     # as opposed to SIMSOPT and STELLOPT where variables are assumed fixed, in DESC
     # we assume variables are free. Here we decide which ones to fix, starting with
@@ -76,20 +78,20 @@
     )
     Z_modes = eq.surface.Z_basis.modes[
         np.max(np.abs(eq.surface.Z_basis.modes), 1) > k, :
     ]
     # next we create the constraints, using the mode number arrays just created
     # if we didn't pass those in, it would fix all the modes (like for the profiles)
     constraints = (
-        ForceBalance(),  # J x B - grad(p) = 0
-        FixBoundaryR(modes=R_modes),
-        FixBoundaryZ(modes=Z_modes),
-        FixPressure(),
-        FixCurrent(),
-        FixPsi(),
+        ForceBalance(eq=eqfam[-1]),  # J x B - grad(p) = 0
+        FixBoundaryR(eq=eqfam[-1], modes=R_modes),
+        FixBoundaryZ(eq=eqfam[-1], modes=Z_modes),
+        FixPressure(eq=eqfam[-1]),
+        FixCurrent(eq=eqfam[-1]),
+        FixPsi(eq=eqfam[-1]),
     )
     # this is the default optimizer, which re-solves the equilibrium at each step
     optimizer = Optimizer("proximal-lsq-exact")
     # we get a new equilibrium by optimizing the old one and passing copy=True.
     # otherwise, we could modify the original equilibrium in place
     eq_new, out = eqfam[-1].optimize(
         objective=objective,
```

### Comparing `desc-opt-0.9.0/desc/examples/precise_QA_output.h5` & `desc-opt-0.9.1/desc/examples/precise_QA_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/examples/precise_QH_output.h5` & `desc-opt-0.9.1/desc/examples/precise_QH_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/geometry/core.py` & `desc-opt-0.9.1/desc/geometry/core.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/geometry/curve.py` & `desc-opt-0.9.1/desc/geometry/curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,25 +150,33 @@
         self._Z_transform.grid = self.grid
 
     @property
     def N(self):
         """Maximum mode number."""
         return max(self.R_basis.N, self.Z_basis.N)
 
-    def change_resolution(self, N=None, NFP=None):
+    def change_resolution(self, N=None, NFP=None, sym=None):
         """Change the maximum toroidal resolution."""
-        if ((N is not None) and (N != self.N)) or (
-            (NFP is not None) and (NFP != self.NFP)
+        if (
+            ((N is not None) and (N != self.N))
+            or ((NFP is not None) and (NFP != self.NFP))
+            or (sym is not None)
+            and (sym != self.sym)
         ):
             self._NFP = NFP if NFP is not None else self.NFP
+            self._sym = sym if sym is not None else self.sym
             N = N if N is not None else self.N
             R_modes_old = self.R_basis.modes
             Z_modes_old = self.Z_basis.modes
-            self.R_basis.change_resolution(N=N, NFP=self.NFP)
-            self.Z_basis.change_resolution(N=N, NFP=self.NFP)
+            self.R_basis.change_resolution(
+                N=N, NFP=self.NFP, sym="cos" if self.sym else self.sym
+            )
+            self.Z_basis.change_resolution(
+                N=N, NFP=self.NFP, sym="sin" if self.sym else self.sym
+            )
             if hasattr(self.grid, "change_resolution"):
                 self.grid.change_resolution(
                     self.grid.L, self.grid.M, self.grid.N, self.NFP
                 )
             self._R_transform, self._Z_transform = self._get_transforms(self.grid)
             self.R_n = copy_coeffs(self.R_n, R_modes_old, self.R_basis.modes)
             self.Z_n = copy_coeffs(self.Z_n, Z_modes_old, self.Z_basis.modes)
@@ -766,15 +774,15 @@
         theta = transform.grid.nodes[:, 2]
         return jnp.trapz(T, theta)
 
     # TODO: methods for converting between representations
 
 
 class FourierPlanarCurve(Curve):
-    """Curve that lines in a plane.
+    """Curve that lies in a plane.
 
     Parameterized by a point (the center of the curve), a vector (normal to the plane),
     and a Fourier series defining the radius from the center as a function of
     a polar angle theta.
 
     Parameters
     ----------
```

### Comparing `desc-opt-0.9.0/desc/geometry/surface.py` & `desc-opt-0.9.1/desc/geometry/surface.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,14 @@
         NFP=1,
         sym="auto",
         rho=1,
         grid=None,
         name="",
         check_orientation=True,
     ):
-
         if R_lmn is None:
             R_lmn = np.array([10, 1])
             modes_R = np.array([[0, 0], [1, 0]])
         if Z_lmn is None:
             Z_lmn = np.array([0, -1])
             modes_Z = np.array([[0, 0], [-1, 0]])
         if modes_Z is None:
@@ -178,26 +177,28 @@
         self._R_transform.grid = self.grid
         self._Z_transform.grid = self.grid
 
     def change_resolution(self, *args, **kwargs):
         """Change the maximum poloidal and toroidal resolution."""
         assert (
             ((len(args) in [2, 3]) and len(kwargs) == 0)
-            or ((len(args) in [2, 3]) and len(kwargs) == 1 and "NFP" in kwargs)
+            or ((len(args) in [2, 3]) and len(kwargs) in [1, 2])
             or (len(args) == 0)
         ), (
             "change_resolution should be called with 2 (M,N) or 3 (L,M,N) "
             + "positional arguments or only keyword arguments."
         )
         L = kwargs.pop("L", None)
         M = kwargs.pop("M", None)
         N = kwargs.pop("N", None)
         NFP = kwargs.pop("NFP", None)
+        sym = kwargs.pop("sym", None)
         assert len(kwargs) == 0, "change_resolution got unexpected kwarg: {kwargs}"
         self._NFP = NFP if NFP is not None else self.NFP
+        self._sym = sym if sym is not None else self.sym
         if L is not None:
             warnings.warn(
                 "FourierRZToroidalSurface does not have radial resolution, ignoring L"
             )
         if len(args) == 2:
             M, N = args
         elif len(args) == 3:
@@ -208,16 +209,20 @@
             or ((M is not None) and (M != self.M))
             or (NFP is not None)
         ):
             M = M if M is not None else self.M
             N = N if N is not None else self.N
             R_modes_old = self.R_basis.modes
             Z_modes_old = self.Z_basis.modes
-            self.R_basis.change_resolution(M=M, N=N, NFP=self.NFP)
-            self.Z_basis.change_resolution(M=M, N=N, NFP=self.NFP)
+            self.R_basis.change_resolution(
+                M=M, N=N, NFP=self.NFP, sym="cos" if self.sym else self.sym
+            )
+            self.Z_basis.change_resolution(
+                M=M, N=N, NFP=self.NFP, sym="sin" if self.sym else self.sym
+            )
             if hasattr(self.grid, "change_resolution"):
                 self.grid.change_resolution(
                     self.grid.L, self.grid.M, self.grid.N, self.NFP
                 )
             self._R_transform, self._Z_transform = self._get_transforms(self.grid)
             self.R_lmn = copy_coeffs(self.R_lmn, R_modes_old, self.R_basis.modes)
             self.Z_lmn = copy_coeffs(self.Z_lmn, Z_modes_old, self.Z_basis.modes)
@@ -744,38 +749,48 @@
         self._R_transform.grid = self.grid
         self._Z_transform.grid = self.grid
 
     def change_resolution(self, *args, **kwargs):
         """Change the maximum radial and poloidal resolution."""
         assert (
             ((len(args) in [2, 3]) and len(kwargs) == 0)
-            or ((len(args) in [2, 3]) and len(kwargs) == 1 and "NFP" in kwargs)
+            or ((len(args) in [2, 3]) and len(kwargs) in [1, 2])
             or (len(args) == 0)
         ), (
             "change_resolution should be called with 2 (M,N) or 3 (L,M,N) "
             + "positional arguments or only keyword arguments."
         )
         L = kwargs.pop("L", None)
         M = kwargs.pop("M", None)
         N = kwargs.pop("N", None)
+        sym = kwargs.pop("sym", None)
         assert len(kwargs) == 0, "change_resolution got unexpected kwarg: {kwargs}"
+        self._sym = sym if sym is not None else self.sym
         if N is not None:
             warnings.warn(
                 "ZernikeRZToroidalSection does not have toroidal resolution, ignoring N"
             )
         if len(args) == 2:
             L, M = args
         elif len(args) == 3:
             L, M, N = args
 
         if ((L is not None) and (L != self.L)) or ((M is not None) and (M != self.M)):
+            L = L if L is not None else self.L
+            M = M if M is not None else self.M
             R_modes_old = self.R_basis.modes
             Z_modes_old = self.Z_basis.modes
-            self.R_basis.change_resolution(L=L, M=M)
-            self.Z_basis.change_resolution(L=L, M=M)
+            self.R_basis.change_resolution(
+                L=L, M=M, sym="cos" if self.sym else self.sym
+            )
+            self.Z_basis.change_resolution(
+                L=L, M=M, sym="sin" if self.sym else self.sym
+            )
+            if hasattr(self.grid, "change_resolution"):
+                self.grid.change_resolution(self.grid.L, self.grid.M, self.grid.N)
             self._R_transform, self._Z_transform = self._get_transforms(self.grid)
             self.R_lmn = copy_coeffs(self.R_lmn, R_modes_old, self.R_basis.modes)
             self.Z_lmn = copy_coeffs(self.Z_lmn, Z_modes_old, self.Z_basis.modes)
             self._L = L
             self._M = M
 
     @property
```

### Comparing `desc-opt-0.9.0/desc/geometry/utils.py` & `desc-opt-0.9.1/desc/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/grid.py` & `desc-opt-0.9.1/desc/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,43 +154,43 @@
         nodes = self.nodes.copy().astype(float)
         nodes[:, 1] %= 2 * np.pi
         nodes[:, 2] %= 2 * np.pi / self.NFP
         # reduce weights for duplicated nodes
         _, inverse, counts = np.unique(
             nodes, axis=0, return_inverse=True, return_counts=True
         )
-        duplicates = np.tile(np.atleast_2d(counts[inverse]).T, 3)
-        temp_spacing = np.copy(self.spacing)
-        temp_spacing /= duplicates ** (1 / 3)
+        duplicates = counts[inverse]
+        temp_spacing = self.spacing.copy()
+        temp_spacing = (temp_spacing.T / duplicates ** (1 / 3)).T
         # scale weights sum to full volume
         temp_spacing *= (4 * np.pi**2 / temp_spacing.prod(axis=1).sum()) ** (1 / 3)
         self._weights = temp_spacing.prod(axis=1)
 
         # Spacing is the differential element used for integration over surfaces.
         # For this, 2 columns of the matrix are used.
         # Spacing is rescaled below to get the correct double product for each pair
         # of columns in grid.spacing.
         # The reduction of weight on duplicate nodes should be accounted for
         # by the 2 columns of spacing which span the surface.
-        self._spacing /= duplicates ** (1 / 2)
+        self._spacing = (self.spacing.T / duplicates ** (1 / 2)).T
         # Note we rescale 3 columns by the factor that 'should' rescale 2 columns,
         # so grid.spacing is valid for integrals over all surface labels.
         # Because a surface integral always ignores 1 column, with this approach,
         # duplicates nodes are scaled down properly regardless of which two columns
         # span the surface.
 
         # scale areas sum to full area
         # The following operation is not a general solution to return the weight
         # removed from the duplicate nodes back to the unique nodes.
         # (For the 3 predefined grid types this line of code has no effect).
         # For this reason, duplicates should typically be deleted rather than rescaled.
         # Note we multiply each column by duplicates^(1/6) to account for the extra
         # division by duplicates^(1/2) in one of the columns above.
         self._spacing *= (
-            4 * np.pi**2 / (self.spacing * duplicates ** (1 / 6)).prod(axis=1).sum()
+            4 * np.pi**2 / (self.spacing.T * duplicates ** (1 / 6)).prod(axis=0).sum()
         ) ** (1 / 3)
 
     def _create_nodes(self, nodes):
         """Allow for custom node creation.
 
         Parameters
         ----------
```

### Comparing `desc-opt-0.9.0/desc/interpolate.py` & `desc-opt-0.9.1/desc/interpolate.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,16 @@
         - `'cubic'`: C1 cubic splines (aka local splines)
         - `'cubic2'`: C2 cubic splines (aka natural splines)
         - `'catmull-rom'`: C1 cubic centripetal "tension" splines
         - `'cardinal'`: c1 cubic general tension splines. If used, can also pass keyword
             parameter `c` in float[0,1] to specify tension
         - `'monotonic'`: C1 cubic splines that attempt to preserve monotonicity in the
             data, and will not introduce new extrama in the interpolated points
+        - `'monotonic-0'`: same as `'monotonic'` but with 0 first derivatives at both
+            endpoints
     derivative : int
         derivative order to calculate
     extrap : bool, float, array-like
         whether to extrapolate values beyond knots (True) or return nan (False),
         or a specified value to return for query points outside the bounds. Can
         also be passed as a 2 element array or tuple to specify different conditions
         for xq<x[0] and x[-1]<xq
@@ -87,15 +89,22 @@
                 jnp.take(f, i - 1, axis) + delta * dxi * df,
             )
         elif derivative == 1:
             fq = df * dxi
         else:
             fq = jnp.zeros((xq.size, *f.shape[1:]))
 
-    elif method in ["cubic", "cubic2", "cardinal", "catmull-rom", "monotonic"]:
+    elif method in [
+        "cubic",
+        "cubic2",
+        "cardinal",
+        "catmull-rom",
+        "monotonic",
+        "monotonic-0",
+    ]:
         i = jnp.clip(jnp.searchsorted(x, xq, side="right"), 1, len(x) - 1)
         if fx is None:
             fx = _approx_df(x, f, method, axis, **kwargs)
 
         dx = x[i] - x[i - 1]
         delta = xq - x[i - 1]
         dxi = jnp.where(dx == 0, 0, 1 / dx)
@@ -648,14 +657,15 @@
                     + jnp.take(df, jnp.arange(1, df.shape[axis]), axis, mode="wrap")
                 ),
                 jnp.take(df, jnp.array([-1]), axis, mode="wrap"),
             ],
             axis=axis,
         )
         return fx
+
     if method == "cubic2":
         dx = jnp.diff(x)
         df = jnp.diff(f, axis=axis)
         if df.ndim > dx.ndim:
             dx = jnp.expand_dims(dx, tuple(range(1, df.ndim)))
             dx = jnp.moveaxis(dx, 0, axis)
         dxi = jnp.where(dx == 0, 0, 1 / dx)
@@ -691,14 +701,15 @@
             ],
             axis=axis,
         )
         b = jnp.moveaxis(b, axis, 0).reshape((b.shape[axis], -1))
         fx = jnp.linalg.solve(A, b)
         fx = jnp.moveaxis(fx.reshape(f.shape), 0, axis)
         return fx
+
     if method in ["cardinal", "catmull-rom"]:
         dx = x[2:] - x[:-2]
         df = jnp.take(f, jnp.arange(2, f.shape[axis]), axis, mode="wrap") - jnp.take(
             f, jnp.arange(0, f.shape[axis] - 2), axis, mode="wrap"
         )
         dxi = jnp.where(dx == 0, 0, 1 / dx)
         if df.ndim > dxi.ndim:
@@ -725,15 +736,16 @@
         )
         if method == "cardinal":
             c = kwargs.get("c", 0)
         else:
             c = 0
         fx = (1 - c) * jnp.concatenate([fx0, df, fx1], axis=axis)
         return fx
-    if method == "monotonic":
+
+    if method in ["monotonic", "monotonic-0"]:
         f = jnp.moveaxis(f, axis, 0)
         fshp = f.shape
         if f.ndim == 1:
             # So that _edge_case doesn't end up assigning to scalars
             x = x[:, None]
             f = f[:, None]
         hk = x[1:] - x[:-1]
@@ -745,32 +757,39 @@
         w1 = 2 * hk[1:] + hk[:-1]
         w2 = hk[1:] + 2 * hk[:-1]
 
         whmean = (w1 / mk[:-1] + w2 / mk[1:]) / (w1 + w2)
 
         dk = jnp.where(condition, 0, 1.0 / whmean)
 
-        # special case endpoints, as suggested in
-        # Cleve Moler, Numerical Computing with MATLAB, Chap 3.6 (pchiptx.m)
-        def _edge_case(h0, h1, m0, m1):
-            # one-sided three-point estimate for the derivative
-            d = ((2 * h0 + h1) * m0 - h0 * m1) / (h0 + h1)
-
-            # try to preserve shape
-            mask = jnp.sign(d) != jnp.sign(m0)
-            mask2 = (jnp.sign(m0) != jnp.sign(m1)) & (jnp.abs(d) > 3.0 * jnp.abs(m0))
-            mmm = (~mask) & mask2
+        if method == "monotonic-0":
+            d0 = jnp.zeros((1, 1))
+            d1 = jnp.zeros((1, 1))
+
+        else:
+            # special case endpoints, as suggested in
+            # Cleve Moler, Numerical Computing with MATLAB, Chap 3.6 (pchiptx.m)
+            def _edge_case(h0, h1, m0, m1):
+                # one-sided three-point estimate for the derivative
+                d = ((2 * h0 + h1) * m0 - h0 * m1) / (h0 + h1)
+
+                # try to preserve shape
+                mask = jnp.sign(d) != jnp.sign(m0)
+                mask2 = (jnp.sign(m0) != jnp.sign(m1)) & (
+                    jnp.abs(d) > 3.0 * jnp.abs(m0)
+                )
+                mmm = (~mask) & mask2
 
-            d = jnp.where(mask, 0.0, d)
-            d = jnp.where(mmm, 3.0 * m0, d)
+                d = jnp.where(mask, 0.0, d)
+                d = jnp.where(mmm, 3.0 * m0, d)
+                return d
 
-            return d
+            d0 = _edge_case(hk[0], hk[1], mk[0], mk[1])[None]
+            d1 = _edge_case(hk[-1], hk[-2], mk[-1], mk[-2])[None]
 
-        d0 = _edge_case(hk[0], hk[1], mk[0], mk[1])[None]
-        d1 = _edge_case(hk[-1], hk[-2], mk[-1], mk[-2])[None]
         dk = jnp.concatenate([d0, dk, d1])
         return dk.reshape(fshp)
 
 
 # fmt: off
 A_TRICUBIC = np.array([
     [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, # noqa: E501
```

### Comparing `desc-opt-0.9.0/desc/io/ascii_io.py` & `desc-opt-0.9.1/desc/io/ascii_io.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/io/core_io.py` & `desc-opt-0.9.1/desc/io/core_io.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/io/equilibrium_io.py` & `desc-opt-0.9.1/desc/io/equilibrium_io.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/io/hdf5_io.py` & `desc-opt-0.9.1/desc/io/hdf5_io.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/io/input_reader.py` & `desc-opt-0.9.1/desc/io/input_reader.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/io/pickle_io.py` & `desc-opt-0.9.1/desc/io/pickle_io.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/magnetic_fields.py` & `desc-opt-0.9.1/desc/magnetic_fields.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/objectives/__init__.py` & `desc-opt-0.9.1/desc/objectives/__init__.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/objectives/_bootstrap.py` & `desc-opt-0.9.1/desc/objectives/_bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,27 +90,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             grid = LinearGrid(
                 M=eq.M_grid,
                 N=eq.N_grid,
                 NFP=eq.NFP,
                 sym=eq.sym,
                 rho=np.linspace(1 / 5, 1, 5),
```

### Comparing `desc-opt-0.9.0/desc/objectives/_equilibrium.py` & `desc-opt-0.9.1/desc/objectives/_equilibrium.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,27 +85,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             if eq.node_pattern is None or eq.node_pattern in [
                 "jacobi",
                 "cheb1",
                 "cheb2",
                 "ocs",
                 "linear",
@@ -267,27 +268,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             if eq.node_pattern is None or eq.node_pattern in [
                 "jacobi",
                 "cheb1",
                 "cheb2",
                 "ocs",
                 "linear",
@@ -440,27 +442,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             if eq.node_pattern is None or eq.node_pattern in [
                 "jacobi",
                 "cheb1",
                 "cheb2",
                 "ocs",
                 "linear",
@@ -615,27 +618,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             if eq.node_pattern in [
                 "jacobi",
                 "cheb1",
                 "cheb2",
                 "ocs",
                 "linear",
@@ -801,27 +805,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             if eq.node_pattern is None or eq.node_pattern in [
                 "jacobi",
                 "cheb1",
                 "cheb2",
                 "ocs",
                 "linear",
```

### Comparing `desc-opt-0.9.0/desc/objectives/_generic.py` & `desc-opt-0.9.1/desc/objectives/_generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,27 +103,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             grid = QuadratureGrid(eq.L_grid, eq.M_grid, eq.N_grid, eq.NFP)
         else:
             grid = self._grid
 
         def getvars(fun):
             pattern = r"data\[(.*?)\]"
@@ -236,27 +237,28 @@
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
         self._units = "(" + data_index[self.f]["units"] + ")"
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             grid = QuadratureGrid(eq.L_grid, eq.M_grid, eq.N_grid, eq.NFP)
         else:
             grid = self._grid
 
         if data_index[self.f]["dim"] == 0:
             self._dim_f = 1
@@ -350,27 +352,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             grid = LinearGrid(
                 L=eq.L_grid,
                 M=eq.M_grid,
                 N=eq.N_grid,
                 NFP=eq.NFP,
                 sym=eq.sym,
@@ -527,27 +530,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             grid = LinearGrid(
                 L=eq.L_grid,
                 M=eq.M_grid,
                 N=eq.N_grid,
                 NFP=eq.NFP,
                 sym=eq.sym,
```

### Comparing `desc-opt-0.9.0/desc/objectives/_geometry.py` & `desc-opt-0.9.1/desc/objectives/_geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,27 +71,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             grid = QuadratureGrid(L=eq.L_grid, M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
         else:
             grid = self._grid
 
         self._dim_f = 1
         self._data_keys = ["R0/a"]
@@ -192,27 +193,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             grid = QuadratureGrid(L=eq.L_grid, M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
         else:
             grid = self._grid
 
         self._dim_f = 1
         self._data_keys = ["a_major/a_minor"]
@@ -313,27 +315,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             grid = QuadratureGrid(L=eq.L_grid, M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
         else:
             grid = self._grid
 
         self._dim_f = 1
         self._data_keys = ["V"]
@@ -472,51 +475,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def print_value(self, *args, **kwargs):
-        """Print the value of the objective."""
-        f = self.compute(*args, **kwargs)
-        print("Maximum " + self._print_value_fmt.format(jnp.max(f)) + self._units)
-        print("Minimum " + self._print_value_fmt.format(jnp.min(f)) + self._units)
-        print("Average " + self._print_value_fmt.format(jnp.mean(f)) + self._units)
-
-        if self._normalize:
-            print(
-                "Maximum "
-                + self._print_value_fmt.format(jnp.max(f / self.normalization))
-                + "(normalized)"
-            )
-            print(
-                "Minimum "
-                + self._print_value_fmt.format(jnp.min(f / self.normalization))
-                + "(normalized)"
-            )
-            print(
-                "Average "
-                + self._print_value_fmt.format(jnp.mean(f / self.normalization))
-                + "(normalized)"
-            )
-
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._surface_grid is None:
             surface_grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
         else:
             surface_grid = self._surface_grid
         if self._plasma_grid is None:
             plasma_grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
         else:
@@ -591,14 +571,38 @@
             plasma_coords[:, None, :] - self._surface_coords[None, :, :], axis=-1
         )
         if self._use_softmin:  # do softmin
             return jnp.apply_along_axis(jax_softmin, 0, d, self._alpha)
         else:  # do hardmin
             return d.min(axis=0)
 
+    def print_value(self, *args, **kwargs):
+        """Print the value of the objective."""
+        f = self.compute(*args, **kwargs)
+        print("Maximum " + self._print_value_fmt.format(jnp.max(f)) + self._units)
+        print("Minimum " + self._print_value_fmt.format(jnp.min(f)) + self._units)
+        print("Average " + self._print_value_fmt.format(jnp.mean(f)) + self._units)
+
+        if self._normalize:
+            print(
+                "Maximum "
+                + self._print_value_fmt.format(jnp.max(f / self.normalization))
+                + "(normalized)"
+            )
+            print(
+                "Minimum "
+                + self._print_value_fmt.format(jnp.min(f / self.normalization))
+                + "(normalized)"
+            )
+            print(
+                "Average "
+                + self._print_value_fmt.format(jnp.mean(f / self.normalization))
+                + "(normalized)"
+            )
+
 
 class MeanCurvature(_Objective):
     """Target a particular value for the mean curvature.
 
     The mean curvature H of a surface is an extrinsic measure of curvature that locally
     describes the curvature of an embedded surface in Euclidean space.
 
@@ -656,27 +660,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
         else:
             grid = self._grid
 
         self._dim_f = grid.num_nodes
         self._data_keys = ["curvature_H"]
@@ -789,27 +794,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
         else:
             grid = self._grid
 
         self._dim_f = grid.num_nodes
         self._data_keys = ["curvature_k1", "curvature_k2"]
@@ -917,27 +923,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
         else:
             grid = self._grid
 
         self._dim_f = grid.num_nodes
         self._data_keys = ["L_grad(B)"]
```

### Comparing `desc-opt-0.9.0/desc/objectives/_qs.py` & `desc-opt-0.9.1/desc/objectives/_qs.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,27 +91,28 @@
         self._print_value_fmt = (
             "Quasi-symmetry ({},{}) Boozer error: ".format(
                 self.helicity[0], self.helicity[1]
             )
             + "{:10.3e} "
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         M_booz = self.M_booz or 2 * eq.M
         N_booz = self.N_booz or 2 * eq.N
 
         if self._grid is None:
             grid = LinearGrid(M=2 * M_booz, N=2 * N_booz, NFP=eq.NFP, sym=False)
         else:
             grid = self._grid
@@ -279,27 +280,28 @@
         self._print_value_fmt = (
             "Quasi-symmetry ({},{}) two-term error: ".format(
                 self.helicity[0], self.helicity[1]
             )
             + "{:10.3e} "
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP, sym=eq.sym)
         else:
             grid = self._grid
 
         self._dim_f = grid.num_nodes
         self._data_keys = ["f_C"]
@@ -437,27 +439,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP, sym=eq.sym)
         else:
             grid = self._grid
 
         self._dim_f = grid.num_nodes
         self._data_keys = ["f_T"]
@@ -577,27 +580,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP, sym=eq.sym)
         else:
             grid = self._grid
 
         self._dim_f = grid.num_nodes
         self._data_keys = ["isodynamicity"]
```

### Comparing `desc-opt-0.9.0/desc/objectives/_stability.py` & `desc-opt-0.9.1/desc/objectives/_stability.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,27 +75,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._grid is None:
             grid = LinearGrid(
                 M=eq.M_grid,
                 N=eq.N_grid,
                 NFP=eq.NFP,
                 sym=eq.sym,
                 rho=np.linspace(1 / 5, 1, 5),
@@ -267,26 +268,27 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
         """
+        eq = eq or self._eq
         if self._grid is None:
             grid = LinearGrid(
                 M=eq.M_grid,
                 N=eq.N_grid,
                 NFP=eq.NFP,
                 sym=eq.sym,
                 rho=np.linspace(1 / 5, 1, 5),
```

### Comparing `desc-opt-0.9.0/desc/objectives/linear_objectives.py` & `desc-opt-0.9.1/desc/objectives/linear_objectives.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,27 +57,28 @@
             bounds=None,
             weight=1,
             normalize=False,
             normalize_target=False,
             name=name,
         )
 
-    def build(self, eq, use_jit=False, verbose=1):
+    def build(self, eq=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         modes = eq.surface.R_basis.modes
         idx = np.arange(eq.surface.R_basis.num_modes)
 
         self._dim_f = idx.size
         self._A = np.zeros((self._dim_f, eq.R_basis.num_modes))
         for i, (l, m, n) in enumerate(eq.R_basis.modes):
             if eq.bdry_mode == "lcfs":
@@ -139,27 +140,28 @@
             bounds=None,
             weight=1,
             normalize=False,
             normalize_target=False,
             name=name,
         )
 
-    def build(self, eq, use_jit=False, verbose=1):
+    def build(self, eq=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         modes = eq.surface.Z_basis.modes
         idx = np.arange(eq.surface.Z_basis.num_modes)
 
         self._dim_f = idx.size
         self._A = np.zeros((self._dim_f, eq.Z_basis.num_modes))
         for i, (l, m, n) in enumerate(eq.Z_basis.modes):
             if eq.bdry_mode == "lcfs":
@@ -250,27 +252,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=False, verbose=1):
+    def build(self, eq=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._modes is False or self._modes is None:  # no modes
             modes = np.array([[]], dtype=int)
             idx = np.array([], dtype=int)
         elif self._modes is True:  # all modes
             modes = eq.surface.R_basis.modes
             idx = np.arange(eq.surface.R_basis.num_modes)
         else:  # specified modes
@@ -401,27 +404,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=False, verbose=1):
+    def build(self, eq=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._modes is False or self._modes is None:  # no modes
             modes = np.array([[]], dtype=int)
             idx = np.array([], dtype=int)
         elif self._modes is True:  # all modes
             modes = eq.surface.Z_basis.modes
             idx = np.arange(eq.surface.Z_basis.num_modes)
         else:  # specified modes
@@ -518,27 +522,28 @@
             bounds=None,
             weight=1,
             normalize=False,
             normalize_target=False,
             name=name,
         )
 
-    def build(self, eq, use_jit=False, verbose=1):
+    def build(self, eq=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         L_basis = eq.L_basis
 
         if L_basis.sym:
             self._A = np.zeros((0, L_basis.num_modes))
         else:
             # l(rho,0,0) = 0
             # at theta=zeta=0, basis for lamba reduces to just a polynomial in rho
@@ -599,27 +604,28 @@
     _units = "(radians)"
     _print_value_fmt = "Theta - Theta SFL error: {:10.3e} "
 
     def __init__(self, eq=None, name="Theta SFL"):
 
         super().__init__(eq=eq, target=0, weight=1, name=name)
 
-    def build(self, eq, use_jit=False, verbose=1):
+    def build(self, eq=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         idx = np.arange(eq.L_basis.num_modes)
         modes_idx = idx
         self._idx = idx
 
         self._dim_f = modes_idx.size
 
         self.target = np.zeros_like(modes_idx)
@@ -706,27 +712,28 @@
             bounds=bounds,
             weight=weight,
             name=name,
             normalize=normalize,
             normalize_target=normalize_target,
         )
 
-    def build(self, eq, use_jit=False, verbose=1):
+    def build(self, eq=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         R_basis = eq.R_basis
 
         if self._modes is False or self._modes is None:  # no modes
             modes = np.array([[]], dtype=int)
             idx = np.array([], dtype=int)
         elif self._modes is True:  # all modes
             modes = eq.axis.R_basis.modes
@@ -867,27 +874,28 @@
             bounds=bounds,
             weight=weight,
             name=name,
             normalize=normalize,
             normalize_target=normalize_target,
         )
 
-    def build(self, eq, use_jit=False, verbose=1):
+    def build(self, eq=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         Z_basis = eq.Z_basis
 
         if self._modes is False or self._modes is None:  # no modes
             modes = np.array([[]], dtype=int)
             idx = np.array([], dtype=int)
         elif self._modes is True:  # all modes
             modes = eq.axis.Z_basis.modes
@@ -1032,27 +1040,28 @@
             bounds=bounds,
             weight=weight,
             name=name,
             normalize=normalize,
             normalize_target=normalize_target,
         )
 
-    def build(self, eq, use_jit=False, verbose=1):
+    def build(self, eq=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._modes is True:  # all modes
             modes = eq.R_basis.modes
             idx = np.arange(eq.R_basis.num_modes)
             modes_idx = idx
         else:  # specified modes
             modes = np.atleast_2d(self._modes)
             dtype = {
@@ -1176,27 +1185,28 @@
             bounds=bounds,
             weight=weight,
             name=name,
             normalize=normalize,
             normalize_target=normalize_target,
         )
 
-    def build(self, eq, use_jit=False, verbose=1):
+    def build(self, eq=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._modes is True:  # all modes
             modes = eq.Z_basis.modes
             idx = np.arange(eq.Z_basis.num_modes)
             modes_idx = idx
         else:  # specified modes
             modes = np.atleast_2d(self._modes)
             dtype = {
@@ -1335,27 +1345,28 @@
             bounds=bounds,
             weight=weight,
             name=name,
             normalize=normalize,
             normalize_target=normalize_target,
         )
 
-    def build(self, eq, use_jit=False, verbose=1):
+    def build(self, eq=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._modes is True:  # all modes
             modes = eq.R_basis.modes
             idx = np.arange(eq.R_basis.num_modes)
         else:  # specified modes
             modes = np.atleast_2d(self._modes)
             dtype = {
                 "names": ["f{}".format(i) for i in range(3)],
@@ -1499,27 +1510,28 @@
             bounds=bounds,
             weight=weight,
             name=name,
             normalize=normalize,
             normalize_target=normalize_target,
         )
 
-    def build(self, eq, use_jit=False, verbose=1):
+    def build(self, eq=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._modes is True:  # all modes
             modes = eq.Z_basis.modes
             idx = np.arange(eq.Z_basis.num_modes)
         else:  # specified modes
             modes = np.atleast_2d(self._modes)
             dtype = {
                 "names": ["f{}".format(i) for i in range(3)],
@@ -1651,29 +1663,30 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, profile=None, use_jit=False, verbose=1):
+    def build(self, eq=None, profile=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium
             Equilibrium that will be optimized to satisfy the Objective.
         profile : Profile, optional
             profile to fix
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if self._profile is None or self._profile.params.size != eq.L + 1:
             self._profile = profile
 
         # find indices to fix
         if self._indices is False or self._indices is None:  # no indices to fix
             self._idx = np.array([], dtype=int)
         elif self._indices is True:  # all indices of Profile.params
@@ -1751,27 +1764,28 @@
             normalize=normalize,
             normalize_target=normalize_target,
             profile=profile,
             indices=indices,
             name=name,
         )
 
-    def build(self, eq, use_jit=False, verbose=1):
+    def build(self, eq=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if eq.pressure is None:
             raise RuntimeError(
                 "Attempting to fix pressure on an equilibrium with no "
                 + "pressure profile assigned"
             )
         profile = eq.pressure
         if self._normalize:
@@ -1865,27 +1879,28 @@
             normalize=normalize,
             normalize_target=normalize_target,
             profile=profile,
             indices=indices,
             name=name,
         )
 
-    def build(self, eq, use_jit=False, verbose=1):
+    def build(self, eq=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if eq.iota is None:
             raise RuntimeError(
                 "Attempt to fix rotational transform on an equilibrium with no "
                 + "rotational transform profile assigned"
             )
         profile = eq.iota
         super().build(eq, profile, use_jit, verbose)
@@ -1974,27 +1989,28 @@
             normalize=normalize,
             normalize_target=normalize_target,
             profile=profile,
             indices=indices,
             name=name,
         )
 
-    def build(self, eq, use_jit=False, verbose=1):
+    def build(self, eq=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if eq.current is None:
             raise RuntimeError(
                 "Attempting to fix toroidal current on an equilibrium with no "
                 + "current profile assigned"
             )
         profile = eq.current
         if self._normalize:
@@ -2086,27 +2102,28 @@
             normalize=normalize,
             normalize_target=normalize_target,
             profile=profile,
             indices=indices,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if eq.electron_temperature is None:
             raise RuntimeError(
                 "Attempting to fix electron temperature on an equilibrium with no "
                 + "electron temperature profile assigned"
             )
         profile = eq.electron_temperature
         if self._normalize:
@@ -2198,27 +2215,28 @@
             normalize=normalize,
             normalize_target=normalize_target,
             profile=profile,
             indices=indices,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if eq.electron_density is None:
             raise RuntimeError(
                 "Attempting to fix electron density on an equilibrium with no "
                 + "electron density profile assigned"
             )
         profile = eq.electron_density
         if self._normalize:
@@ -2310,27 +2328,28 @@
             normalize=normalize,
             normalize_target=normalize_target,
             profile=profile,
             indices=indices,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if eq.ion_temperature is None:
             raise RuntimeError(
                 "Attempting to fix ion temperature on an equilibrium with no "
                 + "ion temperature profile assigned"
             )
         profile = eq.ion_temperature
         if self._normalize:
@@ -2424,27 +2443,28 @@
             normalize=normalize,
             normalize_target=normalize_target,
             profile=profile,
             indices=indices,
             name=name,
         )
 
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         if eq.atomic_number is None:
             raise RuntimeError(
                 "Attempting to fix atomic number on an equilibrium with no "
                 + "atomic number profile assigned"
             )
         profile = eq.atomic_number
         super().build(eq, profile, use_jit, verbose)
@@ -2518,27 +2538,28 @@
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
             name=name,
         )
 
-    def build(self, eq, use_jit=False, verbose=1):
+    def build(self, eq=None, use_jit=False, verbose=1):
         """Build constant arrays.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         self._dim_f = 1
 
         if self._target_from_user is None:
             self.target = eq.Psi
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
```

### Comparing `desc-opt-0.9.0/desc/objectives/nae_utils.py` & `desc-opt-0.9.1/desc/objectives/nae_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,52 +162,60 @@
         modes = []
         target = NAEcoeff * r
         for k in range(1, int((desc_eq.L + 1) / 2) + 1):
             modes.append([2 * k - 1, 1, n])
             sum_weights.append([(-1) ** k * k])
         modes = np.atleast_2d(modes)
         sum_weights = -np.atleast_1d(sum_weights)
-        Rcon = FixSumModesR(target=target, sum_weights=sum_weights, modes=modes)
+        Rcon = FixSumModesR(
+            eq=desc_eq, target=target, sum_weights=sum_weights, modes=modes
+        )
         Rconstraints += (Rcon,)
     # Z_1_neg1_n
     for n, NAEcoeff in zip(Zbasis_cos.modes[:, 2], coeffs["Z_1_neg1_n"]):
         sum_weights = []
         modes = []
         target = NAEcoeff * r
         for k in range(1, int((desc_eq.L + 1) / 2) + 1):
             modes.append([2 * k - 1, -1, n])
             sum_weights.append([(-1) ** k * k])
         modes = np.atleast_2d(modes)
         sum_weights = -np.atleast_1d(sum_weights)
-        Zcon = FixSumModesZ(target=target, sum_weights=sum_weights, modes=modes)
+        Zcon = FixSumModesZ(
+            eq=desc_eq, target=target, sum_weights=sum_weights, modes=modes
+        )
         Zconstraints += (Zcon,)
 
     # R_1_neg1_n
     for n, NAEcoeff in zip(Rbasis_sin.modes[:, 2], coeffs["R_1_neg1_n"]):
         sum_weights = []
         modes = []
         target = NAEcoeff * r
         for k in range(1, int((desc_eq.L + 1) / 2) + 1):
             modes.append([2 * k - 1, -1, n])
             sum_weights.append([(-1) ** k * k])
         modes = np.atleast_2d(modes)
         sum_weights = -np.atleast_1d(sum_weights)
-        Rcon = FixSumModesR(target=target, sum_weights=sum_weights, modes=modes)
+        Rcon = FixSumModesR(
+            eq=desc_eq, target=target, sum_weights=sum_weights, modes=modes
+        )
         Rconstraints += (Rcon,)
     # Z_1_1_n
     for n, NAEcoeff in zip(Zbasis_sin.modes[:, 2], coeffs["Z_1_1_n"]):
         sum_weights = []
         modes = []
         target = NAEcoeff * r
         for k in range(1, int((desc_eq.L + 1) / 2) + 1):
             modes.append([2 * k - 1, 1, n])
             sum_weights.append([(-1) ** k * k])
         modes = np.atleast_2d(modes)
         sum_weights = -np.atleast_1d(sum_weights)
-        Zcon = FixSumModesZ(target=target, sum_weights=sum_weights, modes=modes)
+        Zcon = FixSumModesZ(
+            eq=desc_eq, target=target, sum_weights=sum_weights, modes=modes
+        )
         Zconstraints += (Zcon,)
 
     return Rconstraints, Zconstraints
 
 
 def make_RZ_cons_1st_order(qsc, desc_eq):
     """Make the first order NAE constraints for a DESC equilibrium.
```

### Comparing `desc-opt-0.9.0/desc/objectives/normalization.py` & `desc-opt-0.9.1/desc/objectives/normalization.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/objectives/objective_funs.py` & `desc-opt-0.9.1/desc/objectives/objective_funs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Base classes for objectives."""
 
+import warnings
 from abc import ABC, abstractmethod
 from inspect import getfullargspec
 
 import numpy as np
 
 from desc.backend import block_diag, jit, jnp, use_jax
 from desc.compute import arg_order
@@ -17,49 +18,41 @@
 class ObjectiveFunction(IOAble):
     """Objective function comprised of one or more Objectives.
 
     Parameters
     ----------
     objectives : tuple of Objective
         List of objectives to be minimized.
-    eq : Equilibrium, optional
-        Equilibrium that will be optimized to satisfy the objectives.
     use_jit : bool, optional
         Whether to just-in-time compile the objectives and derivatives.
     deriv_mode : {"batched", "blocked"}
         method for computing derivatives. "batched" is generally faster, "blocked" may
         use less memory. Note that the "blocked" Hessian will only be block diagonal.
     verbose : int, optional
         Level of output.
 
     """
 
     _io_attrs_ = ["_objectives"]
 
-    def __init__(
-        self, objectives, eq=None, use_jit=True, deriv_mode="batched", verbose=1
-    ):
-
+    def __init__(self, objectives, use_jit=True, deriv_mode="batched", verbose=1):
         if not isinstance(objectives, (tuple, list)):
             objectives = (objectives,)
         assert all(
             isinstance(obj, _Objective) for obj in objectives
         ), "members of ObjectiveFunction should be instances of _Objective"
         assert use_jit in {True, False}
-        assert deriv_mode in {"batched", "blocked"}
+        assert deriv_mode in {"batched", "blocked", "looped"}
 
         self._objectives = objectives
         self._use_jit = use_jit
         self._deriv_mode = deriv_mode
         self._built = False
         self._compiled = False
 
-        if eq is not None:
-            self.build(eq, use_jit=self._use_jit, verbose=verbose)
-
     def set_args(self, *args):
         """Set which arguments the objective should expect.
 
         Defaults to args from all sub-objectives. Additional arguments can be passed in.
         """
         self._args = list(np.concatenate([obj.args for obj in self.objectives]))
         self._args += list(args)
@@ -133,19 +126,23 @@
             )
             self._jac_unscaled = lambda x: jnp.hstack(
                 [self._derivatives["jac_unscaled"][arg](x) for arg in self.args]
             )
             self._hess = lambda x: block_diag(
                 *[self._derivatives["hess"][arg](x) for arg in self.args]
             )
-        if self._deriv_mode == "batched":
+        if self._deriv_mode in {"batched", "looped"}:
             self._grad = Derivative(self.compute_scalar, mode="grad")
             self._hess = Derivative(self.compute_scalar, mode="hess")
+        if self._deriv_mode == "batched":
             self._jac_scaled = Derivative(self.compute_scaled, mode="fwd")
             self._jac_unscaled = Derivative(self.compute_unscaled, mode="fwd")
+        if self._deriv_mode == "looped":
+            self._jac_scaled = Derivative(self.compute_scaled, mode="looped")
+            self._jac_unscaled = Derivative(self.compute_unscaled, mode="looped")
 
     def jit(self):  # noqa: C901
         """Apply JIT to compute methods, or re-apply after updating self."""
         # can't loop here because del doesn't work on getattr
         # main idea is that when jitting a method, jax replaces that method
         # with a CompiledFunction object, with self compiled in. To re-jit
         # (ie, after updating attributes of self), we just need to delete the jax
@@ -210,19 +207,31 @@
 
         try:
             del self.jvp_unscaled
         except AttributeError:
             pass
         self.jvp_unscaled = jit(self.jvp_unscaled)
 
+        try:
+            del self.vjp_scaled
+        except AttributeError:
+            pass
+        self.vjp_scaled = jit(self.vjp_scaled)
+
+        try:
+            del self.vjp_unscaled
+        except AttributeError:
+            pass
+        self.vjp_unscaled = jit(self.vjp_unscaled)
+
         for obj in self._objectives:
             if obj._use_jit:
                 obj.jit()
 
-    def build(self, eq, use_jit=None, verbose=1):
+    def build(self, eq=None, use_jit=None, verbose=1):
         """Build the objective.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
@@ -469,14 +478,44 @@
         elif len(v) == 3:
             return Derivative.compute_jvp3(
                 self.compute_unscaled, 0, 0, 0, v[0], v[1], v[2], x
             )
         else:
             raise NotImplementedError("Cannot compute JVP higher than 3rd order.")
 
+    def vjp_scaled(self, v, x):
+        """Compute vector-Jacobian product of the objective function.
+
+        Uses the scaled form of the objective.
+
+        Parameters
+        ----------
+        v : ndarray
+            Vector to left-multiply the Jacobian by.
+        x : ndarray
+            Optimization variables.
+
+        """
+        return Derivative.compute_vjp(self.compute_scaled, 0, v, x)
+
+    def vjp_unscaled(self, v, x):
+        """Compute vector-Jacobian product of the objective function.
+
+        Uses the unscaled form of the objective.
+
+        Parameters
+        ----------
+        v : ndarray
+            Vector to left-multiply the Jacobian by.
+        x : ndarray
+            Optimization variables.
+
+        """
+        return Derivative.compute_vjp(self.compute_unscaled, 0, v, x)
+
     def compile(self, mode="auto", verbose=1):
         """Call the necessary functions to ensure the function is compiled.
 
         Parameters
         ----------
         mode : {"auto", "lsq", "scalar", "bfgs", "all"}
             Whether to compile for least squares optimization or scalar optimization.
@@ -641,15 +680,15 @@
 
 
 class _Objective(IOAble, ABC):
     """Objective (or constraint) used in the optimization of an Equilibrium.
 
     Parameters
     ----------
-    eq : Equilibrium, optional
+    eq : Equilibrium
         Equilibrium that will be optimized to satisfy the Objective.
     target : float, ndarray, optional
         Target value(s) of the objective. Only used if bounds is None.
         len(target) must be equal to Objective.dim_f
     bounds : tuple, optional
         Lower and upper bounds on the objective. Overrides target.
         len(bounds[0]) and len(bounds[1]) must be equal to Objective.dim_f
@@ -686,15 +725,14 @@
         target=0,
         bounds=None,
         weight=1,
         normalize=True,
         normalize_target=True,
         name=None,
     ):
-
         assert np.all(np.asarray(weight) > 0)
         assert normalize in {True, False}
         assert normalize_target in {True, False}
         assert (bounds is None) or (isinstance(bounds, tuple) and len(bounds) == 2)
         assert (bounds is None) or (target is None), "Cannot use both bounds and target"
         self._target = target
         self._bounds = bounds
@@ -707,16 +745,22 @@
         self._built = False
         # if args is already set don't overwrite it
         self._args = getattr(
             self,
             "_args",
             [arg for arg in getfullargspec(self.compute)[0] if arg != "self"],
         )
-        if eq is not None:
-            self.build(eq)
+        self._eq = eq
+        if eq is None:
+            warnings.warn(
+                FutureWarning(
+                    "Creating an Objective without specifying the Equilibrium to"
+                    " optimize is deprecated, in the future this will raise an error."
+                )
+            )
 
     def _set_dimensions(self, eq):
         """Set state vector component dimensions."""
         self._dimensions = {}
         for arg in arg_order:
             self._dimensions[arg] = np.atleast_1d(getattr(eq, arg)).size
 
@@ -835,16 +879,17 @@
 
         """
         self.target = np.atleast_1d(getattr(eq, self.target_arg, self.target))
         if self._use_jit:
             self.jit()
 
     @abstractmethod
-    def build(self, eq, use_jit=True, verbose=1):
+    def build(self, eq=None, use_jit=True, verbose=1):
         """Build constant arrays."""
+        eq = eq or self._eq
         self._check_dimensions()
         self._set_dimensions(eq)
         self._set_derivatives()
         if use_jit is not None:
             self._use_jit = use_jit
         if self._use_jit:
             self.jit()
```

### Comparing `desc-opt-0.9.0/desc/optimize/_constraint_wrappers.py` & `desc-opt-0.9.1/desc/optimize/_constraint_wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,32 +59,31 @@
         self._objective = objective
         self._objectives = [objective]
         self._constraints = constraints
         self._built = False
         # don't want to compile this, just use the compiled objective
         self._use_jit = False
         self._compiled = False
+        self._eq = eq
 
-        if eq is not None:
-            self.build(eq, verbose=verbose)
-
-    def build(self, eq, use_jit=None, verbose=1):
+    def build(self, eq=None, use_jit=None, verbose=1):
         """Build the objective.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
             Note: unused by this class, should pass to sub-objectives directly.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         timer = Timer()
         timer.start("Linear constraint projection build")
 
         # we don't always build here because in ~all cases the user doesn't interact
         # with this directly, so if the user wants to manually rebuild they should
         # do it before this wrapper is created for them.
         if not self._objective.built:
@@ -310,14 +309,48 @@
         J : ndarray
             Jacobian matrix.
         """
         x = self.recover(x_reduced)
         df = self._objective.jac_scaled(x)
         return df[:, self._unfixed_idx] @ self._Z
 
+    def vjp_scaled(self, v, x_reduced):
+        """Compute vector-Jacobian product of the objective function.
+
+        Uses the scaled form of the objective.
+
+        Parameters
+        ----------
+        v : ndarray
+            Vector to left-multiply the Jacobian by.
+        x_reduced : ndarray
+            Optimization variables.
+
+        """
+        x = self.recover(x_reduced)
+        df = self._objective.vjp_scaled(v, x)
+        return df[self._unfixed_idx] @ self._Z
+
+    def vjp_unscaled(self, v, x_reduced):
+        """Compute vector-Jacobian product of the objective function.
+
+        Uses the unscaled form of the objective.
+
+        Parameters
+        ----------
+        v : ndarray
+            Vector to left-multiply the Jacobian by.
+        x_reduced : ndarray
+            Optimization variables.
+
+        """
+        x = self.recover(x_reduced)
+        df = self._objective.vjp_unscaled(v, x)
+        return df[self._unfixed_idx] @ self._Z
+
     @property
     def target_scaled(self):
         """ndarray: target vector."""
         return self._objective.target_scaled
 
     @property
     def bounds_scaled(self):
@@ -388,17 +421,15 @@
         solve_options.setdefault("verbose", 0)
         self._perturb_options = perturb_options
         self._solve_options = solve_options
         self._built = False
         # don't want to compile this, just use the compiled objective and constraint
         self._use_jit = False
         self._compiled = False
-
-        if eq is not None:
-            self.build(eq, verbose=verbose)
+        self._eq = eq
 
     def set_args(self, *args):
         """Set which arguments the objective should expect.
 
         Defaults to args from all sub-objectives. Additional arguments can be passed in.
         """
         # this is everything taken by either objective
@@ -473,37 +504,41 @@
             A = c.derivatives["jac_unscaled"]["Z_lmn"](
                 *[jnp.zeros(c.dimensions[arg]) for arg in c.args]
             )
             Ainv = np.linalg.pinv(A)
             dxdZb = np.eye(self._dim_x_full)[:, self._x_idx_full["Z_lmn"]] @ Ainv
             self._dxdc = np.hstack((self._dxdc, dxdZb))
 
-    def build(self, eq, use_jit=None, verbose=1):  # noqa: C901
+    def build(self, eq=None, use_jit=None, verbose=1):  # noqa: C901
         """Build the objective.
 
         Parameters
         ----------
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
             Note: unused by this class, should pass to sub-objectives directly.
         verbose : int, optional
             Level of output.
 
         """
+        eq = eq or self._eq
         timer = Timer()
         timer.start("Proximal projection build")
 
         self._eq = eq.copy()
         self._linear_constraints = get_fixed_boundary_constraints(
+            eq=eq,
             iota=self._eq.iota is not None,
             kinetic=self._eq.electron_temperature is not None,
         )
-        self._linear_constraints = maybe_add_self_consistency(self._linear_constraints)
+        self._linear_constraints = maybe_add_self_consistency(
+            eq, self._linear_constraints
+        )
 
         # we don't always build here because in ~all cases the user doesn't interact
         # with this directly, so if the user wants to manually rebuild they should
         # do it before this wrapper is created for them.
         if not self._objective.built:
             self._objective.build(self._eq, verbose=verbose)
         if not self._constraint.built:
@@ -764,14 +799,44 @@
         -------
         H : ndarray
             Hessian matrix.
         """
         J = self.jac_scaled(x)
         return J.T @ J
 
+    def vjp_scaled(self, v, x):
+        """Compute vector-Jacobian product of the objective function.
+
+        Uses the scaled form of the objective.
+
+        Parameters
+        ----------
+        v : ndarray
+            Vector to left-multiply the Jacobian by.
+        x : ndarray
+            Optimization variables.
+
+        """
+        raise NotImplementedError
+
+    def vjp_unscaled(self, v, x):
+        """Compute vector-Jacobian product of the objective function.
+
+        Uses the unscaled form of the objective.
+
+        Parameters
+        ----------
+        v : ndarray
+            Vector to left-multiply the Jacobian by.
+        x : ndarray
+            Optimization variables.
+
+        """
+        raise NotImplementedError
+
     @property
     def target_scaled(self):
         """ndarray: target vector."""
         return self._objective.target_scaled
 
     @property
     def bounds_scaled(self):
```

### Comparing `desc-opt-0.9.0/desc/optimize/_desc_wrappers.py` & `desc-opt-0.9.1/desc/optimize/_desc_wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,25 @@
 from .fmin_scalar import fmintr
 from .least_squares import lsqtr
 from .optimizer import register_optimizer
 from .stochastic import sgd
 
 
 @register_optimizer(
-    name="fmin-auglag",
-    description="Augmented Lagrangian method with trust region subproblem.",
+    name=["fmin-auglag", "fmin-auglag-bfgs"],
+    description=[
+        "Augmented Lagrangian method with trust region subproblem.",
+        "Augmented Lagrangian method with trust region subproblem. Uses BFGS to"
+        + " approximate hessian",
+    ],
     scalar=True,
     equality_constraints=True,
     inequality_constraints=True,
     stochastic=False,
-    hessian=True,
+    hessian=[True, False],
     GPU=True,
 )
 def _optimize_desc_aug_lagrangian(
     objective, constraint, x0, method, x_scale, verbose, stoptol, options=None
 ):
     """Wrapper for desc.optimize.fmin_lag_ls_stel.
 
@@ -67,31 +71,33 @@
     options = {} if options is None else options
     if not isinstance(x_scale, str) and jnp.allclose(x_scale, 1):
         options.setdefault("initial_trust_ratio", 1e-3)
         options.setdefault("max_trust_radius", 1.0)
     options["max_nfev"] = stoptol["max_nfev"]
     options["max_ngev"] = stoptol["max_ngev"]
     options["max_nhev"] = stoptol["max_nhev"]
+    hess = objective.hess if "bfgs" not in method else "bfgs"
 
     if constraint is not None:
         lb, ub = constraint.bounds_scaled
         constraint_wrapped = NonlinearConstraint(
             constraint.compute_scaled,
             lb,
             ub,
             constraint.jac_scaled,
         )
+        constraint_wrapped.vjp = constraint.vjp_scaled
     else:
         constraint_wrapped = None
 
     result = fmin_auglag(
         objective.compute_scalar,
         x0=x0,
         grad=objective.grad,
-        hess=objective.hess,
+        hess=hess,
         bounds=(-jnp.inf, jnp.inf),
         constraint=constraint_wrapped,
         args=(),
         x_scale=x_scale,
         ftol=stoptol["ftol"],
         xtol=stoptol["xtol"],
         gtol=stoptol["gtol"],
```

### Comparing `desc-opt-0.9.0/desc/optimize/_scipy_wrappers.py` & `desc-opt-0.9.1/desc/optimize/_scipy_wrappers.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/optimize/aug_lagrangian.py` & `desc-opt-0.9.1/desc/optimize/aug_lagrangian.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Augmented Langrangian for scalar valued objectives."""
 
-from scipy.optimize import NonlinearConstraint, OptimizeResult
+from scipy.optimize import BFGS, NonlinearConstraint, OptimizeResult
+from termcolor import colored
 
 from desc.backend import jnp
 from desc.optimize.fmin_scalar import fmintr
 
 from .bound_utils import find_active_constraints
 from .utils import (
     check_termination,
@@ -14,15 +15,15 @@
 )
 
 
 def fmin_auglag(  # noqa: C901 - FIXME: simplify this
     fun,
     x0,
     grad,
-    hess,
+    hess="bfgs",
     bounds=(-jnp.inf, jnp.inf),
     constraint=None,
     args=(),
     x_scale=1,
     ftol=1e-6,
     xtol=1e-6,
     gtol=1e-6,
@@ -124,52 +125,68 @@
 
     def lagfun(z, y, mu, *args):
         c = constraint_wrapped.fun(z, *args)
         return fun_wrapped(z, *args) - jnp.dot(y, c) + mu / 2 * jnp.dot(c, c)
 
     def laggrad(z, y, mu, *args):
         c = constraint_wrapped.fun(z, *args)
-        J = constraint_wrapped.jac(z, *args)
-        return grad_wrapped(z, *args) - jnp.dot(y, J) + mu * jnp.dot(c, J)
+        yJ = constraint_wrapped.vjp(y - mu * c, z, *args)
+        return grad_wrapped(z, *args) - yJ
 
-    assert callable(hess_wrapped)
-    if callable(constraint_wrapped.hess):
+    if isinstance(hess_wrapped, str) and hess_wrapped.lower() == "bfgs":
+        hess_init_scale = options.pop("hessian_init_scale", "auto")
+        hess_exception_strategy = options.pop(
+            "hessian_exception_strategy", "damp_update"
+        )
+        hess_min_curvature = options.pop("hessian_minimum_curvature", None)
+        hess_wrapped = BFGS(
+            hess_exception_strategy, hess_min_curvature, hess_init_scale
+        )
+    if isinstance(hess_wrapped, BFGS):
+        if hasattr(hess_wrapped, "n"):  # assume its already been initialized
+            assert hess_wrapped.approx_type == "hess"
+            assert hess.n == z0.size
+        else:
+            hess_wrapped.initialize(z0.size, "hess")
+        laghess = hess_wrapped
+
+    elif callable(constraint_wrapped.hess) and callable(hess_wrapped):
 
         def laghess(z, y, mu, *args):
             c = constraint_wrapped.fun(z, *args)
             Hf = hess_wrapped(z, *args)
             Jc = constraint_wrapped.jac(z, *args)
             Hc1 = constraint_wrapped.hess(z, y)
             Hc2 = constraint_wrapped.hess(z, c)
             return Hf - Hc1 + mu * (Hc2 + jnp.dot(Jc.T, Jc))
 
-    else:
+    elif callable(hess_wrapped):
 
         def laghess(z, y, mu, *args):
             H = hess_wrapped(z, *args)
             J = constraint_wrapped.jac(z, *args)
             # ignoring higher order derivatives of constraints for now
             return H + mu * jnp.dot(J.T, J)
 
-    # TODO: figure out how to let BFGS maintain state between subproblems, otherwise
-    # it doesn't really converge
+    else:
+        raise ValueError(colored("hess should either be a callable or 'bfgs'", "red"))
 
     nfev = 0
     ngev = 0
     nhev = 0
     iteration = 0
 
     z = z0.copy()
     f = fun_wrapped(z, *args)
     c = constraint_wrapped.fun(z)
     nfev += 1
 
     mu = options.pop("initial_penalty_parameter", 10)
-    y = options.pop("initial_multipliers", None)
-    if y is None:  # use least squares multiplier estimates
+    y = options.pop("initial_multipliers", jnp.zeros_like(c))
+    if y == "least_squares":  # use least squares multiplier estimates
         _J = constraint_wrapped.jac(z, *args)
         _g = grad_wrapped(z, *args)
         y = jnp.linalg.lstsq(_J.T, _g)[0]
         y = jnp.nan_to_num(y, nan=0.0, posinf=0.0, neginf=0.0)
 
     if maxiter is None:
         maxiter = z.size * 100
```

### Comparing `desc-opt-0.9.0/desc/optimize/aug_lagrangian_ls.py` & `desc-opt-0.9.1/desc/optimize/aug_lagrangian_ls.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,16 +149,16 @@
     z = z0.copy()
     f = fun_wrapped(z, *args)
     cost = 1 / 2 * jnp.dot(f, f)
     c = constraint_wrapped.fun(z)
     nfev += 1
 
     mu = options.pop("initial_penalty_parameter", 10)
-    y = options.pop("initial_multipliers", None)
-    if y is None:  # use least squares multiplier estimates
+    y = options.pop("initial_multipliers", jnp.zeros_like(c))
+    if y == "least_squares":  # use least squares multiplier estimates
         _J = constraint_wrapped.jac(z, *args)
         _g = f @ jac_wrapped(z, *args)
         y = jnp.linalg.lstsq(_J.T, _g)[0]
         y = jnp.nan_to_num(y, nan=0.0, posinf=0.0, neginf=0.0)
 
     if maxiter is None:
         maxiter = z.size * 100
```

### Comparing `desc-opt-0.9.0/desc/optimize/bound_utils.py` & `desc-opt-0.9.1/desc/optimize/bound_utils.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/optimize/fmin_scalar.py` & `desc-opt-0.9.1/desc/optimize/fmin_scalar.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,30 +134,31 @@
     x = make_strictly_feasible(x, lb, ub)
 
     f = fun(x, *args)
     nfev += 1
     g = grad(x, *args)
     ngev += 1
 
-    if callable(hess):
-        H = hess(x, *args)
-        nhev += 1
-        bfgs = False
-    elif isinstance(hess, str) and hess.lower() == "bfgs":
+    if isinstance(hess, str) and hess.lower() == "bfgs":
         hess_init_scale = options.pop("hessian_init_scale", "auto")
         hess_exception_strategy = options.pop(
             "hessian_exception_strategy", "damp_update"
         )
         hess_min_curvature = options.pop("hessian_minimum_curvature", None)
         hess = BFGS(hess_exception_strategy, hess_min_curvature, hess_init_scale)
-        hess.initialize(N, "hess")
-        H = hess.get_matrix()
-        bfgs = True
+    if callable(hess):
+        H = hess(x, *args)
+        nhev += 1
+        bfgs = False
     elif isinstance(hess, BFGS):
-        hess.initialize(N, "hess")
+        if hasattr(hess, "n"):  # assume its already been initialized
+            assert hess.approx_type == "hess"
+            assert hess.n == N
+        else:
+            hess.initialize(N, "hess")
         bfgs = True
         H = hess.get_matrix()
     else:
         raise ValueError(colored("hess should either be a callable or 'bfgs'", "red"))
 
     if method == "dogleg":
         subproblem = solve_trust_region_dogleg
```

### Comparing `desc-opt-0.9.0/desc/optimize/least_squares.py` & `desc-opt-0.9.1/desc/optimize/least_squares.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/optimize/optimizer.py` & `desc-opt-0.9.1/desc/optimize/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,25 +140,25 @@
         # TODO: document options
         timer = Timer()
         options = {} if options is None else options
         wrapper, method = _parse_method(self.method)
 
         linear_constraints, nonlinear_constraint = _parse_constraints(constraints)
         objective, nonlinear_constraint = _maybe_wrap_nonlinear_constraints(
-            objective, nonlinear_constraint, self.method, options
+            eq, objective, nonlinear_constraint, self.method, options
         )
 
         if not isinstance(objective, ProximalProjection):
             # need to include self consistency constraints
-            linear_constraints = maybe_add_self_consistency(linear_constraints)
+            linear_constraints = maybe_add_self_consistency(eq, linear_constraints)
         if len(linear_constraints):
-            objective = LinearConstraintProjection(objective, linear_constraints)
+            objective = LinearConstraintProjection(objective, linear_constraints, eq=eq)
             if nonlinear_constraint is not None:
                 nonlinear_constraint = LinearConstraintProjection(
-                    nonlinear_constraint, linear_constraints
+                    nonlinear_constraint, linear_constraints, eq=eq
                 )
         if not objective.built:
             objective.build(eq, verbose=verbose)
         if nonlinear_constraint is not None and not nonlinear_constraint.built:
             nonlinear_constraint.build(eq, verbose=verbose)
         if nonlinear_constraint is not None:
             objective, nonlinear_constraint = combine_args(
@@ -323,15 +323,17 @@
     if len(nonlinear_constraints):
         nonlinear_constraints = ObjectiveFunction(nonlinear_constraints)
     else:
         nonlinear_constraints = None
     return linear_constraints, nonlinear_constraints
 
 
-def _maybe_wrap_nonlinear_constraints(objective, nonlinear_constraint, method, options):
+def _maybe_wrap_nonlinear_constraints(
+    eq, objective, nonlinear_constraint, method, options
+):
     """Use ProximalProjection to handle nonlinear constraints."""
     wrapper, method = _parse_method(method)
     if nonlinear_constraint is None:
         if wrapper is not None:
             warnings.warn(
                 f"No nonlinear constraints detected, ignoring wrapper method {wrapper}"
             )
@@ -353,14 +355,15 @@
         perturb_options = options.pop("perturb_options", {})
         solve_options = options.pop("solve_options", {})
         objective = ProximalProjection(
             objective,
             constraint=nonlinear_constraint,
             perturb_options=perturb_options,
             solve_options=solve_options,
+            eq=eq,
         )
         nonlinear_constraint = None
     return objective, nonlinear_constraint
 
 
 def _get_default_tols(
     method,
```

### Comparing `desc-opt-0.9.0/desc/optimize/stochastic.py` & `desc-opt-0.9.1/desc/optimize/stochastic.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/optimize/tr_subproblems.py` & `desc-opt-0.9.1/desc/optimize/tr_subproblems.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/optimize/utils.py` & `desc-opt-0.9.1/desc/optimize/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,20 +119,38 @@
             x, s = z2xs(z)
             H = constraint.hess(x, y, *args)
             return jnp.pad(H, (0, nslack))
 
     else:  # using BFGS
         conhess_wrapped = constraint.hess
 
+    if hasattr(constraint, "vjp"):
+
+        def vjp_wrapped(y, z, *args):
+            x, s = z2xs(z)
+            I = jnp.eye(nslack)
+            Js = jnp.zeros((ncon, nslack))
+            Js = put(Js, Index[ineq_mask, :], -I)
+            vjpx = constraint.vjp(y, x, *args)
+            vjps = jnp.dot(y, Js)
+            return jnp.concatenate([vjpx, vjps])
+
+    else:
+
+        def vjp_wrapped(y, z, *args):
+            J = conjac_wrapped(z, *args)
+            return jnp.dot(y, J)
+
     newcon = copy.copy(constraint)
     newcon.fun = confun_wrapped
     newcon.jac = conjac_wrapped
     newcon.hess = conhess_wrapped
     newcon.lb = target
     newcon.ub = target
+    newcon.vjp = vjp_wrapped
 
     return z0, fun_wrapped, grad_wrapped, hess_wrapped, newcon, zbounds, z2xs
 
 
 @jit
 def gershgorin_bounds(H):
     """Upper and lower bounds for eigenvalues of a square matrix.
```

### Comparing `desc-opt-0.9.0/desc/perturbations.py` & `desc-opt-0.9.1/desc/perturbations.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     # make sure things are at least 1D for jnp.concatenate later
     # in case only a single delta is being passed
     for key in deltas.keys():
         deltas[key] = jnp.atleast_1d(deltas[key])
 
     if not objective.built:
         objective.build(eq, verbose=verbose)
-    constraints = maybe_add_self_consistency(constraints)
+    constraints = maybe_add_self_consistency(eq=eq, constraints=constraints)
     con_args = []
     for con in constraints:
         con_args += con.args
         if not con.built:
             con.build(eq, verbose=verbose)
     objective.set_args(*con_args)
 
@@ -541,17 +541,17 @@
         )
     if verbose > 0:
         print("Number of parameters: {}".format(dim_opt))
         print("Number of objectives: {}".format(objective_g.dim_f))
 
     # FIXME: generalize to other constraints
     constraints = get_fixed_boundary_constraints(
-        iota=eq.iota is not None, kinetic=eq.electron_temperature is not None
+        eq=eq, iota=eq.iota is not None, kinetic=eq.electron_temperature is not None
     )
-    constraints = maybe_add_self_consistency(constraints)
+    constraints = maybe_add_self_consistency(eq=eq, constraints=constraints)
     con_args = []
     for con in constraints:
         con_args += con.args
         if not con.built:
             con.build(eq, verbose=verbose)
     con_args += objective_f.args + objective_g.args
     objective_f.set_args(*con_args)
```

### Comparing `desc-opt-0.9.0/desc/plotting.py` & `desc-opt-0.9.1/desc/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import numpy as np
 from matplotlib import cycler, rcParams
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from scipy.integrate import solve_ivp
 from scipy.interpolate import Rbf
 from termcolor import colored
 
+from desc.backend import sign
 from desc.basis import fourier, zernike_radial_poly
 from desc.compute import data_index, get_transforms
 from desc.compute.utils import compress, surface_averages
 from desc.grid import Grid, LinearGrid
 from desc.utils import flatten_list
 from desc.vmec_utils import ptolemy_linear_transform
 
@@ -115,15 +116,14 @@
     cols : int, optional
         Number of columns of subplots to create.
     figsize : tuple of 2 floats
         Figure size (width, height) in inches. Default is (6, 6).
     equal : bool
         Whether axes should have equal scales for x and y.
 
-
     Returns
     -------
     fig : matplotlib.figure.Figure
         Figure being plotted to.
     ax : matplotlib.axes.Axes or ndarray of Axes
         Axes being plotted to.
 
@@ -176,15 +176,14 @@
     """Get grid for plotting.
 
     Parameters
     ----------
     kwargs
          Any arguments taken by LinearGrid.
 
-
     Returns
     -------
     grid : LinearGrid
          Grid of coordinates to evaluate at.
 
     """
     grid_args = {
@@ -211,15 +210,14 @@
     """Find which axes are being plotted.
 
     Parameters
     ----------
     grid : Grid
         Grid of coordinates to evaluate at.
 
-
     Returns
     -------
     axes : tuple of int
         Which axes of the grid are being plotted.
 
     """
     plot_axes = [0, 1, 2]
@@ -243,15 +241,14 @@
     name : str
         Name of variable to plot.
     grid : Grid
         Grid of coordinates to evaluate at.
     component : str, optional
         For vector variables, which element to plot. Default is the norm of the vector.
 
-
     Returns
     -------
     data : float array of shape (M, L, N)
         Computed quantity.
 
     """
     if name not in data_index:
@@ -306,35 +303,31 @@
         Whether to include radial mode numbers in the x-axis or not.
     M : bool
         Whether to include poloidal mode numbers in the x-axis or not.
     N : bool
         Whether to include toroidal mode numbers in the x-axis or not.
     ax : matplotlib AxesSubplot, optional
         Axis to plot on.
-
     **kwargs : fig,ax and plotting properties
         Specify properties of the figure, axis, and plot appearance e.g.::
 
             plot_X(figsize=(4,6))
 
         Valid keyword arguments are:
 
         figsize: tuple of length 2, the size of the figure (to be passed to matplotlib)
         title_font_size: integer, font size of the title
 
-
-
     Returns
     -------
     fig : matplotlib.figure.Figure
         Figure being plotted to.
     ax : matplotlib.axes.Axes or ndarray of Axes
         Axes being plotted to.
 
-
     Examples
     --------
     .. image:: ../../_static/images/plotting/plot_coefficients.png
 
     .. code-block:: python
 
         from desc.plotting import plot_coefficients
@@ -968,28 +961,28 @@
     label = label.split("~")
     if data_index[name]["coordinates"] == "r":
         # If the quantity is a surface function, averaging it again has no
         # effect, regardless of whether sqrt(g) is used.
         # So we avoid surface averaging it and forgo the <> around the label.
         label = r"$ " + label[0][1:] + r" ~" + "~".join(label[1:])
         plot_data_ylabel_key = f"{name}"
+        values = compress(grid, values)
     elif with_sqrt_g:
         # flux surface average
         label = r"$\langle " + label[0][1:] + r" \rangle~" + "~".join(label[1:])
-        sqrt_g, _ = _compute(eq, "sqrt(g)", grid, reshape=False)
-        values = surface_averages(grid, q=values, sqrt_g=sqrt_g)
         plot_data_ylabel_key = f"<{name}>_fsa"
+        sqrt_g, _ = _compute(eq, "sqrt(g)", grid, reshape=False)
+        values = surface_averages(grid, q=values, sqrt_g=sqrt_g, expand_out=False)
     else:
         # theta average
         label = (
             r"$\langle " + label[0][1:] + r" \rangle_{\theta}~" + "~".join(label[1:])
         )
-        values = surface_averages(grid, q=values)
         plot_data_ylabel_key = f"<{name}>_fsa"
-    values = compress(grid, values)
+        values = surface_averages(grid, q=values, expand_out=False)
 
     if norm_F:
         # normalize force by B pressure gradient
         norm_name = kwargs.pop("norm_name", "<|grad(|B|^2)|/2mu0>_vol")
         norm_data, _ = _compute(eq, norm_name, grid, reshape=False)
         values = values / np.nanmean(np.abs(norm_data))  # normalize
     if log:
@@ -1381,15 +1374,15 @@
     grid_kwargs = {
         "rho": np.linspace(0, 1, NR),
         "NFP": nfp,
         "theta": theta,
         "zeta": phi,
     }
     if plot_theta:
-        # Note: theta* (also known as vartheta) is the poloidal straight field-line
+        # Note: theta* (also known as vartheta) is the poloidal straight field line
         # angle in PEST-like flux coordinates
         t_grid = _get_grid(**grid_kwargs)
         tnr, tnt, tnz = t_grid.num_rho, t_grid.num_theta, t_grid.num_zeta
         v_grid = Grid(
             eq.map_coordinates(
                 t_grid.nodes, ["rho", "theta_sfl", "phi"], ["rho", "theta", "zeta"]
             ),
@@ -1665,15 +1658,14 @@
         * ``cmap``: colormap to use for plotting, discretized into len(eqs) colors
         * ``colors``: array of colors to use for each Equilibrium
         * ``ls``: array of line styles to use for each Equilibrium
         * ``lw``: array of line widths to use for each Equilibrium
         * ``label_fontsize``: float, fontsize of the x and y labels
         * ``legend_fontsize``: float, fontsize of the legend
 
-
     Returns
     -------
     fig : matplotlib.figure.Figure
         Figure being plotted to.
     ax : matplotlib.axes.Axes or ndarray of Axes
         Axes being plotted to.
     plot_data : dict
@@ -1997,14 +1989,15 @@
     -------
     fig : matplotlib.figure.Figure
         Figure being plotted to
     ax : matplotlib.axes.Axes or ndarray of Axes
         Axes being plotted to
     plot_data : dict
         dictionary of the data plotted, only returned if ``return_data=True``
+
     """
     figsize = kwargs.pop("figsize", None)
     lw = kwargs.pop("lw", 2)
     ls = kwargs.pop("ls", "-")
     color = kwargs.pop("color", "current")
     color = kwargs.pop("c", color)
     cbar = False
@@ -2102,15 +2095,15 @@
     log : bool, optional
         Whether to use a log scale.
     B0 : bool, optional
         Whether to include the m=n=0 mode.
     norm : bool, optional
         Whether to normalize the magnitudes such that B0=1 Tesla.
     num_modes : int, optional
-        How many modes to include. Default (-1) is all.
+        How many modes to include. Use -1 for all modes.
     rho : int or ndarray, optional
         Radial coordinates of the flux surfaces to evaluate at,
         or number of surfaces in (0,1]
     ax : matplotlib AxesSubplot, optional
         Axis to plot on.
     return_data : bool
         if True, return the data plotted as well as fig,ax
@@ -2122,15 +2115,14 @@
         Valid keyword arguments are:
 
         * ``figsize``: tuple of length 2, the size of the figure (to be passed to
           matplotlib)
         * ``lw``: float, linewidth
         * ``ls``: str, linestyle
 
-
     Returns
     -------
     fig : matplotlib.figure.Figure
         Figure being plotted to.
     ax : matplotlib.axes.Axes or ndarray of Axes
         Axes being plotted to.
     plot_data : dict
@@ -2230,34 +2222,40 @@
     return fig, ax
 
 
 def plot_boozer_surface(
     eq,
     grid_compute=None,
     grid_plot=None,
+    rho=1,
     fill=False,
-    ncontours=100,
+    ncontours=30,
+    fieldlines=0,
     ax=None,
     return_data=False,
     **kwargs,
 ):
     """Plot :math:`|B|` on a surface vs the Boozer poloidal and toroidal angles.
 
     Parameters
     ----------
     eq : Equilibrium
         Object from which to plot.
     grid_compute : Grid, optional
         grid to use for computing boozer spectrum
     grid_plot : Grid, optional
         grid to plot on
+    rho : float, optional
+        Radial coordinate of flux surface. Used only if grids are not specified.
     fill : bool, optional
         Whether the contours are filled, i.e. whether to use `contourf` or `contour`.
     ncontours : int, optional
         Number of contours to plot.
+    fieldlines : int, optional
+        Number of (linearly spaced) magnetic fieldlines to plot. Default is 0 (none).
     ax : matplotlib AxesSubplot, optional
         Axis to plot on.
     return_data : bool
         if True, return the data plotted as well as fig,ax
     **kwargs : dict, optional
         Specify properties of the figure, axis, and plot appearance e.g.::
 
@@ -2288,22 +2286,29 @@
 
         from desc.plotting import plot_boozer_surface
         fig, ax = plot_boozer_surface(eq)
 
     """
     if grid_compute is None:
         grid_kwargs = {
-            "M": 6 * eq.M + 1,
-            "N": 6 * eq.N + 1,
+            "rho": rho,
+            "M": 4 * eq.M,
+            "N": 4 * eq.N,
             "NFP": eq.NFP,
             "endpoint": False,
         }
         grid_compute = _get_grid(**grid_kwargs)
     if grid_plot is None:
-        grid_kwargs = {"M": 100, "N": 100, "NFP": eq.NFP, "endpoint": True}
+        grid_kwargs = {
+            "rho": rho,
+            "theta": 91,
+            "zeta": 91,
+            "NFP": eq.NFP,
+            "endpoint": True,
+        }
         grid_plot = _get_grid(**grid_kwargs)
 
     M_booz = kwargs.pop("M_booz", 2 * eq.M)
     N_booz = kwargs.pop("N_booz", 2 * eq.N)
     title_font_size = kwargs.pop("title_font_size", None)
 
     transforms_compute = get_transforms(
@@ -2311,14 +2316,15 @@
     )
     transforms_plot = get_transforms(
         "|B|_mn", eq=eq, grid=grid_plot, M_booz=M_booz, N_booz=N_booz
     )
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         data = eq.compute("|B|_mn", grid=grid_compute, transforms=transforms_compute)
+    iota = compress(grid_compute, data["iota"])
     data = transforms_plot["B"].transform(data["|B|_mn"])
     data = data.reshape((grid_plot.num_theta, grid_plot.num_zeta), order="F")
 
     fig, ax = _format_ax(ax, figsize=kwargs.pop("figsize", None))
     divider = make_axes_locatable(ax)
 
     contourf_kwargs = {}
@@ -2331,41 +2337,54 @@
 
     assert (
         len(kwargs) == 0
     ), f"plot_boozer_surface got unexpected keyword argument: {kwargs.keys()}"
 
     cax_kwargs = {"size": "5%", "pad": 0.05}
 
-    xx = (
+    zz = (
         grid_plot.nodes[:, 2]
         .reshape((grid_plot.num_theta, grid_plot.num_zeta), order="F")
         .squeeze()
     )
-    yy = (
+    tt = (
         grid_plot.nodes[:, 1]
         .reshape((grid_plot.num_theta, grid_plot.num_zeta), order="F")
         .squeeze()
     )
 
     if fill:
-        im = ax.contourf(xx, yy, data, **contourf_kwargs)
+        im = ax.contourf(zz, tt, data, **contourf_kwargs)
     else:
-        im = ax.contour(xx, yy, data, **contourf_kwargs)
+        im = ax.contour(zz, tt, data, **contourf_kwargs)
     cax = divider.append_axes("right", **cax_kwargs)
     cbar = fig.colorbar(im, cax=cax)
     cbar.update_ticks()
 
+    if fieldlines:
+        theta0 = np.linspace(0, 2 * np.pi, fieldlines, endpoint=False)
+        zeta = np.linspace(0, 2 * np.pi / grid_plot.NFP, 100)
+        alpha = np.atleast_2d(theta0) + iota * np.atleast_2d(zeta).T
+        alpha1 = np.where(np.logical_and(alpha >= 0, alpha <= 2 * np.pi), alpha, np.nan)
+        alpha2 = np.where(
+            np.logical_or(alpha < 0, alpha > 2 * np.pi),
+            alpha % (sign(iota) * 2 * np.pi) + (sign(iota) < 0) * (2 * np.pi),
+            np.nan,
+        )
+        alphas = np.hstack((alpha1, alpha2))
+        ax.plot(zeta, alphas, color="k", ls="-", lw=2)
+
     ax.set_xlabel(r"$\zeta_{Boozer}$")
     ax.set_ylabel(r"$\theta_{Boozer}$")
     ax.set_title(r"$|\mathbf{B}|~(T)$", fontsize=title_font_size)
 
     fig.set_tight_layout(True)
     plot_data = {}
-    plot_data["zeta_Boozer"] = xx
-    plot_data["theta_Boozer"] = yy
+    plot_data["zeta_Boozer"] = zz
+    plot_data["theta_Boozer"] = tt
     plot_data["|B|"] = data
 
     if return_data:
         return fig, ax, plot_data
 
     return fig, ax
 
@@ -2467,15 +2486,15 @@
 
     data = None
     f_B = np.array([])
     f_C = np.array([])
     f_T = np.array([])
     plot_data = {}
     for i, r in enumerate(rho):
-        grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP, rho=np.array(r))
+        grid = LinearGrid(M=2 * eq.M_grid, N=2 * eq.N_grid, NFP=eq.NFP, rho=np.array(r))
         if fB:
             transforms = get_transforms(
                 "|B|_mn", eq=eq, grid=grid, M_booz=M_booz, N_booz=N_booz
             )
             if i == 0:  # only need to do this once for the first rho surface
                 matrix, modes, idx = ptolemy_linear_transform(
                     transforms["B"].basis.modes,
@@ -2605,15 +2624,14 @@
 
         Valid keyword arguments are:
 
         * ``figsize``: tuple of length 2, the size of the figure (to be passed to
           matplotlib)
         * ``title_font_size``: integer, font size of the title
 
-
     Returns
     -------
     fig : matplotlib.figure.Figure
         Figure being plotted to.
     ax : matplotlib.axes.Axes or ndarray of Axes
         Axes being plotted to.
     plot_data : dict
@@ -2725,15 +2743,14 @@
     ax : matplotlib.axes.Axes, ndarray of axes, or dict of axes
         Axes used for plotting. A single axis is used for 1d basis functions,
         2d or 3d bases return an ndarray or dict of axes.    return_data : bool
         if True, return the data plotted as well as fig,ax
     plot_data : dict
         dictionary of the data plotted, only returned if ``return_data=True``
 
-
     Examples
     --------
     .. image:: ../../_static/images/plotting/plot_basis.png
 
     .. code-block:: python
 
         from desc.plotting import plot_basis
@@ -2777,18 +2794,15 @@
     elif basis.__class__.__name__ == "FourierSeries":
         nmax = abs(basis.modes[:, 2]).max()
         grid = LinearGrid(zeta=100, NFP=basis.NFP, endpoint=True)
         z = grid.nodes[:, 2]
         fig, ax = plt.subplots(figsize=kwargs.get("figsize", (6, 4)))
 
         f = basis.evaluate(grid.nodes)
-        plot_data = {}
-        plot_data["n"] = basis.modes[:, 2]
-        plot_data["amplitude"] = []
-        plot_data["zeta"] = z
+        plot_data = {"n": basis.modes[:, 2], "amplitude": [], "zeta": z}
 
         for fi, n in zip(f.T, basis.modes[:, 2]):
             ax.plot(z, fi, label="$n={:d}$".format(int(n)))
             plot_data["amplitude"].append(fi)
 
         ax.set_xlabel("$\\zeta$")
         ax.set_ylabel("$f_n(\\zeta)$")
@@ -2820,20 +2834,21 @@
         hratios = np.ones(2 * mmax + 2)
         hratios[0] = kwargs.get("title_ratio", 0.1)
         gs = matplotlib.gridspec.GridSpec(
             2 * mmax + 2, 2 * nmax + 2, width_ratios=wratios, height_ratios=hratios
         )
         ax = np.empty((2 * mmax + 1, 2 * nmax + 1), dtype=object)
         f = basis.evaluate(grid.nodes)
-        plot_data = {}
-        plot_data["m"] = basis.modes[:, 1]
-        plot_data["n"] = basis.modes[:, 2]
-        plot_data["amplitude"] = []
-        plot_data["zeta"] = z
-        plot_data["theta"] = t
+        plot_data = {
+            "m": basis.modes[:, 1],
+            "n": basis.modes[:, 2],
+            "amplitude": [],
+            "zeta": z,
+            "theta": t,
+        }
 
         for fi, m, n in zip(f.T, basis.modes[:, 1], basis.modes[:, 2]):
             ax[mmax + m, nmax + n] = plt.subplot(gs[mmax + m + 1, n + nmax])
             ax[mmax + m, nmax + n].set_xticks(
                 [
                     0,
                     np.pi / basis.NFP / 2,
@@ -3182,15 +3197,15 @@
     return_data=False,
     **kwargs,
 ):
     r"""Plots field lines on specified flux surface.
 
     Traces field lines at specified initial vartheta (:math:`\\vartheta`) seed
     locations, then plots them.
-    Field lines traced by first finding the corresponding straight-field-line (SFL)
+    Field lines traced by first finding the corresponding straight field line (SFL)
     coordinates :math:`(\\rho,\\vartheta,\\phi)` for each field line, then
     converting those to the computational :math:`(\\rho,\\theta,\\phi)` coordinates,
     then finally computing from those the toroidal :math:`(R,\\phi,Z)` coordinates of
     each field line.
 
     The SFL angle coordinates are found with the SFL relation:
 
@@ -3411,16 +3426,14 @@
         the following keys: ['B_R'], ['B_Z'], and ['B_phi'], corresponding to the
         interpolating object for each cylindrical component of the magnetic field.
     return_B_interp: bool, default False
         If true, in addition to returning the fig, axis and field line coordinates,
         will also return the dictionary of interpolating radial basis functions
         interpolating the magnetic field in (R,phi,Z)
 
-
-
     Returns
     -------
     fig : matplotlib.figure.Figure
         figure being plotted to
     ax : matplotlib.axes.Axes or ndarray of Axes
         axes being plotted to
     field_line_coords : dict
@@ -3567,16 +3580,14 @@
     theta0 : float
         theta to find closest grid point to.
     phi0 : float
         phi to find closest grid point to.
     grid : Grid
         grid to find closest point on
 
-
-
     Returns
     -------
     idx_pt : int
         index of the grid node closest to the given point.
 
     """
     rhos = grid.nodes[:, 0]
@@ -3603,14 +3614,15 @@
 
 def _field_line_Rbf(rho, theta0, phi_end, grid, Rs, Zs, B_interp, phi0=0):
     """Integrate along interpolated field lines.
 
     Takes the initial poloidal angle you want to seed a field line at (at phi=0),
     and integrates along the field line to the specified phi_end. returns fR,fZ,fPhi,
     the R,Z,Phi coordinates of the field line trajectory.
+
     """
     fR = []
     fZ = []
     fPhi = []
     idx0 = _find_idx(rho, theta0, phi0, grid)
     curr_R = Rs[idx0]
     curr_Z = Zs[idx0]
```

### Comparing `desc-opt-0.9.0/desc/profiles.py` & `desc-opt-0.9.1/desc/profiles.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/transform.py` & `desc-opt-0.9.1/desc/transform.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/utils.py` & `desc-opt-0.9.1/desc/utils.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc/vmec.py` & `desc-opt-0.9.1/desc/vmec.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,20 +144,21 @@
         m, n, L_mn = ptolemy_identity_fwd(xm, xn, s=lmns, c=lmnc)
         eq.L_lmn = fourier_to_zernike(m, n, L_mn, eq.L_basis)
 
         eq = ensure_positive_jacobian(eq)
 
         # apply boundary conditions
         constraints = (
-            FixBoundaryR(),
-            FixBoundaryZ(),
-            BoundaryRSelfConsistency(),
-            BoundaryZSelfConsistency(),
+            FixBoundaryR(eq=eq),
+            FixBoundaryZ(eq=eq),
+            BoundaryRSelfConsistency(eq=eq),
+            BoundaryZSelfConsistency(eq=eq),
         )
-        objective = ObjectiveFunction(constraints, eq=eq, verbose=0)
+        objective = ObjectiveFunction(constraints, verbose=0)
+        objective.build()
         _, _, _, _, _, project, recover = factorize_linear_constraints(
             constraints, objective.args
         )
         args = objective.unpack_state(recover(project(objective.x(eq))))
         for key, value in args.items():
             setattr(eq, key, value)
 
@@ -247,16 +248,19 @@
 
         mgrid_file = file.createVariable("mgrid_file", "S1", ("dim_00200",))
         mgrid_file[:] = stringtochar(
             np.array(["none" + " " * 196], "S" + str(file.dimensions["dim_00200"].size))
         )
 
         ier_flag = file.createVariable("ier_flag", np.int32)
-        ier_flag.long_name = "error flag (0 = solved equilibrium, 1 = unsolved)"
-        ier_flag[:] = int(not eq.solved)
+        ier_flag.long_name = (
+            "error flag (DESC always outputs 0; "
+            + "manually check for a good equilibrium solution)"
+        )
+        ier_flag[:] = 0
 
         lfreeb = file.createVariable("lfreeb__logical__", np.int32)
         lfreeb.long_name = "free boundary logical (0 = fixed boundary)"
         lfreeb[:] = 0
 
         lrecon = file.createVariable("lrecon__logical__", np.int32)
         lrecon.long_name = "reconstruction logical (0 = no reconstruction)"
@@ -538,34 +542,30 @@
         jdotb.units = "N/m^3"
         jdotb[:] = compress(grid, data["<J*B>"])
         jdotb[0] = 0
 
         jcuru = file.createVariable("jcuru", np.float64, ("radius",))
         jcuru.long_name = "flux surface average of sqrt(g)*J^theta"
         jcuru.units = "A/m^3"
-        jcuru[:] = compress(
+        jcuru[:] = surface_averages(
             grid,
-            surface_averages(
-                grid,
-                data["sqrt(g)"] * data["J^theta"] / (2 * data["rho"]),
-                sqrt_g=data["sqrt(g)"],
-            ),
+            data["sqrt(g)"] * data["J^theta"] / (2 * data["rho"]),
+            sqrt_g=data["sqrt(g)"],
+            expand_out=False,
         )
         jcuru[0] = 0
 
         jcurv = file.createVariable("jcurv", np.float64, ("radius",))
         jcuru.long_name = "flux surface average of sqrt(g)*J^zeta"
         jcurv.units = "A/m^3"
-        jcurv[:] = compress(
+        jcurv[:] = surface_averages(
             grid,
-            surface_averages(
-                grid,
-                data["sqrt(g)"] * data["J^zeta"] / (2 * data["rho"]),
-                sqrt_g=data["sqrt(g)"],
-            ),
+            data["sqrt(g)"] * data["J^zeta"] / (2 * data["rho"]),
+            sqrt_g=data["sqrt(g)"],
+            expand_out=False,
         )
         jcurv[0] = 0
 
         # Mercier stability
         DShear = file.createVariable("DShear", np.float64, ("radius",))
         DShear.long_name = "Mercier stability criterion magnetic shear term"
         DShear.units = "1/Wb^2"
```

### Comparing `desc-opt-0.9.0/desc/vmec_utils.py` & `desc-opt-0.9.1/desc/vmec_utils.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/desc_opt.egg-info/PKG-INFO` & `desc-opt-0.9.1/desc_opt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desc-opt
-Version: 0.9.0
+Version: 0.9.1
 Summary: Computes, analyzes and optimizes 3D MHD equilibria for stellarators and tokamaks
 Home-page: https://github.com/PlasmaControl/DESC/
 Author: Daniel Dudt, Rory Conlin, Dario Panici, Egemen Kolemen
 Author-email: PlasmaControl@princeton.edu
 License: MIT
 Project-URL: Issues Tracker, https://github.com/PlasmaControl/DESC/issues
 Project-URL: Contributing, https://github.com/PlasmaControl/DESC/blob/master/CONTRIBUTING.rst
```

### Comparing `desc-opt-0.9.0/desc_opt.egg-info/SOURCES.txt` & `desc-opt-0.9.1/desc_opt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/setup.cfg` & `desc-opt-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/setup.py` & `desc-opt-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/tests/test_axis_limits.py` & `desc-opt-0.9.1/tests/test_axis_limits.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         """Test continuity of <|B|>. Failure indicates B0 limit is wrong."""
 
         def test(eq, expected_at_axis):
             delta = 1e-3
             epsilon = 1e-6
             rho = np.linspace(0, delta, 10)
             lg = LinearGrid(rho=rho, M=7, N=7, NFP=eq.NFP, sym=eq.sym)
-            b_mag_fsa_no_sqrt_g = compress(
-                lg, surface_averages(lg, eq.compute("|B|", grid=lg)["|B|"])
+            b_mag_fsa_no_sqrt_g = surface_averages(
+                lg, eq.compute("|B|", grid=lg)["|B|"], expand_out=False
             )
             # check continuity
             assert np.isfinite(b_mag_fsa_no_sqrt_g).all()
             np.testing.assert_allclose(
                 b_mag_fsa_no_sqrt_g[:-1], b_mag_fsa_no_sqrt_g[1:], atol=epsilon
             )
             # check value
```

### Comparing `desc-opt-0.9.0/tests/test_backend.py` & `desc-opt-0.9.1/tests/test_backend.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Tests for backend functions."""
 
 import numpy as np
 import pytest
 
-from desc.backend import put, sign
+from desc.backend import put, sign, vmap
 
 
 @pytest.mark.unit
 def test_put():
     """Test put function as replacement for fancy array indexing."""
     a = np.array([0, 0, 0])
     b = np.array([1, 2, 3])
@@ -19,7 +19,21 @@
 
 @pytest.mark.unit
 def test_sign():
     """Test modified sign function to return +1 for x=0."""
     assert sign(4) == 1
     assert sign(0) == 1
     assert sign(-10.3) == -1
+
+
+@pytest.mark.unit
+def test_vmap():
+    """Test lax numpy implementation of Python's map function."""
+    a = np.arange(6)
+    inputs = np.stack([a, a[::-1], -a])
+
+    def f(x):
+        return x[: x.size // 2] ** 3
+
+    outputs = np.array([[0, 1, 8], [125, 64, 27], [0, -1, -8]])
+    np.testing.assert_allclose(vmap(f)(inputs), outputs)
+    np.testing.assert_allclose(vmap(f, out_axes=1)(inputs), outputs.T)
```

### Comparing `desc-opt-0.9.0/tests/test_basis.py` & `desc-opt-0.9.1/tests/test_basis.py`

 * *Files 4% similar despite different names*

```diff
@@ -300,7 +300,50 @@
         basis = DoubleFourierSeries(M=2, N=4)
         fr = basis.evaluate(nodes, derivatives=[1, 0, 0])
         assert np.all(fr == 0)
 
         basis = ZernikePolynomial(L=2, M=3)
         fz = basis.evaluate(nodes, derivatives=[0, 0, 1])
         assert np.all(fz == 0)
+
+    @pytest.mark.unit
+    def test_basis_resolutions_assert_integers(self):
+        """Test that basis modes are asserted as integers."""
+        L = 3.0
+        M = 3.0
+        N = 3.0
+
+        basis = PowerSeries(L=L)
+        assert isinstance(basis.L, int)
+        assert basis.L == 3
+
+        basis = FourierSeries(N=N)
+        assert isinstance(basis.N, int)
+        assert basis.N == 3
+
+        basis = DoubleFourierSeries(M=M, N=N)
+        assert isinstance(basis.M, int)
+        assert isinstance(basis.N, int)
+        assert basis.M == 3
+        assert basis.N == 3
+
+        basis = ZernikePolynomial(L=L, M=M)
+        assert isinstance(basis.M, int)
+        assert isinstance(basis.L, int)
+        assert basis.M == 3
+        assert basis.L == 3
+
+        L = 3.1
+        M = 3.1
+        N = 3.1
+
+        with pytest.raises(AssertionError):
+            PowerSeries(L=L)
+
+        with pytest.raises(AssertionError):
+            FourierSeries(N=N)
+
+        with pytest.raises(AssertionError):
+            DoubleFourierSeries(M=M, N=N)
+
+        with pytest.raises(AssertionError):
+            ZernikePolynomial(L=L, M=M)
```

### Comparing `desc-opt-0.9.0/tests/test_bootstrap.py` & `desc-opt-0.9.1/tests/test_bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1169,16 +1169,17 @@
         grid = QuadratureGrid(
             L=LMN_resolution,
             M=LMN_resolution,
             N=LMN_resolution,
             NFP=eq.NFP,
         )
         obj = ObjectiveFunction(
-            BootstrapRedlConsistency(grid=grid, helicity=helicity), eq
+            BootstrapRedlConsistency(eq=eq, grid=grid, helicity=helicity)
         )
+        obj.build()
         scalar_objective1 = obj.compute_scalar(obj.x(eq))
 
         # Scale |B|, changing <J*B> and <J*B>_Redl by "factor":
         factor = 2.0
         eq.Psi *= np.sqrt(factor)
         # Scale n and T to vary neoclassical <J*B> at fixed nu*:
         eq.electron_density = PowerSeriesProfile(
@@ -1187,16 +1188,17 @@
         eq.electron_temperature = PowerSeriesProfile(
             factor ** (2.0 / 5) * Te0 * np.array([1.02, -3, 3, -1]), modes=[0, 2, 4, 6]
         )
         eq.ion_temperature = PowerSeriesProfile(
             factor ** (2.0 / 5) * Ti0 * np.array([1.02, -3, 3, -1]), modes=[0, 2, 4, 6]
         )
         obj = ObjectiveFunction(
-            BootstrapRedlConsistency(grid=grid, helicity=helicity), eq
+            BootstrapRedlConsistency(eq=eq, grid=grid, helicity=helicity)
         )
+        obj.build()
         scalar_objective2 = obj.compute_scalar(obj.x(eq))
 
         # Scale size, changing <J*B> and <J*B>_Redl by "factor":
         factor = 3.0
         eq.Psi = Psi0 / factor**2
         eq.R_lmn /= factor
         eq.Z_lmn /= factor
@@ -1209,16 +1211,17 @@
         eq.electron_temperature = PowerSeriesProfile(
             factor ** (-2.0 / 5) * Te0 * np.array([1.02, -3, 3, -1]), modes=[0, 2, 4, 6]
         )
         eq.ion_temperature = PowerSeriesProfile(
             factor ** (-2.0 / 5) * Ti0 * np.array([1.02, -3, 3, -1]), modes=[0, 2, 4, 6]
         )
         obj = ObjectiveFunction(
-            BootstrapRedlConsistency(grid=grid, helicity=helicity), eq
+            BootstrapRedlConsistency(eq=eq, grid=grid, helicity=helicity)
         )
+        obj.build()
         scalar_objective3 = obj.compute_scalar(obj.x(eq))
 
         results = np.array([scalar_objective1, scalar_objective2, scalar_objective3])
 
         # Compute the expected objective from
         # ½ ∫dρ [(⟨J⋅B⟩_MHD - ⟨J⋅B⟩_Redl) / (J_ref B_ref)]²
         scales = compute_scaling_factors(eq)
@@ -1257,19 +1260,20 @@
                 M=M,
                 N=N,
                 NFP=eq.NFP,
                 **kwargs,
             )
             obj = ObjectiveFunction(
                 BootstrapRedlConsistency(
+                    eq=eq,
                     grid=grid,
                     helicity=helicity,
                 ),
-                eq,
             )
+            obj.build()
             scalar_objective = obj.compute_scalar(obj.x(eq))
             print(f"grid_type:{grid_type} L:{L} M:{M} N:{N} obj:{scalar_objective}")
             return scalar_objective
 
         results = []
 
         # Loop over grid types. For LinearGrid we need to drop the
@@ -1342,45 +1346,46 @@
         )
 
         eq.solve(
             verbose=3,
             ftol=1e-8,
             constraints=get_fixed_boundary_constraints(kinetic=True),
             optimizer=Optimizer("lsq-exact"),
-            objective=ObjectiveFunction(objectives=ForceBalance()),
+            objective=ObjectiveFunction(objectives=ForceBalance(eq=eq)),
         )
 
         initial_output_file = str(
             TmpDir.join("test_bootstrap_consistency_iota_initial.h5")
         )
         print("initial_output_file:", initial_output_file)
         eq.save(initial_output_file)
 
         # Done establishing the initial condition. Now set up the optimization.
 
         constraints = (
-            ForceBalance(),
-            FixBoundaryR(),
-            FixBoundaryZ(),
-            FixElectronDensity(),
-            FixElectronTemperature(),
-            FixIonTemperature(),
-            FixAtomicNumber(),
-            FixPsi(),
+            ForceBalance(eq=eq),
+            FixBoundaryR(eq=eq),
+            FixBoundaryZ(eq=eq),
+            FixElectronDensity(eq=eq),
+            FixElectronTemperature(eq=eq),
+            FixIonTemperature(eq=eq),
+            FixAtomicNumber(eq=eq),
+            FixPsi(eq=eq),
         )
 
         # grid for bootstrap consistency objective:
         grid = LinearGrid(
             rho=np.linspace(1e-4, 1 - 1e-4, (num_iota_points - 1) * 2 + 1),
             M=eq.M * 2,
             N=eq.N * 2,
             NFP=eq.NFP,
         )
         objective = ObjectiveFunction(
             BootstrapRedlConsistency(
+                eq=eq,
                 grid=grid,
                 helicity=helicity,
             )
         )
         eq, _ = eq.optimize(
             verbose=3,
             objective=objective,
@@ -1461,46 +1466,47 @@
         eq.current.change_resolution(current_L)
 
         eq.solve(
             verbose=3,
             ftol=1e-8,
             constraints=get_fixed_boundary_constraints(kinetic=True, iota=False),
             optimizer=Optimizer("lsq-exact"),
-            objective=ObjectiveFunction(objectives=ForceBalance()),
+            objective=ObjectiveFunction(objectives=ForceBalance(eq=eq)),
         )
 
         initial_output_file = str(
             TmpDir.join("test_bootstrap_consistency_current_initial.h5")
         )
         print("initial_output_file:", initial_output_file)
         eq.save(initial_output_file)
 
         # Done establishing the initial condition. Now set up the optimization.
 
         constraints = (
-            ForceBalance(),
-            FixBoundaryR(),
-            FixBoundaryZ(),
-            FixElectronDensity(),
-            FixElectronTemperature(),
-            FixIonTemperature(),
-            FixAtomicNumber(),
-            FixCurrent(indices=[0]),
-            FixPsi(),
+            ForceBalance(eq=eq),
+            FixBoundaryR(eq=eq),
+            FixBoundaryZ(eq=eq),
+            FixElectronDensity(eq=eq),
+            FixElectronTemperature(eq=eq),
+            FixIonTemperature(eq=eq),
+            FixAtomicNumber(eq=eq),
+            FixCurrent(eq=eq, indices=[0]),
+            FixPsi(eq=eq),
         )
 
         # grid for bootstrap consistency objective:
         grid = QuadratureGrid(
             L=current_L * 2,
             M=eq.M * 2,
             N=eq.N * 2,
             NFP=eq.NFP,
         )
         objective = ObjectiveFunction(
             BootstrapRedlConsistency(
+                eq=eq,
                 grid=grid,
                 helicity=helicity,
             )
         )
         eq, _ = eq.optimize(
             verbose=3,
             objective=objective,
@@ -1532,92 +1538,93 @@
         assert np.min(J_dot_B_MHD) > -5.4e6
         np.testing.assert_allclose(J_dot_B_MHD, J_dot_B_Redl, atol=5e5)
 
 
 @pytest.mark.unit
 def test_bootstrap_objective_build():
     """Test defaults and warnings in bootstrap objective build method."""
-    obj = BootstrapRedlConsistency()
     # can't build without profiles
     eq = Equilibrium(L=3, M=3, N=3, NFP=2)
     with pytest.raises(RuntimeError):
-        obj.build(eq)
+        BootstrapRedlConsistency(eq=eq).build()
     eq = Equilibrium(
         L=3, M=3, N=3, NFP=2, electron_temperature=1e3, electron_density=1e21
     )
     eq.electron_density = None
     with pytest.raises(RuntimeError):
-        obj.build(eq)
+        BootstrapRedlConsistency(eq=eq).build()
     eq = Equilibrium(
         L=3, M=3, N=3, NFP=2, electron_temperature=1e3, electron_density=1e21
     )
     eq.ion_temperature = None
     with pytest.raises(RuntimeError):
-        obj.build(eq)
+        BootstrapRedlConsistency(eq=eq).build()
     eq = Equilibrium(
         L=3, M=3, N=3, NFP=2, electron_temperature=1e3, electron_density=1e25
     )
     # density too high
     with pytest.warns(UserWarning):
-        obj.build(eq)
+        BootstrapRedlConsistency(eq=eq).build()
     eq = Equilibrium(
         L=3, M=3, N=3, NFP=2, electron_temperature=1e5, electron_density=1e21
     )
     # electron temperature too high
     with pytest.warns(UserWarning):
-        obj.build(eq)
+        BootstrapRedlConsistency(eq=eq).build()
     eq = Equilibrium(
         L=3,
         M=3,
         N=3,
         NFP=2,
         electron_temperature=1e3,
         electron_density=1e21,
         ion_temperature=1e5,
     )
     # ion temperature too high
     with pytest.warns(UserWarning):
-        obj.build(eq)
+        BootstrapRedlConsistency(eq=eq).build()
     eq = Equilibrium(
         L=3,
         M=3,
         N=3,
         NFP=2,
         electron_temperature=1e3,
         electron_density=1e1,
         ion_temperature=1e3,
     )
     # density too low
     with pytest.warns(UserWarning):
-        obj.build(eq)
+        BootstrapRedlConsistency(eq=eq).build()
     eq = Equilibrium(
         L=3,
         M=3,
         N=3,
         NFP=2,
         electron_temperature=3,
         electron_density=1e21,
         ion_temperature=1e3,
     )
     # electron temperature too low
     with pytest.warns(UserWarning):
-        obj.build(eq)
+        BootstrapRedlConsistency(eq=eq).build()
     eq = Equilibrium(
         L=3,
         M=3,
         N=3,
         NFP=2,
         electron_temperature=1e3,
         electron_density=1e21,
         ion_temperature=1,
     )
     # ion temperature too low
     with pytest.warns(UserWarning):
-        obj.build(eq)
+        BootstrapRedlConsistency(eq=eq).build()
 
+    obj = BootstrapRedlConsistency(eq=eq)
+    obj.build()
     # make sure default grid has the right nodes
     assert obj._transforms["grid"].num_theta == 13
     assert obj._transforms["grid"].num_zeta == 13
     assert obj._transforms["grid"].num_rho == 5
     np.testing.assert_allclose(
         obj._transforms["grid"].nodes[obj._transforms["grid"].unique_rho_idx, 0],
         np.array([0.2, 0.4, 0.6, 0.8, 1.0]),
```

### Comparing `desc-opt-0.9.0/tests/test_coils.py` & `desc-opt-0.9.1/tests/test_coils.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/tests/test_compute_funs.py` & `desc-opt-0.9.1/tests/test_compute_funs.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/tests/test_configuration.py` & `desc-opt-0.9.1/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/tests/test_constrain_current.py` & `desc-opt-0.9.1/tests/test_constrain_current.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/tests/test_curves.py` & `desc-opt-0.9.1/tests/test_curves.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/tests/test_derivatives.py` & `desc-opt-0.9.1/tests/test_derivatives.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,33 @@
         x = rando.random(17)
 
         jac = AutoDiffDerivative(fun, block_size=4, shape=A.shape)
         np.testing.assert_allclose(jac(x), A)
         jac = AutoDiffDerivative(fun, num_blocks=3, shape=A.shape)
         np.testing.assert_allclose(jac(x), A)
 
+    @pytest.mark.unit
+    def test_jac_looped(self):
+        """Test computing the jacobian by explicit looping jvp."""
+
+        def test_fun(x, y, a):
+            return jnp.cos(x) + x * y + a
+
+        x = np.array([1, 5, 0.01, 200])
+        y = np.array([60, 1, 100, 0.02])
+        a = -2.0
+
+        jac1 = AutoDiffDerivative(test_fun, argnum=0, mode="fwd")
+        J1 = jac1.compute(x, y, a)
+
+        jac2 = AutoDiffDerivative(test_fun, argnum=0, mode="looped")
+        J2 = jac2.compute(x, y, a)
+
+        np.testing.assert_allclose(J1, J2, atol=1e-8)
+
 
 class TestJVP:
     """Test calculation of jacobian vector products."""
 
     @staticmethod
     def fun(x, c1, c2):
         """Function for testing."""
@@ -134,14 +153,15 @@
     x = np.ones(3).astype(float)
     c1 = np.arange(3).astype(float)
     c2 = np.arange(3).astype(float) + 2
 
     dx = np.array([1, 2, 3]).astype(float)
     dc1 = np.array([3, 4, 5]).astype(float)
     dc2 = np.array([-3, 1, -2]).astype(float)
+    y = np.array([1, 2, 3, 4])
 
     @pytest.mark.unit
     def test_autodiff_jvp(self):
         """Tests using AD for JVP calculation."""
         df = AutoDiffDerivative.compute_jvp(
             self.fun, 0, self.dx, self.x, self.c1, self.c2
         )
@@ -338,7 +358,19 @@
             self.x,
             self.c1,
             self.c2,
         )
         np.testing.assert_allclose(
             df, np.array([-33858.0, -55584.0, -77310.0, -99036.0]), rtol=1e-4
         )
+
+    @pytest.mark.unit
+    def test_vjp(self):
+        """Tests using AD and FD for VJP calculation."""
+        df = AutoDiffDerivative.compute_vjp(
+            self.fun, 0, self.y, self.x, self.c1, self.c2
+        )
+        np.testing.assert_allclose(df, np.array([180.0, 3360.0, 19440.0]))
+        df = FiniteDiffDerivative.compute_vjp(
+            self.fun, 0, self.y, self.x, self.c1, self.c2
+        )
+        np.testing.assert_allclose(df, np.array([180.0, 3360.0, 19440.0]), rtol=1e-4)
```

### Comparing `desc-opt-0.9.0/tests/test_equilibrium.py` & `desc-opt-0.9.1/tests/test_equilibrium.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import numpy as np
 import pytest
 from netCDF4 import Dataset
 
 import desc.examples
 from desc.__main__ import main
+from desc.backend import sign
 from desc.equilibrium import EquilibriaFamily, Equilibrium
 from desc.grid import Grid, LinearGrid
 from desc.io import InputReader
 from desc.objectives import get_equilibrium_objective
 
 from .utils import area_difference, compute_coords
 
@@ -178,14 +179,60 @@
     eq.change_resolution(L_grid=10, M_grid=10, N_grid=10)
     assert eq.L_grid == 10
     assert eq.M_grid == 10
     assert eq.N_grid == 10
 
 
 @pytest.mark.unit
+def test_eq_change_symmetry():
+    """Test changing stellarator symmetry."""
+    eq = Equilibrium(L=2, M=2, N=2, NFP=2, sym=False)
+    idx_sin = np.nonzero(
+        sign(eq.R_basis.modes[:, 1]) * sign(eq.R_basis.modes[:, 2]) < 0
+    )[0]
+    idx_cos = np.nonzero(
+        sign(eq.R_basis.modes[:, 1]) * sign(eq.R_basis.modes[:, 2]) > 0
+    )[0]
+    sin_modes = eq.R_basis.modes[idx_sin, :]
+    cos_modes = eq.R_basis.modes[idx_cos, :]
+
+    # stellarator symmetric
+    eq.change_resolution(sym=True)
+    assert eq.sym
+    assert eq.R_basis.sym == "cos"
+    assert not np.any(
+        [np.any(np.all(i == eq.R_basis.modes, axis=-1)) for i in sin_modes]
+    )
+    assert eq.Z_basis.sym == "sin"
+    assert not np.any(
+        [np.any(np.all(i == eq.Z_basis.modes, axis=-1)) for i in cos_modes]
+    )
+    assert eq.L_basis.sym == "sin"
+    assert not np.any(
+        [np.any(np.all(i == eq.L_basis.modes, axis=-1)) for i in cos_modes]
+    )
+    assert eq.surface.sym
+    assert eq.surface.R_basis.sym == "cos"
+    assert eq.surface.Z_basis.sym == "sin"
+
+    # undo symmetry
+    eq.change_resolution(sym=False)
+    assert not eq.sym
+    assert not eq.R_basis.sym
+    assert np.all([np.any(np.all(i == eq.R_basis.modes, axis=-1)) for i in sin_modes])
+    assert not eq.Z_basis.sym
+    assert np.all([np.any(np.all(i == eq.Z_basis.modes, axis=-1)) for i in cos_modes])
+    assert not eq.L_basis.sym
+    assert np.all([np.any(np.all(i == eq.L_basis.modes, axis=-1)) for i in cos_modes])
+    assert not eq.surface.sym
+    assert not eq.surface.R_basis.sym
+    assert not eq.surface.Z_basis.sym
+
+
+@pytest.mark.unit
 def test_resolution():
     """Test changing equilibrium spectral resolution."""
     eq1 = Equilibrium(L=5, M=6, N=7, L_grid=8, M_grid=9, N_grid=10)
     eq2 = Equilibrium()
 
     assert eq1.resolution != eq2.resolution
     eq2.change_resolution(**eq1.resolution)
@@ -260,9 +307,9 @@
 @pytest.mark.unit
 def test_change_NFP():
     """Test that changing the eq NFP correctly changes everything."""
     with warnings.catch_warnings():
         warnings.simplefilter("error")
         eq = desc.examples.get("HELIOTRON")
         eq.change_resolution(NFP=4)
-        obj = get_equilibrium_objective()
-        obj.build(eq)
+        obj = get_equilibrium_objective(eq=eq)
+        obj.build()
```

### Comparing `desc-opt-0.9.0/tests/test_examples.py` & `desc-opt-0.9.1/tests/test_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,19 +155,21 @@
         eq1.L_grid = res
         eq1.M_grid = res
         eq2.change_resolution(L=res, M=res)
         eq2.L_grid = res
         eq2.M_grid = res
 
         # force balances on the same grids
-        obj1 = ObjectiveFunction(ForceBalance())
+        obj1 = ObjectiveFunction(ForceBalance(eq=eq1))
         eq1.solve(objective=obj1)
 
         # force balances on different grids
-        obj2 = ObjectiveFunction((RadialForceBalance(), HelicalForceBalance()))
+        obj2 = ObjectiveFunction(
+            (RadialForceBalance(eq=eq2), HelicalForceBalance(eq=eq2))
+        )
         eq2.solve(objective=obj2)
 
         np.testing.assert_allclose(eq1.R_lmn, eq2.R_lmn, atol=5e-4)
         np.testing.assert_allclose(eq1.Z_lmn, eq2.Z_lmn, atol=5e-4)
         np.testing.assert_allclose(eq1.L_lmn, eq2.L_lmn, atol=2e-3)
 
     test(iota=True)
@@ -180,48 +182,48 @@
     # decrease resolution and double pressure so no longer in force balance
     eq = desc.examples.get("DSHAPE")
     eq.change_resolution(L=eq.M, L_grid=eq.M_grid)
     eq.p_l *= 2
 
     # target force balance residuals with |F| <= 1e3 N
     obj = ObjectiveFunction(
-        ForceBalance(normalize=False, normalize_target=False, bounds=(-1e3, 1e3)), eq=eq
+        ForceBalance(normalize=False, normalize_target=False, bounds=(-1e3, 1e3), eq=eq)
     )
     eq.solve(objective=obj, ftol=1e-16, xtol=1e-16, maxiter=100, verbose=3)
 
     # check that all errors are nearly 0, since residual values are within target bounds
     f = obj.compute_scaled_error(obj.x(eq))
     np.testing.assert_allclose(f, 0, atol=1e-4)
 
 
 @pytest.mark.regression
-def test_1d_optimization(SOLOVEV):
+def test_1d_optimization():
     """Tests 1D optimization for target aspect ratio."""
     eq = desc.examples.get("SOLOVEV")
-    objective = ObjectiveFunction(AspectRatio(target=2.5))
+    objective = ObjectiveFunction(AspectRatio(eq=eq, target=2.5))
     constraints = (
-        ForceBalance(),
-        FixBoundaryR(),
-        FixBoundaryZ(modes=eq.surface.Z_basis.modes[0:-1, :]),
-        FixPressure(),
-        FixIota(),
-        FixPsi(),
+        ForceBalance(eq=eq),
+        FixBoundaryR(eq=eq),
+        FixBoundaryZ(eq=eq, modes=eq.surface.Z_basis.modes[0:-1, :]),
+        FixPressure(eq=eq),
+        FixIota(eq=eq),
+        FixPsi(eq=eq),
     )
     options = {"perturb_options": {"order": 1}}
     with pytest.warns((FutureWarning, UserWarning)):
         eq.optimize(objective, constraints, optimizer="lsq-exact", options=options)
 
     np.testing.assert_allclose(eq.compute("R0/a")["R0/a"], 2.5, rtol=2e-4)
 
 
 @pytest.mark.regression
 def test_1d_optimization_old():
     """Tests 1D optimization for target aspect ratio."""
     eq = desc.examples.get("SOLOVEV")
-    objective = ObjectiveFunction(AspectRatio(target=2.5))
+    objective = ObjectiveFunction(AspectRatio(eq=eq, target=2.5))
     eq._optimize(
         objective,
         copy=False,
         solve_options={"verbose": 0},
         perturb_options={
             "dZb": True,
             "subspace": vmec_boundary_subspace(eq, ZBS=[0, 1]),
@@ -235,16 +237,16 @@
     """Run 1 step of the precise QH optimization example from Landreman & Paul."""
     grid = LinearGrid(
         M=eq.M, N=eq.N, NFP=eq.NFP, rho=np.array([0.6, 0.8, 1.0]), sym=True
     )
 
     objective = ObjectiveFunction(
         (
-            QuasisymmetryTwoTerm(helicity=(1, eq.NFP), grid=grid),
-            AspectRatio(target=8, weight=1e2),
+            QuasisymmetryTwoTerm(eq=eq, helicity=(1, eq.NFP), grid=grid),
+            AspectRatio(eq=eq, target=8, weight=1e2),
         ),
         verbose=0,
     )
     R_modes = np.vstack(
         (
             [0, 0, 0],
             eq.surface.R_basis.modes[
@@ -252,20 +254,20 @@
             ],
         )
     )
     Z_modes = eq.surface.Z_basis.modes[
         np.max(np.abs(eq.surface.Z_basis.modes), 1) > n + 1, :
     ]
     constraints = (
-        ForceBalance(),
-        FixBoundaryR(modes=R_modes),
-        FixBoundaryZ(modes=Z_modes),
-        FixPressure(),
-        FixCurrent(),
-        FixPsi(),
+        ForceBalance(eq=eq),
+        FixBoundaryR(eq=eq, modes=R_modes),
+        FixBoundaryZ(eq=eq, modes=Z_modes),
+        FixPressure(eq=eq),
+        FixCurrent(eq=eq),
+        FixPsi(eq=eq),
     )
     optimizer = Optimizer("proximal-lsq-exact")
     eq1, history = eq.optimize(
         objective=objective,
         constraints=constraints,
         optimizer=optimizer,
         maxiter=50,
@@ -289,16 +291,16 @@
     eq1 = load(".//tests//inputs//precise_QH_step1.h5")
     eq1a = run_qh_step(0, eq0)
     rho_err, theta_err = area_difference_desc(eq1, eq1a, Nr=1, Nt=1)
     # only need crude tolerances here to make sure the boundaries are
     # similar, the main test is ensuring its not pathological and has good qs
     assert rho_err.mean() < 1
 
-    obj = QuasisymmetryBoozer(helicity=(1, eq1a.NFP))
-    obj.build(eq1a)
+    obj = QuasisymmetryBoozer(helicity=(1, eq1a.NFP), eq=eq1a)
+    obj.build()
     B_asym = obj.compute(*obj.xs(eq1a))
     np.testing.assert_array_less(B_asym, 1e-1)
 
 
 @pytest.mark.regression
 @pytest.mark.solve
 def test_qh_optimization2():
@@ -307,16 +309,16 @@
     eq2 = load(".//tests//inputs//precise_QH_step2.h5")
     eq2a = run_qh_step(1, eq1)
     rho_err, theta_err = area_difference_desc(eq2, eq2a, Nr=1, Nt=1)
     # only need crude tolerances here to make sure the boundaries are
     # similar, the main test is ensuring its not pathological and has good qs
     assert rho_err.mean() < 1
 
-    obj = QuasisymmetryBoozer(helicity=(1, eq2a.NFP))
-    obj.build(eq2a)
+    obj = QuasisymmetryBoozer(helicity=(1, eq2a.NFP), eq=eq2a)
+    obj.build()
     B_asym = obj.compute(*obj.xs(eq2a))
     np.testing.assert_array_less(B_asym, 1e-2)
 
 
 @pytest.mark.regression
 @pytest.mark.solve
 @pytest.mark.mpl_image_compare(remove_text=True, tolerance=15)
@@ -326,16 +328,16 @@
     eq3 = load(".//tests//inputs//precise_QH_step3.h5")
     eq3a = run_qh_step(2, eq2)
     rho_err, theta_err = area_difference_desc(eq3, eq3a, Nr=1, Nt=1)
     # only need crude tolerances here to make sure the boundaries are
     # similar, the main test is ensuring its not pathological and has good qs
     assert rho_err.mean() < 1
 
-    obj = QuasisymmetryBoozer(helicity=(1, eq3a.NFP))
-    obj.build(eq3a)
+    obj = QuasisymmetryBoozer(helicity=(1, eq3a.NFP), eq=eq3a)
+    obj.build()
     B_asym = obj.compute(*obj.xs(eq3a))
     np.testing.assert_array_less(B_asym, 1e-3)
 
     fig, ax = plot_boozer_surface(eq3a)
     return fig
 
 
@@ -465,28 +467,28 @@
             Z_modes_to_fix.append([0, m, n])
         else:
             print(f"Freeing Z mode: m={m}, n={n}")
     Z_modes_to_fix = np.array(Z_modes_to_fix)
     eq.solve(
         verbose=3,
         ftol=1e-8,
-        constraints=get_fixed_boundary_constraints(profiles=False),
-        objective=ObjectiveFunction(objectives=CurrentDensity()),
+        constraints=get_fixed_boundary_constraints(eq=eq, profiles=False),
+        objective=ObjectiveFunction(objectives=CurrentDensity(eq=eq)),
     )
     ##################################
     # Done creating initial condition.
     # Now define optimization problem.
     ##################################
     constraints = (
-        CurrentDensity(),
-        FixBoundaryR(modes=R_modes_to_fix),
-        FixBoundaryZ(modes=Z_modes_to_fix),
-        FixPressure(),
-        FixCurrent(),
-        FixPsi(),
+        CurrentDensity(eq=eq),
+        FixBoundaryR(eq=eq, modes=R_modes_to_fix),
+        FixBoundaryZ(eq=eq, modes=Z_modes_to_fix),
+        FixPressure(eq=eq),
+        FixCurrent(eq=eq),
+        FixPsi(eq=eq),
     )
     # Objective function, for both desc and simsopt:
     # f = (aspect - 8)^2 + (2pi)^{-2} \int dtheta \int d\zeta [f_C(rho=1)]^2
     # grid for quasisymmetry objective:
     grid = LinearGrid(
         M=eq.M,
         N=eq.N,
@@ -495,17 +497,19 @@
     )
     # Cancel factor of 1/2 in desc objective which is not present in simsopt:
     aspect_weight = np.sqrt(2)
     # Also scale QS weight so objective is approximately independent of grid resolution:
     qs_weight = np.sqrt(len(grid.weights) / (8 * (np.pi**4)))
     objective = ObjectiveFunction(
         (
-            AspectRatio(target=aspect_target, weight=aspect_weight, normalize=False),
+            AspectRatio(
+                eq=eq, target=aspect_target, weight=aspect_weight, normalize=False
+            ),
             QuasisymmetryTwoTerm(
-                helicity=(1, nfp), grid=grid, weight=qs_weight, normalize=False
+                eq=eq, helicity=(1, nfp), grid=grid, weight=qs_weight, normalize=False
             ),
         )
     )
     eq2, result = eq.optimize(
         verbose=3,
         objective=objective,
         constraints=constraints,
@@ -533,15 +537,15 @@
 
     eq_fit = eq.copy()
 
     # this has all the constraints we need,
     #  iota=False specifies we want to fix current instead of iota
     cs = get_NAE_constraints(eq, qsc, iota=False, order=1)
 
-    objectives = ForceBalance()
+    objectives = ForceBalance(eq=eq)
     obj = ObjectiveFunction(objectives)
 
     eq.solve(verbose=3, ftol=1e-2, objective=obj, maxiter=50, xtol=1e-6, constraints=cs)
 
     # Make sure axis is same
     np.testing.assert_almost_equal(orig_Rax_val, eq.axis.R_n)
     np.testing.assert_almost_equal(orig_Zax_val, eq.axis.Z_n)
@@ -630,15 +634,15 @@
 
     eq_fit = eq.copy()
 
     # this has all the constraints we need,
     #  iota=False specifies we want to fix current instead of iota
     cs = get_NAE_constraints(eq, qsc, iota=False, order=1)
 
-    objectives = ForceBalance()
+    objectives = ForceBalance(eq=eq)
     obj = ObjectiveFunction(objectives)
 
     eq.solve(
         verbose=3, ftol=1e-2, objective=obj, maxiter=100, xtol=1e-6, constraints=cs
     )
 
     # Make sure axis is same
```

### Comparing `desc-opt-0.9.0/tests/test_geometry.py` & `desc-opt-0.9.1/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/tests/test_grid.py` & `desc-opt-0.9.1/tests/test_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tests for Grid classes."""
 
 import numpy as np
 import pytest
 from scipy import special
 
 from desc.basis import FourierZernikeBasis
-from desc.compute.utils import compress, surface_averages, surface_integrals
+from desc.compute.utils import surface_averages
 from desc.equilibrium import Equilibrium
 from desc.grid import (
     ConcentricGrid,
     Grid,
     LinearGrid,
     QuadratureGrid,
     dec_to_cf,
@@ -587,33 +587,14 @@
         cg = ConcentricGrid(2, 3, 4)
         cg.change_resolution(3, 4, 5)
         assert cg.L == 3
         assert cg.M == 4
         assert cg.N == 5
 
     @pytest.mark.unit
-    def test_enforce_symmetry_sum(self):
-        """Test that enforce_symmetry sums dtheta to 2pi.
-
-        Relies on correctness of surface_integrals.
-        """
-
-        def test(grid):
-            # check if theta nodes cover the circumference of the theta curve
-            dtheta_sums = surface_integrals(grid, q=1 / grid.spacing[:, 2])
-            np.testing.assert_allclose(dtheta_sums, 2 * np.pi * grid.num_zeta)
-
-        # Before enforcing symmetry,
-        # this grid has 2 surfaces near axis lacking theta > pi nodes.
-        # These edge cases should be handled correctly.
-        # Otherwise, a dimension mismatch or broadcast error should be raised.
-        test(ConcentricGrid(L=20, M=3, N=2, sym=True))
-        test(LinearGrid(L=20, M=3, N=2, sym=True))
-
-    @pytest.mark.unit
     def test_enforce_symmetry(self):
         """Test correctness of enforce_symmetry() for uniformly spaced nodes.
 
         Unlike enforce_symmetry(), the algorithm used in LinearGrid for
         symmetry also works if the nodes are not uniformly spaced. This test
         compares the two methods when the grid is uniformly spaced in theta,
         as a means to ensure enforce_symmetry() is correct.
@@ -726,15 +707,15 @@
             # random data with specified average on each surface
             coeffs = np.random.rand(basis.num_modes)
             coeffs[np.where((basis.modes[:, 1:] == [0, 0]).all(axis=1))[0]] = 0
             coeffs[np.where((basis.modes == [0, 0, 0]).all(axis=1))[0]] = true_avg
 
             # compute average for each surface in grid
             values = transform.transform(coeffs)
-            numerical_avg = compress(grid, surface_averages(grid, values))
+            numerical_avg = surface_averages(grid, values, expand_out=False)
             if isinstance(grid, ConcentricGrid):
                 # values closest to axis are never accurate enough
                 numerical_avg = numerical_avg[1:]
             np.testing.assert_allclose(
                 numerical_avg,
                 true_avg,
                 err_msg=str(type(grid)) + " " + str(grid.sym),
@@ -781,15 +762,15 @@
                 r_unique = r[grid.unique_rho_idx]
                 dr = np.empty_like(r_unique)
                 dr[0] = (r_unique[0] + r_unique[1]) / 2
                 dr[1:-1] = (r_unique[2:] - r_unique[:-2]) / 2
                 dr[-1] = 1 - (r_unique[-2] + r_unique[-1]) / 2
             else:
                 dr = 1 / grid.num_rho
-            expected_integral = np.sum(dr * compress(grid, function_of_rho))
+            expected_integral = np.sum(dr * function_of_rho[grid.unique_rho_idx])
             true_integral = np.log(1.35 / 0.35)
             midpoint_rule_error_bound = np.max(dr) ** 2 / 24 * (2 / 0.35**3)
             right_riemann_error_bound = dr * (1 / 0.35 - 1 / 1.35)
             np.testing.assert_allclose(
                 expected_integral,
                 true_integral,
                 rtol=0,
```

### Comparing `desc-opt-0.9.0/tests/test_input_output.py` & `desc-opt-0.9.1/tests/test_input_output.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/tests/test_interpolate.py` & `desc-opt-0.9.1/tests/test_interpolate.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
         fq = interp1d(x, xp, fp, method="catmull-rom")
         np.testing.assert_allclose(fq, f(x), rtol=1e-6, atol=1e-5)
 
         fq = interp1d(x, xp, fp, method="monotonic")
         np.testing.assert_allclose(fq, f(x), rtol=1e-4, atol=1e-3)
 
+        fq = interp1d(x, xp, fp, method="monotonic-0")
+        np.testing.assert_allclose(fq, f(x), rtol=1e-4, atol=1e-2)
+
     @pytest.mark.unit
     def test_interp1d_extrap_periodic(self):
         """Test extrapolation and periodic BC of 1d interpolation."""
         xp = np.linspace(0, 2 * np.pi, 200)
         x = np.linspace(-1, 2 * np.pi + 1, 10000)
         f = lambda x: np.sin(x)
         fp = f(xp)
@@ -62,16 +65,20 @@
         """Ensure monotonic interpolation is actually monotonic."""
         # true function is just linear with a jump discontinuity at x=1.5
         x = np.linspace(-4, 5, 10)
         f = np.heaviside(x - 1.5, 0) + 0.1 * x
         xq = np.linspace(-4, 5, 1000)
         dfc = interp1d(xq, x, f, derivative=1, method="cubic")
         dfm = interp1d(xq, x, f, derivative=1, method="monotonic")
+        dfm0 = interp1d(xq, x, f, derivative=1, method="monotonic-0")
         assert dfc.min() < 0  # cubic interpolation undershoots, giving negative slope
         assert dfm.min() > 0  # monotonic interpolation doesn't
+        assert dfm0.min() >= 0  # monotonic-0 doesn't overshoot either
+        # ensure monotonic-0 has 0 slope at end points
+        np.testing.assert_allclose(dfm0[np.array([0, -1])], 0, atol=1e-12)
 
 
 class TestInterp2D:
     """Tests for interp2d function."""
 
     @pytest.mark.unit
     def test_interp2d(self):
```

### Comparing `desc-opt-0.9.0/tests/test_linear_objectives.py` & `desc-opt-0.9.1/tests/test_linear_objectives.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     # symmetric cases automatically satisfy gauge freedom, no constraint needed.
     eq = Equilibrium.load(
         load_from=str(DummyStellarator["output_path"]), file_format="hdf5"
     )
     eq.change_resolution(L=2, M=1, N=1)
     correct_constraint_matrix = np.zeros((0, 5))
     lam_con = FixLambdaGauge(eq)
+    lam_con.build()
     np.testing.assert_array_equal(lam_con._A, correct_constraint_matrix)
 
 
 @pytest.mark.unit
 def test_LambdaGauge_asym():
     """Test that lambda gauge is fixed correctly for asymmetric equilibrium."""
     # just testing the gauge condition
@@ -80,14 +81,15 @@
         ),
         "axis": np.array([[-1, 0, -0.2], [0, 3.4, 0], [1, 0.2, 0]]),
         "objective": "force",
         "optimizer": "lsq-exact",
     }
     eq = Equilibrium(**inputs)
     lam_con = FixLambdaGauge(eq)
+    lam_con.build()
 
     # make sure that any lambda in the null space gives lambda==0 at theta=zeta=0
     Z = scipy.linalg.null_space(lam_con._A)
     grid = LinearGrid(L=10, theta=[0], zeta=[0])
     for z in Z.T:
         eq.L_lmn = z
         lam = eq.compute("lambda", grid=grid)["lambda"]
@@ -107,44 +109,46 @@
     np.testing.assert_allclose(surf.Z_lmn, surf5.Z_lmn, atol=1e-12)
 
 
 @pytest.mark.unit
 def test_constrain_bdry_with_only_one_mode():
     """Test Fixing boundary with a surface with only one mode in its basis."""
     eq = Equilibrium()
-    FixZ = BoundaryZSelfConsistency()
+    FixZ = BoundaryZSelfConsistency(eq=eq)
     try:
-        FixZ.build(eq)
+        FixZ.build()
     except Exception:
         pytest.fail(
             "Error encountered when attempting to constrain surface with"
             + " only one mode in its basis"
         )
 
 
 @pytest.mark.unit
 def test_constrain_asserts():
     """Test error checking for incompatible constraints."""
     eqi = Equilibrium(iota=PowerSeriesProfile(0, 0), pressure=PowerSeriesProfile(0, 0))
     eqc = Equilibrium(current=PowerSeriesProfile(0))
     # nonexistent toroidal current can't be constrained
     with pytest.raises(RuntimeError):
-        eqi.solve(constraints=FixCurrent())
+        eqi.solve(constraints=FixCurrent(eq=eqi))
     # nonexistent rotational transform can't be constrained
     with pytest.raises(RuntimeError):
-        eqc.solve(constraints=FixIota())
+        eqc.solve(constraints=FixIota(eq=eqc))
     # toroidal current and rotational transform can't be constrained simultaneously
     with pytest.raises(ValueError):
-        eqi.solve(constraints=(FixCurrent(), FixIota()))
+        eqi.solve(constraints=(FixCurrent(eq=eqi), FixIota(eq=eqi)))
     with pytest.raises(AssertionError):
-        eqi.solve(constraints=(FixPressure(target=2), FixPressure(target=1)))
+        eqi.solve(
+            constraints=(FixPressure(eq=eqi, target=2), FixPressure(eq=eqi, target=1))
+        )
     # cannot use two incompatible constraints
     with pytest.raises(AssertionError):
-        con1 = FixCurrent(target=eqc.c_l)
-        con2 = FixCurrent(target=eqc.c_l + 1)
+        con1 = FixCurrent(target=eqc.c_l, eq=eqc)
+        con2 = FixCurrent(target=eqc.c_l + 1, eq=eqc)
         eqc.solve(constraints=(con1, con2))
 
 
 @pytest.mark.regression
 @pytest.mark.solve
 @pytest.mark.slow
 def test_fixed_mode_solve():
@@ -152,29 +156,29 @@
     # Reset DSHAPE to initial guess, fix a mode, and then resolve
     # and check that the mode stayed fix
     L = 1
     M = 1
     eq = desc.examples.get("DSHAPE")
     eq.set_initial_guess()
     fixR = FixModeR(
-        modes=np.array([L, M, 0])
+        eq=eq, modes=np.array([L, M, 0])
     )  # no target supplied, so defaults to the eq's current R_LMN coeff
     fixZ = FixModeZ(
-        modes=np.array([L, -M, 0])
+        eq=eq, modes=np.array([L, -M, 0])
     )  # no target supplied, so defaults to the eq's current Z_LMN coeff
     orig_R_val = eq.R_lmn[eq.R_basis.get_idx(L=L, M=M, N=0)]
     orig_Z_val = eq.Z_lmn[eq.Z_basis.get_idx(L=L, M=-M, N=0)]
 
     constraints = (
-        FixLambdaGauge(),
-        FixPressure(),
-        FixIota(),
-        FixPsi(),
-        FixBoundaryR(),
-        FixBoundaryZ(),
+        FixLambdaGauge(eq=eq),
+        FixPressure(eq=eq),
+        FixIota(eq=eq),
+        FixPsi(eq=eq),
+        FixBoundaryR(eq=eq),
+        FixBoundaryZ(eq=eq),
         fixR,
         fixZ,
     )
 
     eq.solve(
         verbose=3,
         ftol=1e-2,
@@ -200,35 +204,35 @@
     # and check that the mode sum stayed fix
     modes_R = np.array([[1, 1, 0], [2, 2, 0]])
     modes_Z = np.array([[1, -1, 0], [2, -2, 0]])
 
     eq = desc.examples.get("DSHAPE")
     eq.set_initial_guess()
     fixR = FixSumModesR(
-        modes=modes_R, sum_weights=np.array([1, 2])
+        eq=eq, modes=modes_R, sum_weights=np.array([1, 2])
     )  # no target supplied, so defaults to the eq's current sum
     fixZ = FixSumModesZ(
-        modes=modes_Z, sum_weights=np.array([1, 2])
+        eq=eq, modes=modes_Z, sum_weights=np.array([1, 2])
     )  # no target supplied, so defaults to the eq's current sum
     orig_R_val = (
         eq.R_lmn[eq.R_basis.get_idx(L=modes_R[0, 0], M=modes_R[0, 1], N=0)]
         + 2 * eq.R_lmn[eq.R_basis.get_idx(L=modes_R[1, 0], M=modes_R[1, 1], N=0)]
     )
     orig_Z_val = (
         eq.Z_lmn[eq.Z_basis.get_idx(L=modes_Z[0, 0], M=modes_Z[0, 1], N=0)]
         + 2 * eq.Z_lmn[eq.Z_basis.get_idx(L=modes_Z[1, 0], M=modes_Z[1, 1], N=0)]
     )
 
     constraints = (
-        FixLambdaGauge(),
-        FixPressure(),
-        FixIota(),
-        FixPsi(),
-        FixBoundaryR(),
-        FixBoundaryZ(),
+        FixLambdaGauge(eq=eq),
+        FixPressure(eq=eq),
+        FixIota(eq=eq),
+        FixPsi(eq=eq),
+        FixBoundaryR(eq=eq),
+        FixBoundaryZ(eq=eq),
         fixR,
         fixZ,
     )
 
     eq.solve(
         verbose=3,
         ftol=1e-2,
@@ -259,20 +263,20 @@
     # also tests zero lambda solve
     eq = Equilibrium()
 
     orig_R_val = eq.axis.R_n
     orig_Z_val = eq.axis.Z_n
 
     constraints = (
-        FixThetaSFL(),
-        FixPressure(),
-        FixCurrent(),
-        FixPsi(),
-        FixAxisR(),
-        FixAxisZ(),
+        FixThetaSFL(eq=eq),
+        FixPressure(eq=eq),
+        FixCurrent(eq=eq),
+        FixPsi(eq=eq),
+        FixAxisR(eq=eq),
+        FixAxisZ(eq=eq),
     )
 
     eq.solve(
         verbose=3,
         ftol=1e-2,
         objective="force",
         maxiter=10,
@@ -285,17 +289,17 @@
     np.testing.assert_allclose(np.zeros_like(eq.L_lmn), eq.L_lmn, atol=1e-14)
 
 
 @pytest.mark.unit
 def test_factorize_linear_constraints_asserts():
     """Test error checking for factorize_linear_constraints."""
     eq = Equilibrium()
-    constraints = get_fixed_boundary_constraints(iota=False)
+    constraints = get_fixed_boundary_constraints(eq=eq, iota=False)
     for con in constraints:
-        con.build(eq, verbose=0)
+        con.build(verbose=0)
     constraints[3].bounds = (0, 1)  # bounds on FixPsi
 
     from desc.objectives.utils import factorize_linear_constraints
 
     with pytest.raises(ValueError):
         xp, A, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
             constraints, arg_order
@@ -307,31 +311,33 @@
     """Ensure that passing an equilibrium to init builds the objective correctly.
 
     Related to gh issue #378
     """
     eq = Equilibrium(M=3, N=1)
 
     # initialize the constraints without building
-    fbR1 = FixBoundaryR()
-    fbZ1 = FixBoundaryZ()
+    fbR1 = FixBoundaryR(eq=eq)
+    fbZ1 = FixBoundaryZ(eq=eq)
     for obj in (fbR1, fbZ1):
-        obj.build(eq)
+        obj.build()
 
     arg = fbR1.args[0]
     A = fbR1.derivatives["jac_scaled"][arg](np.zeros(fbR1.dimensions[arg]))
     assert np.max(np.abs(A)) == 1
     assert A.shape == (eq.surface.R_basis.num_modes, eq.surface.R_basis.num_modes)
 
     arg = fbZ1.args[0]
     A = fbZ1.derivatives["jac_scaled"][arg](np.zeros(fbZ1.dimensions[arg]))
     assert np.max(np.abs(A)) == 1
     assert A.shape == (eq.surface.Z_basis.num_modes, eq.surface.Z_basis.num_modes)
 
     fbR1 = FixBoundaryR(eq=eq)
     fbZ1 = FixBoundaryZ(eq=eq)
+    for obj in (fbR1, fbZ1):
+        obj.build()
 
     arg = fbR1.args[0]
     A = fbR1.derivatives["jac_scaled"][arg](np.zeros(fbR1.dimensions[arg]))
     assert np.max(np.abs(A)) == 1
     assert A.shape == (eq.surface.R_basis.num_modes, eq.surface.R_basis.num_modes)
 
     arg = fbZ1.args[0]
@@ -347,27 +353,27 @@
     eqk = Equilibrium(
         L=3,
         M=3,
         N=3,
         electron_temperature=np.array([1, 0, -1]),
         electron_density=np.array([2, 0, -2]),
     )
-    pcon = (FixPressure(),)
+    pcon = (FixPressure(eq=eqk),)
     kcon = (
-        FixAtomicNumber(),
-        FixElectronDensity(),
-        FixElectronTemperature(),
-        FixIonTemperature(),
+        FixAtomicNumber(eq=eqp),
+        FixElectronDensity(eq=eqp),
+        FixElectronTemperature(eq=eqp),
+        FixIonTemperature(eq=eqp),
     )
     for con in pcon:
         with pytest.raises(RuntimeError):
-            con.build(eqk)
+            con.build()
     for con in kcon:
         with pytest.raises(RuntimeError):
-            con.build(eqp)
+            con.build()
 
 
 @pytest.mark.unit
 def test_correct_indexing_passed_modes():
     """Test Indexing when passing in specified modes, related to gh issue #380."""
     n = 1
 
@@ -375,16 +381,16 @@
 
     grid = LinearGrid(
         M=eq.M, N=eq.N, NFP=eq.NFP, rho=np.array([0.6, 0.8, 1.0]), sym=True
     )
 
     objective = ObjectiveFunction(
         (
-            QuasisymmetryTwoTerm(weight=1e-2, helicity=(1, -eq.NFP), grid=grid),
-            AspectRatio(target=8, weight=1e2),
+            QuasisymmetryTwoTerm(eq=eq, weight=1e-2, helicity=(1, -eq.NFP), grid=grid),
+            AspectRatio(eq=eq, target=8, weight=1e2),
         ),
         verbose=0,
     )
     R_modes = np.vstack(
         (
             [0, 0, 0],
             eq.surface.R_basis.modes[
@@ -392,22 +398,22 @@
             ],
         )
     )
     Z_modes = eq.surface.Z_basis.modes[
         np.max(np.abs(eq.surface.Z_basis.modes), 1) > n + 1, :
     ]
     constraints = (
-        FixBoundaryR(modes=R_modes, normalize=False),
-        FixBoundaryZ(modes=Z_modes, normalize=False),
-        BoundaryRSelfConsistency(),
-        BoundaryZSelfConsistency(),
+        FixBoundaryR(eq=eq, modes=R_modes, normalize=False),
+        FixBoundaryZ(eq=eq, modes=Z_modes, normalize=False),
+        BoundaryRSelfConsistency(eq=eq),
+        BoundaryZSelfConsistency(eq=eq),
     )
     for con in constraints:
-        con.build(eq, verbose=0)
-    objective.build(eq)
+        con.build(verbose=0)
+    objective.build()
     objective.set_args("Rb_lmn", "Zb_lmn")
     from desc.objectives.utils import factorize_linear_constraints
 
     xp, A, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
         constraints,
         objective.args,
     )
@@ -432,16 +438,16 @@
 
     grid = LinearGrid(
         M=eq.M, N=eq.N, NFP=eq.NFP, rho=np.array([0.6, 0.8, 1.0]), sym=True
     )
 
     objective = ObjectiveFunction(
         (
-            QuasisymmetryTwoTerm(weight=1e-2, helicity=(1, -eq.NFP), grid=grid),
-            AspectRatio(target=8, weight=1e2),
+            QuasisymmetryTwoTerm(eq=eq, weight=1e-2, helicity=(1, -eq.NFP), grid=grid),
+            AspectRatio(eq=eq, target=8, weight=1e2),
         ),
         verbose=0,
     )
     R_modes = np.vstack(
         (
             [0, 0, 0],
             eq.surface.R_basis.modes[
@@ -458,18 +464,18 @@
         np.max(np.abs(eq.surface.Z_basis.modes), 1) > n + 1, :
     ]
     idxs = []
     for mode in Z_modes:
         idxs.append(eq.surface.Z_basis.get_idx(*mode))
     target_Z = eq.surface.Z_lmn[idxs]
     constraints = (
-        FixBoundaryR(modes=R_modes, normalize=False, target=target_R),
-        FixBoundaryZ(modes=Z_modes, normalize=False, target=target_Z),
-        BoundaryRSelfConsistency(),
-        BoundaryZSelfConsistency(),
+        FixBoundaryR(eq=eq, modes=R_modes, normalize=False, target=target_R),
+        FixBoundaryZ(eq=eq, modes=Z_modes, normalize=False, target=target_Z),
+        BoundaryRSelfConsistency(eq=eq),
+        BoundaryZSelfConsistency(eq=eq),
     )
     for con in constraints:
         con.build(eq, verbose=0)
     objective.build(eq)
     objective.set_args("Rb_lmn", "Zb_lmn")
     from desc.objectives.utils import factorize_linear_constraints
 
@@ -498,16 +504,16 @@
 
     grid = LinearGrid(
         M=eq.M, N=eq.N, NFP=eq.NFP, rho=np.array([0.6, 0.8, 1.0]), sym=True
     )
 
     objective = ObjectiveFunction(
         (
-            QuasisymmetryTwoTerm(weight=1e-2, helicity=(1, -eq.NFP), grid=grid),
-            AspectRatio(target=8, weight=1e2),
+            QuasisymmetryTwoTerm(eq=eq, weight=1e-2, helicity=(1, -eq.NFP), grid=grid),
+            AspectRatio(eq=eq, target=8, weight=1e2),
         ),
         verbose=0,
     )
     R_modes = np.vstack(
         (
             eq.axis.R_basis.modes[np.max(np.abs(eq.axis.R_basis.modes), 1) > n + 1, :],
             [0, 0, 0],
@@ -515,28 +521,29 @@
     )
     R_modes = np.flip(R_modes, 0)
 
     Z_modes = eq.axis.Z_basis.modes[np.max(np.abs(eq.axis.Z_basis.modes), 1) > n + 1, :]
     Z_modes = np.flip(Z_modes, 0)
 
     constraints = (
-        FixAxisR(modes=R_modes, normalize=False),
-        FixAxisZ(modes=Z_modes, normalize=False),
-        FixModeR(modes=np.array([[1, 1, 1], [2, 2, 2]]), normalize=False),
-        FixModeZ(modes=np.array([[1, 1, -1], [2, 2, -2]]), normalize=False),
+        FixAxisR(eq=eq, modes=R_modes, normalize=False),
+        FixAxisZ(eq=eq, modes=Z_modes, normalize=False),
+        FixModeR(eq=eq, modes=np.array([[1, 1, 1], [2, 2, 2]]), normalize=False),
+        FixModeZ(eq=eq, modes=np.array([[1, 1, -1], [2, 2, -2]]), normalize=False),
         FixSumModesR(
+            eq=eq,
             modes=np.array([[3, 3, 3], [4, 4, 4]]),
             normalize=False,
             sum_weights=np.ones(2),
         ),
-        FixSumModesZ(modes=np.array([[3, 3, -3], [4, 4, -4]]), normalize=False),
+        FixSumModesZ(eq=eq, modes=np.array([[3, 3, -3], [4, 4, -4]]), normalize=False),
     )
     for con in constraints:
-        con.build(eq, verbose=0)
-    objective.build(eq)
+        con.build(verbose=0)
+    objective.build()
     from desc.objectives.utils import factorize_linear_constraints
 
     xp, A, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
         constraints,
         objective.args,
     )
 
@@ -560,16 +567,16 @@
 
     grid = LinearGrid(
         M=eq.M, N=eq.N, NFP=eq.NFP, rho=np.array([0.6, 0.8, 1.0]), sym=True
     )
 
     objective = ObjectiveFunction(
         (
-            QuasisymmetryTwoTerm(weight=1e-2, helicity=(1, -eq.NFP), grid=grid),
-            AspectRatio(target=8, weight=1e2),
+            QuasisymmetryTwoTerm(eq=eq, weight=1e-2, helicity=(1, -eq.NFP), grid=grid),
+            AspectRatio(eq=eq, target=8, weight=1e2),
         ),
         verbose=0,
     )
     R_modes = np.vstack(
         (
             eq.axis.R_basis.modes[np.max(np.abs(eq.axis.R_basis.modes), 1) > n + 1, :],
             [0, 0, 0],
@@ -585,60 +592,64 @@
     Z_modes = np.flip(Z_modes, 0)
     idxs = []
     for mode in Z_modes:
         idxs.append(eq.axis.Z_basis.get_idx(*mode))
     target_Z = eq.axis.Z_n[idxs]
 
     constraints = (
-        FixAxisR(modes=R_modes, normalize=False, target=target_R),
-        FixAxisZ(modes=Z_modes, normalize=False, target=target_Z),
+        FixAxisR(eq=eq, modes=R_modes, normalize=False, target=target_R),
+        FixAxisZ(eq=eq, modes=Z_modes, normalize=False, target=target_Z),
         FixModeR(
+            eq=eq,
             modes=np.array([[1, 1, 1], [2, 2, 2]]),
             target=np.array(
                 [
                     eq.R_lmn[eq.R_basis.get_idx(*(1, 1, 1))],
                     eq.R_lmn[eq.R_basis.get_idx(*(2, 2, 2))],
                 ]
             ),
             normalize=False,
         ),
         FixModeZ(
+            eq=eq,
             modes=np.array([[1, 1, -1], [2, 2, -2]]),
             target=np.array(
                 [
                     eq.Z_lmn[eq.Z_basis.get_idx(*(1, 1, -1))],
                     eq.Z_lmn[eq.Z_basis.get_idx(*(2, 2, -2))],
                 ]
             ),
             normalize=False,
         ),
         FixSumModesR(
+            eq=eq,
             modes=np.array([[3, 3, 3], [4, 4, 4]]),
             target=np.array(
                 [
                     eq.R_lmn[eq.R_basis.get_idx(*(3, 3, 3))]
                     + eq.R_lmn[eq.R_basis.get_idx(*(4, 4, 4))]
                 ]
             ),
             normalize=False,
         ),
         FixSumModesZ(
+            eq=eq,
             modes=np.array([[3, 3, -3], [4, 4, -4]]),
             target=np.array(
                 [
                     eq.Z_lmn[eq.Z_basis.get_idx(*(3, 3, -3))]
                     + eq.Z_lmn[eq.Z_basis.get_idx(*(4, 4, -4))]
                 ]
             ),
             normalize=False,
         ),
     )
     for con in constraints:
-        con.build(eq, verbose=0)
-    objective.build(eq)
+        con.build(verbose=0)
+    objective.build()
     from desc.objectives.utils import factorize_linear_constraints
 
     xp, A, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
         constraints,
         objective.args,
     )
 
@@ -654,70 +665,70 @@
 
 
 @pytest.mark.unit
 def test_FixBoundary_with_single_weight():
     """Test Fixing boundary with only a single, passed weight."""
     eq = Equilibrium()
     w = 1.1
-    FixZ = FixBoundaryZ(modes=np.array([[0, -1, 0]]), weight=w)
-    FixZ.build(eq)
+    FixZ = FixBoundaryZ(eq=eq, modes=np.array([[0, -1, 0]]), weight=w)
+    FixZ.build()
     np.testing.assert_array_equal(FixZ.weight.size, 1)
     np.testing.assert_array_equal(FixZ.weight, w)
-    FixR = FixBoundaryR(modes=np.array([[0, 1, 0]]), weight=w)
-    FixR.build(eq)
+    FixR = FixBoundaryR(eq=eq, modes=np.array([[0, 1, 0]]), weight=w)
+    FixR.build()
     np.testing.assert_array_equal(FixR.weight.size, 1)
     np.testing.assert_array_equal(FixR.weight, w)
 
 
 @pytest.mark.unit
 def test_FixBoundary_passed_target_no_passed_modes_error():
     """Test Fixing boundary with no passed-in modes."""
     eq = Equilibrium()
-    FixZ = FixBoundaryZ(modes=True, target=np.array([[0]]))
+    FixZ = FixBoundaryZ(eq=eq, modes=True, target=np.array([[0]]))
     with pytest.raises(RuntimeError):
-        FixZ.build(eq)
-    FixZ = FixBoundaryZ(modes=False, target=np.array([[0]]))
+        FixZ.build()
+    FixZ = FixBoundaryZ(eq=eq, modes=False, target=np.array([[0]]))
     with pytest.raises(RuntimeError):
-        FixZ.build(eq)
-    FixR = FixBoundaryR(modes=True, target=np.array([[0]]))
+        FixZ.build()
+    FixR = FixBoundaryR(eq=eq, modes=True, target=np.array([[0]]))
     with pytest.raises(RuntimeError):
-        FixR.build(eq)
-    FixR = FixBoundaryR(modes=False, target=np.array([[0]]))
+        FixR.build()
+    FixR = FixBoundaryR(eq=eq, modes=False, target=np.array([[0]]))
     with pytest.raises(RuntimeError):
-        FixR.build(eq)
+        FixR.build()
 
 
 @pytest.mark.unit
 def test_FixAxis_passed_target_no_passed_modes_error():
     """Test Fixing Axis with no passed-in modes."""
     eq = Equilibrium()
-    FixZ = FixAxisZ(modes=True, target=np.array([[0]]))
+    FixZ = FixAxisZ(eq=eq, modes=True, target=np.array([[0]]))
     with pytest.raises(RuntimeError):
-        FixZ.build(eq)
-    FixZ = FixAxisZ(modes=False, target=np.array([[0]]))
+        FixZ.build()
+    FixZ = FixAxisZ(eq=eq, modes=False, target=np.array([[0]]))
     with pytest.raises(RuntimeError):
-        FixZ.build(eq)
-    FixR = FixAxisR(modes=True, target=np.array([[0]]))
+        FixZ.build()
+    FixR = FixAxisR(eq=eq, modes=True, target=np.array([[0]]))
     with pytest.raises(RuntimeError):
-        FixR.build(eq)
-    FixR = FixAxisR(modes=False, target=np.array([[0]]))
+        FixR.build()
+    FixR = FixAxisR(eq=eq, modes=False, target=np.array([[0]]))
     with pytest.raises(RuntimeError):
-        FixR.build(eq)
+        FixR.build()
 
 
 @pytest.mark.unit
 def test_FixMode_passed_target_no_passed_modes_error():
     """Test Fixing Modes with no passed-in modes."""
     eq = Equilibrium()
-    FixZ = FixModeZ(modes=True, target=np.array([[0]]))
+    FixZ = FixModeZ(eq=eq, modes=True, target=np.array([[0]]))
     with pytest.raises(RuntimeError):
-        FixZ.build(eq)
-    FixR = FixModeR(modes=True, target=np.array([[0]]))
+        FixZ.build()
+    FixR = FixModeR(eq=eq, modes=True, target=np.array([[0]]))
     with pytest.raises(RuntimeError):
-        FixR.build(eq)
+        FixR.build()
 
 
 @pytest.mark.unit
 def test_FixSumModes_passed_target_too_long():
     """Test Fixing Modes with more than a size-1 target."""
     # TODO: remove this test if FixSumModes is generalized
     # to accept multiple targets and sets of modes at a time
```

### Comparing `desc-opt-0.9.0/tests/test_magnetic_fields.py` & `desc-opt-0.9.1/tests/test_magnetic_fields.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/tests/test_objective_funs.py` & `desc-opt-0.9.1/tests/test_objective_funs.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
     @pytest.mark.unit
     def test_generic(self):
         """Test GenericObjective for arbitrary quantities."""
 
         def test(f, eq):
             obj = GenericObjective(f, eq=eq)
+            obj.build()
             kwargs = {
                 "R_lmn": eq.R_lmn,
                 "Z_lmn": eq.Z_lmn,
                 "L_lmn": eq.L_lmn,
                 "i_l": eq.i_l,
                 "c_l": eq.c_l,
                 "Psi": eq.Psi,
@@ -80,26 +81,28 @@
             y = data["Y"]
             r = jnp.sqrt(x**2 + y**2)
             return r
 
         eq = Equilibrium()
         grid = LinearGrid(2, 2, 2)
         objective = ObjectiveFromUser(myfun, eq=eq, grid=grid)
+        objective.build()
         R1 = objective.compute(*objective.xs(eq))
         R2 = eq.compute("R", grid=grid)["R"]
         np.testing.assert_allclose(R1, R2)
 
     @pytest.mark.unit
     def test_volume(self):
         """Test calculation of plasma volume."""
 
         def test(eq):
             obj = Volume(
                 target=10 * np.pi**2, weight=1 / np.pi**2, eq=eq, normalize=False
             )
+            obj.build()
             V = obj.compute_unscaled(eq.R_lmn, eq.Z_lmn)
             V_scaled = obj.compute_scaled_error(eq.R_lmn, eq.Z_lmn)
             V_scalar = obj.compute_scalar(eq.R_lmn, eq.Z_lmn)
             np.testing.assert_allclose(V, 20 * np.pi**2)
             np.testing.assert_allclose(V_scaled, 10)
             np.testing.assert_allclose(V_scalar, 10)
 
@@ -108,83 +111,89 @@
 
     @pytest.mark.unit
     def test_aspect_ratio(self):
         """Test calculation of aspect ratio."""
 
         def test(eq):
             obj = AspectRatio(target=5, weight=1, eq=eq)
+            obj.build()
             AR = obj.compute_unscaled(eq.R_lmn, eq.Z_lmn)
             AR_scaled = obj.compute_scaled_error(eq.R_lmn, eq.Z_lmn)
             np.testing.assert_allclose(AR, 10)
             np.testing.assert_allclose(AR_scaled, 5)
 
         test(Equilibrium(iota=PowerSeriesProfile(0)))
         test(Equilibrium(current=PowerSeriesProfile(0)))
 
     @pytest.mark.unit
     def test_elongation(self):
         """Test calculation of elongation."""
 
         def test(eq):
             obj = Elongation(target=0, weight=2, eq=eq)
+            obj.build()
             f = obj.compute_unscaled(eq.R_lmn, eq.Z_lmn)
             f_scaled = obj.compute_scaled_error(eq.R_lmn, eq.Z_lmn)
             np.testing.assert_allclose(f, 1.3 / 0.7, rtol=5e-3)
             np.testing.assert_allclose(f_scaled, 2 * (1.3 / 0.7), rtol=5e-3)
 
         test(get("HELIOTRON"))
 
     @pytest.mark.unit
     def test_energy(self):
         """Test calculation of MHD energy."""
 
         def test(eq):
             obj = Energy(target=0, weight=mu_0, eq=eq, normalize=False)
+            obj.build()
             W = obj.compute_unscaled(*obj.xs(eq))
             W_scaled = obj.compute_scaled_error(*obj.xs(eq))
             np.testing.assert_allclose(W, 10 / mu_0)
             np.testing.assert_allclose(W_scaled, 10)
 
         test(Equilibrium(node_pattern="quad", iota=PowerSeriesProfile(0)))
         test(Equilibrium(node_pattern="quad", current=PowerSeriesProfile(0)))
 
     @pytest.mark.unit
     def test_target_iota(self):
         """Test calculation of iota profile."""
 
         def test(eq):
             obj = RotationalTransform(target=1, weight=2, eq=eq)
+            obj.build()
             iota = obj.compute_unscaled(*obj.xs(eq))
             iota_scaled = obj.compute_scaled_error(*obj.xs(eq))
             np.testing.assert_allclose(iota, 0)
             np.testing.assert_allclose(iota_scaled, -2 / np.sqrt(3))
 
         test(Equilibrium(iota=PowerSeriesProfile(0)))
         test(Equilibrium(current=PowerSeriesProfile(0)))
 
     @pytest.mark.unit
     def test_toroidal_current(self):
         """Test calculation of toroidal current."""
 
         def test(eq):
             obj = ToroidalCurrent(target=1, weight=2, eq=eq, normalize=False)
+            obj.build()
             I = obj.compute_unscaled(*obj.xs(eq))
             I_scaled = obj.compute_scaled_error(*obj.xs(eq))
             np.testing.assert_allclose(I, 0)
             np.testing.assert_allclose(I_scaled, -2 / np.sqrt(3))
 
         test(Equilibrium(iota=PowerSeriesProfile(0)))
         test(Equilibrium(current=PowerSeriesProfile(0)))
 
     @pytest.mark.unit
     def test_qa_boozer(self):
         """Test calculation of Boozer QA metric."""
 
         def test(eq):
             obj = QuasisymmetryBoozer(eq=eq)
+            obj.build()
             fb = obj.compute_unscaled(*obj.xs(eq))
             np.testing.assert_allclose(fb, 0, atol=1e-12)
 
         test(Equilibrium(L=2, M=2, N=1, iota=PowerSeriesProfile(0)))
         test(Equilibrium(L=2, M=2, N=1, current=PowerSeriesProfile(0)))
 
     @pytest.mark.unit
@@ -201,14 +210,15 @@
             helicity=helicity,
             M_booz=M_booz,
             N_booz=N_booz,
             grid=grid,
             normalize=False,
             eq=eq,
         )
+        obj.build()
         f = obj.compute_unscaled(*obj.xs(eq))
         idx_f = np.argsort(np.abs(f))
 
         # compute all amplitudes in the Boozer spectrum
         transforms = get_transforms(
             "|B|_mn", eq=eq, grid=grid, M_booz=M_booz, N_booz=N_booz
         )
@@ -228,141 +238,158 @@
 
     @pytest.mark.unit
     def test_qs_twoterm(self):
         """Test calculation of two term QS metric."""
 
         def test(eq):
             obj = QuasisymmetryTwoTerm(eq=eq)
+            obj.build()
             fc = obj.compute_unscaled(*obj.xs(eq))
             np.testing.assert_allclose(fc, 0)
 
         test(Equilibrium(iota=PowerSeriesProfile(0)))
         test(Equilibrium(current=PowerSeriesProfile(0)))
 
     @pytest.mark.unit
     def test_qs_tripleproduct(self):
         """Test calculation of triple product QS metric."""
 
         def test(eq):
             obj = QuasisymmetryTripleProduct(eq=eq)
+            obj.build()
             ft = obj.compute_unscaled(*obj.xs(eq))
             np.testing.assert_allclose(ft, 0)
 
         test(Equilibrium(iota=PowerSeriesProfile(0)))
         test(Equilibrium(current=PowerSeriesProfile(0)))
 
     @pytest.mark.unit
     def test_isodynamicity(self):
         """Test calculation of isodynamicity metric."""
 
         def test(eq):
             obj = Isodynamicity(eq=eq)
+            obj.build()
             iso = obj.compute(*obj.xs(eq))
             np.testing.assert_allclose(iso, 0, atol=1e-14)
 
         test(Equilibrium(iota=PowerSeriesProfile(0)))
         test(Equilibrium(current=PowerSeriesProfile(0)))
 
     @pytest.mark.unit
     def test_qs_boozer_grids(self):
         """Test grid compatibility with QS objectives."""
         eq = get("QAS")
 
         # symmetric grid
         grid = LinearGrid(M=eq.M, N=eq.N, NFP=eq.NFP, sym=True)
         with pytest.raises(AssertionError):
-            _ = QuasisymmetryBoozer(eq=eq, grid=grid)
+            QuasisymmetryBoozer(eq=eq, grid=grid).build()
 
         # multiple flux surfaces
         grid = LinearGrid(M=eq.M, N=eq.N, NFP=eq.NFP, rho=[0.25, 0.5, 0.75, 1])
         with pytest.raises(AssertionError):
-            _ = QuasisymmetryBoozer(eq=eq, grid=grid)
+            QuasisymmetryBoozer(eq=eq, grid=grid).build()
 
     @pytest.mark.unit
     def test_mercier_stability(self):
         """Test calculation of mercier stability criteria."""
 
         def test(eq):
             obj = MercierStability(eq=eq)
+            obj.build()
             DMerc = obj.compute_unscaled(*obj.xs(eq))
             np.testing.assert_equal(len(DMerc), obj._transforms["grid"].num_rho)
             np.testing.assert_allclose(DMerc, 0)
 
         test(Equilibrium(iota=PowerSeriesProfile(0)))
         test(Equilibrium(current=PowerSeriesProfile(0)))
 
     @pytest.mark.unit
     def test_magnetic_well(self):
         """Test calculation of magnetic well stability criteria."""
 
         def test(eq):
             obj = MagneticWell(eq=eq)
+            obj.build()
             magnetic_well = obj.compute_unscaled(*obj.xs(eq))
             np.testing.assert_equal(len(magnetic_well), obj._transforms["grid"].num_rho)
             np.testing.assert_allclose(magnetic_well, 0, atol=1e-15)
 
         test(Equilibrium(iota=PowerSeriesProfile(0)))
         test(Equilibrium(current=PowerSeriesProfile(0)))
 
 
 @pytest.mark.unit
 def test_derivative_modes():
-    """Test equality of derivatives using batched and blocked methods."""
+    """Test equality of derivatives using batched, blocked, looped methods."""
     eq = Equilibrium(M=2, N=1, L=2)
-    obj1 = ObjectiveFunction(MagneticWell(), deriv_mode="batched", use_jit=False)
-    obj2 = ObjectiveFunction(MagneticWell(), deriv_mode="blocked", use_jit=False)
-
-    obj1.build(eq)
-    obj2.build(eq)
+    obj1 = ObjectiveFunction(MagneticWell(eq=eq), deriv_mode="batched", use_jit=False)
+    obj2 = ObjectiveFunction(MagneticWell(eq=eq), deriv_mode="blocked", use_jit=False)
+    obj3 = ObjectiveFunction(MagneticWell(eq=eq), deriv_mode="looped", use_jit=False)
+
+    obj1.build()
+    obj2.build()
+    obj3.build()
     x = obj1.x(eq)
     g1 = obj1.grad(x)
     g2 = obj2.grad(x)
+    g3 = obj3.grad(x)
     np.testing.assert_allclose(g1, g2, atol=1e-10)
+    np.testing.assert_allclose(g1, g3, atol=1e-10)
     J1 = obj1.jac_scaled(x)
     J2 = obj2.jac_scaled(x)
+    J3 = obj3.jac_scaled(x)
     np.testing.assert_allclose(J1, J2, atol=1e-10)
+    np.testing.assert_allclose(J1, J3, atol=1e-10)
     J1 = obj1.jac_unscaled(x)
     J2 = obj2.jac_unscaled(x)
+    J3 = obj3.jac_unscaled(x)
     np.testing.assert_allclose(J1, J2, atol=1e-10)
+    np.testing.assert_allclose(J1, J3, atol=1e-10)
     H1 = obj1.hess(x)
     H2 = obj2.hess(x)
+    H3 = obj3.hess(x)
+    # blocked hessian is only block diagonal, so we only check the diag part
     np.testing.assert_allclose(np.diag(H1), np.diag(H2), atol=1e-10)
+    # looped and batched should be full matrices
+    np.testing.assert_allclose(H1, H3, atol=1e-10)
 
 
 @pytest.mark.unit
 def test_rejit():
     """Test that updating attributes and recompiling correctly updates."""
 
     class DummyObjective(_Objective):
         def __init__(self, y, eq=None, target=0, weight=1, name="dummy"):
             self.y = y
             super().__init__(eq=eq, target=target, weight=weight, name=name)
 
-        def build(self, eq, use_jit=True, verbose=1):
+        def build(self, eq=None, use_jit=True, verbose=1):
             self._dim_f = 1
             super().build(eq, use_jit, verbose)
 
         def compute(self, R_lmn):
             return 200 + self.target * self.weight - self.y * R_lmn**3
 
-    obj = DummyObjective(3)
     eq = Equilibrium()
-    obj.build(eq)
+    obj = DummyObjective(3, eq=eq)
+    obj.build()
     assert obj.compute_unscaled(4) == 8
     assert obj.compute_scaled_error(4) == 8
     obj.target = 1
     obj.weight = 2
     assert obj.compute(4) == 10  # compute method is not JIT compiled
     assert obj.compute_scaled_error(4) == 8  # only compute_scaled is JIT compiled
     obj.jit()
     assert obj.compute(4) == 10
     assert obj.compute_scaled_error(4) == 18
 
     objFun = ObjectiveFunction(obj)
-    objFun.build(eq)
+    objFun.build()
     x = objFun.x(eq)
 
     f = objFun.compute_scaled_error(x)
     J = objFun.jac_scaled(x)
     np.testing.assert_allclose(f, [-5598, 402, 396])
     np.testing.assert_allclose(J, np.diag([-1800, 0, -18]))
     objFun.objectives[0].target = 3
@@ -375,26 +402,29 @@
     np.testing.assert_allclose(objFun.jac_scaled(x), J * 4 / 3)
 
 
 @pytest.mark.unit
 def test_generic_compute():
     """Test for gh issue #388."""
     eq = Equilibrium()
-    obj = ObjectiveFunction(AspectRatio(target=2, weight=1), eq=eq)
+    obj = ObjectiveFunction(AspectRatio(target=2, weight=1, eq=eq))
+    obj.build()
     a1 = obj.compute_scalar(obj.x(eq))
-    obj = ObjectiveFunction(GenericObjective("R0/a", target=2, weight=1), eq=eq)
+    obj = ObjectiveFunction(GenericObjective("R0/a", target=2, weight=1, eq=eq))
+    obj.build()
     a2 = obj.compute_scalar(obj.x(eq))
     assert np.allclose(a1, a2)
 
 
 @pytest.mark.unit
 def test_getter_setter():
     """Test getter and setter methods of Objectives."""
     eq = Equilibrium()
     obj = GenericObjective("R", eq=eq)
+    obj.build()
     R = obj.compute_unscaled(*obj.xs(eq))
 
     # target
     target = R - 0.5
     obj.target = target
     np.testing.assert_allclose(obj.target, target)
 
@@ -410,36 +440,36 @@
 
 
 @pytest.mark.unit
 def test_bounds_format():
     """Test that tuple targets are in the format (lower bound, upper bound)."""
     eq = Equilibrium()
     with pytest.raises(AssertionError):
-        _ = GenericObjective("R", bounds=(1,), eq=eq)
+        GenericObjective("R", bounds=(1,), eq=eq).build()
     with pytest.raises(AssertionError):
-        _ = GenericObjective("R", bounds=(1, 2, 3), eq=eq)
+        GenericObjective("R", bounds=(1, 2, 3), eq=eq).build()
     with pytest.raises(ValueError):
-        _ = GenericObjective("R", bounds=(1, -1), eq=eq)
+        GenericObjective("R", bounds=(1, -1), eq=eq).build()
 
 
 @pytest.mark.unit
 def test_target_profiles():
     """Tests for using Profile objects as targets for profile objectives."""
     iota = PowerSeriesProfile([1, 0, -0.3])
     current = PowerSeriesProfile([4, 0, 1, 0, -1])
     eqi = Equilibrium(L=5, N=3, M=3, iota=iota)
     eqc = Equilibrium(L=3, N=3, M=3, current=current)
-    obji = RotationalTransform(target=iota)
-    obji.build(eqc)
+    obji = RotationalTransform(target=iota, eq=eqi)
+    obji.build()
     np.testing.assert_allclose(
         obji.target,
         iota(obji._transforms["grid"].nodes[obji._transforms["grid"].unique_rho_idx]),
     )
-    objc = ToroidalCurrent(target=current)
-    objc.build(eqi)
+    objc = ToroidalCurrent(target=current, eq=eqc)
+    objc.build()
     np.testing.assert_allclose(
         objc.target,
         current(
             objc._transforms["grid"].nodes[objc._transforms["grid"].unique_rho_idx]
         ),
     )
 
@@ -458,94 +488,103 @@
     )
     # For equally spaced grids, should get true d=1
     surf_grid = LinearGrid(M=5, N=6)
     plas_grid = LinearGrid(M=5, N=6)
     obj = PlasmaVesselDistance(
         eq=eq, plasma_grid=plas_grid, surface_grid=surf_grid, surface=surface
     )
+    obj.build()
     d = obj.compute_unscaled(*obj.xs(eq))
     np.testing.assert_allclose(d, a_s - a_p)
 
     # for unequal M, should have error of order M_spacing*a_p
     surf_grid = LinearGrid(M=5, N=6)
     plas_grid = LinearGrid(M=10, N=6)
     obj = PlasmaVesselDistance(
         eq=eq, plasma_grid=plas_grid, surface_grid=surf_grid, surface=surface
     )
+    obj.build()
     d = obj.compute_unscaled(*obj.xs(eq))
     assert abs(d.min() - (a_s - a_p)) < 1e-14
     assert abs(d.max() - (a_s - a_p)) < surf_grid.spacing[0, 1] * a_p
 
     # for unequal N, should have error of order N_spacing*R0
     surf_grid = LinearGrid(M=5, N=6)
     plas_grid = LinearGrid(M=5, N=12)
     obj = PlasmaVesselDistance(
         eq=eq, plasma_grid=plas_grid, surface_grid=surf_grid, surface=surface
     )
+    obj.build()
     d = obj.compute_unscaled(*obj.xs(eq))
     assert abs(d.min() - (a_s - a_p)) < 1e-14
     assert abs(d.max() - (a_s - a_p)) < surf_grid.spacing[0, 2] * R0
 
     grid = LinearGrid(L=3, M=3, N=3)
     eq = Equilibrium()
     surf = FourierRZToroidalSurface()
-    obj = PlasmaVesselDistance(surface=surf, surface_grid=grid, plasma_grid=grid)
+    obj = PlasmaVesselDistance(surface=surf, surface_grid=grid, plasma_grid=grid, eq=eq)
     with pytest.warns(UserWarning):
-        obj.build(eq)
+        obj.build()
 
     # test softmin, should give value less than true minimum
     surf_grid = LinearGrid(M=5, N=6)
     plas_grid = LinearGrid(M=5, N=6)
     obj = PlasmaVesselDistance(
         eq=eq,
         plasma_grid=plas_grid,
         surface_grid=surf_grid,
         surface=surface,
         use_softmin=True,
     )
+    obj.build()
     d = obj.compute_unscaled(*obj.xs(eq))
     assert np.all(np.abs(d) < a_s - a_p)
 
     # for large enough alpha, should be same as actual min
     obj = PlasmaVesselDistance(
         eq=eq,
         plasma_grid=plas_grid,
         surface_grid=surf_grid,
         surface=surface,
         use_softmin=True,
         alpha=100,
     )
+    obj.build()
     d = obj.compute_unscaled(*obj.xs(eq))
     np.testing.assert_allclose(d, a_s - a_p)
 
 
 @pytest.mark.unit
 def test_mean_curvature():
     """Test for mean curvature objective function."""
     # simple case like dshape should have mean curvature negative everywhere
     eq = get("DSHAPE")
     obj = MeanCurvature(eq=eq)
+    obj.build()
     H = obj.compute_unscaled(*obj.xs(eq))
     assert np.all(H <= 0)
 
     # more shaped case like NCSX should have some positive curvature
     eq = get("NCSX")
     obj = MeanCurvature(eq=eq)
+    obj.build()
     H = obj.compute_unscaled(*obj.xs(eq))
     assert np.any(H > 0)
 
 
 @pytest.mark.unit
 def test_principal_curvature():
     """Test for principal curvature objective function."""
     eq1 = get("DSHAPE")
     eq2 = get("NCSX")
     obj1 = PrincipalCurvature(eq=eq1, normalize=False)
+    obj1.build()
     K1 = obj1.compute_unscaled(*obj1.xs(eq1))
     obj2 = PrincipalCurvature(eq=eq2, normalize=False)
+    obj2.build()
     K2 = obj2.compute_unscaled(*obj2.xs(eq2))
 
     # simple test: NCSX should have higher mean absolute curvature than DSHAPE
     assert K1.mean() < K2.mean()
 
 
 @pytest.mark.unit
@@ -560,14 +599,16 @@
     eq1 = Equilibrium(L=2, M=2, N=0, surface=surf1)
     eq2 = Equilibrium(L=2, M=2, N=0, surface=surf2)
     eq1.solve()
     eq2.solve()
 
     obj1 = BScaleLength(eq=eq1, normalize=False)
     obj2 = BScaleLength(eq=eq2, normalize=False)
+    obj1.build()
+    obj2.build()
 
     L1 = obj1.compute_unscaled(*obj1.xs(eq1))
     L2 = obj2.compute_unscaled(*obj2.xs(eq2))
 
     np.testing.assert_array_less(L1, L2)
 
 
@@ -613,17 +654,19 @@
                 + "\n"
             )
 
         assert out.out == corr_out
 
     iota = eq.compute("iota", grid=grid)["iota"]
     obj = RotationalTransform(eq=eq, grid=grid)
+    obj.build()
     test(obj, iota)
     curr = eq.compute("current", grid=grid)["current"]
     obj = ToroidalCurrent(eq=eq, grid=grid)
+    obj.build()
     test(obj, curr, normalize=True)
 
 
 @pytest.mark.unit
 def test_plasma_vessel_distance_print(capsys):
     """Test that the PlasmaVesselDistance objective prints correctly."""
     R0 = 10.0
@@ -636,14 +679,15 @@
         R_lmn=[R0, a_s], Z_lmn=[-a_s], modes_R=[[0, 0], [1, 0]], modes_Z=[[-1, 0]]
     )
     surf_grid = LinearGrid(M=5, N=0)
     plas_grid = LinearGrid(M=5, N=0)
     obj = PlasmaVesselDistance(
         eq=eq, plasma_grid=plas_grid, surface_grid=surf_grid, surface=surface
     )
+    obj.build()
     d = obj.compute_unscaled(*obj.xs(eq))
     np.testing.assert_allclose(d, a_s - a_p)
 
     obj.print_value(*obj.xs(eq))
     out = capsys.readouterr()
 
     corr_out = str(
@@ -676,25 +720,25 @@
     assert out.out == corr_out
 
 
 @pytest.mark.unit
 def test_rebuild():
     """Test that the objective is rebuilt correctly when needed."""
     eq = Equilibrium(L=3, M=3)
-    f_obj = ForceBalance()
+    f_obj = ForceBalance(eq=eq)
     obj = ObjectiveFunction(f_obj)
     eq.solve(maxiter=2, objective=obj)
 
     # this would fail before v0.8.2 when trying to get objective.x
     eq.change_resolution(L=5, M=5)
     obj.build(eq)
     eq.solve(maxiter=2, objective=obj)
 
     eq = Equilibrium(L=3, M=3)
-    f_obj = ForceBalance()
+    f_obj = ForceBalance(eq=eq)
     obj = ObjectiveFunction(f_obj)
     eq.solve(maxiter=2, objective=obj)
     eq.change_resolution(L=5, M=5)
     # this would fail at objective.compile
     obj = ObjectiveFunction(f_obj)
     obj.build(eq)
     eq.solve(maxiter=2, objective=obj)
@@ -702,16 +746,18 @@
 
 @pytest.mark.unit
 def test_jvp_scaled():
     """Test that jvps are scaled correctly."""
     eq = Equilibrium()
     weight = 3
     target = 5
-    objective = ObjectiveFunction(Volume(target=target, normalize=True, weight=weight))
-    objective.build(eq)
+    objective = ObjectiveFunction(
+        Volume(target=target, normalize=True, weight=weight, eq=eq)
+    )
+    objective.build()
     x = objective.x(eq)
     dx = x / 100
     jvp1u = objective.jvp_unscaled((dx,), x)
     jvp2u = objective.jvp_unscaled((dx, dx), x)
     jvp3u = objective.jvp_unscaled((dx, dx, dx), x)
     jvp1s = objective.jvp_scaled((dx,), x)
     jvp2s = objective.jvp_scaled((dx, dx), x)
@@ -731,24 +777,45 @@
         _ = objective.jvp_scaled((dx, dx, dx, dx), x)
 
     with pytest.raises(NotImplementedError):
         _ = objective.jvp_unscaled((dx, dx, dx, dx), x)
 
 
 @pytest.mark.unit
+def test_vjp():
+    """Test that vjps are scaled correctly."""
+    eq = Equilibrium()
+    weight = 3
+    target = 5
+    objective = ObjectiveFunction(
+        ForceBalance(target=target, normalize=True, weight=weight, eq=eq)
+    )
+    objective.build()
+    x = objective.x(eq)
+    y = np.linspace(0, 1, objective.dim_f)
+    vjp1u = objective.vjp_unscaled(y, x)
+    vjp1s = objective.vjp_scaled(y, x)
+    vjp2u = y @ objective.jac_unscaled(x)
+    vjp2s = y @ objective.jac_scaled(x)
+
+    np.testing.assert_allclose(vjp1u, vjp2u, atol=1e-8)
+    np.testing.assert_allclose(vjp1s, vjp2s, atol=1e-8)
+
+
+@pytest.mark.unit
 def test_objective_target_bounds():
     """Test that the target_scaled and bounds_scaled etc. return the right things."""
     eq = Equilibrium()
 
-    vol = Volume(target=3, normalize=True)
-    asp = AspectRatio(bounds=(2, 3), normalize=False)
-    fbl = ForceBalance(normalize=True, bounds=(-1, 2), weight=5)
+    vol = Volume(target=3, normalize=True, eq=eq)
+    asp = AspectRatio(bounds=(2, 3), normalize=False, eq=eq)
+    fbl = ForceBalance(normalize=True, bounds=(-1, 2), weight=5, eq=eq)
 
     objective = ObjectiveFunction((vol, asp, fbl))
-    objective.build(eq)
+    objective.build()
 
     target = objective.target_scaled
     bounds = objective.bounds_scaled
     weight = objective.weights
 
     assert bounds[0][0] == 3 / vol.normalization
     assert bounds[1][0] == 3 / vol.normalization
```

### Comparing `desc-opt-0.9.0/tests/test_optimizer.py` & `desc-opt-0.9.1/tests/test_optimizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -349,42 +349,42 @@
             self._built = True
 
         def compute(self, *args, **kwargs):
             params = self._parse_args(*args, **kwargs)
             x = jnp.concatenate([jnp.atleast_1d(params[arg]) for arg in self.args])
             return x - self._x0
 
+    eq = desc.examples.get("DSHAPE")
+
     np.random.seed(0)
-    objective = ObjectiveFunction(DummyObjective(), use_jit=False)
+    objective = ObjectiveFunction(DummyObjective(eq=eq), use_jit=False)
     # make gradient super noisy so it stalls
     objective.jac_scaled = lambda x: objective._jac_scaled(x) + 1e2 * (
         np.random.random((objective._dim_f, x.size)) - 0.5
     )
 
-    eq = desc.examples.get("DSHAPE")
-
     n = 10
     R_modes = np.vstack(
         (
             [0, 0, 0],
             eq.surface.R_basis.modes[
                 np.max(np.abs(eq.surface.R_basis.modes), 1) > n + 1, :
             ],
         )
     )
     Z_modes = eq.surface.Z_basis.modes[
         np.max(np.abs(eq.surface.Z_basis.modes), 1) > n + 1, :
     ]
     constraints = (
-        ForceBalance(),
-        FixBoundaryR(modes=R_modes),
-        FixBoundaryZ(modes=Z_modes),
-        FixPressure(),
-        FixIota(),
-        FixPsi(),
+        ForceBalance(eq=eq),
+        FixBoundaryR(eq=eq, modes=R_modes),
+        FixBoundaryZ(eq=eq, modes=Z_modes),
+        FixPressure(eq=eq),
+        FixIota(eq=eq),
+        FixPsi(eq=eq),
     )
     optimizer = Optimizer("lsq-exact")
     eq1, history = eq.optimize(
         objective=objective,
         constraints=constraints,
         optimizer=optimizer,
         maxiter=50,
@@ -409,24 +409,24 @@
 
 
 @pytest.mark.unit
 @pytest.mark.slow
 def test_maxiter_1_and_0_solve():
     """Test that solves with maxiter 1 and 0 terminate correctly."""
     # correctly meaning they terminate, instead of looping infinitely
+    eq = desc.examples.get("SOLOVEV")
     constraints = (
-        FixBoundaryR(),
-        FixBoundaryZ(),
-        FixPressure(),
-        FixIota(),
-        FixPsi(),
+        FixBoundaryR(eq=eq),
+        FixBoundaryZ(eq=eq),
+        FixPressure(eq=eq),
+        FixIota(eq=eq),
+        FixPsi(eq=eq),
     )
-    objectives = ForceBalance()
+    objectives = ForceBalance(eq=eq)
     obj = ObjectiveFunction(objectives)
-    eq = desc.examples.get("SOLOVEV")
     for opt in ["lsq-exact", "fmin-dogleg-bfgs"]:
         eq, result = eq.solve(
             maxiter=1, constraints=constraints, objective=obj, optimizer=opt, verbose=3
         )
         assert result["nit"] == 1
     for opt in ["lsq-exact", "fmin-dogleg-bfgs"]:
         eq, result = eq.solve(
@@ -435,38 +435,39 @@
         assert result["nit"] == 0
 
 
 @pytest.mark.unit
 @pytest.mark.slow
 def test_scipy_fail_message():
     """Test that scipy fail message does not cause an error (see PR #434)."""
+    eq = Equilibrium()
     constraints = (
-        FixBoundaryR(),
-        FixBoundaryZ(),
-        FixPressure(),
-        FixCurrent(),
-        FixPsi(),
+        FixBoundaryR(eq=eq),
+        FixBoundaryZ(eq=eq),
+        FixPressure(eq=eq),
+        FixCurrent(eq=eq),
+        FixPsi(eq=eq),
     )
-    objectives = ForceBalance()
+    objectives = ForceBalance(eq=eq)
     obj = ObjectiveFunction(objectives)
-    eq = Equilibrium()
+
     # should fail on maxiter, and should NOT throw an error
     for opt in ["scipy-trf"]:
         eq, result = eq.solve(
             maxiter=3,
             verbose=3,
             constraints=constraints,
             objective=obj,
             optimizer=opt,
             ftol=1e-12,
             xtol=1e-12,
             gtol=1e-12,
         )
         assert "Maximum number of iterations has been exceeded" in result["message"]
-    objectives = Energy()
+    objectives = Energy(eq=eq)
     obj = ObjectiveFunction(objectives)
     for opt in ["scipy-trust-exact"]:
         eq, result = eq.solve(
             maxiter=3,
             verbose=3,
             constraints=constraints,
             objective=obj,
@@ -486,60 +487,62 @@
 
 
 @pytest.mark.unit
 def test_wrappers():
     """Tests for using wrapped objectives."""
     eq = desc.examples.get("SOLOVEV")
     con = (
-        FixBoundaryR(),
-        FixBoundaryZ(),
-        FixIota(),
-        FixPressure(),
-        FixPsi(),
+        FixBoundaryR(eq=eq),
+        FixBoundaryZ(eq=eq),
+        FixIota(eq=eq),
+        FixPressure(eq=eq),
+        FixPsi(eq=eq),
     )
-    con_nl = (ForceBalance(),)
-    obj = ForceBalance()
+    con_nl = (ForceBalance(eq=eq),)
+    obj = ForceBalance(eq=eq)
     with pytest.raises(AssertionError):
         _ = LinearConstraintProjection(obj, con)
     with pytest.raises(ValueError):
         _ = LinearConstraintProjection(ObjectiveFunction(obj), con + con_nl)
     ob = LinearConstraintProjection(ObjectiveFunction(obj), con, eq=eq)
+    ob.build()
     assert ob.built
 
     np.testing.assert_allclose(
         ob.compute_scaled(ob.x(eq)), obj.compute_scaled(*obj.xs(eq))
     )
     np.testing.assert_allclose(
         ob.compute_unscaled(ob.x(eq)), obj.compute_unscaled(*obj.xs(eq))
     )
     np.testing.assert_allclose(ob.target_scaled, obj.target / obj.normalization)
     np.testing.assert_allclose(ob.bounds_scaled[0], obj.target / obj.normalization)
     np.testing.assert_allclose(ob.bounds_scaled[1], obj.target / obj.normalization)
     np.testing.assert_allclose(ob.weights, obj.weight)
 
     con = (
-        FixBoundaryR(),
-        FixBoundaryZ(),
-        FixIota(),
-        FixPressure(),
-        FixPsi(),
+        FixBoundaryR(eq=eq),
+        FixBoundaryZ(eq=eq),
+        FixIota(eq=eq),
+        FixPressure(eq=eq),
+        FixPsi(eq=eq),
     )
-    con_nl = (ForceBalance(),)
-    obj = ForceBalance()
+    con_nl = (ForceBalance(eq=eq),)
+    obj = ForceBalance(eq=eq)
     with pytest.raises(AssertionError):
         _ = ProximalProjection(obj, con[0])
     with pytest.raises(AssertionError):
         _ = ProximalProjection(ObjectiveFunction(con[0]), con[1])
     with pytest.raises(ValueError):
         _ = ProximalProjection(ObjectiveFunction(con[0]), ObjectiveFunction(con[1]))
     with pytest.raises(ValueError):
         _ = ProximalProjection(
             ObjectiveFunction(con[0]), ObjectiveFunction(con + con_nl)
         )
     ob = ProximalProjection(ObjectiveFunction(con[0]), ObjectiveFunction(con_nl), eq=eq)
+    ob.build()
     assert ob.built
 
     np.testing.assert_allclose(
         ob.compute_scaled(ob.x(eq)), con[0].compute_scaled(*con[0].xs(eq))
     )
     np.testing.assert_allclose(
         ob.compute_unscaled(ob.x(eq)), con[0].compute_unscaled(*con[0].xs(eq))
@@ -555,24 +558,24 @@
 
 
 @pytest.mark.unit
 @pytest.mark.slow
 def test_all_optimizers():
     """Just tests that the optimizers run without error, eg tests for the wrappers."""
     eq = desc.examples.get("SOLOVEV")
-    fobj = ObjectiveFunction(ForceBalance())
-    eobj = ObjectiveFunction(Energy())
-    fobj.build(eq)
-    eobj.build(eq)
+    fobj = ObjectiveFunction(ForceBalance(eq=eq))
+    eobj = ObjectiveFunction(Energy(eq=eq))
+    fobj.build()
+    eobj.build()
     constraints = (
-        FixBoundaryR(),
-        FixBoundaryZ(),
-        FixIota(),
-        FixPressure(),
-        FixPsi(),
+        FixBoundaryR(eq=eq),
+        FixBoundaryZ(eq=eq),
+        FixIota(eq=eq),
+        FixPressure(eq=eq),
+        FixPsi(eq=eq),
     )
 
     for opt in optimizers:
         print("TESTING ", opt)
         if optimizers[opt]["scalar"]:
             obj = eobj
         else:
@@ -598,35 +601,35 @@
     """
     eq = desc.examples.get("DSHAPE")
     # increase pressure so no longer in force balance
     eq.p_l *= 1.1
     eq._node_pattern = "quad"
 
     constraints = (
-        FixBoundaryR(modes=[0, 0, 0]),  # fix specified major axis position
-        FixBoundaryZ(),  # fix Z shape but not R
-        FixPressure(),  # fix pressure profile
-        FixIota(),  # fix rotational transform profile
-        FixPsi(),  # fix total toroidal magnetic flux
+        FixBoundaryR(eq=eq, modes=[0, 0, 0]),  # fix specified major axis position
+        FixBoundaryZ(eq=eq),  # fix Z shape but not R
+        FixPressure(eq=eq),  # fix pressure profile
+        FixIota(eq=eq),  # fix rotational transform profile
+        FixPsi(eq=eq),  # fix total toroidal magnetic flux
     )
     # some random constraints to keep the shape from getting wacky
     V = eq.compute("V")["V"]
     Vbounds = (0.95 * V, 1.05 * V)
     AR = eq.compute("R0/a")["R0/a"]
     ARbounds = (0.95 * AR, 1.05 * AR)
     H = eq.compute(
         "curvature_H", grid=LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
     )["curvature_H"]
     Hbounds = ((1 - 0.05 * np.sign(H)) * H, (1 + 0.05 * np.sign(H)) * abs(H))
     constraints += (
-        Volume(bounds=Vbounds),
-        AspectRatio(bounds=ARbounds),
-        MeanCurvature(bounds=Hbounds),
+        Volume(eq=eq, bounds=Vbounds),
+        AspectRatio(eq=eq, bounds=ARbounds),
+        MeanCurvature(eq=eq, bounds=Hbounds),
     )
-    obj = ObjectiveFunction(ForceBalance())
+    obj = ObjectiveFunction(ForceBalance(eq=eq))
     eq2, result = eq.optimize(
         objective=obj,
         constraints=constraints,
         optimizer="scipy-trust-constr",
         maxiter=50,
         verbose=1,
         x_scale="auto",
@@ -793,15 +796,15 @@
         x_scale="auto",
         ftol=0,
         xtol=1e-6,
         gtol=1e-6,
         ctol=1e-6,
         verbose=3,
         maxiter=None,
-        options={},
+        options={"initial_multipliers": "least_squares"},
     )
     print(out1["active_mask"])
     out2 = lsq_auglag(
         vecfun,
         x0,
         jac,
         bounds=(-jnp.inf, jnp.inf),
@@ -810,111 +813,133 @@
         x_scale="auto",
         ftol=0,
         xtol=1e-6,
         gtol=1e-6,
         ctol=1e-6,
         verbose=3,
         maxiter=None,
-        options={},
+        options={"initial_multipliers": "least_squares"},
     )
 
     out3 = minimize(
         fun,
         x0,
         jac=grad,
         hess=hess,
         constraints=constraint,
         method="trust-constr",
         options={"verbose": 3, "maxiter": 1000},
     )
+    out4 = fmin_auglag(
+        fun,
+        x0,
+        grad,
+        hess="bfgs",
+        bounds=(-jnp.inf, jnp.inf),
+        constraint=constraint,
+        args=(),
+        x_scale="auto",
+        ftol=0,
+        xtol=1e-6,
+        gtol=1e-6,
+        ctol=1e-6,
+        verbose=3,
+        maxiter=None,
+        options={"initial_multipliers": "least_squares"},
+    )
 
     np.testing.assert_allclose(out1["x"], out3["x"], rtol=1e-4, atol=1e-4)
     np.testing.assert_allclose(out2["x"], out3["x"], rtol=1e-4, atol=1e-4)
+    np.testing.assert_allclose(out4["x"], out3["x"], rtol=1e-4, atol=1e-4)
 
 
 @pytest.mark.slow
 @pytest.mark.regression
 def test_constrained_AL_lsq():
     """Tests that the least squares augmented Lagrangian optimizer does something."""
     eq = desc.examples.get("SOLOVEV")
 
     constraints = (
-        FixBoundaryR(modes=[0, 0, 0]),  # fix specified major axis position
-        FixBoundaryZ(),  # fix Z shape but not R
-        FixPressure(),  # fix pressure profile
-        FixIota(),  # fix rotational transform profile
-        FixPsi(),  # fix total toroidal magnetic flux
+        FixBoundaryR(eq=eq, modes=[0, 0, 0]),  # fix specified major axis position
+        FixBoundaryZ(eq=eq),  # fix Z shape but not R
+        FixPressure(eq=eq),  # fix pressure profile
+        FixIota(eq=eq),  # fix rotational transform profile
+        FixPsi(eq=eq),  # fix total toroidal magnetic flux
     )
     # some random constraints to keep the shape from getting wacky
     V = eq.compute("V")["V"]
     Vbounds = (0.95 * V, 1.05 * V)
     AR = eq.compute("R0/a")["R0/a"]
     ARbounds = (0.95 * AR, 1.05 * AR)
     constraints += (
-        Volume(bounds=Vbounds),
-        AspectRatio(bounds=ARbounds),
-        MagneticWell(bounds=(0, jnp.inf)),
-        ForceBalance(bounds=(-1e-3, 1e-3), normalize_target=False),
+        Volume(eq=eq, bounds=Vbounds),
+        AspectRatio(eq=eq, bounds=ARbounds),
+        MagneticWell(eq=eq, bounds=(0, jnp.inf)),
+        ForceBalance(eq=eq, bounds=(-1e-3, 1e-3), normalize_target=False),
     )
     H = eq.compute(
         "curvature_H", grid=LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
     )["curvature_H"]
-    obj = ObjectiveFunction(MeanCurvature(target=H))
+    obj = ObjectiveFunction(MeanCurvature(eq=eq, target=H))
+    ctol = 1e-4
     eq2, result = eq.optimize(
         objective=obj,
         constraints=constraints,
         optimizer="lsq-auglag",
         maxiter=500,
         verbose=3,
+        ctol=ctol,
         x_scale="auto",
         copy=True,
         options={},
     )
     V2 = eq2.compute("V")["V"]
     AR2 = eq2.compute("R0/a")["R0/a"]
     Dwell = constraints[-2].compute(*constraints[-2].xs(eq2))
-    assert ARbounds[0] < AR2 < ARbounds[1]
-    assert Vbounds[0] < V2 < Vbounds[1]
+    assert (ARbounds[0] - ctol) < AR2 < (ARbounds[1] + ctol)
+    assert (Vbounds[0] - ctol) < V2 < (Vbounds[1] + ctol)
     assert eq2.is_nested()
-    np.testing.assert_array_less(-Dwell, 0)
+    np.testing.assert_array_less(-Dwell, ctol)
 
 
 @pytest.mark.slow
 @pytest.mark.regression
 def test_constrained_AL_scalar():
     """Tests that the augmented Lagrangian constrained optimizer does something."""
     eq = desc.examples.get("SOLOVEV")
 
     constraints = (
-        FixBoundaryR(modes=[0, 0, 0]),  # fix specified major axis position
-        FixBoundaryZ(),  # fix Z shape but not R
-        FixPressure(),  # fix pressure profile
-        FixIota(),  # fix rotational transform profile
-        FixPsi(),  # fix total toroidal magnetic flux
+        FixBoundaryR(eq=eq, modes=[0, 0, 0]),  # fix specified major axis position
+        FixBoundaryZ(eq=eq),  # fix Z shape but not R
+        FixPressure(eq=eq),  # fix pressure profile
+        FixIota(eq=eq),  # fix rotational transform profile
+        FixPsi(eq=eq),  # fix total toroidal magnetic flux
     )
     V = eq.compute("V")["V"]
     AR = eq.compute("R0/a")["R0/a"]
     constraints += (
-        Volume(target=V),
-        AspectRatio(target=AR),
-        MagneticWell(bounds=(0, jnp.inf)),
-        ForceBalance(bounds=(-1e-3, 1e-3), normalize_target=False),
+        Volume(eq=eq, target=V),
+        AspectRatio(eq=eq, target=AR),
+        MagneticWell(eq=eq, bounds=(0, jnp.inf)),
+        ForceBalance(eq=eq, bounds=(-1e-3, 1e-3), normalize_target=False),
     )
     # Dummy objective to return 0, we just want a feasible solution.
-    obj = ObjectiveFunction(GenericObjective("0"))
+    obj = ObjectiveFunction(GenericObjective("0", eq=eq))
+    ctol = 1e-4
     eq2, result = eq.optimize(
         objective=obj,
         constraints=constraints,
         optimizer="fmin-auglag",
         maxiter=500,
         verbose=3,
+        ctol=ctol,
         x_scale="auto",
         copy=True,
         options={},
     )
     V2 = eq2.compute("V")["V"]
     AR2 = eq2.compute("R0/a")["R0/a"]
     Dwell = constraints[-2].compute(*constraints[-2].xs(eq2))
-    np.testing.assert_allclose(AR, AR2)
-    np.testing.assert_allclose(V, V2)
+    np.testing.assert_allclose(AR, AR2, atol=ctol)
+    np.testing.assert_allclose(V, V2, atol=ctol)
     assert eq2.is_nested()
-    np.testing.assert_array_less(-Dwell, 0)
+    np.testing.assert_array_less(-Dwell, ctol)
```

### Comparing `desc-opt-0.9.0/tests/test_perturbations.py` & `desc-opt-0.9.1/tests/test_perturbations.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 @pytest.mark.unit
 @pytest.mark.slow
 @pytest.mark.solve
 def test_perturbation_orders(SOLOVEV):
     """Test that higher-order perturbations are more accurate."""
     eq = EquilibriaFamily.load(load_from=str(SOLOVEV["desc_h5_path"]))[-1]
 
-    objective = get_equilibrium_objective()
-    constraints = get_fixed_boundary_constraints()
+    objective = get_equilibrium_objective(eq=eq)
+    constraints = get_fixed_boundary_constraints(eq=eq)
 
     # perturb pressure
     tr_ratio = [0.01, 0.25, 0.25]
     dp = np.zeros_like(eq.p_l)
     dp[np.array([0, 2])] = 8e3 * np.array([1, -1])
     deltas = {"p_l": dp}
     eq0 = perturb(
@@ -100,16 +100,16 @@
 @pytest.mark.unit
 def test_perturb_with_float_without_error():
     """Test that perturb works without error if only a single float is passed."""
     # PR #
     # fixed bug where np.concatenate( [float] ) was called resulting in error that
     # np.concatenate cannot concatenate 0-D arrays. This test exercises the fix.
     eq = Equilibrium()
-    objective = get_equilibrium_objective()
-    constraints = get_fixed_boundary_constraints(iota=False)
+    objective = get_equilibrium_objective(eq=eq)
+    constraints = get_fixed_boundary_constraints(eq=eq, iota=False)
 
     # perturb Psi with a float
     deltas = {"Psi": float(eq.Psi)}
     eq = perturb(
         eq,
         objective,
         constraints,
@@ -126,20 +126,22 @@
     # as of v0.6.1, the recover operation from optimal_perturb would give
     # R_lmn etc that are inconsistent with Rb_lmn due to recovering x with the wrong
     # particular solution. Here we do a simple test to ensure the interior and boundary
     # agree
     eq1 = desc.examples.get("DSHAPE")
     eq1.change_resolution(N=1, N_grid=5)
     objective = ObjectiveFunction(
-        ToroidalCurrent(grid=QuadratureGrid(eq1.L, eq1.M, eq1.N), target=0, weight=1)
+        ToroidalCurrent(
+            eq=eq1, grid=QuadratureGrid(eq1.L, eq1.M, eq1.N), target=0, weight=1
+        )
     )
-    constraint = ObjectiveFunction(ForceBalance(target=0))
+    constraint = ObjectiveFunction(ForceBalance(eq=eq1, target=0))
 
-    objective.build(eq1)
-    constraint.build(eq1)
+    objective.build()
+    constraint.build()
 
     R_modes = np.zeros(eq1.surface.R_lmn.size).astype(bool)
     Z_modes = np.zeros(eq1.surface.Z_lmn.size).astype(bool)
 
     Rmask = np.logical_and(
         abs(eq1.surface.R_basis.modes[:, 1]) < 3,
         np.logical_and(
```

### Comparing `desc-opt-0.9.0/tests/test_plotting.py` & `desc-opt-0.9.1/tests/test_plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -706,15 +706,15 @@
 @pytest.mark.unit
 @pytest.mark.slow
 @pytest.mark.mpl_image_compare(remove_text=True, tolerance=tol_2d)
 def test_plot_boozer_surface():
     """Test plotting B in boozer coordinates."""
     eq = get("WISTELL-A")
     fig, ax, data = plot_boozer_surface(
-        eq, M_booz=eq.M, N_booz=eq.N, return_data=True, fill=True
+        eq, M_booz=eq.M, N_booz=eq.N, return_data=True, rho=0.5, fieldlines=4
     )
     for string in [
         "|B|",
         "theta_Boozer",
         "zeta_Boozer",
     ]:
         assert string in data.keys()
```

### Comparing `desc-opt-0.9.0/tests/test_profiles.py` & `desc-opt-0.9.1/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/tests/test_stability_funs.py` & `desc-opt-0.9.1/tests/test_stability_funs.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,14 +219,15 @@
     """Test that the Mercier stability criteria prints correctly."""
     eq = Equilibrium()
     grid = LinearGrid(L=10, M=10, N=5, axis=False)
 
     Dmerc = eq.compute("D_Mercier", grid=grid)["D_Mercier"]
 
     mercier_obj = MercierStability(eq=eq, grid=grid)
+    mercier_obj.build()
     np.testing.assert_allclose(mercier_obj.compute(*mercier_obj.xs(eq)), 0)
     mercier_obj.print_value(*mercier_obj.xs(eq))
     out = capsys.readouterr()
 
     corr_out = str(
         "Precomputing transforms\n"
         + "Maximum "
@@ -261,14 +262,15 @@
 
 @pytest.mark.unit
 def test_magwell_print(capsys):
     """Test that the magnetic well stability criteria prints correctly."""
     eq = desc.examples.get("HELIOTRON")
     grid = LinearGrid(L=12, M=12, N=6, axis=False)
     obj = MagneticWell(eq=eq, grid=grid)
+    obj.build()
 
     magwell = compress(grid, eq.compute("magnetic well", grid=grid)["magnetic well"])
     f = obj.compute(*obj.xs(eq))
     np.testing.assert_allclose(f, magwell)
 
     obj.print_value(*obj.xs(eq))
     out = capsys.readouterr()
```

### Comparing `desc-opt-0.9.0/tests/test_surfaces.py` & `desc-opt-0.9.1/tests/test_surfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
 
         assert c.sym
 
     @pytest.mark.unit
     def test_curvature(self):
         """Tests for gaussian, mean, principle curvatures.
 
-        (kind of pointless since its a flat surface so its always 0)
+        (kind of pointless since it's a flat surface so its always 0)
         """
         s = ZernikeRZToroidalSection()
         grid = LinearGrid(theta=np.pi / 2, rho=0.5)
         s.grid = grid
         K, H, k1, k2 = s.compute_curvature()
         np.testing.assert_allclose(K, 0)
         np.testing.assert_allclose(H, 0)
```

### Comparing `desc-opt-0.9.0/tests/test_transform.py` & `desc-opt-0.9.1/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/tests/test_utils.py` & `desc-opt-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.9.0/tests/test_vmec.py` & `desc-opt-0.9.1/tests/test_vmec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Tests for reading/writing/converting VMEC data."""
 
 import numpy as np
 import pytest
 from netCDF4 import Dataset
 
 from desc.basis import DoubleFourierSeries, FourierZernikeBasis
+from desc.compute.utils import compress
 from desc.equilibrium import EquilibriaFamily, Equilibrium
 from desc.grid import LinearGrid
 from desc.vmec import VMECIO
 from desc.vmec_utils import (
     fourier_to_zernike,
     ptolemy_identity_fwd,
     ptolemy_identity_rev,
@@ -251,25 +252,51 @@
         m, n, x_mn = zernike_to_fourier(x_lmn, basis, rho)
 
         np.testing.assert_allclose(m, m_correct, atol=1e-8)
         np.testing.assert_allclose(n, n_correct, atol=1e-8)
         np.testing.assert_allclose(x_mn, x_mn_correct, atol=1e-8)
 
 
+@pytest.mark.unit
+def test_vmec_load_profiles(TmpDir):
+    """Tests that loading with iota or current profiles give same result."""
+    input_path = "./tests/inputs/wout_SOLOVEV.nc"
+
+    eq_iota = VMECIO.load(input_path, profile="iota")
+    eq_current = VMECIO.load(input_path, profile="current")
+
+    assert eq_iota.current is None
+    assert eq_current.iota is None
+
+    grid = LinearGrid(
+        M=eq_iota.M_grid,
+        N=eq_iota.N_grid,
+        NFP=eq_iota.NFP,
+        rho=np.linspace(0.5, 1.0, 21),
+    )
+    data_iota = eq_iota.compute(["iota", "current"], grid=grid)
+    data_current = eq_current.compute(["iota", "current"], grid=grid)
+
+    iota_iota = compress(grid, data_iota["iota"])
+    iota_current = compress(grid, data_current["iota"])
+    current_iota = compress(grid, data_iota["current"])
+    current_current = compress(grid, data_current["current"])
+
+    np.testing.assert_allclose(iota_iota, iota_current, rtol=2e-2)
+    np.testing.assert_allclose(current_current, current_iota, rtol=2e-2)
+
+
 @pytest.mark.slow
 @pytest.mark.unit
 def test_load_then_save(TmpDir):
     """Tests if loading and then saving gives the original result."""
     input_path = "./tests/inputs/wout_SOLOVEV.nc"
     output_path = str(TmpDir.join("DESC_SOLOVEV.nc"))
 
-    eq = VMECIO.load(input_path, profile="current")
-    assert eq.iota is None
     eq = VMECIO.load(input_path, profile="iota")
-    assert eq.current is None
     VMECIO.save(eq, output_path)
 
     file1 = Dataset(input_path, mode="r")
     file2 = Dataset(output_path, mode="r")
 
     rmnc1 = file1.variables["rmnc"][:]
     rmnc2 = file2.variables["rmnc"][:]
```

### Comparing `desc-opt-0.9.0/versioneer.py` & `desc-opt-0.9.1/versioneer.py`

 * *Files identical despite different names*

