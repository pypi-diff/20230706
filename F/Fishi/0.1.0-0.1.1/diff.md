# Comparing `tmp/fishi-0.1.0.tar.gz` & `tmp/fishi-0.1.1.tar.gz`

## Comparing `fishi-0.1.0.tar` & `fishi-0.1.1.tar`

### file list

```diff
@@ -1,86 +1,87 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fishi-0.1.0/.git
--rw-r--r--   0        0        0    46344 2020-02-02 00:00:00.000000 fishi-0.1.0/SpatSysBio-Python-Package-Find-Name.odt
--rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 fishi-0.1.0/SpatSysBio-Python-Package-Find-Name.pdf
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 fishi-0.1.0/requirements.txt
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fishi-0.1.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 fishi-0.1.0/.github/workflows/linting.yml
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fishi-0.1.0/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 fishi-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/database/__init__.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/database/json.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/database/mongodb.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/model/__init__.py
--rw-r--r--   0        0        0    20795 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/model/fisher_model.py
--rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/model/preprocessing.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/optimization/__init__.py
--rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/optimization/caller.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/optimization/display.py
--rw-r--r--   0        0        0    10075 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/optimization/penalty.py
--rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/optimization/scipy_global_optim.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/plotting/__init__.py
--rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/plotting/plotting.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/solving/__init__.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/solving/criteria.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/solving/display.py
--rw-r--r--   0        0        0    13828 2020-02-02 00:00:00.000000 fishi-0.1.0/Fishi/solving/solve_fsm.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/create_plots.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/make.bat
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/requirements-doc.txt
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/contributing.rst
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/index.rst
--rw-r--r--   0        0        0    30293 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/references.bib
--rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/_static/damped_osci_plots/output_example.txt
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/documentation/database.rst
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/documentation/index.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/documentation/model.rst
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/documentation/optimization.rst
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/documentation/plot_penalty_functions.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/documentation/plotting.rst
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/documentation/solving.rst
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/getting_started/index.rst
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/getting_started/installation.rst
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/getting_started/examples/baranyi_roberts.rst
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/getting_started/examples/damped_oscillator.rst
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/getting_started/examples/index.rst
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/getting_started/examples/pool_model.rst
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/theoretical_overview/index.rst
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/theoretical_overview/theoretical_background/experimental_design.rst
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/theoretical_overview/theoretical_background/index.rst
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/theoretical_overview/theoretical_background/model_formulation.rst
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/theoretical_overview/theoretical_background/optimization.rst
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 fishi-0.1.0/docs/source/theoretical_overview/theoretical_background/sensitivity_calculation.rst
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 fishi-0.1.0/examples/baranyi_roberts.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 fishi-0.1.0/examples/damped_oscillator.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 fishi-0.1.0/examples/limited_growth.py
--rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 fishi-0.1.0/examples/pool_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fishi-0.1.0/test/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fishi-0.1.0/test/database/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 fishi-0.1.0/test/database/test_json.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fishi-0.1.0/test/model/__init__.py
--rw-r--r--   0        0        0    10206 2020-02-02 00:00:00.000000 fishi-0.1.0/test/model/test_fisher_model.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 fishi-0.1.0/test/model/test_preprocessing.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fishi-0.1.0/test/optimization/__init__.py
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 fishi-0.1.0/test/optimization/test_caller.py
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 fishi-0.1.0/test/optimization/test_penalty.py
--rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 fishi-0.1.0/test/optimization/test_scipy_global_optim.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 fishi-0.1.0/test/setUp/__init__.py
--rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 fishi-0.1.0/test/setUp/extended_baranyi.py
--rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 fishi-0.1.0/test/setUp/fisher_model.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 fishi-0.1.0/test/setUp/pool_model.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fishi-0.1.0/test/solving/__init__.py
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 fishi-0.1.0/test/solving/test_convergence.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 fishi-0.1.0/test/solving/test_covariance.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 fishi-0.1.0/test/solving/test_criterion.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 fishi-0.1.0/test/solving/test_observable_generation.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 fishi-0.1.0/test/solving/test_solver.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fishi-0.1.0/tools/analyze_docker.py
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 fishi-0.1.0/tools/symbolic_diff.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 fishi-0.1.0/tools/tools.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fishi-0.1.0/.gitignore
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 fishi-0.1.0/LICENSE
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 fishi-0.1.0/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 fishi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 fishi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fishi-0.1.1/.git
+-rw-r--r--   0        0        0    46344 2020-02-02 00:00:00.000000 fishi-0.1.1/SpatSysBio-Python-Package-Find-Name.odt
+-rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 fishi-0.1.1/SpatSysBio-Python-Package-Find-Name.pdf
+-rwxr-xr-x   0        0        0      213 2020-02-02 00:00:00.000000 fishi-0.1.1/release.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fishi-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fishi-0.1.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 fishi-0.1.1/.github/workflows/linting.yml
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fishi-0.1.1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 fishi-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/database/__init__.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/database/json.py
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/database/mongodb.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/model/__init__.py
+-rw-r--r--   0        0        0    20795 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/model/fisher_model.py
+-rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/model/preprocessing.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/optimization/__init__.py
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/optimization/caller.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/optimization/display.py
+-rw-r--r--   0        0        0    10075 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/optimization/penalty.py
+-rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/optimization/scipy_global_optim.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/plotting/__init__.py
+-rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/plotting/plotting.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/solving/__init__.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/solving/criteria.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/solving/display.py
+-rw-r--r--   0        0        0    13828 2020-02-02 00:00:00.000000 fishi-0.1.1/Fishi/solving/solve_fsm.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/create_plots.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/requirements-doc.txt
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/contributing.rst
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/index.rst
+-rw-r--r--   0        0        0    30293 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/references.bib
+-rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/_static/damped_osci_plots/output_example.txt
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/documentation/database.rst
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/documentation/index.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/documentation/model.rst
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/documentation/optimization.rst
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/documentation/plot_penalty_functions.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/documentation/plotting.rst
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/documentation/solving.rst
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/getting_started/index.rst
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/getting_started/installation.rst
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/getting_started/examples/baranyi_roberts.rst
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/getting_started/examples/damped_oscillator.rst
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/getting_started/examples/index.rst
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/getting_started/examples/pool_model.rst
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/theoretical_overview/index.rst
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/theoretical_overview/theoretical_background/experimental_design.rst
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/theoretical_overview/theoretical_background/index.rst
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/theoretical_overview/theoretical_background/model_formulation.rst
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/theoretical_overview/theoretical_background/optimization.rst
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 fishi-0.1.1/docs/source/theoretical_overview/theoretical_background/sensitivity_calculation.rst
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 fishi-0.1.1/examples/baranyi_roberts.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 fishi-0.1.1/examples/damped_oscillator.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 fishi-0.1.1/examples/limited_growth.py
+-rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 fishi-0.1.1/examples/pool_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fishi-0.1.1/test/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fishi-0.1.1/test/database/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 fishi-0.1.1/test/database/test_json.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fishi-0.1.1/test/model/__init__.py
+-rw-r--r--   0        0        0    10206 2020-02-02 00:00:00.000000 fishi-0.1.1/test/model/test_fisher_model.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 fishi-0.1.1/test/model/test_preprocessing.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fishi-0.1.1/test/optimization/__init__.py
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 fishi-0.1.1/test/optimization/test_caller.py
+-rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 fishi-0.1.1/test/optimization/test_penalty.py
+-rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 fishi-0.1.1/test/optimization/test_scipy_global_optim.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 fishi-0.1.1/test/setUp/__init__.py
+-rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 fishi-0.1.1/test/setUp/extended_baranyi.py
+-rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 fishi-0.1.1/test/setUp/fisher_model.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 fishi-0.1.1/test/setUp/pool_model.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fishi-0.1.1/test/solving/__init__.py
+-rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 fishi-0.1.1/test/solving/test_convergence.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 fishi-0.1.1/test/solving/test_covariance.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 fishi-0.1.1/test/solving/test_criterion.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 fishi-0.1.1/test/solving/test_observable_generation.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 fishi-0.1.1/test/solving/test_solver.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fishi-0.1.1/tools/analyze_docker.py
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 fishi-0.1.1/tools/symbolic_diff.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 fishi-0.1.1/tools/tools.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fishi-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 fishi-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 fishi-0.1.1/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 fishi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 fishi-0.1.1/PKG-INFO
```

