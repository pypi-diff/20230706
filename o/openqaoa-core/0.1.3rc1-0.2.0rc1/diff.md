# Comparing `tmp/openqaoa-core-0.1.3rc1.tar.gz` & `tmp/openqaoa-core-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openqaoa-core-0.1.3rc1.tar", last modified: Fri Jun 30 09:16:30 2023, max compression
+gzip compressed data, was "openqaoa-core-0.2.0rc1.tar", last modified: Thu Jul  6 05:58:22 2023, max compression
```

## Comparing `openqaoa-core-0.1.3rc1.tar` & `openqaoa-core-0.2.0rc1.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.936320 openqaoa-core-0.1.3rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-06-30 09:16:30.936320 openqaoa-core-0.1.3rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.916319 openqaoa-core-0.1.3rc1/openqaoa/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.916319 openqaoa-core-0.1.3rc1/openqaoa/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30166 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/algorithms/baseworkflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.916319 openqaoa-core-0.1.3rc1/openqaoa/algorithms/qaoa/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/algorithms/qaoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28187 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/algorithms/qaoa/qaoa_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    28182 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/algorithms/qaoa/qaoa_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    20846 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/algorithms/qaoa/qaoa_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.920320 openqaoa-core-0.1.3rc1/openqaoa/algorithms/rqaoa/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/algorithms/rqaoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/algorithms/rqaoa/rqaoa_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/algorithms/rqaoa/rqaoa_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/algorithms/rqaoa/rqaoa_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/algorithms/rqaoa/rqaoa_workflow_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/algorithms/workflow_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.920320 openqaoa-core-0.1.3rc1/openqaoa/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/backends/basebackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/backends/basedevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/backends/cost_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/backends/devices_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/backends/gates_vectorized.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/backends/plugin_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/backends/qaoa_analytical_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/backends/qaoa_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/backends/qaoa_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    30340 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/backends/qaoa_vectorized.py
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/backends/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.920320 openqaoa-core-0.1.3rc1/openqaoa/derivatives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/derivatives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33483 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/derivatives/derivative_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/derivatives/qfim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.920320 openqaoa-core-0.1.3rc1/openqaoa/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/logger_vqa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.924320 openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/CANS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/SPSA.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/grad_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/iCANS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/natural_grad_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/newton_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/stochastic_grad_descent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.924320 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.924320 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/fourier/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/fourier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31659 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/fourier/reconstruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.924320 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/math/
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14426 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/math/is_independent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/math/matrix_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    30070 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/math/multi_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/math/quantum.py
--rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/math/single_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/math/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.924320 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/numpy/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/numpy/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/numpy/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/optimization_methods_pennylane.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.924320 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/gradient_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/momentum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/nesterov_momentum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/rms_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    32442 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/rotosolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/spsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/qaoa_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    32425 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/optimizers/training_vqa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.928320 openqaoa-core-0.1.3rc1/openqaoa/problems/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/problems/binpacking.py
--rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/problems/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/problems/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/problems/knapsack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/problems/maximalindependentset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/problems/maximumcut.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/problems/minimumvertexcover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/problems/numberpartition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/problems/portfoliooptimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/problems/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/problems/qubo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/problems/shortestpath.py
--rw-r--r--   0 runner    (1001) docker     (123)    13680 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/problems/tsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/problems/vehiclerouting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.928320 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.928320 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/ansatz_constructor/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/ansatz_constructor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/ansatz_constructor/baseparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/ansatz_constructor/gatemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/ansatz_constructor/gatemaplabel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/ansatz_constructor/gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/ansatz_constructor/hamiltonianmapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21325 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/ansatz_constructor/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/ansatz_constructor/rotationangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.928320 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/annealingparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/extendedparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    27328 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/fourierparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    12468 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/standardparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/variational_baseparams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/variational_params_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/variational_params_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    63680 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/openqaoa/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.932320 openqaoa-core-0.1.3rc1/openqaoa_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-06-30 09:16:30.000000 openqaoa-core-0.1.3rc1/openqaoa_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-30 09:16:30.000000 openqaoa-core-0.1.3rc1/openqaoa_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:16:30.000000 openqaoa-core-0.1.3rc1/openqaoa_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-30 09:16:30.000000 openqaoa-core-0.1.3rc1/openqaoa_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 09:16:30.000000 openqaoa-core-0.1.3rc1/openqaoa_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:16:30.936320 openqaoa-core-0.1.3rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:16:30.936320 openqaoa-core-0.1.3rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_analytical_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    25650 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_bin_packing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_custom_mixer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_derivative.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)    13376 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_gate_applicators_vectorized.py
--rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_knapsack.py
--rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_maximum_cut.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_minimum_vertex_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_mis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_number_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    47708 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19308 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_optimizers_pennylane.py
--rw-r--r--   0 runner    (1001) docker     (123)    30215 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_parameters_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_portfolio_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_qubo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_result_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    31783 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    21036 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_rqaoa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_sample_from_wavefunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_shortest_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_simulators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_tsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    50252 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    27539 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_vectorized.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_vrp.py
--rw-r--r--   0 runner    (1001) docker     (123)    63781 2023-06-30 09:15:43.000000 openqaoa-core-0.1.3rc1/tests/test_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.534081 openqaoa-core-0.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-06 05:58:22.534081 openqaoa-core-0.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.514081 openqaoa-core-0.2.0rc1/openqaoa/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.518081 openqaoa-core-0.2.0rc1/openqaoa/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30166 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/algorithms/baseworkflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.518081 openqaoa-core-0.2.0rc1/openqaoa/algorithms/qaoa/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/algorithms/qaoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28187 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/algorithms/qaoa/qaoa_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28182 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/algorithms/qaoa/qaoa_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20846 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/algorithms/qaoa/qaoa_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.518081 openqaoa-core-0.2.0rc1/openqaoa/algorithms/rqaoa/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/algorithms/rqaoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/algorithms/rqaoa/rqaoa_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/algorithms/rqaoa/rqaoa_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/algorithms/rqaoa/rqaoa_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/algorithms/rqaoa/rqaoa_workflow_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/algorithms/workflow_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.518081 openqaoa-core-0.2.0rc1/openqaoa/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/backends/basebackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/backends/basedevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/backends/cost_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/backends/devices_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/backends/gates_vectorized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/backends/plugin_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/backends/qaoa_analytical_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/backends/qaoa_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/backends/qaoa_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30340 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/backends/qaoa_vectorized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/backends/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.518081 openqaoa-core-0.2.0rc1/openqaoa/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/derivatives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33483 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/derivatives/derivative_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/derivatives/qfim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.518081 openqaoa-core-0.2.0rc1/openqaoa/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/logger_vqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.522081 openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/CANS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/SPSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/grad_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/iCANS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/natural_grad_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/newton_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/stochastic_grad_descent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.522081 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.522081 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/fourier/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/fourier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31659 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/fourier/reconstruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.522081 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14426 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/math/is_independent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/math/matrix_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30070 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/math/multi_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/math/quantum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/math/single_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/math/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.522081 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/numpy/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/numpy/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/numpy/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/optimization_methods_pennylane.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.522081 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/gradient_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/nesterov_momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/rms_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32442 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/rotosolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/spsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/qaoa_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32425 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/optimizers/training_vqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.526081 openqaoa-core-0.2.0rc1/openqaoa/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/problems/binpacking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/problems/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/problems/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/problems/knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/problems/maximalindependentset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/problems/maximumcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/problems/minimumvertexcover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/problems/numberpartition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/problems/portfoliooptimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/problems/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/problems/qubo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/problems/shortestpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13680 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/problems/tsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/problems/vehiclerouting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.526081 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.526081 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/ansatz_constructor/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/ansatz_constructor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/ansatz_constructor/baseparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/ansatz_constructor/gatemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/ansatz_constructor/gatemaplabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/ansatz_constructor/gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/ansatz_constructor/hamiltonianmapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21325 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/ansatz_constructor/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/ansatz_constructor/rotationangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.526081 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/annealingparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/extendedparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27328 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/fourierparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12468 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/standardparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/variational_baseparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/variational_params_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/variational_params_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63680 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/openqaoa/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.530081 openqaoa-core-0.2.0rc1/openqaoa_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-06 05:58:22.000000 openqaoa-core-0.2.0rc1/openqaoa_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-06 05:58:22.000000 openqaoa-core-0.2.0rc1/openqaoa_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 05:58:22.000000 openqaoa-core-0.2.0rc1/openqaoa_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-06 05:58:22.000000 openqaoa-core-0.2.0rc1/openqaoa_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 05:58:22.000000 openqaoa-core-0.2.0rc1/openqaoa_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 05:58:22.534081 openqaoa-core-0.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:58:22.534081 openqaoa-core-0.2.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_analytical_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25650 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_bin_packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_custom_mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13376 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_gate_applicators_vectorized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_maximum_cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_minimum_vertex_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_mis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_number_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47708 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19308 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_optimizers_pennylane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30215 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_parameters_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_portfolio_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_qubo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_result_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31783 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21036 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_rqaoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_sample_from_wavefunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_shortest_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_simulators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_tsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50252 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27539 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_vectorized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_vrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63781 2023-07-06 05:57:36.000000 openqaoa-core-0.2.0rc1/tests/test_workflows.py
```

### Comparing `openqaoa-core-0.1.3rc1/LICENSE` & `openqaoa-core-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/PKG-INFO` & `openqaoa-core-0.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openqaoa-core
-Version: 0.1.3rc1
+Version: 0.2.0rc1
 Summary: OpenQAOA is a python open-source multi-backend Software Development Kit to create, customise and execute the Quantum Approximate Optimisation Algorithm (QAOA) on Noisy Intermediate-Scale Quantum (NISQ) devices, and simulators
 Home-page: https://github.com/entropicalabs/openqaoa
 Author: Entropica Labs
 License: MIT
 Keywords: quantum optimisation SDK
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `openqaoa-core-0.1.3rc1/README.md` & `openqaoa-core-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/algorithms/baseworkflow.py` & `openqaoa-core-0.2.0rc1/openqaoa/algorithms/baseworkflow.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/algorithms/qaoa/qaoa_benchmark.py` & `openqaoa-core-0.2.0rc1/openqaoa/algorithms/qaoa/qaoa_benchmark.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/algorithms/qaoa/qaoa_result.py` & `openqaoa-core-0.2.0rc1/openqaoa/algorithms/qaoa/qaoa_result.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/algorithms/qaoa/qaoa_workflow.py` & `openqaoa-core-0.2.0rc1/openqaoa/algorithms/qaoa/qaoa_workflow.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/algorithms/rqaoa/rqaoa_result.py` & `openqaoa-core-0.2.0rc1/openqaoa/algorithms/rqaoa/rqaoa_result.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/algorithms/rqaoa/rqaoa_utils.py` & `openqaoa-core-0.2.0rc1/openqaoa/algorithms/rqaoa/rqaoa_utils.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/algorithms/rqaoa/rqaoa_workflow.py` & `openqaoa-core-0.2.0rc1/openqaoa/algorithms/rqaoa/rqaoa_workflow.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/algorithms/rqaoa/rqaoa_workflow_properties.py` & `openqaoa-core-0.2.0rc1/openqaoa/algorithms/rqaoa/rqaoa_workflow_properties.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/algorithms/workflow_properties.py` & `openqaoa-core-0.2.0rc1/openqaoa/algorithms/workflow_properties.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/backends/basebackend.py` & `openqaoa-core-0.2.0rc1/openqaoa/backends/basebackend.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/backends/basedevice.py` & `openqaoa-core-0.2.0rc1/openqaoa/backends/basedevice.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/backends/cost_function.py` & `openqaoa-core-0.2.0rc1/openqaoa/backends/cost_function.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/backends/devices_core.py` & `openqaoa-core-0.2.0rc1/openqaoa/backends/devices_core.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/backends/gates_vectorized.py` & `openqaoa-core-0.2.0rc1/openqaoa/backends/gates_vectorized.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/backends/plugin_finder.py` & `openqaoa-core-0.2.0rc1/openqaoa/backends/plugin_finder.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/backends/qaoa_analytical_sim.py` & `openqaoa-core-0.2.0rc1/openqaoa/backends/qaoa_analytical_sim.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/backends/qaoa_backend.py` & `openqaoa-core-0.2.0rc1/openqaoa/backends/qaoa_backend.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/backends/qaoa_device.py` & `openqaoa-core-0.2.0rc1/openqaoa/backends/qaoa_device.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/backends/qaoa_vectorized.py` & `openqaoa-core-0.2.0rc1/openqaoa/backends/qaoa_vectorized.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/backends/wrapper.py` & `openqaoa-core-0.2.0rc1/openqaoa/backends/wrapper.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/derivatives/derivative_functions.py` & `openqaoa-core-0.2.0rc1/openqaoa/derivatives/derivative_functions.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/derivatives/qfim.py` & `openqaoa-core-0.2.0rc1/openqaoa/derivatives/qfim.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/logger_vqa.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/logger_vqa.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/CANS.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/CANS.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/SPSA.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/SPSA.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/grad_descent.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/grad_descent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/iCANS.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/iCANS.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/natural_grad_descent.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/natural_grad_descent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/newton_descent.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/newton_descent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/rmsprop.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/rmsprop.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/optimization_methods/stochastic_grad_descent.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/optimization_methods/stochastic_grad_descent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/__init__.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/fourier/__init__.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/fourier/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/fourier/reconstruct.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/fourier/reconstruct.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/math/__init__.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/math/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/math/is_independent.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/math/is_independent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/math/matrix_manipulation.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/math/matrix_manipulation.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/math/multi_dispatch.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/math/multi_dispatch.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/math/quantum.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/math/quantum.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/math/single_dispatch.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/math/single_dispatch.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/math/utils.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/math/utils.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/numpy/__init__.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/numpy/fft.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/numpy/fft.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/numpy/linalg.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/numpy/random.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/numpy/random.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/numpy/tensor.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/numpy/tensor.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/numpy/wrapper.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/numpy/wrapper.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/optimization_methods_pennylane.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/optimization_methods_pennylane.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/__init__.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/adagrad.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/adam.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/gradient_descent.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/momentum.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/momentum.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/nesterov_momentum.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/nesterov_momentum.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/rms_prop.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/rms_prop.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/rotosolve.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/rotosolve.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/spsa.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/pennylane/pennylane_optimizers/spsa.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/qaoa_optimizer.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/qaoa_optimizer.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/optimizers/training_vqa.py` & `openqaoa-core-0.2.0rc1/openqaoa/optimizers/training_vqa.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/problems/binpacking.py` & `openqaoa-core-0.2.0rc1/openqaoa/problems/binpacking.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/problems/converters.py` & `openqaoa-core-0.2.0rc1/openqaoa/problems/converters.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/problems/helper_functions.py` & `openqaoa-core-0.2.0rc1/openqaoa/problems/helper_functions.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/problems/knapsack.py` & `openqaoa-core-0.2.0rc1/openqaoa/problems/knapsack.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/problems/maximalindependentset.py` & `openqaoa-core-0.2.0rc1/openqaoa/problems/maximalindependentset.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/problems/maximumcut.py` & `openqaoa-core-0.2.0rc1/openqaoa/problems/maximumcut.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/problems/minimumvertexcover.py` & `openqaoa-core-0.2.0rc1/openqaoa/problems/minimumvertexcover.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/problems/numberpartition.py` & `openqaoa-core-0.2.0rc1/openqaoa/problems/numberpartition.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/problems/portfoliooptimization.py` & `openqaoa-core-0.2.0rc1/openqaoa/problems/portfoliooptimization.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/problems/problem.py` & `openqaoa-core-0.2.0rc1/openqaoa/problems/problem.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/problems/qubo.py` & `openqaoa-core-0.2.0rc1/openqaoa/problems/qubo.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/problems/shortestpath.py` & `openqaoa-core-0.2.0rc1/openqaoa/problems/shortestpath.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/problems/tsp.py` & `openqaoa-core-0.2.0rc1/openqaoa/problems/tsp.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/problems/vehiclerouting.py` & `openqaoa-core-0.2.0rc1/openqaoa/problems/vehiclerouting.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/ansatz_constructor/baseparams.py` & `openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/ansatz_constructor/baseparams.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/ansatz_constructor/gatemap.py` & `openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/ansatz_constructor/gatemap.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/ansatz_constructor/gatemaplabel.py` & `openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/ansatz_constructor/gatemaplabel.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/ansatz_constructor/gates.py` & `openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/ansatz_constructor/gates.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/ansatz_constructor/hamiltonianmapper.py` & `openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/ansatz_constructor/hamiltonianmapper.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/ansatz_constructor/operators.py` & `openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/ansatz_constructor/operators.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/ansatz_constructor/rotationangle.py` & `openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/ansatz_constructor/rotationangle.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/__init__.py` & `openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/annealingparams.py` & `openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/annealingparams.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/extendedparams.py` & `openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/extendedparams.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/fourierparams.py` & `openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/fourierparams.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/standardparams.py` & `openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/standardparams.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/variational_baseparams.py` & `openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/variational_baseparams.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/variational_params_converters.py` & `openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/variational_params_converters.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/qaoa_components/variational_parameters/variational_params_factory.py` & `openqaoa-core-0.2.0rc1/openqaoa/qaoa_components/variational_parameters/variational_params_factory.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa/utilities.py` & `openqaoa-core-0.2.0rc1/openqaoa/utilities.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa_core.egg-info/PKG-INFO` & `openqaoa-core-0.2.0rc1/openqaoa_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openqaoa-core
-Version: 0.1.3rc1
+Version: 0.2.0rc1
 Summary: OpenQAOA is a python open-source multi-backend Software Development Kit to create, customise and execute the Quantum Approximate Optimisation Algorithm (QAOA) on Noisy Intermediate-Scale Quantum (NISQ) devices, and simulators
 Home-page: https://github.com/entropicalabs/openqaoa
 Author: Entropica Labs
 License: MIT
 Keywords: quantum optimisation SDK
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `openqaoa-core-0.1.3rc1/openqaoa_core.egg-info/SOURCES.txt` & `openqaoa-core-0.2.0rc1/openqaoa_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/openqaoa_core.egg-info/requires.txt` & `openqaoa-core-0.2.0rc1/openqaoa_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/setup.py` & `openqaoa-core-0.2.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_analytical_simulator.py` & `openqaoa-core-0.2.0rc1/tests/test_analytical_simulator.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_backends.py` & `openqaoa-core-0.2.0rc1/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_benchmark.py` & `openqaoa-core-0.2.0rc1/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_bin_packing.py` & `openqaoa-core-0.2.0rc1/tests/test_bin_packing.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_converters.py` & `openqaoa-core-0.2.0rc1/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_custom_mixer.py` & `openqaoa-core-0.2.0rc1/tests/test_custom_mixer.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_derivative.py` & `openqaoa-core-0.2.0rc1/tests/test_derivative.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_devices.py` & `openqaoa-core-0.2.0rc1/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_gate_applicators_vectorized.py` & `openqaoa-core-0.2.0rc1/tests/test_gate_applicators_vectorized.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_knapsack.py` & `openqaoa-core-0.2.0rc1/tests/test_knapsack.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_logger.py` & `openqaoa-core-0.2.0rc1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_maximum_cut.py` & `openqaoa-core-0.2.0rc1/tests/test_maximum_cut.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_minimum_vertex_cover.py` & `openqaoa-core-0.2.0rc1/tests/test_minimum_vertex_cover.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_mis.py` & `openqaoa-core-0.2.0rc1/tests/test_mis.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_number_partition.py` & `openqaoa-core-0.2.0rc1/tests/test_number_partition.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_operators.py` & `openqaoa-core-0.2.0rc1/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_optimizers.py` & `openqaoa-core-0.2.0rc1/tests/test_optimizers.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_optimizers_pennylane.py` & `openqaoa-core-0.2.0rc1/tests/test_optimizers_pennylane.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_parameters.py` & `openqaoa-core-0.2.0rc1/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_parameters_plots.py` & `openqaoa-core-0.2.0rc1/tests/test_parameters_plots.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_portfolio_optimization.py` & `openqaoa-core-0.2.0rc1/tests/test_portfolio_optimization.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_qubo.py` & `openqaoa-core-0.2.0rc1/tests/test_qubo.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_result_object.py` & `openqaoa-core-0.2.0rc1/tests/test_result_object.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_results.py` & `openqaoa-core-0.2.0rc1/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_rqaoa.py` & `openqaoa-core-0.2.0rc1/tests/test_rqaoa.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_sample_from_wavefunction.py` & `openqaoa-core-0.2.0rc1/tests/test_sample_from_wavefunction.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_shortest_path.py` & `openqaoa-core-0.2.0rc1/tests/test_shortest_path.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_simulators.py` & `openqaoa-core-0.2.0rc1/tests/test_simulators.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_tsp.py` & `openqaoa-core-0.2.0rc1/tests/test_tsp.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_utilities.py` & `openqaoa-core-0.2.0rc1/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_vectorized.py` & `openqaoa-core-0.2.0rc1/tests/test_vectorized.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_vrp.py` & `openqaoa-core-0.2.0rc1/tests/test_vrp.py`

 * *Files identical despite different names*

### Comparing `openqaoa-core-0.1.3rc1/tests/test_workflows.py` & `openqaoa-core-0.2.0rc1/tests/test_workflows.py`

 * *Files identical despite different names*