### Comparing `fishi-0.1.0/SpatSysBio-Python-Package-Find-Name.odt` & `fishi-0.1.1/SpatSysBio-Python-Package-Find-Name.odt`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/SpatSysBio-Python-Package-Find-Name.pdf` & `fishi-0.1.1/SpatSysBio-Python-Package-Find-Name.pdf`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/.github/workflows/build.yml` & `fishi-0.1.1/.github/workflows/build.yml`

 * *Files 0% similar despite different names*

```diff
@@ -20,13 +20,13 @@
           python -m pip install --upgrade pip build hatch
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
       - name: Build package
         run:
           python -m build
       - name: Install package
         run:
-          pip install dist/Fishi*.tar.gz
+          pip install dist/fishi*.tar.gz
       - name: Yield the package
         uses: actions/upload-artifact@v3
         with:
           name: Fishi
-          path: dist/Fishi*.tar.gz
+          path: dist/fishi*.tar.gz
```

### Comparing `fishi-0.1.0/.github/workflows/linting.yml` & `fishi-0.1.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/.github/workflows/sphinx.yml` & `fishi-0.1.1/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/.github/workflows/test.yml` & `fishi-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/Fishi/database/json.py` & `fishi-0.1.1/Fishi/database/json.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/Fishi/database/mongodb.py` & `fishi-0.1.1/Fishi/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/Fishi/model/fisher_model.py` & `fishi-0.1.1/Fishi/model/fisher_model.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/Fishi/model/preprocessing.py` & `fishi-0.1.1/Fishi/model/preprocessing.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/Fishi/optimization/caller.py` & `fishi-0.1.1/Fishi/optimization/caller.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/Fishi/optimization/display.py` & `fishi-0.1.1/Fishi/optimization/display.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/Fishi/optimization/penalty.py` & `fishi-0.1.1/Fishi/optimization/penalty.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/Fishi/optimization/scipy_global_optim.py` & `fishi-0.1.1/Fishi/optimization/scipy_global_optim.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/Fishi/plotting/plotting.py` & `fishi-0.1.1/Fishi/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/Fishi/solving/criteria.py` & `fishi-0.1.1/Fishi/solving/criteria.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/Fishi/solving/display.py` & `fishi-0.1.1/Fishi/solving/display.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/Fishi/solving/solve_fsm.py` & `fishi-0.1.1/Fishi/solving/solve_fsm.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/Makefile` & `fishi-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/make.bat` & `fishi-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/source/conf.py` & `fishi-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/source/index.rst` & `fishi-0.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/source/references.bib` & `fishi-0.1.1/docs/source/references.bib`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/source/_static/damped_osci_plots/output_example.txt` & `fishi-0.1.1/docs/source/_static/damped_osci_plots/output_example.txt`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/source/documentation/index.rst` & `fishi-0.1.1/docs/source/documentation/index.rst`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/source/documentation/optimization.rst` & `fishi-0.1.1/docs/source/documentation/optimization.rst`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/source/documentation/plot_penalty_functions.py` & `fishi-0.1.1/docs/source/documentation/plot_penalty_functions.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/source/getting_started/installation.rst` & `fishi-0.1.1/docs/source/getting_started/installation.rst`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/source/getting_started/examples/baranyi_roberts.rst` & `fishi-0.1.1/docs/source/getting_started/examples/baranyi_roberts.rst`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/source/getting_started/examples/damped_oscillator.rst` & `fishi-0.1.1/docs/source/getting_started/examples/damped_oscillator.rst`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/source/theoretical_overview/index.rst` & `fishi-0.1.1/docs/source/theoretical_overview/index.rst`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/source/theoretical_overview/theoretical_background/experimental_design.rst` & `fishi-0.1.1/docs/source/theoretical_overview/theoretical_background/experimental_design.rst`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/source/theoretical_overview/theoretical_background/model_formulation.rst` & `fishi-0.1.1/docs/source/theoretical_overview/theoretical_background/model_formulation.rst`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/source/theoretical_overview/theoretical_background/optimization.rst` & `fishi-0.1.1/docs/source/theoretical_overview/theoretical_background/optimization.rst`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/docs/source/theoretical_overview/theoretical_background/sensitivity_calculation.rst` & `fishi-0.1.1/docs/source/theoretical_overview/theoretical_background/sensitivity_calculation.rst`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/examples/baranyi_roberts.py` & `fishi-0.1.1/examples/baranyi_roberts.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/examples/damped_oscillator.py` & `fishi-0.1.1/examples/damped_oscillator.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/examples/limited_growth.py` & `fishi-0.1.1/examples/limited_growth.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/examples/pool_model.py` & `fishi-0.1.1/examples/pool_model.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/test/database/test_json.py` & `fishi-0.1.1/test/database/test_json.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/test/model/test_fisher_model.py` & `fishi-0.1.1/test/model/test_fisher_model.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/test/model/test_preprocessing.py` & `fishi-0.1.1/test/model/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/test/optimization/test_caller.py` & `fishi-0.1.1/test/optimization/test_caller.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/test/optimization/test_penalty.py` & `fishi-0.1.1/test/optimization/test_penalty.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/test/optimization/test_scipy_global_optim.py` & `fishi-0.1.1/test/optimization/test_scipy_global_optim.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/test/setUp/extended_baranyi.py` & `fishi-0.1.1/test/setUp/extended_baranyi.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/test/setUp/fisher_model.py` & `fishi-0.1.1/test/setUp/fisher_model.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/test/setUp/pool_model.py` & `fishi-0.1.1/test/setUp/pool_model.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/test/solving/test_convergence.py` & `fishi-0.1.1/test/solving/test_convergence.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/test/solving/test_covariance.py` & `fishi-0.1.1/test/solving/test_covariance.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/test/solving/test_criterion.py` & `fishi-0.1.1/test/solving/test_criterion.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/test/solving/test_observable_generation.py` & `fishi-0.1.1/test/solving/test_observable_generation.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/test/solving/test_solver.py` & `fishi-0.1.1/test/solving/test_solver.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/tools/symbolic_diff.py` & `fishi-0.1.1/tools/symbolic_diff.py`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/tools/tools.md` & `fishi-0.1.1/tools/tools.md`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/LICENSE` & `fishi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/README.md` & `fishi-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fishi-0.1.0/pyproject.toml` & `fishi-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Fishi"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Jonas Pleyer", email="jonas.pleyer@fdm.uni-freiburg.de" },
   { name="Polina Gaindrik", email="p.gaindrik@tsenso.com" },
 ]
 dependencies = [
   "matplotlib",
   "numpy",
```

### Comparing `fishi-0.1.0/PKG-INFO` & `fishi-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fishi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Optimal experimental design utilizing the Fischer information matrix
 Project-URL: Home-page, https://github.com/Spatial-Systems-Biology-Freiburg/Model-Design-Fischer-Information-Matrix
 Project-URL: Bug Tracker, https://github.com/Spatial-Systems-Biology-Freiburg/Model-Design-Fischer-Information-Matrix/issues
 Project-URL: Documentation, https://spatial-systems-biology-freiburg.github.io/Fishi/
 Project-URL: Source code, https://github.com/Spatial-Systems-Biology-Freiburg/Fishi
 Author-email: Jonas Pleyer <jonas.pleyer@fdm.uni-freiburg.de>, Polina Gaindrik <p.gaindrik@tsenso.com>
 License-File: LICENSE
```

