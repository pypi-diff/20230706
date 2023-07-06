# Comparing `tmp/parmoo-0.2.2.tar.gz` & `tmp/parmoo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parmoo-0.2.2.tar", last modified: Tue Apr 25 22:38:12 2023, max compression
+gzip compressed data, was "parmoo-0.3.0.tar", last modified: Thu Jul  6 18:23:03 2023, max compression
```

## Comparing `parmoo-0.2.2.tar` & `parmoo-0.3.0.tar`

### file list

```diff
@@ -1,180 +1,186 @@
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.745400 parmoo-0.2.2/
--rw-r--r--   0 tyler      (501) staff       (20)     4222 2023-04-25 22:34:22.000000 parmoo-0.2.2/CHANGELOG.rst
--rw-r--r--   0 tyler      (501) staff       (20)     3111 2022-05-10 21:22:59.000000 parmoo-0.2.2/CONTRIBUTING.rst
--rw-r--r--   0 tyler      (501) staff       (20)     1525 2023-02-21 22:52:41.000000 parmoo-0.2.2/LICENSE
--rw-r--r--   0 tyler      (501) staff       (20)      600 2022-05-10 21:22:59.000000 parmoo-0.2.2/MANIFEST.in
--rw-r--r--   0 tyler      (501) staff       (20)     1695 2023-04-25 22:38:12.745129 parmoo-0.2.2/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)    11817 2023-04-25 22:34:22.000000 parmoo-0.2.2/README.rst
--rw-r--r--   0 tyler      (501) staff       (20)      113 2023-04-10 20:01:13.000000 parmoo-0.2.2/REQUIREMENTS
--rw-r--r--   0 tyler      (501) staff       (20)       91 2023-02-21 22:52:41.000000 parmoo-0.2.2/SUPPORT.rst
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.627248 parmoo-0.2.2/docs/
--rw-r--r--   0 tyler      (501) staff       (20)      671 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/Makefile
--rw-r--r--   0 tyler      (501) staff       (20)       45 2022-05-10 21:22:59.000000 parmoo-0.2.2/docs/REQUIREMENTS.txt
--rw-r--r--   0 tyler      (501) staff       (20)    12729 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/about.rst
--rw-r--r--   0 tyler      (501) staff       (20)      257 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/api.rst
--rw-r--r--   0 tyler      (501) staff       (20)     3586 2023-04-24 18:05:49.000000 parmoo-0.2.2/docs/conf.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.629319 parmoo-0.2.2/docs/dev-guide/
--rw-r--r--   0 tyler      (501) staff       (20)       36 2022-05-10 21:22:59.000000 parmoo-0.2.2/docs/dev-guide/contributing.rst
--rw-r--r--   0 tyler      (501) staff       (20)      162 2022-05-10 21:22:59.000000 parmoo-0.2.2/docs/dev-guide/modules.rst
--rw-r--r--   0 tyler      (501) staff       (20)       33 2022-05-10 21:22:59.000000 parmoo-0.2.2/docs/dev-guide/release-notes.rst
--rw-r--r--   0 tyler      (501) staff       (20)     1961 2023-02-21 22:52:43.000000 parmoo-0.2.2/docs/dev-guide/release-proc.rst
--rw-r--r--   0 tyler      (501) staff       (20)     2831 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/extras.rst
--rw-r--r--   0 tyler      (501) staff       (20)    30292 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/how-to-write.rst
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.642820 parmoo-0.2.2/docs/img/
--rw-r--r--   0 tyler      (501) staff       (20)   395713 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/img/algorithm-flowchart.png
--rw-r--r--   0 tyler      (501) staff       (20)   142159 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/img/des-obj-space.png
--rw-r--r--   0 tyler      (501) staff       (20)   133860 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/img/des-sim-obj-space.png
--rw-r--r--   0 tyler      (501) staff       (20)    24057 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/img/icon-ParMOO.png
--rw-r--r--   0 tyler      (501) staff       (20)     2551 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/img/icon-ParMOO.svg
--rw-r--r--   0 tyler      (501) staff       (20)    36996 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/img/icon-ParMOO_space.png
--rw-r--r--   0 tyler      (501) staff       (20)    51610 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/img/logo-ParMOO.png
--rw-r--r--   0 tyler      (501) staff       (20)     4441 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/img/logo-ParMOO.svg
--rw-r--r--   0 tyler      (501) staff       (20)    71259 2022-05-10 21:22:59.000000 parmoo-0.2.2/docs/img/logo-ParMOO_white.png
--rw-r--r--   0 tyler      (501) staff       (20)   175826 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/img/moop-uml.png
--rw-r--r--   0 tyler      (501) staff       (20)   261708 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/img/moop-uml.svg
--rw-r--r--   0 tyler      (501) staff       (20)     1705 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/img/moop.uml
--rw-r--r--   0 tyler      (501) staff       (20)  7658326 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/img/parmoo_movie.gif
--rw-r--r--   0 tyler      (501) staff       (20)     1580 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/index.rst
--rw-r--r--   0 tyler      (501) staff       (20)     4789 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/install.rst
--rw-r--r--   0 tyler      (501) staff       (20)      862 2022-05-10 21:22:59.000000 parmoo-0.2.2/docs/latex_index.rst
--rw-r--r--   0 tyler      (501) staff       (20)      799 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/make.bat
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.670338 parmoo-0.2.2/docs/modules/
--rw-r--r--   0 tyler      (501) staff       (20)     1090 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/acquisitions.rst
--rw-r--r--   0 tyler      (501) staff       (20)      366 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/class_api.rst
--rw-r--r--   0 tyler      (501) staff       (20)      795 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/constraints.rst
--rw-r--r--   0 tyler      (501) staff       (20)      211 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/dev_tools.rst
--rw-r--r--   0 tyler      (501) staff       (20)     2698 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/dtlz.rst
--rw-r--r--   0 tyler      (501) staff       (20)      493 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/libe.rst
--rw-r--r--   0 tyler      (501) staff       (20)      735 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/libraries.rst
--rw-r--r--   0 tyler      (501) staff       (20)      583 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/moop.rst
--rw-r--r--   0 tyler      (501) staff       (20)      753 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/objectives.rst
--rw-r--r--   0 tyler      (501) staff       (20)     1639 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/optimizers.rst
--rw-r--r--   0 tyler      (501) staff       (20)      853 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/searches.rst
--rw-r--r--   0 tyler      (501) staff       (20)      253 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/simulations.rst
--rw-r--r--   0 tyler      (501) staff       (20)     1098 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/structs.rst
--rw-r--r--   0 tyler      (501) staff       (20)      713 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/surrogates.rst
--rw-r--r--   0 tyler      (501) staff       (20)      338 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/util.rst
--rw-r--r--   0 tyler      (501) staff       (20)     2890 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/modules/viz.rst
--rw-r--r--   0 tyler      (501) staff       (20)    11145 2023-04-24 18:05:49.000000 parmoo-0.2.2/docs/quickstart.rst
--rw-r--r--   0 tyler      (501) staff       (20)     1390 2023-04-25 22:34:22.000000 parmoo-0.2.2/docs/refs.rst
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.672046 parmoo-0.2.2/docs/tutorials/
--rw-r--r--   0 tyler      (501) staff       (20)     4527 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/tutorials/basic-tutorials.rst
--rw-r--r--   0 tyler      (501) staff       (20)      678 2022-05-10 21:22:59.000000 parmoo-0.2.2/docs/tutorials/libe-tutorial.rst
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.684337 parmoo-0.2.2/examples/
--rw-r--r--   0 tyler      (501) staff       (20)     1010 2023-02-21 22:52:41.000000 parmoo-0.2.2/examples/Makefile
--rw-r--r--   0 tyler      (501) staff       (20)    16534 2023-04-24 18:05:49.000000 parmoo-0.2.2/examples/Pareto Front.jpeg
--rw-r--r--   0 tyler      (501) staff       (20)     1972 2022-05-10 21:22:59.000000 parmoo-0.2.2/examples/advanced_ex.out
--rw-r--r--   0 tyler      (501) staff       (20)     3765 2022-05-10 17:20:56.000000 parmoo-0.2.2/examples/advanced_ex.py
--rw-r--r--   0 tyler      (501) staff       (20)     1635 2023-02-21 22:52:41.000000 parmoo-0.2.2/examples/checkpointing.out
--rw-r--r--   0 tyler      (501) staff       (20)     2299 2022-05-10 21:22:59.000000 parmoo-0.2.2/examples/checkpointing.py
--rw-r--r--   0 tyler      (501) staff       (20)      955 2023-04-24 18:05:49.000000 parmoo-0.2.2/examples/libe_basic_ex.out
--rw-r--r--   0 tyler      (501) staff       (20)     2243 2023-02-21 22:52:41.000000 parmoo-0.2.2/examples/libe_basic_ex.py
--rw-r--r--   0 tyler      (501) staff       (20)      153 2022-07-11 19:27:11.000000 parmoo-0.2.2/examples/named_var_ex.out
--rw-r--r--   0 tyler      (501) staff       (20)     1620 2022-05-10 21:22:59.000000 parmoo-0.2.2/examples/named_var_ex.py
--rw-r--r--   0 tyler      (501) staff       (20)      108 2022-07-11 19:27:11.000000 parmoo-0.2.2/examples/precomputed_data.out
--rw-r--r--   0 tyler      (501) staff       (20)     1409 2022-06-15 17:14:45.000000 parmoo-0.2.2/examples/precomputed_data.py
--rw-r--r--   0 tyler      (501) staff       (20)     1409 2023-04-24 18:05:49.000000 parmoo-0.2.2/examples/quickstart.out
--rw-r--r--   0 tyler      (501) staff       (20)     1575 2023-02-21 22:52:41.000000 parmoo-0.2.2/examples/quickstart.py
--rw-r--r--   0 tyler      (501) staff       (20)      582 2022-07-11 19:27:11.000000 parmoo-0.2.2/examples/unnamed_var_ex.out
--rw-r--r--   0 tyler      (501) staff       (20)     2336 2022-05-10 21:22:59.000000 parmoo-0.2.2/examples/unnamed_var_ex.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.689890 parmoo-0.2.2/parmoo/
--rw-r--r--   0 tyler      (501) staff       (20)      385 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/__init__.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.693600 parmoo-0.2.2/parmoo/acquisitions/
--rw-r--r--   0 tyler      (501) staff       (20)      104 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/acquisitions/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     9122 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/acquisitions/epsilon_constraint.py
--rw-r--r--   0 tyler      (501) staff       (20)    15030 2023-04-10 18:11:54.000000 parmoo-0.2.2/parmoo/acquisitions/weighted_sum.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.695745 parmoo-0.2.2/parmoo/constraints/
--rw-r--r--   0 tyler      (501) staff       (20)       60 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/constraints/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     3448 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/constraints/const_func.py
--rw-r--r--   0 tyler      (501) staff       (20)    18473 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/constraints/const_lib.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.697137 parmoo-0.2.2/parmoo/extras/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/extras/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    36753 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/extras/libe.py
--rw-r--r--   0 tyler      (501) staff       (20)   127469 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/moop.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.700816 parmoo-0.2.2/parmoo/objectives/
--rw-r--r--   0 tyler      (501) staff       (20)       54 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/objectives/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    22933 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/objectives/dtlz.py
--rw-r--r--   0 tyler      (501) staff       (20)     3448 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/objectives/obj_func.py
--rw-r--r--   0 tyler      (501) staff       (20)    16981 2022-07-26 17:47:19.000000 parmoo-0.2.2/parmoo/objectives/obj_lib.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.704385 parmoo-0.2.2/parmoo/optimizers/
--rw-r--r--   0 tyler      (501) staff       (20)      122 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/optimizers/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    17274 2023-04-10 18:11:54.000000 parmoo-0.2.2/parmoo/optimizers/gps_search.py
--rw-r--r--   0 tyler      (501) staff       (20)    20784 2023-04-10 18:11:54.000000 parmoo-0.2.2/parmoo/optimizers/lbfgsb.py
--rw-r--r--   0 tyler      (501) staff       (20)     8330 2023-04-10 18:11:54.000000 parmoo-0.2.2/parmoo/optimizers/random_search.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.705564 parmoo-0.2.2/parmoo/searches/
--rw-r--r--   0 tyler      (501) staff       (20)       44 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/searches/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     3736 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/searches/latin_hypercube.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.708606 parmoo-0.2.2/parmoo/simulations/
--rw-r--r--   0 tyler      (501) staff       (20)       31 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/simulations/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    31184 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/simulations/dtlz.py
--rw-r--r--   0 tyler      (501) staff       (20)     1921 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/simulations/sim_func.py
--rw-r--r--   0 tyler      (501) staff       (20)     3905 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/simulations/simple.py
--rw-r--r--   0 tyler      (501) staff       (20)    16723 2023-04-10 18:11:54.000000 parmoo-0.2.2/parmoo/structs.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.710862 parmoo-0.2.2/parmoo/surrogates/
--rw-r--r--   0 tyler      (501) staff       (20)       51 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/surrogates/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    33863 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/surrogates/gaussian_proc.py
--rw-r--r--   0 tyler      (501) staff       (20)    17196 2023-03-17 16:31:56.000000 parmoo-0.2.2/parmoo/surrogates/linear_model.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.713497 parmoo-0.2.2/parmoo/tests/
--rw-r--r--   0 tyler      (501) staff       (20)      103 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/.coveragerc
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.715011 parmoo-0.2.2/parmoo/tests/.pytest_cache/
--rw-r--r--   0 tyler      (501) staff       (20)      194 2022-02-21 21:48:43.000000 parmoo-0.2.2/parmoo/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 tyler      (501) staff       (20)      295 2022-02-21 21:48:43.000000 parmoo-0.2.2/parmoo/tests/.pytest_cache/README.md
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.614036 parmoo-0.2.2/parmoo/tests/.pytest_cache/v/
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.716990 parmoo-0.2.2/parmoo/tests/.pytest_cache/v/cache/
--rw-r--r--   0 tyler      (501) staff       (20)     1948 2022-03-04 02:25:24.000000 parmoo-0.2.2/parmoo/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 tyler      (501) staff       (20)        2 2022-03-04 02:25:24.000000 parmoo-0.2.2/parmoo/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.2/parmoo/tests/__init__.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.718943 parmoo-0.2.2/parmoo/tests/libe_tests/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.2/parmoo/tests/libe_tests/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     1305 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/tests/libe_tests/libe_funcs.py
--rw-r--r--   0 tyler      (501) staff       (20)     3003 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/tests/libe_tests/test_libe_gen.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.727130 parmoo-0.2.2/parmoo/tests/regression_tests/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.2/parmoo/tests/regression_tests/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     2984 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz1_obj.py
--rw-r--r--   0 tyler      (501) staff       (20)     3032 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz1_sim.py
--rw-r--r--   0 tyler      (501) staff       (20)     2456 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz2_obj.py
--rw-r--r--   0 tyler      (501) staff       (20)     2411 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz2_sim.py
--rw-r--r--   0 tyler      (501) staff       (20)     3042 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz3_obj.py
--rw-r--r--   0 tyler      (501) staff       (20)     3391 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz3_sim.py
--rw-r--r--   0 tyler      (501) staff       (20)     1941 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz5_sim.py
--rw-r--r--   0 tyler      (501) staff       (20)     2173 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_infeasible_prob.py
--rw-r--r--   0 tyler      (501) staff       (20)     2581 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_mixed_variables.py
--rw-r--r--   0 tyler      (501) staff       (20)     2226 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_user_func.py
--rwxr-xr-x   0 tyler      (501) staff       (20)     2691 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/run-tests.sh
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.740940 parmoo-0.2.2/parmoo/tests/unit_tests/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.2/parmoo/tests/unit_tests/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     8679 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_const_lib.py
--rw-r--r--   0 tyler      (501) staff       (20)     4039 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_epsilon_constraint.py
--rw-r--r--   0 tyler      (501) staff       (20)    15426 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_gaussian_proc.py
--rw-r--r--   0 tyler      (501) staff       (20)     7513 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_gps_search.py
--rw-r--r--   0 tyler      (501) staff       (20)     1649 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_latin_hypercube.py
--rw-r--r--   0 tyler      (501) staff       (20)     8800 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_lbfgsb.py
--rw-r--r--   0 tyler      (501) staff       (20)     6545 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_libe.py
--rw-r--r--   0 tyler      (501) staff       (20)    79942 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_moop.py
--rw-r--r--   0 tyler      (501) staff       (20)    27995 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_moop_embeddings.py
--rw-r--r--   0 tyler      (501) staff       (20)    16562 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_moop_grads.py
--rw-r--r--   0 tyler      (501) staff       (20)     7035 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_obj_dtlz.py
--rw-r--r--   0 tyler      (501) staff       (20)     8378 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_obj_lib.py
--rw-r--r--   0 tyler      (501) staff       (20)     3572 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_random_search.py
--rw-r--r--   0 tyler      (501) staff       (20)     4745 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_sims_dtlz.py
--rw-r--r--   0 tyler      (501) staff       (20)     1708 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_sims_simple.py
--rw-r--r--   0 tyler      (501) staff       (20)     1093 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_structs.py
--rw-r--r--   0 tyler      (501) staff       (20)    10127 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_util.py
--rw-r--r--   0 tyler      (501) staff       (20)    24842 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_viz_without_dash.py
--rw-r--r--   0 tyler      (501) staff       (20)     7451 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_weighted_sum.py
--rw-r--r--   0 tyler      (501) staff       (20)    18801 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/util.py
--rw-r--r--   0 tyler      (501) staff       (20)       22 2023-04-25 22:34:22.000000 parmoo-0.2.2/parmoo/version.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.744480 parmoo-0.2.2/parmoo/viz/
--rw-r--r--   0 tyler      (501) staff       (20)      320 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/viz/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    35252 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/viz/dashboard.py
--rw-r--r--   0 tyler      (501) staff       (20)     6079 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/viz/graph.py
--rw-r--r--   0 tyler      (501) staff       (20)    17752 2023-04-24 17:53:17.000000 parmoo-0.2.2/parmoo/viz/plot.py
--rw-r--r--   0 tyler      (501) staff       (20)    14067 2023-04-25 22:34:22.000000 parmoo-0.2.2/parmoo/viz/utilities.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.691837 parmoo-0.2.2/parmoo.egg-info/
--rw-r--r--   0 tyler      (501) staff       (20)     1695 2023-04-25 22:38:11.000000 parmoo-0.2.2/parmoo.egg-info/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)     4530 2023-04-25 22:38:12.000000 parmoo-0.2.2/parmoo.egg-info/SOURCES.txt
--rw-r--r--   0 tyler      (501) staff       (20)        1 2023-04-25 22:38:12.000000 parmoo-0.2.2/parmoo.egg-info/dependency_links.txt
--rw-r--r--   0 tyler      (501) staff       (20)      120 2023-04-25 22:38:12.000000 parmoo-0.2.2/parmoo.egg-info/requires.txt
--rw-r--r--   0 tyler      (501) staff       (20)        7 2023-04-25 22:38:12.000000 parmoo-0.2.2/parmoo.egg-info/top_level.txt
--rw-r--r--   0 tyler      (501) staff       (20)       38 2023-04-25 22:38:12.745518 parmoo-0.2.2/setup.cfg
--rw-r--r--   0 tyler      (501) staff       (20)     3421 2023-04-24 18:05:49.000000 parmoo-0.2.2/setup.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.226065 parmoo-0.3.0/
+-rw-r--r--   0 tyler      (501) staff       (20)     7762 2023-07-06 17:43:02.000000 parmoo-0.3.0/CHANGELOG.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     3111 2022-05-10 21:22:59.000000 parmoo-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     1525 2023-02-21 22:52:41.000000 parmoo-0.3.0/LICENSE
+-rw-r--r--   0 tyler      (501) staff       (20)      600 2022-05-10 21:22:59.000000 parmoo-0.3.0/MANIFEST.in
+-rw-r--r--   0 tyler      (501) staff       (20)     1675 2023-07-06 18:23:03.225695 parmoo-0.3.0/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)    12115 2023-07-06 17:43:02.000000 parmoo-0.3.0/README.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      114 2023-07-06 17:43:02.000000 parmoo-0.3.0/REQUIREMENTS
+-rw-r--r--   0 tyler      (501) staff       (20)       91 2023-02-21 22:52:41.000000 parmoo-0.3.0/SUPPORT.rst
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.111384 parmoo-0.3.0/docs/
+-rw-r--r--   0 tyler      (501) staff       (20)      839 2023-07-06 17:43:02.000000 parmoo-0.3.0/docs/Makefile
+-rw-r--r--   0 tyler      (501) staff       (20)       45 2022-05-10 21:22:59.000000 parmoo-0.3.0/docs/REQUIREMENTS.txt
+-rw-r--r--   0 tyler      (501) staff       (20)    12729 2023-02-21 22:52:41.000000 parmoo-0.3.0/docs/about.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      257 2023-02-21 22:52:41.000000 parmoo-0.3.0/docs/api.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     3586 2023-05-01 20:29:09.000000 parmoo-0.3.0/docs/conf.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.113802 parmoo-0.3.0/docs/dev-guide/
+-rw-r--r--   0 tyler      (501) staff       (20)       36 2022-05-10 21:22:59.000000 parmoo-0.3.0/docs/dev-guide/contributing.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      162 2022-05-10 21:22:59.000000 parmoo-0.3.0/docs/dev-guide/modules.rst
+-rw-r--r--   0 tyler      (501) staff       (20)       33 2022-05-10 21:22:59.000000 parmoo-0.3.0/docs/dev-guide/release-notes.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     1982 2023-07-06 17:43:02.000000 parmoo-0.3.0/docs/dev-guide/release-proc.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     2831 2023-02-21 22:52:41.000000 parmoo-0.3.0/docs/extras.rst
+-rw-r--r--   0 tyler      (501) staff       (20)    10596 2023-07-06 17:43:02.000000 parmoo-0.3.0/docs/faqs.rst
+-rw-r--r--   0 tyler      (501) staff       (20)    30604 2023-07-06 17:43:02.000000 parmoo-0.3.0/docs/how-to-write.rst
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.127970 parmoo-0.3.0/docs/img/
+-rw-r--r--   0 tyler      (501) staff       (20)   395713 2023-02-21 22:52:41.000000 parmoo-0.3.0/docs/img/algorithm-flowchart.png
+-rw-r--r--   0 tyler      (501) staff       (20)   142159 2022-05-10 17:20:56.000000 parmoo-0.3.0/docs/img/des-obj-space.png
+-rw-r--r--   0 tyler      (501) staff       (20)   133860 2022-05-10 17:20:56.000000 parmoo-0.3.0/docs/img/des-sim-obj-space.png
+-rw-r--r--   0 tyler      (501) staff       (20)    24057 2022-05-10 17:20:56.000000 parmoo-0.3.0/docs/img/icon-ParMOO.png
+-rw-r--r--   0 tyler      (501) staff       (20)     2551 2022-05-10 17:20:56.000000 parmoo-0.3.0/docs/img/icon-ParMOO.svg
+-rw-r--r--   0 tyler      (501) staff       (20)    36996 2022-05-10 17:20:56.000000 parmoo-0.3.0/docs/img/icon-ParMOO_space.png
+-rw-r--r--   0 tyler      (501) staff       (20)    51610 2022-05-10 17:20:56.000000 parmoo-0.3.0/docs/img/logo-ParMOO.png
+-rw-r--r--   0 tyler      (501) staff       (20)     4441 2022-05-10 17:20:56.000000 parmoo-0.3.0/docs/img/logo-ParMOO.svg
+-rw-r--r--   0 tyler      (501) staff       (20)    71259 2022-05-10 21:22:59.000000 parmoo-0.3.0/docs/img/logo-ParMOO_white.png
+-rw-r--r--   0 tyler      (501) staff       (20)   175826 2023-02-21 22:52:41.000000 parmoo-0.3.0/docs/img/moop-uml.png
+-rw-r--r--   0 tyler      (501) staff       (20)   261708 2023-02-21 22:52:41.000000 parmoo-0.3.0/docs/img/moop-uml.svg
+-rw-r--r--   0 tyler      (501) staff       (20)     1705 2023-02-21 22:52:41.000000 parmoo-0.3.0/docs/img/moop.uml
+-rw-r--r--   0 tyler      (501) staff       (20)  7658326 2022-05-10 17:20:56.000000 parmoo-0.3.0/docs/img/parmoo_movie.gif
+-rw-r--r--   0 tyler      (501) staff       (20)     1614 2023-07-06 17:43:02.000000 parmoo-0.3.0/docs/index.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     4789 2023-02-21 22:52:41.000000 parmoo-0.3.0/docs/install.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      862 2022-05-10 21:22:59.000000 parmoo-0.3.0/docs/latex_index.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      799 2022-05-10 17:20:56.000000 parmoo-0.3.0/docs/make.bat
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.166427 parmoo-0.3.0/docs/modules/
+-rw-r--r--   0 tyler      (501) staff       (20)     1195 2023-07-06 17:43:02.000000 parmoo-0.3.0/docs/modules/acquisitions.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      366 2022-09-09 18:45:50.000000 parmoo-0.3.0/docs/modules/class_api.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      795 2022-09-09 18:45:50.000000 parmoo-0.3.0/docs/modules/constraints.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      211 2022-09-09 18:45:50.000000 parmoo-0.3.0/docs/modules/dev_tools.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     2698 2022-09-09 18:45:50.000000 parmoo-0.3.0/docs/modules/dtlz.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      493 2022-09-09 18:45:50.000000 parmoo-0.3.0/docs/modules/libe.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      735 2022-09-09 18:45:50.000000 parmoo-0.3.0/docs/modules/libraries.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      583 2022-09-09 18:45:50.000000 parmoo-0.3.0/docs/modules/moop.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      753 2022-09-09 18:45:50.000000 parmoo-0.3.0/docs/modules/objectives.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     1639 2022-09-09 18:45:50.000000 parmoo-0.3.0/docs/modules/optimizers.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      853 2022-09-09 18:45:50.000000 parmoo-0.3.0/docs/modules/searches.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      253 2022-09-09 18:45:50.000000 parmoo-0.3.0/docs/modules/simulations.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     1098 2022-09-09 18:45:50.000000 parmoo-0.3.0/docs/modules/structs.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      713 2022-09-09 18:45:50.000000 parmoo-0.3.0/docs/modules/surrogates.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      338 2022-09-09 18:45:50.000000 parmoo-0.3.0/docs/modules/util.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     2890 2023-02-21 22:52:41.000000 parmoo-0.3.0/docs/modules/viz.rst
+-rw-r--r--   0 tyler      (501) staff       (20)    11393 2023-07-06 17:43:02.000000 parmoo-0.3.0/docs/quickstart.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     1390 2023-07-06 17:43:02.000000 parmoo-0.3.0/docs/refs.rst
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.168750 parmoo-0.3.0/docs/tutorials/
+-rw-r--r--   0 tyler      (501) staff       (20)     4526 2023-07-06 17:43:02.000000 parmoo-0.3.0/docs/tutorials/basic-tutorials.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      678 2022-05-10 21:22:59.000000 parmoo-0.3.0/docs/tutorials/libe-tutorial.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     4323 2023-07-06 17:43:02.000000 parmoo-0.3.0/docs/tutorials/local_method.rst
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.180532 parmoo-0.3.0/examples/
+-rw-r--r--   0 tyler      (501) staff       (20)     1249 2023-07-06 17:43:02.000000 parmoo-0.3.0/examples/Makefile
+-rw-r--r--   0 tyler      (501) staff       (20)     1801 2023-07-06 17:43:02.000000 parmoo-0.3.0/examples/advanced_ex.out
+-rw-r--r--   0 tyler      (501) staff       (20)     3918 2023-07-06 17:43:02.000000 parmoo-0.3.0/examples/advanced_ex.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1139 2023-07-06 17:43:02.000000 parmoo-0.3.0/examples/checkpointing.out
+-rw-r--r--   0 tyler      (501) staff       (20)     2360 2023-07-06 17:43:02.000000 parmoo-0.3.0/examples/checkpointing.py
+-rw-r--r--   0 tyler      (501) staff       (20)      460 2023-07-06 17:43:02.000000 parmoo-0.3.0/examples/libe_basic_ex.out
+-rw-r--r--   0 tyler      (501) staff       (20)     2566 2023-07-06 17:43:02.000000 parmoo-0.3.0/examples/libe_basic_ex.py
+-rw-r--r--   0 tyler      (501) staff       (20)     9739 2023-07-06 17:43:02.000000 parmoo-0.3.0/examples/local_method.csv
+-rw-r--r--   0 tyler      (501) staff       (20)    17931 2023-07-06 17:43:02.000000 parmoo-0.3.0/examples/local_method.jpeg
+-rw-r--r--   0 tyler      (501) staff       (20)     3649 2023-07-06 17:43:02.000000 parmoo-0.3.0/examples/local_method.py
+-rw-r--r--   0 tyler      (501) staff       (20)      153 2022-07-11 19:27:11.000000 parmoo-0.3.0/examples/named_var_ex.out
+-rw-r--r--   0 tyler      (501) staff       (20)     1620 2022-05-10 21:22:59.000000 parmoo-0.3.0/examples/named_var_ex.py
+-rw-r--r--   0 tyler      (501) staff       (20)      108 2022-07-11 19:27:11.000000 parmoo-0.3.0/examples/precomputed_data.out
+-rw-r--r--   0 tyler      (501) staff       (20)     1409 2022-06-15 17:14:45.000000 parmoo-0.3.0/examples/precomputed_data.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16932 2023-07-06 17:43:02.000000 parmoo-0.3.0/examples/quickstart.jpeg
+-rw-r--r--   0 tyler      (501) staff       (20)      528 2023-07-06 17:43:02.000000 parmoo-0.3.0/examples/quickstart.out
+-rw-r--r--   0 tyler      (501) staff       (20)     1674 2023-07-06 17:43:02.000000 parmoo-0.3.0/examples/quickstart.py
+-rw-r--r--   0 tyler      (501) staff       (20)      582 2023-06-30 18:53:23.000000 parmoo-0.3.0/examples/unnamed_var_ex.out
+-rw-r--r--   0 tyler      (501) staff       (20)     2397 2023-07-06 17:43:02.000000 parmoo-0.3.0/examples/unnamed_var_ex.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.185784 parmoo-0.3.0/parmoo/
+-rw-r--r--   0 tyler      (501) staff       (20)      385 2023-04-10 20:01:13.000000 parmoo-0.3.0/parmoo/__init__.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.188965 parmoo-0.3.0/parmoo/acquisitions/
+-rw-r--r--   0 tyler      (501) staff       (20)      125 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/acquisitions/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    20927 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/acquisitions/epsilon_constraint.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16542 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/acquisitions/weighted_sum.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.190621 parmoo-0.3.0/parmoo/constraints/
+-rw-r--r--   0 tyler      (501) staff       (20)       60 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/constraints/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3448 2023-02-21 22:52:41.000000 parmoo-0.3.0/parmoo/constraints/const_func.py
+-rw-r--r--   0 tyler      (501) staff       (20)    18473 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/constraints/const_lib.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.191866 parmoo-0.3.0/parmoo/extras/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/extras/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    40493 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/extras/libe.py
+-rw-r--r--   0 tyler      (501) staff       (20)   145705 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/moop.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.194514 parmoo-0.3.0/parmoo/objectives/
+-rw-r--r--   0 tyler      (501) staff       (20)       54 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/objectives/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    22933 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/objectives/dtlz.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3448 2023-02-21 22:52:41.000000 parmoo-0.3.0/parmoo/objectives/obj_func.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16981 2023-05-15 20:54:00.000000 parmoo-0.3.0/parmoo/objectives/obj_lib.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.197017 parmoo-0.3.0/parmoo/optimizers/
+-rw-r--r--   0 tyler      (501) staff       (20)      122 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/optimizers/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    13379 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/optimizers/gps_search.py
+-rw-r--r--   0 tyler      (501) staff       (20)    13856 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/optimizers/lbfgsb.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5578 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/optimizers/random_search.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.198007 parmoo-0.3.0/parmoo/searches/
+-rw-r--r--   0 tyler      (501) staff       (20)       44 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/searches/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3736 2023-02-21 22:52:41.000000 parmoo-0.3.0/parmoo/searches/latin_hypercube.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.200654 parmoo-0.3.0/parmoo/simulations/
+-rw-r--r--   0 tyler      (501) staff       (20)       31 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/simulations/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    31519 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/simulations/dtlz.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1921 2023-02-21 22:52:41.000000 parmoo-0.3.0/parmoo/simulations/sim_func.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3905 2023-04-10 20:01:13.000000 parmoo-0.3.0/parmoo/simulations/simple.py
+-rw-r--r--   0 tyler      (501) staff       (20)    26261 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/structs.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.202497 parmoo-0.3.0/parmoo/surrogates/
+-rw-r--r--   0 tyler      (501) staff       (20)       51 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/surrogates/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    37549 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/surrogates/gaussian_proc.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17196 2023-03-17 16:31:56.000000 parmoo-0.3.0/parmoo/surrogates/linear_model.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.204318 parmoo-0.3.0/parmoo/tests/
+-rw-r--r--   0 tyler      (501) staff       (20)      103 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/tests/.coveragerc
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.205324 parmoo-0.3.0/parmoo/tests/.pytest_cache/
+-rw-r--r--   0 tyler      (501) staff       (20)      194 2022-02-21 21:48:43.000000 parmoo-0.3.0/parmoo/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 tyler      (501) staff       (20)      295 2022-02-21 21:48:43.000000 parmoo-0.3.0/parmoo/tests/.pytest_cache/README.md
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.096789 parmoo-0.3.0/parmoo/tests/.pytest_cache/v/
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.206347 parmoo-0.3.0/parmoo/tests/.pytest_cache/v/cache/
+-rw-r--r--   0 tyler      (501) staff       (20)     1948 2022-03-04 02:25:24.000000 parmoo-0.3.0/parmoo/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 tyler      (501) staff       (20)        2 2022-03-04 02:25:24.000000 parmoo-0.3.0/parmoo/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.3.0/parmoo/tests/__init__.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.207863 parmoo-0.3.0/parmoo/tests/libe_tests/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.3.0/parmoo/tests/libe_tests/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1305 2023-07-02 21:17:30.000000 parmoo-0.3.0/parmoo/tests/libe_tests/libe_funcs.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3025 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/tests/libe_tests/test_libe_gen.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.213380 parmoo-0.3.0/parmoo/tests/regression_tests/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.3.0/parmoo/tests/regression_tests/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2984 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/tests/regression_tests/test_dtlz1_obj.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3032 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/tests/regression_tests/test_dtlz1_sim.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2456 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/tests/regression_tests/test_dtlz2_obj.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2439 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/tests/regression_tests/test_dtlz2_sim.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3042 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/tests/regression_tests/test_dtlz3_obj.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3391 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/tests/regression_tests/test_dtlz3_sim.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1941 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/tests/regression_tests/test_dtlz5_sim.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2173 2023-02-21 22:52:41.000000 parmoo-0.3.0/parmoo/tests/regression_tests/test_infeasible_prob.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2581 2023-02-21 22:52:41.000000 parmoo-0.3.0/parmoo/tests/regression_tests/test_mixed_variables.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2226 2022-05-10 17:20:56.000000 parmoo-0.3.0/parmoo/tests/regression_tests/test_user_func.py
+-rwxr-xr-x   0 tyler      (501) staff       (20)     2691 2023-04-10 20:01:13.000000 parmoo-0.3.0/parmoo/tests/run-tests.sh
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.222549 parmoo-0.3.0/parmoo/tests/unit_tests/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.3.0/parmoo/tests/unit_tests/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8679 2023-04-10 20:01:13.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_const_lib.py
+-rw-r--r--   0 tyler      (501) staff       (20)     9097 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_epsilon_constraint.py
+-rw-r--r--   0 tyler      (501) staff       (20)    18280 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_gaussian_proc.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7655 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_gps_search.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1649 2023-04-10 20:01:13.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_latin_hypercube.py
+-rw-r--r--   0 tyler      (501) staff       (20)     9014 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_lbfgsb.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6745 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_libe.py
+-rw-r--r--   0 tyler      (501) staff       (20)    86338 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_moop.py
+-rw-r--r--   0 tyler      (501) staff       (20)    27995 2023-04-10 20:01:13.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_moop_embeddings.py
+-rw-r--r--   0 tyler      (501) staff       (20)    64104 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_moop_ev.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16606 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_moop_grads.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7035 2023-04-10 20:01:13.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_obj_dtlz.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8378 2023-04-10 20:01:13.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_obj_lib.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3595 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_random_search.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4745 2023-04-10 20:01:13.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_sims_dtlz.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1708 2023-04-10 20:01:13.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_sims_simple.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1093 2023-02-21 22:52:41.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_structs.py
+-rw-r--r--   0 tyler      (501) staff       (20)    10127 2023-04-10 20:01:13.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_util.py
+-rw-r--r--   0 tyler      (501) staff       (20)    24842 2023-04-10 20:01:13.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_viz_without_dash.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8479 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/tests/unit_tests/test_weighted_sum.py
+-rw-r--r--   0 tyler      (501) staff       (20)    18801 2023-04-10 20:01:13.000000 parmoo-0.3.0/parmoo/util.py
+-rw-r--r--   0 tyler      (501) staff       (20)       22 2023-07-06 17:43:02.000000 parmoo-0.3.0/parmoo/version.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.225111 parmoo-0.3.0/parmoo/viz/
+-rw-r--r--   0 tyler      (501) staff       (20)      320 2023-02-21 22:52:41.000000 parmoo-0.3.0/parmoo/viz/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    35252 2023-02-21 22:52:41.000000 parmoo-0.3.0/parmoo/viz/dashboard.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6079 2023-02-21 22:52:41.000000 parmoo-0.3.0/parmoo/viz/graph.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17752 2023-04-24 17:53:17.000000 parmoo-0.3.0/parmoo/viz/plot.py
+-rw-r--r--   0 tyler      (501) staff       (20)    14067 2023-05-01 20:29:09.000000 parmoo-0.3.0/parmoo/viz/utilities.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-07-06 18:23:03.187631 parmoo-0.3.0/parmoo.egg-info/
+-rw-r--r--   0 tyler      (501) staff       (20)     1675 2023-07-06 18:23:02.000000 parmoo-0.3.0/parmoo.egg-info/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)     4692 2023-07-06 18:23:03.000000 parmoo-0.3.0/parmoo.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        1 2023-07-06 18:23:02.000000 parmoo-0.3.0/parmoo.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler      (501) staff       (20)      127 2023-07-06 18:23:02.000000 parmoo-0.3.0/parmoo.egg-info/requires.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        7 2023-07-06 18:23:02.000000 parmoo-0.3.0/parmoo.egg-info/top_level.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       38 2023-07-06 18:23:03.226141 parmoo-0.3.0/setup.cfg
+-rw-r--r--   0 tyler      (501) staff       (20)     3428 2023-07-06 17:43:02.000000 parmoo-0.3.0/setup.py
```

### Comparing `parmoo-0.2.2/CONTRIBUTING.rst` & `parmoo-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/LICENSE` & `parmoo-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/MANIFEST.in` & `parmoo-0.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/PKG-INFO` & `parmoo-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: parmoo
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python library for parallel multiobjective simulation optimization
 Home-page: https://github.com/parmoo/parmoo
 Author: Tyler H. Chang, Stefan M. Wild, et al.
 Author-email: parmoo@mcs.anl.gov
 License: BSD 3-clause
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
@@ -37,9 +36,7 @@
 
 ParMOO also seeks to exploit structure in simulation optimization problems,
 by modeling simulations separately from surrogates.
 
 
 ParMOO is distributed under a BSD 3-clause license.
 
-
-
```

### Comparing `parmoo-0.2.2/README.rst` & `parmoo-0.3.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -210,64 +210,70 @@
 Now we can add objectives and constraints using ``MOOP.addObjective(*args)``
 and ``MOOP.addConstraint(*args)``. In this example, there are 2 objectives
 (each corresponding to a single simulation output) and one constraint.
 
 .. code-block:: python
 
    # First objective just returns the first simulation output
-   my_moop.addObjective({'name': "f1", 'obj_func': lambda x, s: s["MySim"][0]})
+   def f1(x, s): return s["MySim"][0]
+   my_moop.addObjective({'name': "f1", 'obj_func': f1})
    # Second objective just returns the second simulation output
-   my_moop.addObjective({'name': "f2", 'obj_func': lambda x, s: s["MySim"][1]})
+   def f2(x, s): return s["MySim"][1]
+   my_moop.addObjective({'name': "f2", 'obj_func': f2})
    # Add a single constraint, that x[0] >= 0.1
-   my_moop.addConstraint({'name': "c1",
-                          'constraint': lambda x, s: 0.1 - x["x1"]})
+   def c1(x, s): return 0.1 - x["x1"]
+   my_moop.addConstraint({'name': "c1", 'constraint': c1})
 
 Finally, we must add one or more acquisition functions using
 ``MOOP.addAcquisition(*args)``. These are used to scalarize the surrogate
 problems. The number of acquisition functions typically determines the
 number of simulation evaluations per batch. This is useful to know if you
 are using a parallel solver.
 
 .. code-block:: python
 
-   from parmoo.acquisitions import UniformWeights
+   from parmoo.acquisitions import RandomConstraint
 
    # Add 3 acquisition functions
    for i in range(3):
-      my_moop.addAcquisition({'acquisition': UniformWeights,
+      my_moop.addAcquisition({'acquisition': RandomConstraint,
                               'hyperparams': {}})
 
 Finally, the MOOP is solved using the ``MOOP.solve(budget)`` method, and the
 results can be viewed using ``MOOP.getPF()`` method.
 
 .. code-block:: python
 
+   import pandas as pd
+
    my_moop.solve(5) # Solve with 5 iterations of ParMOO algorithm
-   results = my_moop.getPF() # Extract the results
+   results = my_moop.getPF(format="pandas") # Extract the results as pandas df
 
 After executing the above block of code, the ``results`` variable points to
-a numpy structured array, each of whose entries corresponds to a
-nondominated objective value in the ``my_moop`` object's final database.
-You can reference individual fields in the ``results`` array by using the
+a pandas_ dataframe, each of whose rows corresponds to a nondominated
+objective value in the ``my_moop`` object's final database.
+You can reference individual columns in the ``results`` array by using the
 ``name`` keys that were assigned during ``my_moop``'s construction, or
 plot the results by using the viz_ library.
 
 Congratulations, you now know enough to get started solving MOOPs with
 ParMOO!
 
 Next steps:
 
  * Learn more about all that ParMOO has to offer (including saving and
    checkpointing, INFO-level logging, advanced problem definitions, and
    different surrogate and solver options) at our ReadTheDocs_ page.
  * Explore the advanced examples (including a ``libEnsemble`` example)
    in the ``examples`` directory.
  * Install libEnsemble_ and get started solving MOOPs in parallel.
+ * See some of our pre-built solvers in the parmoo_solver_farm_.
  * To interactively explore your solutions, install its extra dependencies and
    use our built-in viz_ tool.
+ * For more advice, consult our FAQs_.
 
 Resources
 ---------
 
 To seek support or report issues, e-mail:
 
  * ``parmoo@mcs.anl.gov``
@@ -302,29 +308,31 @@
 
 .. code-block:: bibtex
 
     @techreport{parmoo-docs,
         title       = {{ParMOO}: {P}ython library for parallel multiobjective simulation optimization},
         author      = {Chang, Tyler H. and Wild, Stefan M. and Dickinson, Hyrum},
         institution = {Argonne National Laboratory},
-        number      = {Version 0.2.2},
+        number      = {Version 0.3.0},
         year        = {2023},
         url         = {https://parmoo.readthedocs.io/en/latest}
     }
 
 .. _Actions: https://github.com/parmoo/parmoo/actions
 .. _CONTRIBUTING: https://github.com/parmoo/parmoo/blob/main/CONTRIBUTING.rst
 .. _dash: https://dash.plotly.com
+.. _FAQs: https://parmoo.readthedocs.io/en/latest/faqs.html
 .. _flake8: https://flake8.pycqa.org/en/latest
 .. _GitHub: https://github.com/parmoo/parmoo
 .. _kaleido: https://github.com/plotly/Kaleido
 .. _libEnsemble: https://github.com/Libensemble/libensemble
 .. _LICENSE: https://github.com/parmoo/parmoo/blob/main/LICENSE
 .. _numpy: https://numpy.org
 .. _pandas: https://pandas.pydata.org
+.. _parmoo_solver_farm: https://github.com/parmoo/parmoo-solver-farm
 .. _plotly: https://plotly.com/python
 .. _pyDOE: https://pythonhosted.org/pyDOE
 .. _pytest: https://docs.pytest.org/en/7.0.x
 .. _pytest-cov: https://pytest-cov.readthedocs.io/en/latest
 .. _Python: https://www.python.org/downloads
 .. _ReadTheDocs: https://parmoo.readthedocs.org
 .. _scipy: https://scipy.org
```

### Comparing `parmoo-0.2.2/docs/about.rst` & `parmoo-0.3.0/docs/about.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/conf.py` & `parmoo-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/dev-guide/release-proc.rst` & `parmoo-0.3.0/docs/dev-guide/release-proc.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 - A release branch should be taken off ``develop`` (or ``develop`` pulls
   controlled).
 
 - Release notes for this version are added to the ``CHANGELOG.rst`` file.
 
 - Version number is updated wherever it appears and ``+dev`` suffix is removed
-  (in ``parmoo/version.py`` and ``README.rst``).
+  (in ``parmoo/version.py``, ``README.rst``, and ``docs/refs.rst``).
 
 - Check ``README.rst`` *Citing ParMOO* and ``docs/refs.rst`` for correctness.
 
 - ``setup.py`` and ``parmoo/__init__.py`` are checked to ensure all
   information is up to date.
 
 - ``MANIFEST.in`` is checked. Locally, try out ``python setup.py sdist`` and
@@ -56,9 +56,10 @@
 - Create a new commit on develop that appends ``+dev`` to the version number
   (wherever it appears).
 
 After release
 -------------
 
 - Ensure all relevant GitHub issues are closed.
+
 - Check that the conda-forge package has tracked latest release
   and update dependency list if needed.
```

### Comparing `parmoo-0.2.2/docs/extras.rst` & `parmoo-0.3.0/docs/extras.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/how-to-write.rst` & `parmoo-0.3.0/docs/how-to-write.rst`

 * *Files 1% similar despite different names*

```diff
@@ -589,17 +589,17 @@
 After you have added all of the design variables, simulations, objectives,
 and constraints to your MOOP, you must add one or more acquisitions
 using the :meth:`MOOP.addAcquisition(*args) <moop.MOOP.addAcquisition>`
 method.
 
 .. code-block:: python
 
-    from parmoo.acquisitions import UniformWeights, FixedWeights
+    from parmoo.acquisitions import RandomConstraint, FixedWeights
 
-    moop.addAcquisition({'acquisition': UniformWeights})
+    moop.addAcquisition({'acquisition': RandomConstraint})
     moop.addAcquisition({'acquisition': FixedWeights,
                          'hyperparams': {'weights': np.array([0.5, 0.5])}})
 
 The acquisition dictionary may contain two keys:
  * ``acquisition`` (required) specifies one
    :mod:`AcquisitionFunction <structs.AcquisitionFunction>`
    that you would like to use for this problem; and
@@ -792,14 +792,25 @@
 After solving the MOOP, you can view the results using
 :meth:`MOOP.getPF() <moop.MOOP.getPF>`.
 
 .. code-block:: python
 
     soln = moop.getPF()
 
+The output format defaults to a numpy structured array.
+However, you can change it to a pandas dataframe using the optional
+``format`` argument.
+
+.. code-block:: python
+
+    soln = moop.getPF(format="pandas")
+
+Note that ``format="pandas"`` is only supported when working with
+:ref:`named outputs <naming>`.
+
 To get the full simulation and objective databases, you can also use
 :meth:`MOOP.getSimulationData() <moop.MOOP.getSimulationData>`
 and
 :meth:`MOOP.getObjectiveData() <moop.MOOP.getObjectiveData>`.
 
 .. code-block:: python
```

### Comparing `parmoo-0.2.2/docs/img/algorithm-flowchart.png` & `parmoo-0.3.0/docs/img/algorithm-flowchart.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/img/des-obj-space.png` & `parmoo-0.3.0/docs/img/des-obj-space.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/img/des-sim-obj-space.png` & `parmoo-0.3.0/docs/img/des-sim-obj-space.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/img/icon-ParMOO.png` & `parmoo-0.3.0/docs/img/icon-ParMOO.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/img/icon-ParMOO.svg` & `parmoo-0.3.0/docs/img/icon-ParMOO.svg`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/img/icon-ParMOO_space.png` & `parmoo-0.3.0/docs/img/icon-ParMOO_space.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/img/logo-ParMOO.png` & `parmoo-0.3.0/docs/img/logo-ParMOO.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/img/logo-ParMOO.svg` & `parmoo-0.3.0/docs/img/logo-ParMOO.svg`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/img/logo-ParMOO_white.png` & `parmoo-0.3.0/docs/img/logo-ParMOO_white.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/img/moop-uml.png` & `parmoo-0.3.0/docs/img/moop-uml.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/img/moop-uml.svg` & `parmoo-0.3.0/docs/img/moop-uml.svg`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/img/moop.uml` & `parmoo-0.3.0/docs/img/moop.uml`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/img/parmoo_movie.gif` & `parmoo-0.3.0/docs/img/parmoo_movie.gif`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/index.rst` & `parmoo-0.3.0/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -35,28 +35,30 @@
    :caption: User Guide:
 
    quickstart
    install
    about
    how-to-write
    extras
+   faqs
    refs
 
 .. toctree::
    :maxdepth: 2
    :caption: API:
 
    api
 
 .. toctree::
    :maxdepth: 2
    :caption: Tutorials:
 
    tutorials/basic-tutorials
    tutorials/libe-tutorial
+   tutorials/local_method
 
 .. toctree::
    :maxdepth: 2
    :caption: Developer Guide:
 
    dev-guide/contributing
    dev-guide/release-proc
```

### Comparing `parmoo-0.2.2/docs/install.rst` & `parmoo-0.3.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/latex_index.rst` & `parmoo-0.3.0/docs/latex_index.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/make.bat` & `parmoo-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/modules/acquisitions.rst` & `parmoo-0.3.0/docs/modules/acquisitions.rst`

 * *Files 5% similar despite different names*

```diff
@@ -43,7 +43,13 @@
 ..    :members: acquisitions/epsilon_constraint
 
 .. autoclass:: RandomConstraint
    :member-order: bysource
    :members:
 
    .. automethod:: __init__
+
+.. autoclass:: EI_RandomConstraint
+   :member-order: bysource
+   :members:
+
+   .. automethod:: __init__
```

### Comparing `parmoo-0.2.2/docs/modules/constraints.rst` & `parmoo-0.3.0/docs/modules/constraints.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/modules/dtlz.rst` & `parmoo-0.3.0/docs/modules/dtlz.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/modules/libraries.rst` & `parmoo-0.3.0/docs/modules/libraries.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/modules/moop.rst` & `parmoo-0.3.0/docs/modules/moop.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/modules/objectives.rst` & `parmoo-0.3.0/docs/modules/objectives.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/modules/optimizers.rst` & `parmoo-0.3.0/docs/modules/optimizers.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/modules/searches.rst` & `parmoo-0.3.0/docs/modules/searches.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/modules/structs.rst` & `parmoo-0.3.0/docs/modules/structs.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/modules/surrogates.rst` & `parmoo-0.3.0/docs/modules/surrogates.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/modules/viz.rst` & `parmoo-0.3.0/docs/modules/viz.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/docs/quickstart.rst` & `parmoo-0.3.0/docs/quickstart.rst`

 * *Files 4% similar despite different names*

```diff
@@ -201,51 +201,55 @@
 :meth:`MOOP.addConstraint(*args) <moop.MOOP.addConstraint>`.
 In this example, there are 2 objectives (each corresponding to a single
 simulation output) and one constraint.
 
 .. code-block:: python
 
    # First objective just returns the first simulation output
-   my_moop.addObjective({'name': "f1", 'obj_func': lambda x, s: s["MySim"][0]})
+   def f1(x, s): return s["MySim"][0]
+   my_moop.addObjective({'name': "f1", 'obj_func': f1})
    # Second objective just returns the second simulation output
-   my_moop.addObjective({'name': "f2", 'obj_func': lambda x, s: s["MySim"][1]})
+   def f2(x, s): return s["MySim"][1]
+   my_moop.addObjective({'name': "f2", 'obj_func': f2})
    # Add a single constraint, that x[0] >= 0.1
-   my_moop.addConstraint({'name': "c1",
-                          'constraint': lambda x, s: 0.1 - x["x1"]})
+   def c1(x, s): return 0.1 - x["x1"]
+   my_moop.addConstraint({'name': "c1", 'constraint': c1})
 
 Finally, we must add one or more acquisition functions using
 :meth:`MOOP.addAcquisition(*args) <moop.MOOP.addAcquisition>`.
 These are used to scalarize the surrogate problems.
 The number of acquisition functions
 typically determines the number of simulation evaluations per batch.
 This is useful to know if you are using a parallel solver.
 
 .. code-block:: python
 
-   from parmoo.acquisitions import UniformWeights
+   from parmoo.acquisitions import RandomConstraint
 
    # Add 3 acquisition functions
    for i in range(3):
-      my_moop.addAcquisition({'acquisition': UniformWeights,
+      my_moop.addAcquisition({'acquisition': RandomConstraint,
                               'hyperparams': {}})
 
 Finally, the MOOP is solved using the
 :meth:`MOOP.solve(budget) <moop.MOOP.solve>` method, and the
 results can be viewed using
 :meth:`MOOP.getPF() <moop.MOOP.getPF>`.
 
 .. code-block:: python
 
+   import pandas as pd
+
    my_moop.solve(5) # Solve with 5 iterations of ParMOO algorithm
-   results = my_moop.getPF() # Extract the results
+   results = my_moop.getPF(format="pandas") # Extract the results as pandas df
 
 After executing the above block of code, the ``results`` variable points to
-a numpy structured array, each of whose entries corresponds to a
-nondominated objective value in the ``my_moop`` object's final database.
-You can reference individual fields in the ``results`` array by using the
+a pandas_ dataframe, each of whose rows corresponds to a nondominated
+objective value in the ``my_moop`` object's final database.
+You can reference individual columns in the ``results`` array by using the
 ``name`` keys that were assigned during ``my_moop``'s construction, or
 plot the results by using the :doc:`viz <modules/viz>` library.
 
 Congratulations, you now know enough to get started solving MOOPs!
 
 Minimal Working Example
 -----------------------
@@ -259,15 +263,15 @@
 ``results`` variable, and prints the ``results`` variable to the standard
 output:
 
 .. literalinclude:: ../examples/quickstart.out
 
 And produces the following figure of the Pareto points:
 
-.. figure:: ../examples/Pareto\ Front.jpeg
+.. figure:: ../examples/quickstart.jpeg
     :alt: Scatter plot of the Pareto front after solving demo problem
     :align: center
 
 |
 
 Next Steps
 ----------
@@ -277,16 +281,18 @@
  * If you would like more information on multiobjective optimization
    terminology and ParMOO's methodology, see the
    :doc:`Learn About MOOPs <about>` page.
  * For a full list of basic usage tutorials, see
    :doc:`More Tutorials <tutorials/basic-tutorials>`.
  * To start solving MOOPs on parallel hardware, install libEnsemble_ and
    see the :doc:`libEnsemble tutorial <tutorials/libe-tutorial>`.
+ * See some of our pre-built solvers in the parmoo_solver_farm_.
  * To interactively explore your solutions, install its extra dependencies and
    use our built-in :doc:`viz <modules/viz>` tool.
+ * For more advice, consult our :doc:`FAQs <faqs>`.
 
 Resources
 ---------
 
 To seek support or report issues, e-mail:
 
  * ``parmoo@mcs.anl.gov``
@@ -304,14 +310,15 @@
 .. _flake8: https://flake8.pycqa.org/en/latest
 .. _GitHub: https://github.com/parmoo/parmoo
 .. _kaleido: https://github.com/plotly/Kaleido
 .. _libEnsemble: https://github.com/Libensemble/libensemble
 .. _LICENSE: https://github.com/parmoo/parmoo/blob/main/LICENSE
 .. _numpy: https://numpy.org
 .. _pandas: https://pandas.pydata.org
+.. _parmoo_solver_farm: https://github.com/parmoo/parmoo-solver-farm
 .. _plotly: https://plotly.com/python
 .. _pyDOE: https://pythonhosted.org/pyDOE
 .. _pytest: https://docs.pytest.org/en/7.0.x
 .. _pytest-cov: https://pytest-cov.readthedocs.io/en/latest
 .. _Python: https://www.python.org/downloads
 .. _ReadTheDocs: https://parmoo.readthedocs.org
 .. _scipy: https://scipy.org
```

### Comparing `parmoo-0.2.2/docs/refs.rst` & `parmoo-0.3.0/docs/refs.rst`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 .. code-block:: bibtex
 
     @techreport{parmoo-docs,
         title       = {{ParMOO}: {P}ython library for parallel multiobjective simulation optimization},
         author      = {Chang, Tyler H. and Wild, Stefan M. and Dickinson, Hyrum},
         institution = {Argonne National Laboratory},
-        number      = {Version 0.2.2},
+        number      = {Version 0.3.0},
         year        = {2023},
         url         = {https://parmoo.readthedocs.io/en/latest}
     }
 
 .. _CONTRIBUTING: https://github.com/parmoo/parmoo/blob/main/CONTRIBUTING.rst
 .. _LICENSE: https://github.com/parmoo/parmoo/blob/main/LICENSE
 .. _ReadTheDocs: https://parmoo.readthedocs.org
```

### Comparing `parmoo-0.2.2/docs/tutorials/basic-tutorials.rst` & `parmoo-0.3.0/docs/tutorials/basic-tutorials.rst`

 * *Files 3% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 This is a basic example (see `quickstart.py <https://github.com/parmoo/parmoo/blob/main/examples/quickstart.py>`_) of how to build and solve a MOOP with ParMOO,
 taken from the :doc:`Quickstart <../quickstart>` guide.
 
 .. literalinclude:: ../../examples/quickstart.py
     :language: python
 
 The above code saves all (approximate) Pareto optimal solutions in the
-``results`` variable, and prints the ``results`` variable to the standard
+``results`` dataframe, and prints the ``results`` dataframe to the standard
 output:
 
 .. literalinclude:: ../../examples/quickstart.out
 
 And produces the following figure of the Pareto points:
 
-.. figure:: ../../examples/Pareto\ Front.jpeg
+.. figure:: ../../examples/quickstart.jpeg
     :alt: Scatter plot of the Pareto front after solving demo problem
     :align: center
 
 |
 
 Named Output Types
 ~~~~~~~~~~~~~~~~~~
```

### Comparing `parmoo-0.2.2/docs/tutorials/libe-tutorial.rst` & `parmoo-0.3.0/docs/tutorials/libe-tutorial.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/examples/Makefile` & `parmoo-0.3.0/examples/Makefile`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 OUT_FILES = quickstart.out named_var_ex.out unnamed_var_ex.out \
 			precomputed_data.out checkpointing.out advanced_ex.out \
-			libe_basic_ex.out Pareto\ Front.jpeg
+			local_method.jpeg libe_basic_ex.out quickstart.jpeg
 
 all: $(OUT_FILES)
 
-Pareto Front.jpeg: quickstart.out
+quickstart.jpeg: quickstart.py
+	python3 quickstart.py > quickstart.out
+	mv Pareto\ Front.jpeg quickstart.jpeg
 
 quickstart.out: quickstart.py
 	python3 quickstart.py > quickstart.out
+	mv Pareto\ Front.jpeg quickstart.jpeg
 
 named_var_ex.out: named_var_ex.py
 	python3 named_var_ex.py > named_var_ex.out
 
 unnamed_var_ex.out: unnamed_var_ex.py
 	python3 unnamed_var_ex.py > unnamed_var_ex.out
 
@@ -22,13 +25,17 @@
 	python3 checkpointing.py > checkpointing.out
 	rm -f parmoo.moop parmoo.surrogate.1
 
 advanced_ex.out: advanced_ex.py
 	python3 advanced_ex.py > advanced_ex.out
 	rm -f parmoo.moop parmoo.surrogate.1
 
+local_method.jpeg: local_method.py
+	python3 local_method.py
+	mv Pareto\ Front.jpeg local_method.jpeg
+
 libe_basic_ex.out: libe_basic_ex.py
 	python3 libe_basic_ex.py --comms local --nworkers 3 > libe_basic_ex.out
 	rm -f parmoo.moop parmoo.surrogate.1 libE_stats.txt ensemble.log
 
 clean:
-	rm -f *.out libE_stats.txt ensemble.log
+	rm -f *.out libE_stats.txt ensemble.log *.jpeg
```

### Comparing `parmoo-0.2.2/examples/advanced_ex.py` & `parmoo-0.3.0/examples/advanced_ex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 
 import numpy as np
 from parmoo import MOOP
-from parmoo.acquisitions import UniformWeights, FixedWeights
+from parmoo.acquisitions import RandomConstraint, FixedWeights
 from parmoo.searches import LatinHypercube
 from parmoo.surrogates import GaussRBF
 from parmoo.optimizers import LBFGSB
 
+# Fix the random seed for reproducibility
+np.random.seed(0)
+
 # Create a new MOOP with a derivative-based solver
 my_moop = MOOP(LBFGSB, hyperparams={})
 
 # Add 3 continuous variables named x1, x2, x3
 for i in range(3):
     my_moop.addDesign({'name': "x" + str(i+1),
                        'des_type': "continuous",
@@ -86,15 +89,15 @@
         return np.zeros(1, dtype=sim.dtype)[0]
 
 # Add the single constraint to the problem
 my_moop.addConstraint({'name': "c_x4",
                        'constraint': const_x4})
 
 # Add 2 different acquisition functions to the problem
-my_moop.addAcquisition({'acquisition': UniformWeights})
+my_moop.addAcquisition({'acquisition': RandomConstraint})
 my_moop.addAcquisition({'acquisition': FixedWeights,
                         # Fixed weight with equal weight on both objectives
                         'hyperparams': {'weights': np.array([0.5, 0.5])}})
 
 # Turn on checkpointing -- creates the files parmoo.moop and parmoo.surrogate.1
 my_moop.setCheckpoint(True, checkpoint_data=False, filename="parmoo")
 
@@ -104,16 +107,18 @@
                     format='%(asctime)s %(levelname)-8s %(message)s',
                     datefmt='%Y-%m-%d %H:%M:%S')
 
 # Solve the problem
 my_moop.solve(5)
 
 # Get and print full simulation database
-sim_db = my_moop.getSimulationData()
+sim_db = my_moop.getSimulationData(format="pandas")
 print("Simulation data:")
-print(sim_db)
+for key in sim_db.keys():
+    print(f"\t{key}:")
+    print(sim_db[key])
 
 # Get and print results
-soln = my_moop.getPF()
+soln = my_moop.getPF(format="pandas")
 print("\n\n")
 print("Solution points:")
 print(soln)
```

### Comparing `parmoo-0.2.2/examples/checkpointing.out` & `parmoo-0.3.0/examples/checkpointing.out`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,18 @@
-[(0.79432817, 0, 3.53225972e-01, 3.21696685e-05, -0.69432817)
- (0.75428911, 0, 3.07236413e-01, 2.08948580e-03, -0.65428911)
- (0.74842973, 0, 3.00775170e-01, 2.65949261e-03, -0.64842973)
- (0.74208208, 0, 2.93852976e-01, 3.35448602e-03, -0.64208208)
- (0.70136828, 0, 2.51370153e-01, 9.72821611e-03, -0.60136828)
- (0.68964953, 0, 2.39756663e-01, 1.21772261e-02, -0.58964953)
- (0.61103625, 0, 1.68950798e-01, 3.57072991e-02, -0.51103625)
- (0.5849132 , 0, 1.48158173e-01, 4.62623305e-02, -0.4849132 )
- (0.50538467, 0, 9.32597987e-02, 8.67981908e-02, -0.40538467)
- (0.47806531, 0, 7.73203180e-02, 1.03641943e-01, -0.37806531)
- (0.47025281, 0, 7.30365826e-02, 1.08733208e-01, -0.37025281)
- (0.43328659, 0, 5.44226336e-02, 1.34478724e-01, -0.33328659)
- (0.40936081, 0, 4.38319487e-02, 1.52598977e-01, -0.30936081)
- (0.40643112, 0, 4.26138083e-02, 1.54896461e-01, -0.30643112)
- (0.40154831, 0, 4.06217212e-02, 1.58763749e-01, -0.30154831)
- (0.3756694 , 0, 3.08597394e-02, 1.80056455e-01, -0.2756694 )
- (0.35108734, 0, 2.28273846e-02, 2.01522575e-01, -0.25108734)
- (0.33448578, 0, 1.80864247e-02, 2.16703490e-01, -0.23448578)
- (0.32459808, 0, 1.55246824e-02, 2.26006982e-01, -0.22459808)
- (0.30994965, 0, 1.20889246e-02, 2.40149350e-01, -0.20994965)
- (0.30262543, 0, 1.05319783e-02, 2.47381466e-01, -0.20262543)
- (0.29920746, 0, 9.84211978e-03, 2.50793170e-01, -0.19920746)
- (0.28065277, 0, 6.50486944e-03, 2.69721544e-01, -0.18065277)
- (0.2469228 , 0, 2.20174956e-03, 3.05894384e-01, -0.1469228 )
- (0.19333394, 0, 4.44363953e-05, 3.68043712e-01, -0.09333394)] 
+[(0.79013666, 0, 3.48261275e-01, 9.72855201e-05, -0.69013666)
+ (0.7895263 , 0, 3.47541259e-01, 1.09698380e-04, -0.6895263 )
+ (0.73488156, 0, 2.86098283e-01, 4.24041125e-03, -0.63488156)
+ (0.70656124, 0, 2.56604287e-01, 8.73080244e-03, -0.60656124)
+ (0.68409101, 0, 2.34344111e-01, 1.34348928e-02, -0.58409101)
+ (0.67237225, 0, 2.23135544e-01, 1.62888423e-02, -0.57237225)
+ (0.5784217 , 0, 1.43202981e-01, 4.90969442e-02, -0.4784217 )
+ (0.53031761, 0, 1.09109723e-01, 7.27285920e-02, -0.43031761)
+ (0.51322778, 0, 9.81116425e-02, 8.22383058e-02, -0.41322778)
+ (0.49723345, 0, 8.83477213e-02, 9.16675863e-02, -0.39723345)
+ (0.44987019, 0, 6.24351129e-02, 1.22590882e-01, -0.34987019)
+ (0.40591372, 0, 4.24004606e-02, 1.55303995e-01, -0.30591372)
+ (0.39028872, 0, 3.62097978e-02, 1.67863331e-01, -0.29028872)
+ (0.38995793, 0, 3.60840145e-02, 1.68134501e-01, -0.28995793)
+ (0.38287784, 0, 3.34443041e-02, 1.73990897e-01, -0.28287784)
+ (0.25435646, 0, 2.95462529e-03, 2.97726867e-01, -0.15435646)
+ (0.20137796, 0, 1.89878434e-06, 3.58348342e-01, -0.10137796)] 
  dtype=[('x1', '<f8'), ('x2', '<i4'), ('f1', '<f8'), ('f2', '<f8'), ('c1', '<f8')]
```

### Comparing `parmoo-0.2.2/examples/checkpointing.py` & `parmoo-0.3.0/examples/checkpointing.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 from parmoo import MOOP
 from parmoo.searches import LatinHypercube
 from parmoo.surrogates import GaussRBF
 from parmoo.acquisitions import UniformWeights
 from parmoo.optimizers import LocalGPS
 import logging
 
+# Fix the random seed for reproducibility
+np.random.seed(0)
+
 # Create a new MOOP
 my_moop = MOOP(LocalGPS)
 
 # Add 1 continuous and 1 categorical design variable
 my_moop.addDesign({'name': "x1",
                    'des_type': "continuous",
                    'lb': 0.0, 'ub': 1.0})
```

### Comparing `parmoo-0.2.2/examples/libe_basic_ex.py` & `parmoo-0.3.0/examples/libe_basic_ex.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 import numpy as np
 from parmoo.extras.libe import libE_MOOP
 from parmoo.searches import LatinHypercube
 from parmoo.surrogates import GaussRBF
 from parmoo.acquisitions import UniformWeights
 from parmoo.optimizers import LocalGPS
 
+# When running with MPI, we need to keep track of which thread is the manager
+# using libensemble.tools.parse_args()
+from libensemble.tools import parse_args
+_, is_manager, _, _ = parse_args()
+
 # All functions are defined below.
 
 def sim_func(x):
    if x["x2"] == 0:
       return np.array([(x["x1"] - 0.2) ** 2, (x["x1"] - 0.8) ** 2])
    else:
       return np.array([99.9, 99.9])
@@ -22,14 +27,17 @@
 
 def const_c1(x, s):
     return 0.1 - x["x1"]
 
 # When using libEnsemble with Python MP, the "solve" command must be enclosed
 # in an "if __name__ == '__main__':" block, as shown below
 if __name__ == "__main__":
+    # Fix the random seed for reproducibility
+    np.random.seed(0)
+
     # Create a libE_MOOP
     my_moop = libE_MOOP(LocalGPS)
     
     # Add 2 design variables (one continuous and one categorical)
     my_moop.addDesign({'name': "x1",
                        'des_type': "continuous",
                        'lb': 0.0, 'ub': 1.0})
@@ -57,11 +65,12 @@
                                'hyperparams': {}})
     
     # Turn on checkpointing -- creates files parmoo.moop & parmoo.surrogate.1
     my_moop.setCheckpoint(True, checkpoint_data=False, filename="parmoo")
     
     # Use sim_max = 30 to perform just 30 simulations
     my_moop.solve(sim_max=30)
-    results = my_moop.getPF()
     
-    # Display the solution
-    print(results, "\n dtype=" + str(results.dtype))
+    # Display the solution -- this "if" clause is needed when running with MPI
+    if is_manager:
+        results = my_moop.getPF(format="pandas")
+        print(results)
```

### Comparing `parmoo-0.2.2/examples/named_var_ex.py` & `parmoo-0.3.0/examples/named_var_ex.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/examples/precomputed_data.py` & `parmoo-0.3.0/examples/precomputed_data.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/examples/quickstart.py` & `parmoo-0.3.0/examples/quickstart.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 
 import numpy as np
+import pandas as pd
 from parmoo import MOOP
 from parmoo.searches import LatinHypercube
 from parmoo.surrogates import GaussRBF
-from parmoo.acquisitions import UniformWeights
+from parmoo.acquisitions import RandomConstraint
 from parmoo.optimizers import LocalGPS
 
+# Fix the random seed for reproducibility
+np.random.seed(0)
+
 my_moop = MOOP(LocalGPS)
 
 my_moop.addDesign({'name': "x1",
                    'des_type': "continuous",
                    'lb': 0.0, 'ub': 1.0})
 my_moop.addDesign({'name': "x2", 'des_type': "categorical",
                    'levels': ["good", "bad"]})
@@ -23,26 +27,29 @@
 my_moop.addSimulation({'name': "MySim",
                        'm': 2,
                        'sim_func': sim_func,
                        'search': LatinHypercube,
                        'surrogate': GaussRBF,
                        'hyperparams': {'search_budget': 20}})
 
-my_moop.addObjective({'name': "f1", 'obj_func': lambda x, s: s["MySim"][0]})
-my_moop.addObjective({'name': "f2", 'obj_func': lambda x, s: s["MySim"][1]})
+def f1(x, s): return s["MySim"][0]
+def f2(x, s): return s["MySim"][1]
+my_moop.addObjective({'name': "f1", 'obj_func': f1})
+my_moop.addObjective({'name': "f2", 'obj_func': f2})
 
-my_moop.addConstraint({'name': "c1", 'constraint': lambda x, s: 0.1 - x["x1"]})
+def c1(x, s): return 0.1 - x["x1"]
+my_moop.addConstraint({'name': "c1", 'constraint': c1})
 
 for i in range(3):
-   my_moop.addAcquisition({'acquisition': UniformWeights,
+   my_moop.addAcquisition({'acquisition': RandomConstraint,
                            'hyperparams': {}})
 
 my_moop.solve(5)
-results = my_moop.getPF()
+results = my_moop.getPF(format="pandas")
 
 # Display solution
-print(results, "\n dtype=" + str(results.dtype))
+print(results)
 
 # Plot results -- must have extra viz dependencies installed
 from parmoo.viz import scatter
 # The optional arg `output` exports directly to jpg instead of interactive mode
 scatter(my_moop, output="jpeg")
```

### Comparing `parmoo-0.2.2/examples/unnamed_var_ex.out` & `parmoo-0.3.0/examples/unnamed_var_ex.out`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/examples/unnamed_var_ex.py` & `parmoo-0.3.0/examples/unnamed_var_ex.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 import numpy as np
 from parmoo import MOOP
 from parmoo.searches import LatinHypercube
 from parmoo.surrogates import GaussRBF
 from parmoo.acquisitions import UniformWeights
 from parmoo.optimizers import LocalGPS
 
+# Fix the random seed for reproducibility
+np.random.seed(0)
+
 my_moop = MOOP(LocalGPS)
 
 # Define a simulation to use below
 def sim_func(x):
     return np.array([(x[0]) ** 2, (x[0] - 1.0) ** 2])
 
 # Add a design variable, simulation, objective, and constraint, w/o name key
```

### Comparing `parmoo-0.2.2/parmoo/acquisitions/weighted_sum.py` & `parmoo-0.3.0/parmoo/acquisitions/weighted_sum.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,24 +57,33 @@
         # Set the bound constraints
         self.lb = lb
         self.ub = ub
         # Initialize the weights array
         self.weights = np.zeros(o)
         return
 
-    def setTarget(self, data, lagrange_func, history):
+    def useSD(self):
+        """ Query whether this method uses uncertainties.
+
+        When False, allows users to shortcut expensive uncertainty
+        computations.
+
+        """
+
+        return False
+
+    def setTarget(self, data, penalty_func, history):
         """ Randomly generate a new vector of scalarizing weights.
 
         Args:
             data (dict): A dictionary specifying the current function
                 evaluation database.
 
-            lagrange_func (function): A function whose components correspond
-                to constraint violation amounts.
-
+            penalty_func (function): A function of one (x) or two (x, sx)
+                inputs that evaluates the (penalized) objectives.
 
             history (dict): Another unused argument for this function.
 
         Returns:
             numpy.ndarray: A 1d array containing the 'best' feasible starting
             point for the scalarized problem (if any previous evaluations
             were feasible) or the point in the existing database that is
@@ -104,21 +113,21 @@
                     if data['f_vals'].shape[1] != self.o:
                         raise ValueError("The rows of f_vals must have " +
                                          "length o")
                 else:
                     no_data = True
             else:
                 no_data = True
-        # Check whether lagrange_func() has an appropriate signature
-        if callable(lagrange_func):
-            if len(inspect.signature(lagrange_func).parameters) != 1:
-                raise ValueError("lagrange_func() must accept exactly one"
+        # Check whether penalty_func() has an appropriate signature
+        if callable(penalty_func):
+            if len(inspect.signature(penalty_func).parameters) not in [1, 2]:
+                raise ValueError("penalty_func() must accept exactly one"
                                  + " input")
         else:
-            raise TypeError("lagrange_func() must be callable")
+            raise TypeError("penalty_func() must be callable")
         if no_data:
             # If data is empty, then the Pareto front is empty
             pf = {'x_vals': np.zeros((0, self.n)),
                   'f_vals': np.zeros((0, self.o)),
                   'c_vals': np.zeros((0, 1))}
         else:
             # Get the Pareto front
@@ -130,31 +139,42 @@
         if pf['x_vals'].shape[0] == 0:
             # Randomly search for a good starting point
             x_min = np.random.random_sample(self.n) * (self.ub - self.lb) \
                     + self.lb
             for count in range(1000):
                 x = np.random.random_sample(self.n) * (self.ub - self.lb) \
                     + self.lb
-                if np.dot(self.weights, lagrange_func(x)) \
-                   < np.dot(self.weights, lagrange_func(x_min)):
+                if np.dot(self.weights, penalty_func(x)) \
+                   < np.dot(self.weights, penalty_func(x_min)):
                     x_min[:] = x[:]
             return x_min
         else:
             i = np.argmin(np.asarray([np.dot(self.weights, fi)
                                       for fi in pf['f_vals']]))
             x = pf['x_vals'][i, :]
             return x
 
-    def scalarize(self, f_vals):
+    def scalarize(self, f_vals, x_vals, s_vals_mean, s_vals_sd):
         """ Scalarize a vector of function values using the current weights.
 
         Args:
             f_vals (numpy.ndarray): A 1d array specifying the function
                 values to be scalarized.
 
+            x_vals (np.ndarray): A 1D array specifying a vector the design
+                point corresponding to f_vals (unused by this method).
+
+            s_vals_mean (np.ndarray): A 1D array specifying the expected
+                simulation outputs for the x value being scalarized
+                (unused by this method).
+
+            s_vals_sd (np.ndarray): A 1D array specifying the standard
+                deviation for each of the simulation outputs (unused by
+                this method).
+
         Returns:
             float: The scalarized value.
 
         """
 
         # Check that the function values are legal
         if isinstance(f_vals, np.ndarray):
@@ -253,23 +273,33 @@
                     # Assign the weights
                     self.weights = hyperparams['weights'].flatten()
         else:
             # If no weights were provided, use an even weighting
             self.weights = np.ones(self.o) / float(self.o)
         return
 
-    def setTarget(self, data, lagrange_func, history):
+    def useSD(self):
+        """ Querry whether this method uses uncertainties.
+
+        When False, allows users to shortcut expensive uncertainty
+        computations.
+
+        """
+
+        return False
+
+    def setTarget(self, data, penalty_func, history):
         """ Randomly generate a feasible starting point.
 
         Args:
             data (dict): A dictionary specifying the current function
                 evaluation database.
 
-            lagrange_func (function): A function whose components correspond
-                to constraint violation amounts.
+            penalty_func (function): A function of one (x) or two (x, sx)
+                inputs that evaluates the (penalized) objectives.
 
             history (dict): Another unused argument for this function.
 
         Returns:
             numpy.ndarray: A 1d array containing the 'best' feasible starting
             point for the scalarized problem (if any previous evaluations
             were feasible) or the point in the existing database that is
@@ -299,21 +329,21 @@
                     if data['f_vals'].shape[1] != self.o:
                         raise ValueError("The rows of f_vals must have " +
                                          "length o")
                 else:
                     no_data = True
             else:
                 no_data = True
-        # Check whether lagrange_func() has an appropriate signature
-        if callable(lagrange_func):
-            if len(inspect.signature(lagrange_func).parameters) != 1:
-                raise ValueError("lagrange_func() must accept exactly one"
+        # Check whether penalty_func() has an appropriate signature
+        if callable(penalty_func):
+            if len(inspect.signature(penalty_func).parameters) not in [1, 2]:
+                raise ValueError("penalty_func() must accept exactly one"
                                  + " input")
         else:
-            raise TypeError("lagrange_func() must be callable")
+            raise TypeError("penalty_func() must be callable")
         if no_data:
             # If data is empty, then the Pareto front is empty
             pf = {'x_vals': np.zeros((0, self.n)),
                   'f_vals': np.zeros((0, self.o)),
                   'c_vals': np.zeros((0, 1))}
         else:
             # Get the Pareto front
@@ -322,31 +352,42 @@
         if pf['x_vals'].shape[0] == 0:
             # Randomly search for a good starting point
             x_min = np.random.random_sample(self.n) * (self.ub - self.lb) \
                     + self.lb
             for count in range(1000):
                 x = np.random.random_sample(self.n) * (self.ub - self.lb) \
                     + self.lb
-                if np.dot(self.weights, lagrange_func(x)) \
-                   < np.dot(self.weights, lagrange_func(x_min)):
+                if np.dot(self.weights, penalty_func(x)) \
+                   < np.dot(self.weights, penalty_func(x_min)):
                     x_min[:] = x[:]
             return x_min
         else:
             i = np.argmin(np.asarray([np.dot(self.weights, fi)
                                       for fi in pf['f_vals']]))
             x = pf['x_vals'][i, :]
             return x
 
-    def scalarize(self, f_vals):
+    def scalarize(self, f_vals, x_vals, s_vals_mean, s_vals_sd):
         """ Scalarize a vector of function values using the current weights.
 
         Args:
             f_vals (numpy.ndarray): A 1d array specifying the function
                 values to be scalarized.
 
+            x_vals (np.ndarray): A 1D array specifying a vector the design
+                point corresponding to f_vals (unused by this method).
+
+            s_vals_mean (np.ndarray): A 1D array specifying the expected
+                simulation outputs for the x value being scalarized
+                (unused by this method).
+
+            s_vals_sd (np.ndarray): A 1D array specifying the standard
+                deviation for each of the simulation outputs (unused by
+                this method).
+
         Returns:
             float: The scalarized value.
 
         """
 
         # Check that the function values are legal
         if isinstance(f_vals, np.ndarray):
```

### Comparing `parmoo-0.2.2/parmoo/constraints/const_func.py` & `parmoo-0.3.0/parmoo/constraints/const_func.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/constraints/const_lib.py` & `parmoo-0.3.0/parmoo/constraints/const_lib.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/extras/libe.py` & `parmoo-0.3.0/parmoo/extras/libe.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 the `gen_specs` dict, then import and use `parmoo_persis_gen` as the libE
 gen func.
 
 """
 
 import numpy as np
 from parmoo import MOOP
+import warnings
 
 
 def parmoo_persis_gen(H, persis_info, gen_specs, libE_info):
     """ A persistent ParMOO generator function for libEnsemble.
 
     This generator function is meant to be called from within libEnsemble.
 
@@ -186,31 +187,32 @@
 
     ParMOO's logging feature is not active for the `libE_MOOP` class
     since libEnsemble already provides this feature.
 
     After defining the MOOP and setting up checkpointing and logging,
     use the following method to solve the MOOP (using libEnsemble
     to distribute simulation evaluations):
-     * ``libE_MOOP.solve(sim_max=200, wt_max=3600, profile=False)``
+     * ``libE_MOOP.solve(iter_max=None, sim_max=None, wt_max=864000,
+                         profile=False)``
 
     The following methods are used for managing ParMOO's internal
     simulation/objective databases. Note that these databases are
     maintained separately from libEnsemble's simulation database:
      * ``libE_MOOP.check_sim_db(x, s_name)``
      * ``libE_MOOP.update_sim_db(x, sx, s_name)``
      * ``libE_MOOP.evaluateSimulation(x, s_name)``
      * ``libE_MOOP.addData(x, sx)``
      * ``libE_MOOP.iterate(k)``
      * ``libE_MOOP.updateAll(k, batch)``
 
     Finally, the following methods are used to retrieve data after the
     problem has been solved:
-     * ``libE_MOOP.getPF()``
-     * ``libE_MOOP.getSimulationData()``
-     * ``libE_MOOP.getObjectiveData()``
+     * ``libE_MOOP.getPF(format='ndarray')``
+     * ``libE_MOOP.getSimulationData(format='ndarray')``
+     * ``libE_MOOP.getObjectiveData(format='ndarray')``
 
     Other private methods from the MOOP class do not work for a libE_MOOP.
 
     """
 
     __slots__ = ['moop']
 
@@ -665,42 +667,90 @@
                 H_o[self.moop.sim_names[j][0]][i] = \
                     self.moop.sim_funcs[j](xx)
             else:
                 H_o['f'][i, :self.moop.m[j]] = \
                     self.moop.sim_funcs[j](H['x'][i])
         return H_o, persis_info
 
-    def solve(self, sim_max=200, wt_max=3600, profile=False):
+    def solve(self, iter_max=None, sim_max=None, wt_max=864000, profile=False):
         """ Solve a MOOP using ParMOO + libEnsemble.
 
         If desired, be sure to turn on checkpointing before starting the
         solve, using:
 
         ``MOOP.setCheckpoint(checkpoint, [checkpoint_data, filename])``
 
         ParMOO will solve the MOOP and use libEnsemble to distribute
         simulations over available resources.
 
         Args:
+            iter_max (int): The max number of ParMOO iterations to be
+                performed by libEnsemble (default is unlimited).
+
             sim_max (int): The max number of simulation to be performed by
-                libEnsemble (default is 200).
+                libEnsemble (default is unlimited).
 
             wt_max (int): The max number of seconds that the simulation may
-                run for (the default is 3600 secs, i.e., 1 hr).
+                run for (the default is 864000 secs, i.e., 10 days).
 
             profile (bool): Specifies whether to run libE with the profiler.
 
         """
 
         import sys
         from libensemble.libE import libE
         from libensemble.alloc_funcs.start_only_persistent \
             import only_persistent_gens as alloc_f
         from libensemble.tools import parse_args
 
+        # Check that at least one budget variable was given
+        if iter_max is None and sim_max is None:
+            raise ValueError("At least one of the following arguments " +
+                             "must be set: 'iter_max' or 'sim_max'")
+        # Check that the iter_max is a legal integer
+        if isinstance(iter_max, int):
+            if iter_max < 0:
+                raise ValueError("When present, iter_max must be nonnegative")
+        elif iter_max is not None:
+            raise TypeError("When present, iter_max must be an int type")
+        # Check that the sim_max is a legal integer
+        if isinstance(sim_max, int):
+            if sim_max < 0:
+                raise ValueError("When present, sim_max must be nonnegative")
+        elif sim_max is not None:
+            raise TypeError("When present, sim_max must be an int type")
+        # Set iter_max large enough if None
+        if iter_max is None:
+            if self.moop.s == 0:
+                raise ValueError("If 0 simulations are given, then iter_max" +
+                                 "must be provided")
+            iter_max = sim_max
+        # Count the total search budget
+        total_search_budget = 0
+        for search in self.moop.searches:
+            total_search_budget += search.budget
+        total_sims_per_iter = len(self.moop.acquisitions) * self.moop.s
+        # Count the total sims to exhaust iter_max if sim_max is None
+        if sim_max is None:
+            sim_max = total_search_budget + iter_max * total_sims_per_iter
+        # libE only uses sim_max, so set it appropriately
+        sim_max = min(sim_max,
+                      total_search_budget + iter_max * total_sims_per_iter)
+        # Warning for the uninitiated
+        if sim_max <= total_search_budget:
+            warnings.warn("You are running ParMOO with a total search budget" +
+                          f" of {total_search_budget} and a sim_max of " +
+                          f"just {sim_max}... This will result in pure " +
+                          "design space exploration with no exploitation/" +
+                          "optimization. Consider increasing the value of " +
+                          "sim_max, decreasing your search_budget, " +
+                          "or using the iter_max stopping criteria, unless " +
+                          "you are really only interested in design space " +
+                          "exploration without exploitation/optimization.")
+
         # Create libEnsemble dictionaries
         nworkers, is_manager, libE_specs, _ = parse_args()
         if self.moop.use_names:
             libE_specs['final_fields'] = []
             for name in self.moop.des_names:
                 libE_specs['final_fields'].append(name[0])
             for name in self.moop.sim_names:
@@ -757,20 +807,28 @@
 
         exit_criteria = {'sim_max': sim_max, 'wallclock_max': wt_max}
 
         # Perform the run
         H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria,
                                     persis_info, alloc_specs, libE_specs)
 
-        self.moop = persis_info[1]['moop']
+        # When running with MPI, only the manager returns results
+        if is_manager:
+            self.moop = persis_info[1]['moop']
         return
 
-    def getPF(self):
+    def getPF(self, format='ndarray'):
         """ Extract nondominated and efficient sets from internal databases.
 
+        Args:
+            format (str, optional): Either 'ndarray' (default) or 'pandas',
+                in order to produce output as a numpy structured array or
+                pandas dataframe. Note: format='pandas' is only valid for
+                named inputs.
+
         Returns:
             A discrete approximation of the Pareto front and efficient set.
 
             If operating with named variables, then this is a 1d numpy
             structured array whose fields match the names for design
             variables, objectives, and constraints (if any).
 
@@ -782,19 +840,25 @@
                of corresponding efficient design points.
              * c_vals (numpy.ndarray): A 2d numpy.ndarray containing the list
                of corresponding constraint satisfaction scores,
                all less than or equal to 0.
 
         """
 
-        return self.moop.getPF()
+        return self.moop.getPF(format=format)
 
-    def getSimulationData(self):
+    def getSimulationData(self, format='ndarray'):
         """ Extract all computed simulation outputs from the MOOP's database.
 
+        Args:
+            format (str, optional): Either 'ndarray' (default) or 'pandas',
+                in order to produce output as a numpy structured array or
+                pandas dataframe. Note: format='pandas' is only valid for
+                named inputs.
+
         Returns:
             (dict or list) Either a dictionary or list of dictionaries
             containing every point where a simulation was evaluated.
 
             If operating with named variables, then the result is a dict.
             Each key is the name for a different simulation, and each value
             is a 1d numpy structured array whose keys match the
@@ -807,19 +871,25 @@
                of design points that have been evaluated for this
                simulation.
              * s_vals (numpy.ndarray): A 1d or 2d array containing
                the list of corresponding simulation outputs.
 
         """
 
-        return self.moop.getSimulationData()
+        return self.moop.getSimulationData(format=format)
 
-    def getObjectiveData(self):
+    def getObjectiveData(self, format='ndarray'):
         """ Extract all computed objective scores from this MOOP's database.
 
+        Args:
+            format (str, optional): Either 'ndarray' (default) or 'pandas',
+                in order to produce output as a numpy structured array or
+                pandas dataframe. Note: format='pandas' is only valid for
+                named inputs.
+
         Returns:
             A database of all designs that have been fully evaluated,
             and their corresponding objective scores.
 
             If operating with named variables, then this is a 1d numpy
             structured array whose fields match the names for design
             variables, objectives, and constraints (if any).
@@ -831,15 +901,15 @@
                of corresponding objective values.
              * c_vals (numpy.ndarray): A 2d array containing the list
                of corresponding constraint satisfaction scores,
                all less than or equal to 0.
 
         """
 
-        return self.moop.getObjectiveData()
+        return self.moop.getObjectiveData(format=format)
 
     def save(self, filename="parmoo"):
         """ Serialize and save the MOOP object and all of its dependencies.
 
         Args:
             filename (str, optional): The filepath to serialized
                 checkpointing file(s). Do not include file extensions,
```

### Comparing `parmoo-0.2.2/parmoo/moop.py` & `parmoo-0.3.0/parmoo/moop.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 parmoo.moop.MOOP is the base class for defining and solving multiobjective
 optimization problems (MOOPs). Each MOOP object may contain several
 simulations, specified using dictionaries.
 
 """
 
 import numpy as np
-import json
+import pandas as pd
 from parmoo import structs
 import inspect
-import pandas as pd
+import json
+import warnings
 
 
 class MOOP:
     """ Class for defining a multiobjective optimization problem (MOOP).
 
     Upon initialization, supply a scalar optimization procedure and
     dictionary of hyperparameters using the default constructor:
@@ -51,41 +52,43 @@
      * ``MOOP.setCheckpoint(checkpoint, [checkpoint_data, filename])``
 
     ParMOO also offers logging. To turn on logging, activate INFO-level
     logging by importing Python's built-in logging module.
 
     After defining the MOOP and setting up checkpointing and logging info,
     use the following method to solve the MOOP (serially):
-     * ``MOOP.solve(budget)``
+     * ``MOOP.solve(iter_max=None, sim_max=None)``
 
     The following methods are used for solving the MOOP and managing the
     internal simulation/objective databases:
      * ``MOOP.check_sim_db(x, s_name)``
      * ``MOOP.update_sim_db(x, sx, s_name)``
      * ``MOOP.evaluateSimulation(x, s_name)``
      * ``MOOP.addData(x, sx)``
      * ``MOOP.iterate(k)``
      * ``MOOP.updateAll(k, batch)``
 
     Finally, the following methods are used to retrieve data after the
     problem has been solved:
-     * ``MOOP.getPF()``
-     * ``MOOP.getSimulationData()``
-     * ``MOOP.getObjectiveData()``
+     * ``MOOP.getPF(format='ndarray')``
+     * ``MOOP.getSimulationData(format='ndarray')``
+     * ``MOOP.getObjectiveData(format='ndarray')``
 
     The following methods are not recommended for external usage:
      * ``MOOP.__extract__(x)``
      * ``MOOP.__embed__(x)``
      * ``MOOP.__generate_encoding__()``
      * ``MOOP.__unpack_sim__(sx)``
      * ``MOOP.__pack_sim__(sx)``
      * ``MOOP.fitSurrogates()``
      * ``MOOP.updateSurrogates()``
-     * ``MOOP.evaluateSurrogates(x)``
      * ``MOOP.resetSurrogates(center)``
+     * ``MOOP.evaluateSurrogates(x)``
+     * ``MOOP.surrogateUncertainty(x)``
+     * ``MOOP.evaluateObjectives(x)``
      * ``MOOP.evaluateConstraints(x)``
      * ``MOOP.evaluatePenalty(x)``
      * ``MOOP.evaluateGradients(x)``
 
     """
 
     # Slots for the MOOP class
@@ -98,15 +101,15 @@
                  'des_names', 'obj_names', 'const_names',
                  'lam', 'epsilon', 'objectives', 'data', 'sim_funcs',
                  'sim_db', 'des_tols', 'searches', 'surrogates', 'optimizer',
                  'constraints', 'hyperparams', 'acquisitions', 'history',
                  'scale', 'scaled_lb', 'scaled_ub', 'scaled_des_tols',
                  'cat_des_tols', 'custom_des_tols', 'use_names', 'iteration',
                  'checkpoint', 'checkpointfile', 'checkpoint_data',
-                 'new_checkpoint', 'new_data']
+                 'new_checkpoint', 'new_data', 'obj_exp_vals', 'c_exp_vals']
 
     def __embed__(self, x):
         """ Embed a design input as n-dimensional vector for ParMOO.
 
         Args:
             x (numpy.ndarray or numpy structured array): Either a numpy
                 structured array (when working with named design variables)
@@ -475,14 +478,16 @@
         self.sim_funcs = []
         self.sim_db = []
         self.surrogates = []
         # Initialize the objective and constraint lists
         self.o = 0
         self.obj_names = []
         self.objectives = []
+        self.obj_exp_vals = []
+        self.c_exp_vals = []
         self.p = 0
         self.const_names = []
         self.constraints = []
         # Initialize the empty acquisition function list
         self.acquisitions = []
         # Initialize empty history dict
         self.history = {}
@@ -990,52 +995,81 @@
                    maps from R^n X R^m --> R. Interface should match:
                    `cost = obj_func(x, sim_func(x), der=0)`,
                    where `der` is an optional argument specifying whether to
                    take the derivative of the objective function
                     * 0 -- no derivative taken, return f(x, sim_func(x))
                     * 1 -- return derivative wrt x, or
                     * 2 -- return derivative wrt sim(x).
+                 * 'exp_func' (function): An algebraic objective function
+                   that calculates the expected value and distribution of
+                   an objective, given that surrogate outputs are Gaussian
+                   distributed with given mean and variance. Accepts three
+                   inputs. The first input represents x, the second input
+                   is the expected value of S(x), and the third input
+                   represents the standard deviation of S(x) -- assuming
+                   S(x) is Gaussian distributed.
+                   The output is the expected value of f(x, S).
+                   Interface should match:
+                   `cost = exp_func(x, sim_mean, sim_std_dev, der=0,
+                                    sd=False)`,
+                   where `der` is an optional argument specifying whether to
+                   evaluate the derivative
+                    * 0 -- no derivative taken, return f(x, sim_func(x))
+                    * 1 -- return derivative wrt x,
+                    * 2 -- return derivative wrt expected value of sim(x), or
+                    * 3 -- return derivative wrt std deviation of sim(x).
 
         """
 
         # Assert proper order of problem definition
         if len(self.acquisitions) > 0:
             raise RuntimeError("Cannot add more objectives after"
                                + " adding acquisition functions")
-        # Check that arg and 'obj_func' field are legal types
+        # Check that arg and 'exp_func' or 'obj_func' fields are legal types
         for arg in args:
             if not isinstance(arg, dict):
                 raise TypeError("Each arg must be a Python dict")
-            if 'obj_func' in arg:
+            if 'exp_func' in arg:
+                if callable(arg['exp_func']):
+                    if not (len(inspect.signature(arg['exp_func']).parameters)
+                            in [3, 4]):
+                        raise ValueError("The 'exp_func' must take 3 or 4"
+                                         + " arguments")
+                else:
+                    raise TypeError("The 'exp_func' must be callable")
+            elif 'obj_func' in arg:
                 if callable(arg['obj_func']):
                     if not (len(inspect.signature(arg['obj_func']).parameters)
-                            == 2 or
-                            len(inspect.signature(arg['obj_func']).parameters)
-                            == 3):
+                            in [2, 3]):
                         raise ValueError("The 'obj_func' must take 2 "
                                          + "(no derivatives) or 3 "
                                          + "(derivative option) arguments")
                 else:
                     raise TypeError("The 'obj_func' must be callable")
             else:
-                raise AttributeError("The 'obj_func' field must be "
-                                     + "present in each arg")
+                raise AttributeError("The 'exp_func' or 'obj_func' field must "
+                                     + "be present in each arg")
             # Add the objective name
             if 'name' in arg:
                 if not isinstance(arg['name'], str):
                     raise TypeError("When present, 'name' must be a string")
                 else:
                     if any([arg['name'] == dname[0]
                             for dname in self.obj_names]):
                         raise ValueError("arg['name'] must be unique")
                     self.obj_names.append((arg['name'], 'f8'))
             else:
                 self.obj_names.append(("f" + str(self.o + 1), 'f8'))
             # Finally, if all else passed, add the objective
-            self.objectives.append(arg['obj_func'])
+            if 'exp_func' in arg.keys():
+                self.objectives.append(arg['exp_func'])
+                self.obj_exp_vals.append(True)
+            else:
+                self.objectives.append(arg['obj_func'])
+                self.obj_exp_vals.append(False)
             self.o += 1
         return
 
     def addConstraint(self, *args):
         """ Add a new constraint to the MOOP.
 
         Append a new constraint to the problem. The constraint can be
@@ -1053,58 +1087,87 @@
                    negative number when feasible and positive otherwise.
                    Interface should match:
                    `violation = constraint(x, sim_func(x), der=0)`,
                    where `der` is an optional argument specifying whether to
                    take the derivative of the constraint function
                     * 0 -- no derivative taken, return c(x, sim_func(x))
                     * 1 -- return derivative wrt x, or
-                    * 2 -- return derivative wrt sim(x).
+                    * 2 -- return derivative wrt  sim(x).
                    Note that any
                    ``constraint(x, sim_func(x), der=0) <= 0``
                    indicates that x is feaseible, while
                    ``constraint(x, sim_func(x), der=0) > 0``
                    indicates that x is infeasible, violating the constraint by
                    an amount proportional to the output.
                    It is the user's responsibility to ensure that after adding
                    all constraints, the feasible region is nonempty and has
                    nonzero measure in the design space.
+                 * 'exp_func' (function): An algebraic objective function
+                   that calculates the expected value and distribution of
+                   the constraint penalty, given that surrogate outputs are
+                   Gaussian distributed with given mean and variance. Accepts
+                   three inputs. The first input represents x, the second
+                   input is the expected value of S(x), and the third input
+                   represents the standard deviation of S(x) -- assuming
+                   S(x) is Gaussian distributed.
+                   The output is the expected value of c(x, S).
+                   Interface should match:
+                   `penalty = exp_func(x, sim_mean, sim_std_dev, der=0,
+                                       sd=False)`,
+                   where `der` is an optional argument specifying whether to
+                   evaluate the derivative
+                    * 0 -- no derivative taken, return exp val c(x, Sx)
+                    * 1 -- return derivative wrt x,
+                    * 2 -- return derivative wrt expected value of sim(x), or
+                    * 3 -- return derivative wrt std deviation of sim(x).
 
         """
 
         # Check that arg and 'constraint' field are legal types
         for arg in args:
             if not isinstance(arg, dict):
                 raise TypeError("Each arg must be a Python dict")
-            if 'constraint' in arg:
+            if 'exp_func' in arg:
+                if callable(arg['exp_func']):
+                    if not (len(inspect.signature(arg['exp_func']).parameters)
+                            in [3, 4]):
+                        raise ValueError("The 'exp_func' must take 3 or 4"
+                                         + " arguments")
+                else:
+                    raise TypeError("The 'exp_func' must be callable")
+            elif 'constraint' in arg:
                 if callable(arg['constraint']):
                     if not (len(inspect.signature(arg['constraint']).
-                                parameters) == 2 or
-                            len(inspect.signature(arg['constraint']).
-                                parameters) == 3):
+                                parameters) in [2, 3]):
                         raise ValueError("The 'constraint' must take 2 "
                                          + "(no derivatives) or 3 "
                                          + "(derivative option) arguments")
                 else:
                     raise TypeError("The 'constraint' must be callable")
             else:
-                raise AttributeError("The 'constraint' field must be "
-                                     + "present in each arg")
+                raise AttributeError("The 'exp_func' or 'constraint' field "
+                                     + "must be present in each arg")
             # Add the constraint name
             if 'name' in arg:
                 if not isinstance(arg['name'], str):
                     raise TypeError("When present, 'name' must be a string")
                 else:
                     if any([arg['name'] == dname[0]
                             for dname in self.const_names]):
                         raise ValueError("arg['name'] must be unique")
                     self.const_names.append((arg['name'], 'f8'))
             else:
                 self.const_names.append(("c" + str(self.p + 1), 'f8'))
             # Finally, if all else passed, add the constraint
-            self.constraints.append(arg['constraint'])
+            if 'exp_func' in arg.keys():
+                self.constraints.append(arg['exp_func'])
+                self.c_exp_vals.append(True)
+            else:
+                self.constraints.append(arg['constraint'])
+                self.c_exp_vals.append(False)
             self.p += 1
         return
 
     def addAcquisition(self, *args):
         """ Add an acquisition function to the MOOP.
 
         Append a new acquisition function to the problem. In each iteration,
@@ -1467,14 +1530,88 @@
             try:
                 rad = min(si.setCenter(center), rad)
             except NotImplementedError:
                 rad = max(self.scaled_ub - self.scaled_lb)
         return rad
 
     def evaluateSurrogates(self, x):
+        """ Evaluate all simulation surrogates.
+
+        Warning: Not recommended for external usage!
+
+        Args:
+            x (numpy.ndarray): A 1d numpy.ndarray containing the (embedded)
+                design point to evaluate.
+
+        Returns:
+            numpy.ndarray: A 1d numpy.ndarray containing the (embedded) result
+            of the surrogate model evaluations.
+
+        """
+
+        # Check for illegal input
+        if isinstance(x, np.ndarray):
+            if x.shape[0] != self.n:
+                raise ValueError("x must have length n")
+        else:
+            raise TypeError("x must be a numpy array")
+        # Evaluate the surrogate models to approximate the simulation outputs
+        sim = np.zeros(self.m_total)
+        m_count = 0
+        for i, surrogate in enumerate(self.surrogates):
+            sim[m_count:m_count+self.m[i]] = surrogate.evaluate(x)
+            m_count += self.m[i]
+        return sim
+
+    def surrogateUncertainty(self, x, grad=False):
+        """ Evaluate uncertainty (standard deviation) of all surrogates.
+
+        Assumes a Gaussian distribution on simulation outputs.
+
+        Warning: Not recommended for external usage!
+
+        Args:
+            x (numpy.ndarray): A 1d numpy.ndarray containing the (embedded)
+                design point to evaluate.
+
+            grad (bool): Specifies whether or not to evalaute the gradients.
+
+        Returns:
+            numpy.ndarray: (When grad is False) a 1d numpy.ndarray containing
+            the std deviation of the surrogates at x. (When grad is True)
+            a 2d numpy.ndarray containing the Jacobian of gradients of
+            all surrogates uncertainties at x.
+
+        """
+
+        # Check for illegal input
+        if isinstance(x, np.ndarray):
+            if x.shape[0] != self.n:
+                raise ValueError("x must have length n")
+        else:
+            raise TypeError("x must be a numpy array")
+        # If gradient evaluation was requested
+        if grad:
+            dstdD_dx = np.zeros((self.m_total, self.n))
+            m_count = 0
+            for i, surrogate in enumerate(self.surrogates):
+                dstdD_dx[m_count:m_count+self.m[i]] = \
+                    surrogate.stdDevGrad(x)
+                m_count += self.m[i]
+            return dstdD_dx
+        # Otherwise, evaluate the surrogate standard deviations
+        else:
+            sim_stdD = np.zeros(self.m_total)
+            m_count = 0
+            for i, surrogate in enumerate(self.surrogates):
+                sim_stdD[m_count:m_count+self.m[i]] = surrogate.stdDev(x)
+                m_count += self.m[i]
+            return sim_stdD
+
+    def evaluateObjectives(self, x):
         """ Evaluate all objectives using the simulation surrogates as needed.
 
         Warning: Not recommended for external usage!
 
         Args:
             x (numpy.ndarray): A 1d numpy.ndarray containing the (embedded)
                 design point to evaluate.
@@ -1489,22 +1626,31 @@
         if isinstance(x, np.ndarray):
             if x.shape[0] != self.n:
                 raise ValueError("x must have length n")
         else:
             raise TypeError("x must be a numpy array")
         # Evaluate the surrogate models to approximate the simulation outputs
         sim = np.zeros(self.m_total)
+        sim_std_dev = np.zeros(self.m_total)
         m_count = 0
         for i, surrogate in enumerate(self.surrogates):
             sim[m_count:m_count+self.m[i]] = surrogate.evaluate(x)
+            if any(self.obj_exp_vals):
+                sim_std_dev[m_count:m_count+self.m[i]] = surrogate.stdDev(x)
             m_count += self.m[i]
         # Evaluate the objective functions
         fx = np.zeros(self.o)
         for i, obj_func in enumerate(self.objectives):
-            fx[i] = obj_func(self.__extract__(x), self.__unpack_sim__(sim))
+            if self.obj_exp_vals[i]:
+                fx[i] = obj_func(self.__extract__(x),
+                                 self.__unpack_sim__(sim),
+                                 self.__unpack_sim__(sim_std_dev))
+            else:
+                fx[i] = obj_func(self.__extract__(x),
+                                 self.__unpack_sim__(sim))
         # Return the result
         return fx
 
     def evaluateConstraints(self, x):
         """ Evaluate the constraints using the simulation surrogates as needed.
 
         Warning: Not recommended for external usage!
@@ -1528,27 +1674,36 @@
         # Special case if there are no constraints, just return [0]
         if self.p == 0:
             return np.zeros(1)
         # Otherwise, calculate the constraint violations
         else:
             # Evaluate the surrogate models to approximate the sim outputs
             sim = np.zeros(self.m_total)
+            sim_std_dev = np.zeros(self.m_total)
             m_count = 0
             for i, surrogate in enumerate(self.surrogates):
                 sim[m_count:m_count + self.m[i]] = surrogate.evaluate(x)
+                if any(self.c_exp_vals):
+                    sim_std_dev[m_count:m_count+self.m[i]] = \
+                                                    surrogate.stdDev(x)
                 m_count += self.m[i]
             # Evaluate the constraint functions
             cx = np.zeros(self.p)
             for i, constraint_func in enumerate(self.constraints):
-                cx[i] = constraint_func(self.__extract__(x),
-                                        self.__unpack_sim__(sim))
+                if self.c_exp_vals[i]:
+                    cx[i] = constraint_func(self.__extract__(x),
+                                            self.__unpack_sim__(sim),
+                                            self.__unpack_sim__(sim_std_dev))
+                else:
+                    cx[i] = constraint_func(self.__extract__(x),
+                                            self.__unpack_sim__(sim))
             # Return the constraint violations
             return cx
 
-    def evaluatePenalty(self, x):
+    def evaluatePenalty(self, x, sx=None):
         """ Evaluate the penalized objective using the surrogates as needed.
 
         Warning: Not recommended for external usage!
 
         Args:
             x (numpy.ndarray): A 1d numpy.ndarray containing the (embedded)
                 design point to evaluate.
@@ -1563,28 +1718,51 @@
         if isinstance(x, np.ndarray):
             if x.shape[0] != self.n:
                 raise ValueError("x must have length n")
         else:
             raise TypeError("x must be a numpy array")
         # Evaluate the surrogate models to approximate the simulation outputs
         sim = np.zeros(self.m_total)
-        m_count = 0
-        for i, surrogate in enumerate(self.surrogates):
-            sim[m_count:m_count+self.m[i]] = surrogate.evaluate(x)
-            m_count += self.m[i]
+        sim_std_dev = np.zeros(self.m_total)
+        if sx is None:
+            m_count = 0
+            for i, surrogate in enumerate(self.surrogates):
+                sim[m_count:m_count+self.m[i]] = surrogate.evaluate(x)
+                if any(self.obj_exp_vals) or any(self.c_exp_vals):
+                    sim_std_dev[m_count:m_count+self.m[i]] = \
+                                                    surrogate.stdDev(x)
+                m_count += self.m[i]
+        else:
+            if isinstance(sx, np.ndarray):
+                if sx.shape[0] != self.m_total:
+                    raise ValueError("sx must have length m when present")
+            else:
+                raise TypeError("sx must be a numpy array when present")
+            sim[:] = sx[:]
         # Evaluate the objective functions
         fx = np.zeros(self.o)
         for i, obj_func in enumerate(self.objectives):
-            fx[i] = obj_func(self.__extract__(x), self.__unpack_sim__(sim))
+            if self.obj_exp_vals[i]:
+                fx[i] = obj_func(self.__extract__(x),
+                                 self.__unpack_sim__(sim),
+                                 self.__unpack_sim__(sim_std_dev))
+            else:
+                fx[i] = obj_func(self.__extract__(x),
+                                 self.__unpack_sim__(sim))
         # Evaluate the constraint functions
         Lx = np.zeros(self.o)
         if self.p > 0:
-            for constraint_func in self.constraints:
-                cx = constraint_func(self.__extract__(x),
-                                     self.__unpack_sim__(sim))
+            for i, constraint_func in enumerate(self.constraints):
+                if self.c_exp_vals[i]:
+                    cx = constraint_func(self.__extract__(x),
+                                         self.__unpack_sim__(sim),
+                                         self.__unpack_sim__(sim_std_dev))
+                else:
+                    cx = constraint_func(self.__extract__(x),
+                                         self.__unpack_sim__(sim))
                 if cx > 0.0:
                     Lx[:] = Lx[:] + cx
         # Compute the penalized objective score
         Lx[:] = self.lam * Lx[:] + fx[:]
         # Return the result
         return Lx
 
@@ -1607,118 +1785,196 @@
         if isinstance(x, np.ndarray):
             if x.shape[0] != self.n:
                 raise ValueError("x must have length n")
         else:
             raise TypeError("x must be a numpy array")
         # Evaluate the surrogate models to approximate the simulation outputs
         sim = np.zeros(self.m_total)
+        sim_std_dev = np.zeros(self.m_total)
         m_count = 0
         for i, surrogate in enumerate(self.surrogates):
             sim[m_count:m_count+self.m[i]] = surrogate.evaluate(x)
+            if any(self.obj_exp_vals) or any(self.c_exp_vals):
+                sim_std_dev[m_count:m_count+self.m[i]] = surrogate.stdDev(x)
             m_count += self.m[i]
         # Evaluate the gradients of the surrogates
         if self.m_total > 0:
             dsim_dx = np.zeros((self.m_total, self.n))
+            dstdD_dx = np.zeros((self.m_total, self.n))
             m_count = 0
             for i, surrogate in enumerate(self.surrogates):
                 dsim_dx[m_count:m_count+self.m[i], :] = \
                         surrogate.gradient(x)
+                # Also standard deviation gradients
+                if any(self.obj_exp_vals) or any(self.c_exp_vals):
+                    dstdD_dx[m_count:m_count+self.m[i]] = \
+                        surrogate.stdDevGrad(x)
                 m_count += self.m[i]
         # Evaluate the gradients of the objective functions
         df_dx = np.zeros((self.o, self.n))
         for i, obj_func in enumerate(self.objectives):
             # If names are used, unpack the derivative
             if self.use_names:
-                df_dx_tmp = obj_func(self.__extract__(x),
-                                     self.__unpack_sim__(sim),
-                                     der=1)
+                if self.obj_exp_vals[i]:
+                    df_dx_tmp = obj_func(self.__extract__(x),
+                                         self.__unpack_sim__(sim),
+                                         self.__unpack_sim__(sim_std_dev),
+                                         der=1)
+                else:
+                    df_dx_tmp = obj_func(self.__extract__(x),
+                                         self.__unpack_sim__(sim),
+                                         der=1)
                 for j, d_name in enumerate(self.des_names):
                     if self.des_order[j] < self.n_cont:
                         df_dx[i, j] = df_dx_tmp[d_name[0]]
                 df_dx[i, :self.n_cont] = ((df_dx[i, self.des_order])
                                           [:self.n_cont] /
                                           self.scale[:self.n_cont])
             # Otherwise, evaluate normally
             else:
-                df_dx[i, :self.n_cont] = (obj_func(self.__extract__(x),
-                                                   self.__unpack_sim__(sim),
-                                                   der=1)[:self.n_cont] /
-                                          self.scale[:self.n_cont])
+                nn = self.n_cont
+                if self.obj_exp_vals[i]:
+                    df_dx[i, :nn] = (obj_func(self.__extract__(x),
+                                              self.__unpack_sim__(sim),
+                                              self.__unpack_sim__(sim_std_dev),
+                                              der=1)[:self.n_cont] /
+                                     self.scale[:self.n_cont])
+                else:
+                    df_dx[i, :nn] = (obj_func(self.__extract__(x),
+                                              self.__unpack_sim__(sim),
+                                              der=1)[:self.n_cont] /
+                                     self.scale[:self.n_cont])
         # Now evaluate wrt the sims
         if self.m_total > 0:
             df_dsim = np.zeros((self.o, self.m_total))
-            # If names are used, pack the sims
-            if self.use_names:
-                for i, obj_func in enumerate(self.objectives):
-                    df_dsim_tmp = obj_func(self.__extract__(x),
-                                           self.__unpack_sim__(sim),
-                                           der=2)
-                    df_dsim[i, :] = self.__pack_sim__(df_dsim_tmp)
-            else:
-                for i, obj_func in enumerate(self.objectives):
-                    df_dsim[i, :] = obj_func(self.__extract__(x),
-                                             self.__unpack_sim__(sim),
-                                             der=2)
+            for i, obj_func in enumerate(self.objectives):
+                if self.obj_exp_vals[i]:
+                    df_ds_tmp = obj_func(self.__extract__(x),
+                                         self.__unpack_sim__(sim),
+                                         self.__unpack_sim__(sim_std_dev),
+                                         der=2)
+                else:
+                    df_ds_tmp = obj_func(self.__extract__(x),
+                                         self.__unpack_sim__(sim),
+                                         der=2)
+                # If names are used, pack the sims
+                if self.use_names:
+                    df_dsim[i, :] = self.__pack_sim__(df_ds_tmp)
+                else:
+                    df_dsim[i, :] = df_ds_tmp
+        # Now evaluate wrt the std deviations
+        if any(self.obj_exp_vals):
+            df_dstdD = np.zeros((self.o, self.m_total))
+            for i, obj_func in enumerate(self.objectives):
+                if self.obj_exp_vals[i]:
+                    df_dsd_tmp = obj_func(self.__extract__(x),
+                                          self.__unpack_sim__(sim),
+                                          self.__unpack_sim__(sim_std_dev),
+                                          der=3)
+                    # If names are used, pack the sims
+                    if self.use_names:
+                        df_dstdD[i, :] = self.__pack_sim__(df_dsd_tmp)
+                    else:
+                        df_dstdD[i, :] = df_dsd_tmp
         # Finally, evaluate the full objective Jacobian
         dfx = np.zeros((self.o, self.n))
         dfx = df_dx
         if self.m_total > 0:
             dfx = dfx + np.dot(df_dsim, dsim_dx)
+        if any(self.obj_exp_vals):
+            dfx = dfx + np.dot(df_dstdD, dstdD_dx)
         # If there are no constraints, just return zeros
         dcx = np.zeros(self.n)
         # Otherwise, calculate the constraint violation Jacobian
         if self.p > 0:
             # Evaluate the constraint functions
             cx = np.zeros(self.p)
-            for i, constraint_func in enumerate(self.constraints):
-                cx[i] = constraint_func(self.__extract__(x),
-                                        self.__unpack_sim__(sim))
+            for i, const_func in enumerate(self.constraints):
+                if self.c_exp_vals[i]:
+                    cx[i] = const_func(self.__extract__(x),
+                                       self.__unpack_sim__(sim),
+                                       self.__unpack_sim__(sim_std_dev))
+                else:
+                    cx[i] = const_func(self.__extract__(x),
+                                       self.__unpack_sim__(sim))
             # Evaluate the gradients of the constraint functions
             dc_dx = np.zeros((self.p, self.n))
-            for i, constraint_func in enumerate(self.constraints):
+            for i, const_func in enumerate(self.constraints):
+                if self.c_exp_vals[i]:
+                    dc_dx_tmp = const_func(self.__extract__(x),
+                                           self.__unpack_sim__(sim),
+                                           self.__unpack_sim__(sim_std_dev),
+                                           der=1)
+                else:
+                    dc_dx_tmp = const_func(self.__extract__(x),
+                                           self.__unpack_sim__(sim),
+                                           der=1)
                 # If names are used, unpack the derivative
                 if self.use_names:
-                    dc_dx_tmp = constraint_func(self.__extract__(x),
-                                                self.__unpack_sim__(sim),
-                                                der=1)
                     for j, d_name in enumerate(self.des_names):
                         if self.des_order[j] < self.n_cont:
                             dc_dx[i, j] = dc_dx_tmp[d_name[0]]
                     dc_dx[i, :self.n_cont] = ((dc_dx[i, self.des_order])
                                               [:self.n_cont] /
                                               self.scale[:self.n_cont])
                 # Otherwise, evaluate normally
                 else:
-                    dc_dx[i, :self.n_cont] = (constraint_func(
-                                                          self.__extract__(x),
-                                                          sim,
-                                                          der=1)[:self.n_cont]
+                    dc_dx[i, :self.n_cont] = (dc_dx_tmp[:self.n_cont]
                                               / self.scale[:self.n_cont])
             # Now evaluate wrt the sims
             if self.m_total > 0:
                 dc_dsim = np.zeros((self.p, self.m_total))
                 # If names are used, sims need to be packed
                 if self.use_names:
-                    for i, constraint_func in enumerate(self.constraints):
-                        sxx = self.__unpack_sim__(sim)
-                        dc_dsim_tmp = constraint_func(self.__extract__(x),
-                                                      sxx, der=2)
+                    sxx = self.__unpack_sim__(sim)
+                    if any(self.c_exp_vals):
+                        sdxx = self.__unpack_sim__(sim_std_dev)
+                    for i, const_func in enumerate(self.constraints):
+                        if self.c_exp_vals[i]:
+                            dc_dsim_tmp = const_func(self.__extract__(x),
+                                                     sxx, sdxx, der=2)
+                        else:
+                            dc_dsim_tmp = const_func(self.__extract__(x),
+                                                     sxx, der=2)
                         dc_dsim[i, :] = self.__pack_sim__(dc_dsim_tmp)
                 # Otherwise, evaluate normally
                 else:
-                    for i, constraint_func in enumerate(self.constraints):
+                    sxx = self.__unpack_sim__(sim)
+                    if any(self.c_exp_vals):
+                        sdxx = self.__unpack_sim__(sim_std_dev)
+                    for i, const_func in enumerate(self.constraints):
+                        if self.c_exp_vals[i]:
+                            dc_dsim[i, :] = const_func(self.__extract__(x),
+                                                       sxx, sdxx, der=2)
+                        else:
+                            dc_dsim[i, :] = const_func(self.__extract__(x),
+                                                       sxx, der=2)
+            # Now evaluate wrt the std deviations
+            if any(self.c_exp_vals):
+                dc_dstdD = np.zeros((self.p, self.m_total))
+                for i, const_func in enumerate(self.constraints):
+                    if self.c_exp_vals[i]:
                         sxx = self.__unpack_sim__(sim)
-                        dc_dsim[i, :] = constraint_func(self.__extract__(x),
-                                                        sxx, der=2)
+                        sdxx = self.__unpack_sim__(sim_std_dev)
+                        dc_dsd_tmp = const_func(self.__extract__(x),
+                                                sxx, sdxx, der=3)
+                        # If names are used, pack the sims
+                        if self.use_names:
+                            dc_dstdD[i, :] = self.__pack_sim__(dc_dsd_tmp)
+                        else:
+                            dc_dstdD[i, :] = dc_dsd_tmp
             # Finally, evaluate the full Jacobian of the constraints
             for i in range(len(self.constraints)):
                 if cx[i] > 0:
                     dcx[:] = dcx[:] + dc_dx[i, :]
                     if self.m_total > 0:
                         dcx[:] = dcx[:] + np.dot(dc_dsim[i, :], dsim_dx[:, :])
+                    if self.c_exp_vals[i]:
+                        dcx[:] = dcx[:] + np.dot(dc_dstdD[i, :],
+                                                 dstdD_dx[:, :])
         # Construct the Jacobian of the penalized objective function
         dLx = np.zeros((self.o, self.n))
         for i in range(self.o):
             dLx[i, :] = dfx[i, :] + self.lam * dcx[:]
         # Return the result
         return dLx
 
@@ -1747,19 +2003,24 @@
                  * sx[m_0:m_0 + m_1] contains output(s) of sim_func[1],
                  * sx[m_0 + m_1:m_0 + m_1 + m_2] contains the output(s) for
                    sim_func[2], etc.
 
         """
 
         # Initialize the database if needed
+        if any(self.obj_exp_vals):
+            sdx = np.zeros(sx.dtype)
         if self.n_dat == 0:
             self.data['x_vals'][0, :] = self.__embed__(x)
             self.data['f_vals'] = np.zeros((1, self.o))
             for i, obj_func in enumerate(self.objectives):
-                self.data['f_vals'][0, i] = obj_func(x, sx)
+                if self.obj_exp_vals[i]:
+                    self.data['f_vals'][0, i] = obj_func(x, sx, sdx)
+                else:
+                    self.data['f_vals'][0, i] = obj_func(x, sx)
             # Check if there are constraint violations to maintain
             if self.p > 0:
                 self.data['c_vals'] = np.zeros((1, self.p))
                 for i, constraint_func in enumerate(self.constraints):
                     self.data['c_vals'][0, i] = constraint_func(x, sx)
             else:
                 self.data['c_vals'] = np.zeros((1, 1))
@@ -1770,15 +2031,18 @@
             return
         # Otherwise append the objectives
         else:
             self.data['x_vals'] = np.append(self.data['x_vals'],
                                             [self.__embed__(x)], axis=0)
             fx = np.zeros(self.o)
             for i, obj_func in enumerate(self.objectives):
-                fx[i] = obj_func(x, sx)
+                if self.obj_exp_vals[i]:
+                    fx[i] = obj_func(x, sx, sdx)
+                else:
+                    fx[i] = obj_func(x, sx)
             self.data['f_vals'] = np.append(self.data['f_vals'],
                                             [fx], axis=0)
             # Check if there are constraint violations to maintain
             if self.p > 0:
                 cx = np.zeros(self.p)
                 for i, constraint_func in enumerate(self.constraints):
                     cx[i] = constraint_func(x, sx)
@@ -1857,54 +2121,64 @@
             for i, acquisition in enumerate(self.acquisitions):
                 x0[i, :] = acquisition.setTarget(self.data,
                                                  self.evaluatePenalty,
                                                  self.history)
             # Set up the surrogate problem
             opt = self.optimizer(self.o, self.scaled_lb, self.scaled_ub,
                                  self.hyperparams)
-            opt.setObjective(self.evaluateSurrogates)
+            opt.setObjective(self.evaluateObjectives)
+            opt.setSimulation(self.evaluateSurrogates,
+                              self.surrogateUncertainty)
             opt.setPenalty(self.evaluatePenalty, self.evaluateGradients)
             opt.setConstraints(self.evaluateConstraints)
             opt.addAcquisition(*self.acquisitions)
             opt.setReset(self.resetSurrogates)
             # Solve the surrogate problem
             x_vals = opt.solve(x0)
             # Evaluate all of the simulations at the candidate solutions
             if self.s > 0:
                 # For each design in the database
                 for xi in x_vals:
                     # Check whether it has been evaluated by any simulation
                     for i in range(self.s):
                         xxi = self.__extract__(xi)
+                        # This extract embed, while redundant, is necessarry
+                        # for categorical variables to be processed correctly
+                        xxxi = self.__embed__(xxi)
                         if self.use_names:
                             namei = self.sim_names[i][0]
                         else:
                             namei = i
-                        if not any([np.all(np.abs(xi - self.__embed__(xj)) <
-                                    self.scaled_des_tols)
-                                    and namei == j for (xj, j) in batch]) \
+                        if any([np.all(np.abs(xxxi - self.__embed__(xj)) <
+                                       self.scaled_des_tols)
+                                and namei == j for (xj, j) in batch]) \
                            and self.check_sim_db(xxi, i) is None:
                             # If not, add it to the batch
                             batch.append((xxi, namei))
                         else:
                             # Try to improve surrogate (locally then globally)
-                            x_improv = self.surrogates[i].improve(xi, False)
+                            x_improv = self.surrogates[i].improve(xxxi, False)
+                            # Again, this is needed to handle categorical vars
+                            ibatch = [self.__embed__(self.__extract__(xk))
+                                      for xk in x_improv]
                             while (any([any([np.all(np.abs(self.__embed__(xj)
                                                            - xk) <
                                                     self.scaled_des_tols)
                                              and namei == j for (xj, j)
                                              in batch])
-                                        for xk in x_improv]) or
+                                        for xk in ibatch]) or
                                    any([self.check_sim_db(self.__extract__(xk),
                                                           i)
-                                        is not None for xk in x_improv])):
-                                x_improv = self.surrogates[i].improve(xi,
+                                        is not None for xk in ibatch])):
+                                x_improv = self.surrogates[i].improve(xxxi,
                                                                       True)
+                                ibatch = [self.__embed__(self.__extract__(xk))
+                                          for xk in x_improv]
                             # Add improvement points to the batch
-                            for xj in x_improv:
+                            for xj in ibatch:
                                 batch.append((self.__extract__(xj), namei))
             else:
                 # If there were no simulations, just add all points to batch
                 for xi in x_vals:
                     xxi = self.__extract__(xi)
                     if not any([np.all(np.abs(xxi - xj) < self.des_tols)
                                 for (xj, j) in batch]):
@@ -2001,15 +2275,15 @@
                 if is_shared:
                     self.addData(x, self.__unpack_sim__(sim))
         # If checkpointing is on, save the moop before continuing
         if self.checkpoint:
             self.save(filename=self.checkpointfile)
         return
 
-    def solve(self, budget):
+    def solve(self, iter_max=None, sim_max=None):
         """ Solve a MOOP using ParMOO.
 
         If desired, be sure to turn on checkpointing before starting the
         solve, using:
 
         ``MOOP.setCheckpoint(checkpoint, [checkpoint_data, filename])``
 
@@ -2019,29 +2293,63 @@
         import logging
         logging.basicConfig(level=logging.INFO,
             [format='%(asctime)s %(levelname)-8s %(message)s',
              datefmt='%Y-%m-%d %H:%M:%S'])
         ``
 
         Args:
-            budget (int): The max budget for ParMOO's internal iteration
+            iter_max (int): The max limit for ParMOO's internal iteration
                 counter. ParMOO keeps track of how many iterations it has
                 completed internally. This value k specifies the stopping
                 criteria for ParMOO.
 
         """
 
         import logging
 
-        # Check that the budget is a legal integer
-        if isinstance(budget, int):
-            if budget < 0:
-                raise ValueError("budget must be nonnegative")
-        else:
-            raise TypeError("budget must be an int type")
+        # Check that at least one budget variable was given
+        if iter_max is None and sim_max is None:
+            raise ValueError("At least one of the following arguments " +
+                             "must be set: 'iter_max' or 'sim_max'")
+        # Check that the iter_max is a legal integer
+        if isinstance(iter_max, int):
+            if iter_max < 0:
+                raise ValueError("When present, iter_max must be nonnegative")
+        elif iter_max is not None:
+            raise TypeError("When present, iter_max must be an int type")
+        # Check that the sim_max is a legal integer
+        if isinstance(sim_max, int):
+            if sim_max < 0:
+                raise ValueError("When present, sim_max must be nonnegative")
+        elif sim_max is not None:
+            raise TypeError("When present, sim_max must be an int type")
+        # Set iter_max large enough if None
+        if iter_max is None:
+            if self.s == 0:
+                raise ValueError("If 0 simulations are given, then iter_max" +
+                                 "must be provided")
+            iter_max = sim_max
+        # Count total sims to exhaust iter_max if sim_max is None
+        total_search_budget = 0
+        for search in self.searches:
+            total_search_budget += search.budget
+        if sim_max is None:
+            sim_max = total_search_budget
+            sim_max += iter_max * len(self.acquisitions) * self.s + 1
+        # Warning for the uninitiated
+        if sim_max <= total_search_budget:
+            warnings.warn("You are running ParMOO with a total search budget" +
+                          f" of {total_search_budget} and a sim_max of " +
+                          f"just {sim_max}... This will result in pure " +
+                          "design space exploration with no exploitation/" +
+                          "optimization. Consider increasing the value of " +
+                          "sim_max, decreasing your search_budget, " +
+                          "or using the iter_max stopping criteria, unless " +
+                          "you are really only interested in design space " +
+                          "exploration without exploitation/optimization.")
 
         # Print logging info summary of problem setup
         logging.info(" Beginning new run of ParMOO...")
         logging.info(" summary of settings:")
         logging.info(f"   {self.n} design dimensions")
         logging.info(f"     continuous design variables: {self.n_cont}")
         logging.info(f"     categorical design variables: {self.n_cat}")
@@ -2055,23 +2363,28 @@
             logging.info(f"     {self.searches[i].budget} search evaluations" +
                          f" in iteration 0 for simulation {i}")
         logging.info(f"   {self.o} objectives")
         logging.info(f"   {self.p} constraints")
         logging.info(f"   {len(self.acquisitions)} acquisition functions")
         logging.info("   estimated simulation evaluations per iteration:" +
                      f" {len(self.acquisitions) * self.s}")
-        logging.info(f"   iteration limit: {budget}")
+        logging.info(f"   iteration limit: {iter_max}")
+        logging.info(f"   total simulation budget: {sim_max}")
         logging.info(" Done.")
 
         # Perform iterations until budget is exceeded
         logging.info(" Entering main iteration loop:")
 
         # Reset the iteration start
         start = self.iteration
-        for k in range(start, budget + 1):
+        total_sims = 0
+        for k in range(start, iter_max + 1):
+            # Check for the sim_max stop condition
+            if total_sims >= sim_max:
+                break
             # Track iteration counter
             self.iteration = k
             # Generate a batch by running one iteration
             logging.info(f"   Iteration {self.iteration: >4}:")
             logging.info("     generating batch...")
             batch = self.iterate(self.iteration)
             logging.info(f"     {len(batch)} candidate designs generated.")
@@ -2080,28 +2393,38 @@
                 logging.info("     evaluating batch...")
                 for xi in batch:
                     (x, i) = xi
                     logging.info(f"       evaluating design: {x}" +
                                  f" for simulation: {i}...")
                     sx = self.evaluateSimulation(x, i)
                     logging.info(f"         result: {sx}")
+                    # Count total simulations taken
+                    total_sims += 1
+                    if total_sims >= sim_max:
+                        logging.info(f"   sim_max of {sim_max} reached")
                 logging.info(f"     finished evaluating {len(batch)}" +
                              " simulations.")
             logging.info("     updating models and internal databases...")
             # Update the database
             self.updateAll(self.iteration, batch)
             logging.info("   Done.")
         logging.info(" Done.")
         logging.info(f" ParMOO has successfully completed {self.iteration} " +
                      "iterations.")
         return
 
     def getPF(self, format='ndarray'):
         """ Extract nondominated and efficient sets from internal databases.
 
+        Args:
+            format (str, optional): Either 'ndarray' (default) or 'pandas',
+                in order to produce output as a numpy structured array or
+                pandas dataframe. Note: format='pandas' is only valid for
+                named inputs.
+
         Returns:
             A discrete approximation of the Pareto front and efficient set.
 
             If operating with named variables, then this is a 1d numpy
             structured array whose fields match the names for design
             variables, objectives, and constraints (if any).
 
@@ -2152,23 +2475,32 @@
             if self.n_dat > 0:
                 result = {'x_vals': np.asarray([self.__extract__(xi)
                                                 for xi in pf['x_vals']]),
                           'f_vals': pf['f_vals'].copy()}
             if self.p > 0:
                 result['c_vals'] = pf['c_vals'].copy()
         if format == 'pandas':
+            if not self.use_names:
+                raise ValueError("format='pandas' is invalid for unnamed " +
+                                 "inputs")
             return pd.DataFrame(result)
         elif format == 'ndarray':
             return result
         else:
             raise ValueError(str(format) + " is an invalid value for 'format'")
 
     def getSimulationData(self, format='ndarray'):
         """ Extract all computed simulation outputs from the MOOP's database.
 
+        Args:
+            format (str, optional): Either 'ndarray' (default) or 'pandas',
+                in order to produce output as a numpy structured array or
+                pandas dataframe. Note: format='pandas' is only valid for
+                named inputs.
+
         Returns:
             (dict or list) Either a dictionary or list of dictionaries
             containing every point where a simulation was evaluated.
 
             If operating with named variables, then the result is a dict.
             Each key is the name for a different simulation, and each value
             is a 1d numpy structured array whose keys match the
@@ -2208,15 +2540,30 @@
                         result[sname[0]][name][:] = x_vals[name][:]
                     if len(sname) == 2:
                         result[sname[0]]['out'] = self.sim_db[i]['s_vals'][:,
                                                                            0]
                     else:
                         result[sname[0]]['out'] = self.sim_db[i]['s_vals']
             if format == 'pandas':
-                return pd.DataFrame(result)
+                # For simulation data, converting to pandas is a little more
+                # complicated...
+                result_pd = {}
+                for i, snamei in enumerate(result.keys()):
+                    rtempi = {}
+                    for (name, t) in self.des_names:
+                        rtempi[name] = result[snamei][name]
+                    # Need to break apart the output column manually
+                    if self.m[i] > 1:
+                        for i in range(self.m[i]):
+                            rtempi[f'out_{i}'] = result[snamei]['out'][:, i]
+                    else:
+                        rtempi['out'] = result[snamei]['out'][:, 0]
+                    # Create dictionary of dataframes, indexed by sim names
+                    result_pd[snamei] = pd.DataFrame(rtempi)
+                return result_pd
             elif format == 'ndarray':
                 return result
             else:
                 raise ValueError(str(format) + "is an invalid value for "
                                  + "'format'")
         else:
             # Initialize result list
@@ -2229,24 +2576,31 @@
                                          for xi in self.sim_db[i]['x_vals']])
                     result.append({'x_vals': x_vals,
                                    's_vals': self.sim_db[i]['s_vals'].copy()})
                 else:
                     result.append({'x_vals': np.zeros(0),
                                    's_vals': np.zeros(0)})
             if format == 'pandas':
-                return pd.DataFrame(result)
+                raise ValueError("format='pandas' is invalid for unnamed " +
+                                 "inputs")
             elif format == 'ndarray':
                 return result
             else:
                 raise ValueError(str(format) + " is an invalid value for "
                                  + "'format'")
 
     def getObjectiveData(self, format='ndarray'):
         """ Extract all computed objective scores from this MOOP's database.
 
+        Args:
+            format (str, optional): Either 'ndarray' (default) or 'pandas',
+                in order to produce output as a numpy structured array or
+                pandas dataframe. Note: format='pandas' is only valid for
+                named inputs.
+
         Returns:
             A database of all designs that have been fully evaluated,
             and their corresponding objective scores.
 
             If operating with named variables, then this is a 1d numpy
             structured array whose fields match the names for design
             variables, objectives, and constraints (if any).
@@ -2290,14 +2644,17 @@
             if self.n_dat > 0:
                 result = {'x_vals': np.asarray([self.__extract__(xi) for
                                                 xi in self.data['x_vals']]),
                           'f_vals': self.data['f_vals'].copy()}
                 if self.p > 0:
                     result['c_vals'] = self.data['c_vals'].copy()
         if format == 'pandas':
+            if not self.use_names:
+                raise ValueError("format='pandas' is invalid for unnamed " +
+                                 "inputs")
             return pd.DataFrame(result)
         elif format == 'ndarray':
             return result
         else:
             raise ValueError(str(format) + " is an invalid value for 'format'")
 
     def save(self, filename="parmoo"):
@@ -2350,14 +2707,16 @@
                         'n_lvls': self.n_lvls,
                         'des_order': self.des_order,
                         'cat_names': self.cat_names,
                         'sim_names': self.sim_names,
                         'des_names': self.des_names,
                         'obj_names': self.obj_names,
                         'const_names': self.const_names,
+                        'obj_exp_vals': self.obj_exp_vals,
+                        'c_exp_vals': self.c_exp_vals,
                         'lam': self.lam,
                         'des_tols': self.des_tols,
                         'epsilon': self.epsilon,
                         'hyperparams': self.hyperparams,
                         'history': self.history,
                         'use_names': self.use_names,
                         'iteration': self.iteration,
@@ -2559,14 +2918,16 @@
         self.des_order = parmoo_state['des_order']
         self.cat_names = parmoo_state['cat_names']
         self.sim_names = [tuple(item) for item in parmoo_state['sim_names']]
         self.des_names = [tuple(item) for item in parmoo_state['des_names']]
         self.obj_names = [tuple(item) for item in parmoo_state['obj_names']]
         self.const_names = [tuple(item)
                             for item in parmoo_state['const_names']]
+        self.obj_exp_vals = [item for item in parmoo_state['obj_exp_vals']]
+        self.c_exp_vals = [item for item in parmoo_state['c_exp_vals']]
         self.lam = parmoo_state['lam']
         self.des_tols = parmoo_state['des_tols']
         self.epsilon = parmoo_state['epsilon']
         self.hyperparams = parmoo_state['hyperparams']
         self.history = parmoo_state['history']
         self.use_names = parmoo_state['use_names']
         self.iteration = parmoo_state['iteration']
```

### Comparing `parmoo-0.2.2/parmoo/objectives/dtlz.py` & `parmoo-0.3.0/parmoo/objectives/dtlz.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/objectives/obj_func.py` & `parmoo-0.3.0/parmoo/objectives/obj_func.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/objectives/obj_lib.py` & `parmoo-0.3.0/parmoo/objectives/obj_lib.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/searches/latin_hypercube.py` & `parmoo-0.3.0/parmoo/searches/latin_hypercube.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/simulations/dtlz.py` & `parmoo-0.3.0/parmoo/simulations/dtlz.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 """ This module contains simulation function implementations of the DTLZ test
 suite, as described in:
 
-Deb, Thiele, Laumanns, and Zitzler. "Scalable test problems for
-evolutionary multiobjective optimization" in Evolutionary Multiobjective
-Optimization, Theoretical Advances and Applications, Ch. 6 (pp. 105--145).
-Springer-Verlag, London, UK, 2005. Abraham, Jain, and Goldberg (Eds).
+ * Deb, Thiele, Laumanns, and Zitzler. "Scalable test problems for
+   evolutionary multiobjective optimization" in Evolutionary
+   Multiobjective Optimization, Theoretical Advances and Applications,
+   Ch. 6 (pp. 105--145). Springer-Verlag, London, UK, 2005. Abraham,
+   Jain, and Goldberg (Eds).
 
-One drawback of the original DTLZ problems was that their global minima
+When run with default settings, the outputs of ``dtlz{1-7}_sim`` have
+been confirmed against the outputs from the corresponding problems
+in ``pymoo`` up to 8 decimal places of precision.
+
+ * Blank and Deb. "pymoo: Multi-Objective Optimization in Python."
+   IEEE Access 8 (pp. 89497--89509). 2020.
+
+
+One drawback of the original DTLZ problems is that their global minima
 (Pareto points) always corresponded to design points that satisfy
 
 x_i = 0.5, for i = number of objectives, ..., number of design points
 
 or
 
 x_i = 0, for i = number of objectives, ..., number of design points.
@@ -19,16 +28,16 @@
 deterministic algorithms, these solutions may represent either the
 best- or worst-case scenarios.
 
 To make these problems applicable for deterministic algorithms, the
 solution sets must be configurable offset by a user-specified amount,
 as proposed in:
 
-Chang. Mathematical Software for Multiobjective Optimization Problems.
-Ph.D. dissertation, Virginia Tech, Dept. of Computer Science, 2020.
+ * Chang. Mathematical Software for Multiobjective Optimization Problems.
+   Ph.D. dissertation, Virginia Tech, Dept. of Computer Science, 2020.
 
 For the problems DTLZ8 and DTLZ9, only objective outputs are given
 by the simulation function herein. To fully define the problem, also
 use one or more of the corresponding constraint classes included in
 ``parmoo.constraints.dtlz`` [NOT YET IMPLEMENTED].
 
 The full list of simulation functions in this module includes the kernel
@@ -629,18 +638,19 @@
         """
 
         # Extract x into xx, if names are used
         xx = unpack(x, self.des_type)
         # Initialize kernel function
         ker = g2_sim(self.n, self.o, self.offset)
         # Calculate theta values
-        theta = np.zeros(self.o - 1)
-        g2x = ker(xx)
-        for i in range(self.o - 1):
-            theta[i] = np.pi * (1 + 2 * g2x * xx[i]) / (4 * (1 + g2x))
+        theta = np.zeros(self.o)
+        g2x = ker(xx)[0]
+        theta[0] = xx[0]
+        for i in range(1, self.o):
+            theta[i] = (1 + 2 * g2x * xx[i]) / (2 * (1 + g2x))
         # Initialize output array
         fx = np.zeros(self.o)
         fx[:] = (1.0 + g2x)
         # Calculate the output array
         for i in range(self.o):
             for j in range(self.o - 1 - i):
                 fx[i] *= np.cos(np.pi * theta[j] / 2)
@@ -703,18 +713,19 @@
         """
 
         # Extract x into xx, if names are used
         xx = unpack(x, self.des_type)
         # Initialize kernel function
         ker = g3_sim(self.n, self.o, self.offset)
         # Calculate theta values
-        theta = np.zeros(self.o - 1)
-        g3x = ker(xx)
-        for i in range(self.o - 1):
-            theta[i] = np.pi * (1 + 2 * g3x * xx[i]) / (4 * (1 + g3x))
+        theta = np.zeros(self.o)
+        g3x = ker(xx)[0]
+        theta[0] = xx[0]
+        for i in range(1, self.o):
+            theta[i] = (1 + 2 * g3x * xx[i]) / (2 * (1 + g3x))
         # Initialize output array
         fx = np.zeros(self.o)
         fx[:] = (1.0 + g3x)
         # Calculate the output array
         for i in range(self.o):
             for j in range(self.o - 1 - i):
                 fx[i] *= np.cos(np.pi * theta[j] / 2)
@@ -778,20 +789,19 @@
 
         # Extract x into xx, if names are used
         xx = unpack(x, self.des_type)
         # Initialize kernel function
         ker = g4_sim(self.n, self.o, self.offset)
         # Initialize first o-1 entries in the output array
         fx = np.zeros(self.o)
-        print(xx)
         fx[:self.o-1] = xx[:self.o-1]
         # Calculate kernel functions
-        gx = 1.0 + ker(xx)
+        gx = 1.0 + ker(xx)[0]
         hx = (-np.sum(xx[:self.o-1] *
-                      (1.0 + np.sin(3.0 * np.pi * xx[:self.o-1]) / gx))
+                      (1.0 + np.sin(3.0 * np.pi * xx[:self.o-1])) / gx)
                       + float(self.o))
         # Calculate the last entry in the output array
         fx[self.o-1] = gx * hx
         return fx
 
 
 class dtlz8_sim(sim_func):
```

### Comparing `parmoo-0.2.2/parmoo/simulations/sim_func.py` & `parmoo-0.3.0/parmoo/simulations/sim_func.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/simulations/simple.py` & `parmoo-0.3.0/parmoo/simulations/simple.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/surrogates/gaussian_proc.py` & `parmoo-0.3.0/parmoo/surrogates/gaussian_proc.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     This class implements a RBF surrogate with a Gaussian basis, using the
     SurrogateFunction ABC.
 
     """
 
     # Slots for the UniformRandom class
     __slots__ = ['m', 'n', 'lb', 'ub', 'x_vals', 'f_vals', 'eps', 'std_dev',
-                 'nugget', 'weights', 'mean']
+                 'nugget', 'weights', 'mean', 'v', 'w']
 
     def __init__(self, m, lb, ub, hyperparams):
         """ Constructor for the GaussRBF class.
 
         Args:
             m (int): The number of objectives to fit.
 
@@ -63,14 +63,16 @@
         self.n = self.lb.size
         self.mean = np.zeros(self.m)
         self.std_dev = 0.0
         # Create empty database
         self.x_vals = np.zeros((0, self.n))
         self.f_vals = np.zeros((0, self.m))
         self.weights = np.zeros((0, 0))
+        self.v = np.zeros((0, 0))
+        self.w = np.zeros((0, 0))
         # Check for the 'nugget' optional value in hyperparams
         if 'nugget' in hyperparams:
             if isinstance(hyperparams['nugget'], float):
                 self.nugget = hyperparams['nugget']
                 if self.nugget < 0.0:
                     raise ValueError("hyperparams['nugget'] cannot be a"
                                      + " negative number")
@@ -139,31 +141,33 @@
         # Build the Gaussian covariance matrix
         cov = self.__gaussian(cdist(self.x_vals, self.x_vals, 'euclidean'))
         # Add the nugget, if present
         if self.nugget > 0:
             for i in range(self.x_vals.shape[0]):
                 cov[i, i] = cov[i, i] + self.nugget
         # Get eigenvalue decomp to solve the SPD system with multiple RHS
-        w, v = np.linalg.eigh(cov)
+        self.w = np.zeros(cov.shape[0])
+        self.v = np.zeros(cov.shape)
+        self.w, self.v = np.linalg.eigh(cov)
         # Check the smallest singular value for a bad solution
-        sigma_n = np.min(w)
+        sigma_n = np.min(self.w)
         if sigma_n < 0.00000001:
             for i in range(self.x_vals.shape[0]):
                 cov[i, i] = cov[i, i] + 0.00000001 - sigma_n
-            w, v = np.linalg.eigh(cov)
+            self.w, self.v = np.linalg.eigh(cov)
         # Calculate RHS
         rhs = self.f_vals.copy()
         self.mean[:] = np.sum(rhs, axis=0) / rhs.shape[0]
         for i in range(rhs.shape[0]):
             rhs[i, :] = rhs[i, :] - self.mean[:]
         # Finish the solve
         self.weights = np.zeros((self.m, rhs.shape[0]))
         for i in range(self.m):
-            tmp = np.dot(v.transpose(), rhs[:, i]) / w[:]
-            self.weights[i, :] = np.dot(v, tmp)
+            tmp = np.dot(self.v.transpose(), rhs[:, i]) / self.w[:]
+            self.weights[i, :] = np.dot(self.v, tmp)
         return
 
     def update(self, x, f):
         """ Update an existing Gaussian RBF using new data.
 
         Args:
              x (numpy.ndarray): A 2d array containing the list of
@@ -200,44 +204,35 @@
         # Build the Gaussian covariance matrix
         cov = self.__gaussian(cdist(self.x_vals, self.x_vals, 'euclidean'))
         # Add the nugget, if present
         if self.nugget > 0:
             for i in range(self.x_vals.shape[0]):
                 cov[i, i] = cov[i, i] + self.nugget
         # Get eigenvalue decomp to solve the SPD system with multiple RHS
-        w, v = np.linalg.eigh(cov)
+        self.w = np.zeros(cov.shape[0])
+        self.v = np.zeros(cov.shape)
+        self.w, self.v = np.linalg.eigh(cov)
         # Check the smallest singular value for a bad solution
-        sigma_n = np.min(w)
+        sigma_n = np.min(self.w)
         if sigma_n < 0.00000001:
             for i in range(self.x_vals.shape[0]):
                 cov[i, i] = cov[i, i] + 0.00000001 - sigma_n
-            w, v = np.linalg.eigh(cov)
+            self.w, self.v = np.linalg.eigh(cov)
         # Calculate RHS
         rhs = self.f_vals.copy()
         self.mean[:] = np.sum(rhs, axis=0) / rhs.shape[0]
         for i in range(rhs.shape[0]):
             rhs[i, :] = rhs[i, :] - self.mean[:]
         # Finish the solve
         self.weights = np.zeros((self.m, rhs.shape[0]))
         for i in range(self.m):
-            tmp = np.dot(v.transpose(), rhs[:, i]) / w[:]
-            self.weights[i, :] = np.dot(v, tmp)
+            tmp = np.dot(self.v.transpose(), rhs[:, i]) / self.w[:]
+            self.weights[i, :] = np.dot(self.v, tmp)
         return
 
-    def setCenter(self, center):
-        """ This is a dummy subroutine, that does nothing for this class.
-
-        Returns:
-            float: The max of ub - lb, which could be used as the trust region
-            radius for a local optimizer, i.e., the entire design space.
-
-        """
-
-        return max(self.ub - self.lb)
-
     def evaluate(self, x):
         """ Evaluate the Gaussian RBF at a design point.
 
         Args:
             x (numpy.ndarray): A 1d array containing the design point at
                 which to the Gaussian RBF should be evaluated.
 
@@ -285,82 +280,91 @@
         # Evaluate all m gradients at x
         outs = np.zeros((self.x_vals.shape[0], self.n))
         dists = self.__gaussian(cdist(self.x_vals, [x])).flatten()
         for i, xi in enumerate(self.x_vals):
             outs[i, :] = 2.0 * (xi - x) * dists[i] / (self.std_dev ** 2.0)
         return np.dot(self.weights, outs)
 
-    def improve(self, x, global_improv):
-        """ Suggests a design to evaluate to improve the RBF model near x.
+    def stdDev(self, x):
+        """ Evaluate the standard deviation (uncertainty) of the Gaussian RBF at x.
 
         Args:
             x (numpy.ndarray): A 1d array containing the design point at
-                which the RBF should be improved.
-
-            global_improv (Boolean): When True, returns a point for global
-                improvement, ignoring the value of x.
+                which the standard deviation should be evaluated.
 
         Returns:
-            numpy.ndarray: A 2d array containing the list of design points
-            that should be evaluated to improve the RBF models.
+            numpy.ndarray: A 1d array containing the standard deviation at x.
 
         """
 
         # Check that the x is legal
         if not isinstance(x, np.ndarray):
             raise TypeError("x must be a numpy array")
         else:
             if x.size != self.n:
                 raise ValueError("x must have length n")
             elif (np.any(x < self.lb - self.eps) or
                   np.any(x > self.ub + self.eps)):
                 raise ValueError("x cannot be infeasible")
-        # Allocate the output array.
-        x_new = np.zeros(self.n)
-        if global_improv:
-            # If global improvement has been specified, randomly select a
-            # point from within the bound constraints.
-            x_new[:] = self.lb[:] + (np.random.random(self.n)
-                                     * (self.ub[:] - self.lb[:]))
-            while any([np.all(np.abs(x_new - xj) < self.eps)
-                       for xj in self.x_vals]):
-                x_new[:] = self.lb[:] + (np.random.random(self.n)
-                                         * (self.ub[:] - self.lb[:]))
+        # Get vector of Gaussian-transformed distances
+        dists = self.__gaussian(cdist(self.x_vals, [x])).flatten()
+        # Solve using previously factored Kernel matrix
+        stdd_weights = np.zeros(self.v.shape[0])
+        tmp = np.dot(self.v.transpose(), dists) / self.w[:]
+        stdd_weights[:] = np.dot(self.v, tmp)
+        # Evaluate stddev of all m surrogates at x
+        return (np.sqrt(max(self.__gaussian(0.0) -
+                            np.dot(stdd_weights, dists), 0)
+                * np.ones(self.m)))
+
+    def stdDevGrad(self, x):
+        """ Evaluate the gradient of the standard deviation of the GaussRBF at x.
+ 
+        Args:
+            x (numpy.ndarray): A 1d array containing the design point at
+                which the gradient of standard deviation should be evaluated.
+
+        Returns:
+            numpy.ndarray: A 2d array containing the Jacobian matrix of the
+            standard deviation at x.
+
+        """
+
+        # Check that the x is legal
+        if not isinstance(x, np.ndarray):
+            raise TypeError("x must be a numpy array")
         else:
-            # Find the n+1 closest points to x in the current database
-            diffs = np.asarray([np.abs(x - xj) / self.eps
-                                for xj in self.x_vals])
-            dists = np.asarray([np.amax(dj) for dj in diffs])
-            inds = np.argsort(dists)
-            diffs = diffs[inds]
-            if dists[inds[self.n]] > 1.5:
-                # Calculate the normalized sample std dev along each axis
-                stddev = np.asarray(tstd(diffs[:self.n+1], axis=0))
-                stddev[:] = np.maximum(stddev, np.ones(self.n))
-                stddev[:] = stddev[:] / np.amin(stddev)
-                # Sample within B(x, dists[inds[self.n]] / stddev)
-                rad = (dists[inds[self.n]] * self.eps) / stddev
-                x_new = np.fmin(np.fmax(2.0 * (np.random.random(self.n) - 0.5)
-                                        * rad[:] + x, self.lb), self.ub)
-                while any([np.all(np.abs(x_new - xj) < self.eps)
-                           for xj in self.x_vals]):
-                    x_new = np.fmin(np.fmax(2.0 *
-                                            (np.random.random(self.n) - 0.5)
-                                            * rad[:] + x, self.lb), self.ub)
-            else:
-                # If the n+1st nearest point is too close, use global_improv.
-                x_new[:] = self.lb[:] + np.random.random(self.n) \
-                           * (self.ub[:] - self.lb[:])
-                # If the nearest point is too close, resample.
-                while any([np.all(np.abs(x_new - xj) < self.eps)
-                           for xj in self.x_vals]):
-                    x_new[:] = self.lb[:] + (np.random.random(self.n)
-                                             * (self.ub[:] - self.lb[:]))
-        # Return the point to be sampled in a 2d array.
-        return np.asarray([x_new])
+            if x.size != self.n:
+                raise ValueError("x must have length n")
+            elif (np.any(x < self.lb - self.eps) or
+                  np.any(x > self.ub + self.eps)):
+                raise ValueError("x cannot be infeasible")
+        # Get vector of Gaussian-transformed distances
+        dists = self.__gaussian(cdist(self.x_vals, [x])).flatten()
+        # Solve using previously factored Kernel matrix
+        stdd_weights = np.zeros(self.v.shape[0])
+        tmp = np.dot(self.v.transpose(), dists) / self.w[:]
+        stdd_weights[:] = np.dot(self.v, tmp)
+        # Evaluate stddev of all m surrogates at x
+        stdd = np.sqrt(max(self.__gaussian(0.0) - np.dot(stdd_weights, dists),
+                           0))
+        # Evaluate all m gradients at x
+        kgrad = np.zeros((self.x_vals.shape[0], self.n))
+        for i, xi in enumerate(self.x_vals):
+            kgrad[i, :] = 2.0 * (xi - x) * dists[i] / (self.std_dev ** 2.0)
+        # Just return 0 when derivative is undefined (at training points)
+        if stdd < 1.0e-4:
+            result = np.zeros(self.n)
+        else:
+            result = -np.dot(kgrad.T, stdd_weights).flatten() / stdd
+        # Build Jacobian (all m rows identical)
+        jac = np.zeros((self.m, self.n))
+        for i in range(self.m):
+            jac[i, :] = result[:]
+        return jac
 
     def save(self, filename):
         """ Save important data from this class so that it can be reloaded.
 
         Args:
             filename (string): The relative or absolute path to the file
                 where all reload data should be saved.
@@ -378,14 +382,16 @@
         gp_state['lb'] = self.lb.tolist()
         gp_state['ub'] = self.ub.tolist()
         gp_state['x_vals'] = self.x_vals.tolist()
         gp_state['f_vals'] = self.f_vals.tolist()
         gp_state['eps'] = self.eps.tolist()
         gp_state['weights'] = self.weights.tolist()
         gp_state['mean'] = self.mean.tolist()
+        gp_state['v'] = self.v.tolist()
+        gp_state['w'] = self.w.tolist()
         # Save file
         with open(filename, 'w') as fp:
             json.dump(gp_state, fp)
         return
 
     def load(self, filename):
         """ Reload important data into this class after a previous save.
@@ -410,29 +416,31 @@
         self.lb = np.array(gp_state['lb'])
         self.ub = np.array(gp_state['ub'])
         self.x_vals = np.array(gp_state['x_vals'])
         self.f_vals = np.array(gp_state['f_vals'])
         self.eps = np.array(gp_state['eps'])
         self.weights = np.array(gp_state['weights'])
         self.mean = np.array(gp_state['mean'])
+        self.v = np.array(gp_state['v'])
+        self.w = np.array(gp_state['w'])
         return
 
 
 class LocalGaussRBF(SurrogateFunction):
     """ A local RBF surrogate model, using a Gaussian basis.
 
     This class implements a local RBF surrogate with a Gaussian basis,
     using the SurrogateFunction ABC.
 
     """
 
     # Slots for the UniformRandom class
     __slots__ = ['m', 'n', 'lb', 'ub', 'x_vals', 'f_vals', 'eps', 'std_dev',
                  'nugget', 'n_loc', 'loc_inds', 'tr_center', 'weights',
-                 'mean']
+                 'mean', 'v', 'w']
 
     def __init__(self, m, lb, ub, hyperparams):
         """ Constructor for the LocalGaussRBF class.
 
         Args:
             m (int): The number of objectives to fit.
 
@@ -464,14 +472,16 @@
         self.n = self.lb.size
         self.std_dev = 0.0
         # Create empty database
         self.x_vals = np.zeros((0, self.n))
         self.f_vals = np.zeros((0, self.m))
         self.weights = np.zeros((0, 0))
         self.mean = np.zeros(self.m)
+        self.v = np.zeros((0, 0))
+        self.w = np.zeros((0, 0))
         # Initialize trust-region settings
         self.tr_center = np.zeros(0)
         self.loc_inds = []
         # Check for the 'nugget' optional value in hyperparams
         if 'nugget' in hyperparams:
             if isinstance(hyperparams['nugget'], float):
                 self.nugget = hyperparams['nugget']
@@ -622,31 +632,33 @@
                                         self.x_vals[self.loc_inds, :],
                                         'euclidean'))
             # Add the nugget, if present
             if self.nugget > 0:
                 for i in range(len(self.loc_inds)):
                     cov[i, i] = cov[i, i] + self.nugget
             # Get eigenvalue decomp to solve the SPD system with multiple RHS
-            w, v = np.linalg.eigh(cov)
+            self.w = np.zeros(cov.shape[0])
+            self.v = np.zeros(cov.shape)
+            self.w, self.v = np.linalg.eigh(cov)
             # Check the smallest singular value for a bad solution
-            sigma_n = np.min(w)
+            sigma_n = np.min(self.w)
             if sigma_n < 0.00000001:
                 for i in range(len(self.loc_inds)):
                     cov[i, i] = cov[i, i] + 0.00000001 - sigma_n
-                w, v = np.linalg.eigh(cov)
+                self.w, self.v = np.linalg.eigh(cov)
             # Calculate RHS
             rhs = self.f_vals[self.loc_inds, :].copy()
             self.mean[:] = np.sum(rhs, axis=0) / rhs.shape[0]
             for i in range(rhs.shape[0]):
                 rhs[i, :] = rhs[i, :] - self.mean[:]
             # Finish the solve
             self.weights = np.zeros((self.m, rhs.shape[0]))
             for i in range(self.m):
-                tmp = np.dot(v.transpose(), rhs[:, i]) / w[:]
-                self.weights[i, :] = np.dot(v, tmp)
+                tmp = np.dot(self.v.transpose(), rhs[:, i]) / self.w[:]
+                self.weights[i, :] = np.dot(self.v, tmp)
         return self.std_dev
 
     def evaluate(self, x):
         """ Evaluate the Gaussian RBF at a design point.
 
         Args:
             x (numpy.ndarray): A 1d array containing the design point at
@@ -698,14 +710,94 @@
         outs = np.zeros((len(self.loc_inds), self.n))
         dists = self.__gaussian(cdist(self.x_vals[self.loc_inds],
                                       [x])).flatten()
         for i, xi in enumerate(self.x_vals[self.loc_inds]):
             outs[i, :] = 2.0 * (xi - x) * dists[i] / (self.std_dev ** 2.0)
         return np.dot(self.weights, outs)
 
+    def stdDev(self, x):
+        """ Evaluate the standard deviation (uncertainty) of the Gaussian RBF at x.
+
+        Args:
+            x (numpy.ndarray): A 1d array containing the design point at
+                which the standard deviation should be evaluated.
+
+        Returns:
+            numpy.ndarray: A 1d array containing the standard deviation at x.
+
+        """
+
+        # Check that the x is legal
+        if not isinstance(x, np.ndarray):
+            raise TypeError("x must be a numpy array")
+        else:
+            if x.size != self.n:
+                raise ValueError("x must have length n")
+            elif (np.any(x < self.lb - self.eps) or
+                  np.any(x > self.ub + self.eps)):
+                raise ValueError("x cannot be infeasible")
+        # Get vector of Gaussian-transformed distances
+        dists = self.__gaussian(cdist(self.x_vals[self.loc_inds],
+                                [x])).flatten()
+        # Solve using previously factored Kernel matrix
+        stdd_weights = np.zeros(self.v.shape[0])
+        tmp = np.dot(self.v.transpose(), dists) / self.w[:]
+        stdd_weights[:] = np.dot(self.v, tmp)
+        # Evaluate standard deviation of all m surrogates at x
+        return (np.sqrt(max(self.__gaussian(0.0) -
+                            np.dot(stdd_weights, dists), 0)
+                * np.ones(self.m)))
+
+    def stdDevGrad(self, x):
+        """ Evaluate the gradient of the standard deviation of the GaussRBF at x.
+ 
+        Args:
+            x (numpy.ndarray): A 1d array containing the design point at
+                which the gradient of standard deviation should be evaluated.
+
+        Returns:
+            numpy.ndarray: A 2d array containing the Jacobian matrix of the
+            standard deviation at x.
+
+        """
+
+        # Check that the x is legal
+        if not isinstance(x, np.ndarray):
+            raise TypeError("x must be a numpy array")
+        else:
+            if x.size != self.n:
+                raise ValueError("x must have length n")
+            elif (np.any(x < self.lb - self.eps) or
+                  np.any(x > self.ub + self.eps)):
+                raise ValueError("x cannot be infeasible")
+        # Get vector of Gaussian-transformed distances
+        dists = self.__gaussian(cdist(self.x_vals[self.loc_inds],
+                                      [x])).flatten()
+        # Solve using previously factored Kernel matrix
+        stdd_weights = np.zeros(self.v.shape[0])
+        tmp = np.dot(self.v.transpose(), dists) / self.w[:]
+        stdd_weights[:] = np.dot(self.v, tmp)
+        # Evaluate standard deviation of all m surrogates at x
+        stdd = np.sqrt(max(self.__gaussian(0.0) - np.dot(stdd_weights, dists),
+                           0))
+        # Evaluate all m gradients at x
+        kgrad = np.zeros((self.v.shape[0], self.n))
+        for i, xi in enumerate(self.x_vals[self.loc_inds]):
+            kgrad[i, :] = 2.0 * (xi - x) * dists[i] / (self.std_dev ** 2.0)
+        # Just return 0 when derivative is undefined (at training points)
+        if stdd < 1.0e-4:
+            result = np.zeros(self.n)
+        else:
+            result = -np.dot(kgrad.T, stdd_weights).flatten() / stdd
+        # Build Jacobian (all m rows identical)
+        jac = np.zeros((self.m, self.n))
+        for i in range(self.m):
+            jac[i, :] = result[:]
+        return jac
+
     def improve(self, x, global_improv):
         """ Suggests a design to evaluate to improve the RBF model near x.
 
         Args:
             x (numpy.ndarray): A 1d array containing the design point at
                 which the RBF should be improved.
 
@@ -742,15 +834,15 @@
             # Find the n_loc closest points to x in the current database
             diffs = np.asarray([np.abs(x - xj) / self.eps
                                 for xj in self.x_vals])
             dists = np.asarray([np.amax(dj) for dj in diffs])
             inds = np.argsort(dists)
             diffs = diffs[inds]
             if dists[inds[self.n_loc - 1]] > 1.5:
-                # Calculate the normalized sample std dev along each axis
+                # Calculate the normalized sample stddev along each axis
                 stddev = np.asarray(tstd(diffs[:self.n_loc], axis=0))
                 stddev[:] = np.maximum(stddev, np.ones(self.n))
                 stddev[:] = stddev[:] / np.amin(stddev)
                 # Sample within B(x, dists[inds[n_loc - 1]] / stddev)
                 rad = (dists[inds[self.n_loc - 1]] * self.eps) / stddev
                 x_new = np.fmin(np.fmax(2.0 * (np.random.random(self.n) - 0.5)
                                         * rad[:] + x, self.lb), self.ub)
@@ -794,14 +886,16 @@
         gp_state['ub'] = self.ub.tolist()
         gp_state['x_vals'] = self.x_vals.tolist()
         gp_state['f_vals'] = self.f_vals.tolist()
         gp_state['eps'] = self.eps.tolist()
         gp_state['tr_center'] = self.tr_center.tolist()
         gp_state['weights'] = self.weights.tolist()
         gp_state['mean'] = self.mean.tolist()
+        gp_state['v'] = self.v.tolist()
+        gp_state['w'] = self.w.tolist()
         # Save file
         with open(filename, 'w') as fp:
             json.dump(gp_state, fp)
         return
 
     def load(self, filename):
         """ Reload important data into this class after a previous save.
@@ -829,8 +923,10 @@
         self.ub = np.array(gp_state['ub'])
         self.x_vals = np.array(gp_state['x_vals'])
         self.f_vals = np.array(gp_state['f_vals'])
         self.eps = np.array(gp_state['eps'])
         self.tr_center = np.array(gp_state['tr_center'])
         self.weights = np.array(gp_state['weights'])
         self.mean = np.array(gp_state['mean'])
+        self.v = np.array(gp_state['v'])
+        self.w = np.array(gp_state['w'])
         return
```

### Comparing `parmoo-0.2.2/parmoo/surrogates/linear_model.py` & `parmoo-0.3.0/parmoo/surrogates/linear_model.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/.pytest_cache/v/cache/nodeids` & `parmoo-0.3.0/parmoo/tests/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/libe_tests/libe_funcs.py` & `parmoo-0.3.0/parmoo/tests/libe_tests/libe_funcs.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/libe_tests/test_libe_gen.py` & `parmoo-0.3.0/parmoo/tests/libe_tests/test_libe_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     moop.addObjective({'obj_func': obj2_unnamed})
     moop.addObjective({'obj_func': obj3_unnamed})
     # Add 4 acquisition functions
     for i in range(4):
         moop.addAcquisition({'acquisition': RandomConstraint})
     
     # Solve
-    moop.solve()
+    moop.solve(sim_max=200)
     assert(moop.getObjectiveData()['x_vals'].shape[0] == 200)
     
     #print(moop.getPF())
     
     # Create a libE_MOOP with named variables
     moop = libE_MOOP(LocalGPS, hyperparams={})
     # Add n design vars
@@ -76,9 +76,9 @@
     moop.addObjective({'name': "obj2", 'obj_func': obj2_named})
     moop.addObjective({'name': "obj3", 'obj_func': obj3_named})
     # Add 4 acquisition functions
     for i in range(4):
         moop.addAcquisition({'acquisition': RandomConstraint})
     
     # Solve
-    moop.solve()
+    moop.solve(sim_max=200)
     assert(moop.getObjectiveData()['x1'].shape[0] == 200)
```

### Comparing `parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz1_obj.py` & `parmoo-0.3.0/parmoo/tests/regression_tests/test_dtlz1_obj.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz1_sim.py` & `parmoo-0.3.0/parmoo/tests/regression_tests/test_dtlz1_sim.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz2_obj.py` & `parmoo-0.3.0/parmoo/tests/regression_tests/test_dtlz2_obj.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz2_sim.py` & `parmoo-0.3.0/parmoo/tests/regression_tests/test_dtlz2_sim.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                                              type="upper",
                                              bound=4.0)})
 
 # Add 10 acquisition funcitons
 for i in range(10):
     moop.addAcquisition({'acquisition': RandomConstraint, 'hyperparams': {}})
 
-# Solve the problem with 5 iterations
-moop.solve(5)
+# Solve the problem with the equivalent of 5 iterations
+moop.solve(sim_max=150)
 
 # Check that 150 simulations were evaluated
 assert(moop.getObjectiveData()['x_vals'].shape[0] == 150)
 # Check that some solutions were found
 assert(moop.getSimulationData()[0]['x_vals'].shape[0] == 150)
 assert(all([sum(fi**2) <= 4.0 for fi in moop.getPF()['f_vals']]))
```

### Comparing `parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz3_obj.py` & `parmoo-0.3.0/parmoo/tests/regression_tests/test_dtlz3_obj.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz3_sim.py` & `parmoo-0.3.0/parmoo/tests/regression_tests/test_dtlz3_sim.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz5_sim.py` & `parmoo-0.3.0/parmoo/tests/regression_tests/test_dtlz5_sim.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/regression_tests/test_infeasible_prob.py` & `parmoo-0.3.0/parmoo/tests/regression_tests/test_infeasible_prob.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/regression_tests/test_mixed_variables.py` & `parmoo-0.3.0/parmoo/tests/regression_tests/test_mixed_variables.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/regression_tests/test_user_func.py` & `parmoo-0.3.0/parmoo/tests/regression_tests/test_user_func.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/run-tests.sh` & `parmoo-0.3.0/parmoo/tests/run-tests.sh`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_const_lib.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_const_lib.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_gaussian_proc.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_gaussian_proc.py`

 * *Files 16% similar despite different names*

```diff
@@ -80,34 +80,44 @@
     with pytest.raises(ValueError):
         rbf1.improve(np.zeros(2), False)
     with pytest.raises(ValueError):
         rbf1.improve(-np.ones(3), False)
     # Check that the RBFs match on a random evaluation point
     x = np.random.random_sample((3))
     assert (all(rbf1.evaluate(x) == rbf2.evaluate(x)))
+    assert (all(rbf1.stdDev(x) == rbf2.stdDev(x)))
     # Check that the RBFs interpolate, up to 8 decimal digits of precision
     for i in range(x_vals_full.shape[0]):
         assert (np.linalg.norm(rbf1.evaluate(x_vals_full[i])-y_vals_full[i])
                 < 0.00000001)
         assert (np.linalg.norm(rbf2.evaluate(x_vals_full[i])-y_vals_full[i])
                 < 0.00000001)
+        assert (np.max(rbf1.stdDev(x_vals_full[i])) < 1.0e-4)
+        assert (np.max(rbf2.stdDev(x_vals_full[i])) < 1.0e-4)
     # Check that the RBFs compute the same grad, up to 8 digits of precision
     for i in range(x_vals_full.shape[0]):
         assert (np.linalg.norm(rbf1.gradient(x_vals_full[i]) -
                                rbf2.gradient(x_vals_full[i])) < 0.00000001)
+    for i in range(x_vals_full.shape[0]):
+        assert (np.linalg.norm(rbf1.stdDevGrad(x_vals_full[i]) -
+                               rbf2.stdDevGrad(x_vals_full[i])) < 1.0e-4)
     # Check that the RBF gradient evaluates correctly on a known dataset
     x_vals3 = np.eye(3)
     x_vals3 = np.append(x_vals3, [[0.5, 0.5, 0.5]], axis=0)
     y_vals3 = np.asarray([[np.dot(xi, xi)] for xi in x_vals3])
     rbf3 = GaussRBF(1, np.zeros(3), np.ones(3), {})
     rbf3.fit(x_vals3, y_vals3)
     rbf3.setCenter(np.zeros(3))
     y_grad_vals3 = -0.03661401 * np.ones((1, 3))
     assert (np.linalg.norm(rbf3.gradient(x_vals3[-1]) - y_grad_vals3[-1])
             < 1.0e-4)
+    # Check standard deviation calculations
+    xi = np.random.random_sample(3)
+    assert (np.all(rbf3.stdDev(xi) >= 0))
+    assert (np.any(rbf3.stdDevGrad(xi) != 0))
     # Check that the RBF generates feasible local improvement points
     for i in range(4):
         x_improv = rbf3.improve(np.zeros(3), False)
         assert (np.all(x_improv[0] <= np.ones(3)) and
                 np.all(x_improv[0] >= np.zeros(3)))
     # Check that the RBF generates feasible global improvement points
     x_improv = rbf3.improve(x_vals3[-1], True)
@@ -160,14 +170,33 @@
     rbf7.update(x_vals3, y_vals3)
     # Test save and load
     rbf6.save("parmoo.surrogate")
     rbf7.load("parmoo.surrogate")
     xx = np.random.random_sample(3)
     assert (np.all(rbf6.evaluate(xx) == rbf7.evaluate(xx)))
     os.remove("parmoo.surrogate")
+    # Generate a simple 1D RBF and check its stdDev and stdDevGrad are accurate
+    x_vals4 = np.array([[0], [1]])
+    y_vals4 = np.array([[1], [1]])
+    rbf8 = GaussRBF(1, np.zeros(1), np.ones(1), {})
+    rbf8.fit(x_vals4, y_vals4)
+    assert (np.linalg.norm(rbf8.evaluate(np.array([0.5])) - 1.0) < 1.0e-8)
+    assert (np.linalg.norm(rbf8.stdDev(np.array([0.5]))) > 1.0e-1)
+    assert (np.linalg.norm(rbf8.gradient(np.array([0.5]))) < 1.0e-8)
+    assert (np.linalg.norm(rbf8.stdDevGrad(np.array([0.5]))) < 1.0e-4)
+    xx = np.linspace(0, 1).reshape((50, 1))
+    maxind = 0
+    for i, xi in enumerate(xx):
+        if np.all(rbf8.stdDev(xi) > rbf8.stdDev(xx[maxind])):
+            maxind = i
+        if i < 25:
+            assert (np.all(rbf8.stdDevGrad(xi) >= 0))
+        else:
+            assert (np.all(rbf8.stdDevGrad(xi) <= 0))
+    assert (maxind in [24, 25])
     return
 
 
 def test_LocalGaussRBF():
     """ Test the LocalGaussRBF class in surrogates.py.
 
     Generate random x and y values for a 3D input space and 2D output space,
@@ -261,38 +290,48 @@
     with pytest.raises(ValueError):
         rbf1.improve(np.zeros(2), False)
     with pytest.raises(ValueError):
         rbf1.improve(-np.ones(3), False)
     # Check that the RBFs match on a random evaluation point
     x = np.random.random_sample((3))
     assert (all(rbf1.evaluate(x) == rbf2.evaluate(x)))
+    assert (all(rbf1.stdDev(x) == rbf2.stdDev(x)))
     # Check that the RBFs interpolate, up to 8 decimal digits of precision
     for i in range(x_vals_full.shape[0]):
         rbf1.setCenter(x_vals_full[i])
         rbf2.setCenter(x_vals_full[i])
         assert (np.linalg.norm(rbf1.evaluate(x_vals_full[i])-y_vals_full[i])
                 < 0.00000001)
         assert (np.linalg.norm(rbf2.evaluate(x_vals_full[i])-y_vals_full[i])
                 < 0.00000001)
+        assert (np.linalg.norm(rbf1.stdDev(x_vals_full[i]) < 1.0e-4))
+        assert (np.linalg.norm(rbf2.stdDev(x_vals_full[i]) < 1.0e-4))
     # Check that the RBFs compute the same grad, up to 8 digits of precision
     rbf1.setCenter(0.5 * np.ones(3))
     rbf2.setCenter(0.5 * np.ones(3))
     for i in range(x_vals_full.shape[0]):
         assert (np.linalg.norm(rbf1.gradient(x_vals_full[i]) -
                                rbf2.gradient(x_vals_full[i])) < 0.00000001)
+        assert (np.linalg.norm(rbf1.stdDevGrad(x_vals_full[i]) -
+                               rbf2.stdDevGrad(x_vals_full[i])) < 1.0e-4)
     # Check that the RBF gradient evaluates correctly on a known dataset
     x_vals3 = np.eye(3)
     x_vals3 = np.append(x_vals3, [[0.5, 0.5, 0.5]], axis=0)
     y_vals3 = np.asarray([[np.dot(xi, xi)] for xi in x_vals3])
     rbf3 = LocalGaussRBF(1, np.zeros(3), np.ones(3), {})
     rbf3.fit(x_vals3, y_vals3)
     rbf3.setCenter(x_vals3[-1])
     y_grad_vals3 = -0.08798618 * np.ones((1, 3))
     assert (np.linalg.norm(rbf3.gradient(x_vals3[-1]) - y_grad_vals3[-1])
             < 1.0e-4)
+    assert (np.linalg.norm(rbf3.stdDevGrad(x_vals3[-1]) >= 0))
+    # Check standard deviation calculations
+    xi = np.random.random_sample(3)
+    assert (np.all(rbf3.stdDev(xi) >= 0))
+    assert (np.any(rbf3.stdDevGrad(xi) != 0))
     # Check that the RBF generates feasible local improvement points
     for i in range(4):
         x_improv = rbf3.improve(np.zeros(3), False)
         assert (np.all(x_improv[0] <= np.ones(3)) and
                 np.all(x_improv[0] >= np.zeros(3)))
     # Check that the RBF generates feasible global improvement points
     x_improv = rbf3.improve(x_vals3[-1], True)
@@ -351,13 +390,33 @@
     rbf7.update(x_vals3, y_vals3)
     # Test save and load
     rbf6.save("parmoo.surrogate")
     rbf7.load("parmoo.surrogate")
     xx = np.random.random_sample(3)
     assert (np.all(rbf6.evaluate(xx) == rbf7.evaluate(xx)))
     os.remove("parmoo.surrogate")
+    # Generate a simple 1D RBF and check its stdDev and stdDevGrad are accurate
+    x_vals4 = np.array([[0], [1]])
+    y_vals4 = np.array([[1], [1]])
+    rbf8 = LocalGaussRBF(1, np.zeros(1), np.ones(1), {})
+    rbf8.fit(x_vals4, y_vals4)
+    rbf8.setCenter(np.array([0.5]))
+    assert (np.linalg.norm(rbf8.evaluate(np.array([0.5])) - 1.0) < 1.0e-8)
+    assert (np.linalg.norm(rbf8.stdDev(np.array([0.5]))) > 1.0e-1)
+    assert (np.linalg.norm(rbf8.gradient(np.array([0.5]))) < 1.0e-8)
+    assert (np.linalg.norm(rbf8.stdDevGrad(np.array([0.5]))) < 1.0e-4)
+    xx = np.linspace(0, 1).reshape((50, 1))
+    maxind = 0
+    for i, xi in enumerate(xx):
+        if np.all(rbf8.stdDev(xi) > rbf8.stdDev(xx[maxind])):
+            maxind = i
+        if i < 25:
+            assert (np.all(rbf8.stdDevGrad(xi) >= 0))
+        else:
+            assert (np.all(rbf8.stdDevGrad(xi) <= 0))
+    assert (maxind in [24, 25])
     return
 
 
 if __name__ == "__main__":
     test_GaussRBF()
     test_LocalGaussRBF()
```

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_gps_search.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_gps_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     # Initialize the problem dimensions
     n = 3
     o = 2
     lb = np.zeros(n)
     ub = np.ones(n)
     # Create the biobjective function
     def f(z): return np.asarray([-z[0] + z[1] + z[2], z[0] - z[1] + z[2]])
-    def L(z): return np.ones(2)
+    def L(z, sz=1): return f(z) + 5 * (max(0.1 - z[2], 0) + max(z[2] - 0.6, 0))
+    def S(z): return np.ones(2)
+    def SD(z): return np.zeros(2)
     def g(z): return np.ones((2, 3))
     # Create 2 acquisition functions targeting 2 "pure" solutions
     acqu1 = UniformWeights(o, lb, ub, {})
     acqu1.setTarget({}, lambda x: np.zeros(2), {})
     acqu1.weights[:] = 0.0
     acqu1.weights[0] = 1.0
     acqu2 = UniformWeights(o, lb, ub, {})
@@ -64,26 +66,25 @@
     with pytest.raises(ValueError):
         opt.setConstraints(lambda z1, z2: np.zeros(1))
     with pytest.raises(TypeError):
         opt.addAcquisition(5)
     # Add the correct objective and constraints
     opt.setObjective(f)
     opt.setConstraints(lambda z: np.asarray([0.1 - z[2], z[2] - 0.6]))
+    opt.setSimulation(S, SD)
     opt.setPenalty(L, g)
     opt.addAcquisition(acqu1, acqu2, acqu3)
     opt.setReset(lambda x: 100.0)
     # Try to solve with invalid inputs to test error handling
     with pytest.raises(TypeError):
         opt.solve(5)
     with pytest.raises(ValueError):
         opt.solve(np.zeros((3, n-1)))
     with pytest.raises(ValueError):
         opt.solve(np.zeros((4, n)))
-    with pytest.raises(ValueError):
-        opt.solve(-np.ones((3, n)))
     # Solve the surrogate problem with LocalGPS, starting from the centroid
     x = np.zeros((3, n))
     x[:] = 0.5
     (x1, x2, x3) = opt.solve(x)
     # Define the solution
     x1_soln = np.eye(n)[0]
     x1_soln[n-1] = 0.1
@@ -126,15 +127,17 @@
     # Initialize the problem dimensions
     n = 3
     o = 2
     lb = np.zeros(n)
     ub = np.ones(n)
     # Create the biobjective function
     def f(z): return np.asarray([-z[0] + z[1] + z[2], z[0] - z[1] + z[2]])
-    def L(z): return np.ones(2)
+    def L(z, sz=1): return f(z) + 5 * (max(0.1 - z[2], 0) + max(z[2] - 0.6, 0))
+    def S(z): return np.ones(2)
+    def SD(z): return np.zeros(2)
     def g(z): return np.ones((2, 3))
     # Create 2 acquisition functions targeting 2 "pure" solutions
     acqu1 = UniformWeights(o, lb, ub, {})
     acqu1.setTarget({}, lambda x: np.zeros(2), {})
     acqu1.weights[:] = 0.0
     acqu1.weights[0] = 1.0
     acqu2 = UniformWeights(o, lb, ub, {})
@@ -173,26 +176,25 @@
     with pytest.raises(ValueError):
         opt.setConstraints(lambda z1, z2: np.zeros(1))
     with pytest.raises(TypeError):
         opt.addAcquisition(5)
     # Add the correct objective and constraints
     opt.setObjective(f)
     opt.setConstraints(lambda z: np.asarray([0.1 - z[2], z[2] - 0.6]))
+    opt.setSimulation(S, SD)
     opt.setPenalty(L, g)
     opt.addAcquisition(acqu1, acqu2, acqu3)
     opt.setReset(lambda x: 100.0)
     # Try to solve with invalid inputs to test error handling
     with pytest.raises(TypeError):
         opt.solve(5)
     with pytest.raises(ValueError):
         opt.solve(np.zeros((3, n-1)))
     with pytest.raises(ValueError):
         opt.solve(np.zeros((4, n)))
-    with pytest.raises(ValueError):
-        opt.solve(-np.ones((3, n)))
     # Solve the surrogate problem with GlobalGPS, starting from the centroid
     x = np.zeros((3, n))
     x[:, :] = 0.5
     (x1, x2, x3) = opt.solve(x)
     # Define the solution
     x1_soln = np.eye(n)[0]
     x1_soln[n-1] = 0.1
```

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_latin_hypercube.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_latin_hypercube.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_lbfgsb.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_lbfgsb.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,19 @@
     lb = np.zeros(n)
     ub = np.ones(n)
 
     # Create the biobjective function and its penalty function
     def f(z):
         return np.asarray([-z[0] + z[1] + z[2], z[0] - z[1] + z[2]])
 
-    def L(z):
+    def S(z): return np.ones(1)
+
+    def SD(z): return np.zeros(1)
+
+    def L(z, sz=1):
         res = np.asarray([-z[0] + z[1] + z[2], z[0] - z[1] + z[2]])
         if z[2] < 0.1:
             res[:] = res[:] + 2.0 * (0.1 - z[2])
         if z[2] > 0.6:
             res[:] = res[:] + 2.0 * (z[2] - 0.6)
         return res
 
@@ -79,24 +83,25 @@
     with pytest.raises(TypeError):
         opt.setConstraints(5)
     with pytest.raises(ValueError):
         opt.setConstraints(lambda z1, z2: np.zeros(1))
     with pytest.raises(TypeError):
         opt.setPenalty(5, lambda z: np.zeros(1))
     with pytest.raises(ValueError):
-        opt.setPenalty(lambda z1, z2: np.zeros(1), lambda z: np.zeros(1))
+        opt.setPenalty(lambda z1, z2, z3: np.zeros(1), lambda z: np.zeros(1))
     with pytest.raises(TypeError):
         opt.setPenalty(lambda z: np.zeros(1), 5)
     with pytest.raises(ValueError):
         opt.setPenalty(lambda z: np.zeros(1), lambda z1, z2: np.zeros(1))
     with pytest.raises(TypeError):
         opt.addAcquisition(5)
     # Add the correct objective and constraints
     opt.setObjective(f)
     opt.setConstraints(lambda z: np.asarray([0.1 - z[2], z[2] - 0.6]))
+    opt.setSimulation(S, SD)
     opt.setPenalty(L, g)
     opt.addAcquisition(acqu1, acqu2, acqu3)
     opt.setReset(lambda x: 100.0)
     # Try to solve with invalid inputs to test error handling
     with pytest.raises(TypeError):
         opt.solve(5)
     with pytest.raises(ValueError):
@@ -154,15 +159,19 @@
     lb = np.zeros(n)
     ub = np.ones(n)
 
     # Create the biobjective function and its penalty function
     def f(z):
         return np.asarray([-z[0] + z[1] + z[2], z[0] - z[1] + z[2]])
 
-    def L(z):
+    def S(z): return np.ones(1)
+
+    def SD(z): return np.zeros(1)
+
+    def L(z, sz=1):
         res = np.asarray([-z[0] + z[1] + z[2], z[0] - z[1] + z[2]])
         if z[2] < 0.1:
             res[:] = res[:] + 2.0 * (0.1 - z[2])
         if z[2] > 0.6:
             res[:] = res[:] + 2.0 * (z[2] - 0.6)
         return res
 
@@ -203,28 +212,29 @@
     with pytest.raises(TypeError):
         opt.setConstraints(5)
     with pytest.raises(ValueError):
         opt.setConstraints(lambda z1, z2: np.zeros(1))
     with pytest.raises(TypeError):
         opt.setPenalty(5, lambda z: np.zeros(1))
     with pytest.raises(ValueError):
-        opt.setPenalty(lambda z1, z2: np.zeros(1), lambda z: np.zeros(1))
+        opt.setPenalty(lambda z1, z2, z3: np.zeros(1), lambda z: np.zeros(1))
     with pytest.raises(TypeError):
         opt.setPenalty(lambda z: np.zeros(1), 5)
     with pytest.raises(ValueError):
         opt.setPenalty(lambda z: np.zeros(1), lambda z1, z2: np.zeros(1))
     with pytest.raises(TypeError):
         opt.addAcquisition(5)
     with pytest.raises(TypeError):
         opt.setReset(5)
     with pytest.raises(ValueError):
         opt.setReset(lambda z1, z2: 0.0)
     # Add the correct objective and constraints
     opt.setObjective(f)
     opt.setConstraints(lambda z: np.asarray([0.1 - z[2], z[2] - 0.6]))
+    opt.setSimulation(S, SD)
     opt.setPenalty(L, g)
     opt.addAcquisition(acqu1, acqu2, acqu3)
     opt.setReset(lambda x: 100.0)
     # Try to solve with invalid inputs to test error handling
     with pytest.raises(TypeError):
         opt.solve(5)
     with pytest.raises(ValueError):
```

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_libe.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_libe.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,22 +42,22 @@
 def test_libE_MOOP():
     """ Test the libE_MOOP class from extras/libe.py.
 
     Create a problem and check that the databases are empty.
 
     """
 
+    import os
+    import pytest
     from parmoo import MOOP
     from parmoo.searches import LatinHypercube
     from parmoo.surrogates import GaussRBF
     from parmoo.acquisitions import RandomConstraint
     from parmoo.optimizers import LocalGPS
     import numpy as np
-    import os
-    import pytest
 
     try:
         from parmoo.extras.libe import libE_MOOP
     except BaseException:
         pytest.skip("libEnsemble or its dependencies not importable. " +
                     "Skipping.")
 
@@ -187,16 +187,24 @@
     # Hard code bad CL args
     import sys
     sys.argv.append("--comms")
     sys.argv.append("local")
     sys.argv.append("--nworkers")
     sys.argv.append("1")
 
-    # Solve with bad CL args
+    # Solve with unset budget vars
     with pytest.raises(ValueError):
         moop.solve()
 
+    # Solve with bad type
+    with pytest.raises(TypeError):
+        moop.solve(sim_max="100")
+
+    # Solve with bad CL args
+    with pytest.raises(ValueError):
+        moop.solve(sim_max=101)
+
 
 if __name__ == "__main__":
     test_libE_parmoo_persis_gen()
     test_libE_MOOP()
     test_libE_MOOP_bad_solve()
```

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_moop.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_moop.py`

 * *Files 3% similar despite different names*

```diff
@@ -532,15 +532,15 @@
     assert (moop2.check_sim_db(x2, "g2") is not None)
     moop2.evaluateSimulation(y2, "g2")
     assert (moop2.check_sim_db(y2, "g2") is not None)
     return
 
 
 def test_MOOP_evaluateSurrogates():
-    """ Check that the MOOP class handles evaluating objectives properly.
+    """ Check that the MOOP class handles evaluating surrogate models properly.
 
     Initialize a MOOP object and check that the evaluateSurrogates() function
     works correctly.
 
     """
 
     from parmoo import MOOP
@@ -594,37 +594,172 @@
     # Now try some bad evaluations
     with pytest.raises(TypeError):
         moop1.evaluateSurrogates(10.0)
     with pytest.raises(ValueError):
         moop1.evaluateSurrogates(np.zeros(1))
     # Now do some good evaluations and check the results
     assert (np.linalg.norm(moop1.evaluateSurrogates(np.zeros(3)) -
+                           np.asarray([0.0, np.sqrt(3.0), np.sqrt(0.75)]))
+            < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateSurrogates(np.asarray([0.5,
+                                                                0.5, 0.5]))
+                           - np.asarray([np.sqrt(0.75), np.sqrt(0.75), 0.0]))
+            < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateSurrogates(np.asarray([1.0, 0.0,
+                                                                0.0]))
+                           - np.asarray([1.0, np.sqrt(2.0), np.sqrt(0.75)]))
+            < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateSurrogates(np.asarray([0.0, 1.0,
+                                                                0.0]))
+                           - np.asarray([1.0, np.sqrt(2.0), np.sqrt(0.75)]))
+            < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateSurrogates(np.asarray([0.0, 0.0,
+                                                                1.0]))
+                           - np.asarray([1.0, np.sqrt(2.0), np.sqrt(0.75)]))
+            < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateSurrogates(np.ones(3)) -
+                           np.asarray([np.sqrt(3.0), 0.0, np.sqrt(0.75)]))
+            < 0.00000001)
+    assert (np.linalg.norm(moop1.surrogateUncertainty(np.zeros(3)))
+            < 1.0e-4)
+    assert (np.linalg.norm(moop1.surrogateUncertainty(np.asarray([0.5,
+                                                                  0.5, 0.5])))
+            < 1.0e-4)
+    assert (np.linalg.norm(moop1.surrogateUncertainty(np.asarray([1.0,
+                                                                  0.0, 0.0])))
+            < 1.0e-4)
+    assert (np.linalg.norm(moop1.surrogateUncertainty(np.asarray([0.0,
+                                                                  1.0, 0.0])))
+            < 1.0e-4)
+    assert (np.linalg.norm(moop1.surrogateUncertainty(np.asarray([0.0,
+                                                                  0.0, 1.0])))
+            < 1.0e-4)
+    assert (np.linalg.norm(moop1.surrogateUncertainty(np.ones(3))) < 1.0e-4)
+    xi = np.random.random_sample(3)
+    assert (np.linalg.norm(moop1.surrogateUncertainty(xi)) > 1.0e-4)
+    # Adjust the scale and try again
+    moop2 = MOOP(LocalGPS)
+    moop2.addDesign({'lb': -1.0, 'ub': 1.0},
+                    {'lb': 0.0, 'ub': 2.0},
+                    {'lb': -0.5, 'ub': 1.5})
+    moop2.addObjective({'obj_func': lambda x, s: x[0]},
+                       {'obj_func': lambda x, s: s[0]},
+                       {'obj_func': lambda x, s: s[1] + s[2]})
+    moop2.addSimulation(g1, g2)
+    # Evaluate some data points and fit the surrogates
+    moop2.evaluateSimulation(np.zeros(3), 0)
+    moop2.evaluateSimulation(np.zeros(3), 1)
+    moop2.evaluateSimulation(np.asarray([0.5, 0.5, 0.5]), 0)
+    moop2.evaluateSimulation(np.asarray([0.5, 0.5, 0.5]), 1)
+    moop2.evaluateSimulation(np.asarray([1.0, 0.0, 0.0]), 0)
+    moop2.evaluateSimulation(np.asarray([1.0, 0.0, 0.0]), 1)
+    moop2.evaluateSimulation(np.asarray([0.0, 1.0, 0.0]), 0)
+    moop2.evaluateSimulation(np.asarray([0.0, 1.0, 0.0]), 1)
+    moop2.evaluateSimulation(np.asarray([0.0, 0.0, 1.0]), 0)
+    moop2.evaluateSimulation(np.asarray([0.0, 0.0, 1.0]), 1)
+    moop2.evaluateSimulation(np.ones(3), 0)
+    moop2.evaluateSimulation(np.ones(3), 1)
+    moop2.fitSurrogates()
+    # Now compare evaluations against the original surrogate
+    x = moop1.__embed__(np.zeros(3))
+    xx = moop2.__embed__(np.zeros(3))
+    assert (np.linalg.norm(moop1.evaluateSurrogates(x) -
+                           moop2.evaluateSurrogates(xx)) < 0.00000001)
+    x = moop1.__embed__(np.ones(3))
+    xx = moop2.__embed__(np.ones(3))
+    assert (np.linalg.norm(moop1.evaluateSurrogates(x) -
+                           moop2.evaluateSurrogates(xx)) < 0.00000001)
+
+
+def test_MOOP_evaluateObjectives():
+    """ Check that the MOOP class handles evaluating objectives properly.
+
+    Initialize a MOOP object and check that the evaluateObjectives() function
+    works correctly.
+
+    """
+
+    from parmoo import MOOP
+    from parmoo.surrogates import GaussRBF
+    from parmoo.searches import LatinHypercube
+    from parmoo.optimizers import LocalGPS
+    import numpy as np
+    import pytest
+
+    # Create 2 SimGroups for later
+    g1 = {'n': 3,
+          'm': 1,
+          'hyperparams': {},
+          'search': LatinHypercube,
+          'sim_func': lambda x: [np.linalg.norm(x)],
+          'surrogate': GaussRBF}
+    g2 = {'n': 3,
+          'm': 2,
+          'hyperparams': {},
+          'search': LatinHypercube,
+          'sim_func': lambda x: [np.linalg.norm(x-1.0), np.linalg.norm(x-0.5)],
+          'surrogate': GaussRBF}
+    # Initialize a MOOP with 2 SimGroups and 3 objectives
+    moop1 = MOOP(LocalGPS)
+    for i in range(3):
+        moop1.addDesign({'lb': 0.0, 'ub': 1.0})
+    moop1.addSimulation(g1, g2)
+    moop1.addObjective({'obj_func': lambda x, s: x[0]},
+                       {'obj_func': lambda x, s: s[0]},
+                       {'obj_func': lambda x, s: s[1] + s[2]})
+    # Try some bad evaluations
+    with pytest.raises(TypeError):
+        moop1.evaluateSimulation(np.zeros(3), 0.0)
+    with pytest.raises(ValueError):
+        moop1.evaluateSimulation(np.zeros(3), -1)
+    # Evaluate some data points and fit the surrogates
+    moop1.evaluateSimulation(np.zeros(3), 0)
+    moop1.evaluateSimulation(np.zeros(3), 1)
+    moop1.evaluateSimulation(np.array([0.5, 0.5, 0.5]), 0)
+    moop1.evaluateSimulation(np.array([0.5, 0.5, 0.5]), 1)
+    moop1.evaluateSimulation(np.array([1.0, 0.0, 0.0]), 0)
+    moop1.evaluateSimulation(np.array([1.0, 0.0, 0.0]), 1)
+    moop1.evaluateSimulation(np.array([0.0, 1.0, 0.0]), 0)
+    moop1.evaluateSimulation(np.array([0.0, 1.0, 0.0]), 1)
+    moop1.evaluateSimulation(np.array([0.0, 0.0, 1.0]), 0)
+    moop1.evaluateSimulation(np.array([0.0, 0.0, 1.0]), 1)
+    moop1.evaluateSimulation(np.ones(3), 0)
+    moop1.evaluateSimulation(np.ones(3), 1)
+    moop1.fitSurrogates()
+    moop1.resetSurrogates(np.ones(3) * 0.5)
+    # Now try some bad evaluations
+    with pytest.raises(TypeError):
+        moop1.evaluateObjectives(10.0)
+    with pytest.raises(ValueError):
+        moop1.evaluateObjectives(np.zeros(1))
+    # Now do some good evaluations and check the results
+    assert (np.linalg.norm(moop1.evaluateObjectives(np.zeros(3)) -
                            np.asarray([0.0, 0.0, np.sqrt(3.0) +
                                        np.sqrt(0.75)]))
             < 0.00000001)
-    assert (np.linalg.norm(moop1.evaluateSurrogates(np.asarray([0.5,
+    assert (np.linalg.norm(moop1.evaluateObjectives(np.asarray([0.5,
                                                                 0.5, 0.5]))
                            - np.asarray([0.5, np.sqrt(0.75), np.sqrt(0.75)]))
             < 0.00000001)
-    assert (np.linalg.norm(moop1.evaluateSurrogates(np.asarray([1.0, 0.0,
+    assert (np.linalg.norm(moop1.evaluateObjectives(np.asarray([1.0, 0.0,
                                                                 0.0]))
                            - np.asarray([1.0, 1.0, np.sqrt(2.0) +
                                          np.sqrt(0.75)]))
             < 0.00000001)
-    assert (np.linalg.norm(moop1.evaluateSurrogates(np.asarray([0.0, 1.0,
+    assert (np.linalg.norm(moop1.evaluateObjectives(np.asarray([0.0, 1.0,
                                                                 0.0]))
                            - np.asarray([0.0, 1.0, np.sqrt(2.0) +
                                          np.sqrt(0.75)]))
             < 0.00000001)
-    assert (np.linalg.norm(moop1.evaluateSurrogates(np.asarray([0.0, 0.0,
+    assert (np.linalg.norm(moop1.evaluateObjectives(np.asarray([0.0, 0.0,
                                                                 1.0]))
                            - np.asarray([0.0, 1.0, np.sqrt(2.0) +
                                          np.sqrt(0.75)]))
             < 0.00000001)
-    assert (np.linalg.norm(moop1.evaluateSurrogates(np.ones(3)) -
+    assert (np.linalg.norm(moop1.evaluateObjectives(np.ones(3)) -
                            np.asarray([1.0, np.sqrt(3.0), np.sqrt(0.75)]))
             < 0.00000001)
     # Adjust the scale and try again
     moop2 = MOOP(LocalGPS)
     moop2.addDesign({'lb': -1.0, 'ub': 1.0},
                     {'lb': 0.0, 'ub': 2.0},
                     {'lb': -0.5, 'ub': 1.5})
@@ -645,20 +780,20 @@
     moop2.evaluateSimulation(np.asarray([0.0, 0.0, 1.0]), 1)
     moop2.evaluateSimulation(np.ones(3), 0)
     moop2.evaluateSimulation(np.ones(3), 1)
     moop2.fitSurrogates()
     # Now compare evaluations against the original surrogate
     x = moop1.__embed__(np.zeros(3))
     xx = moop2.__embed__(np.zeros(3))
-    assert (np.linalg.norm(moop1.evaluateSurrogates(x) -
-                           moop2.evaluateSurrogates(xx)) < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateObjectives(x) -
+                           moop2.evaluateObjectives(xx)) < 0.00000001)
     x = moop1.__embed__(np.ones(3))
     xx = moop2.__embed__(np.ones(3))
-    assert (np.linalg.norm(moop1.evaluateSurrogates(x) -
-                           moop2.evaluateSurrogates(xx)) < 0.00000001)
+    assert (np.linalg.norm(moop1.evaluateObjectives(x) -
+                           moop2.evaluateObjectives(xx)) < 0.00000001)
 
 
 def test_MOOP_evaluateConstraints():
     """ Check that the MOOP class handles evaluating constraints properly.
 
     Initialize a MOOP object and check that the evaluateConstraints() function
     works correctly.
@@ -1381,27 +1516,27 @@
     for i in range(3):
         moop.addAcquisition({'acquisition': UniformWeights})
     # Solve the MOOP and extract the final database with 6 iterations
     moop.data = {'x_vals': np.zeros((5, 4)),
                  'f_vals': np.zeros((5, 3)),
                  'c_vals': np.zeros((5, 1))}
     moop.data['x_vals'][0, :] = np.asarray([0.0, 0.0, 0.0, 0.0])
-    moop.data['f_vals'][0, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][0, :] = moop.evaluateObjectives(
                                    np.asarray([0.0, 0.0, 0.0, 0.0]))
     moop.data['x_vals'][1, :] = np.asarray([1.0, 0.0, 0.0, 0.0])
-    moop.data['f_vals'][1, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][1, :] = moop.evaluateObjectives(
                                    np.asarray([1.0, 0.0, 0.0, 0.0]))
     moop.data['x_vals'][2, :] = np.asarray([0.0, 1.0, 0.0, 0.0])
-    moop.data['f_vals'][2, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][2, :] = moop.evaluateObjectives(
                                    np.asarray([0.0, 1.0, 0.0, 0.0]))
     moop.data['x_vals'][3, :] = np.asarray([0.0, 0.0, 1.0, 0.0])
-    moop.data['f_vals'][3, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][3, :] = moop.evaluateObjectives(
                                    np.asarray([0.0, 0.0, 1.0, 0.0]))
     moop.data['x_vals'][4, :] = np.asarray([0.0, 0.0, 0.0, 1.0])
-    moop.data['f_vals'][4, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][4, :] = moop.evaluateObjectives(
                                    np.asarray([0.0, 0.0, 0.0, 1.0]))
     moop.n_dat = 5
     soln = moop.getPF()
     assert (soln['f_vals'].shape == (4, 3))
     # Create a toy problem with 4 design variables
     moop = MOOP(LocalGPS, hyperparams={})
     for i in range(4):
@@ -1424,35 +1559,35 @@
     for i in range(3):
         moop.addAcquisition({'acquisition': UniformWeights})
     # Solve the MOOP and extract the final database with 6 iterations
     moop.data = {'x_vals': np.zeros((5, 4)),
                  'f_vals': np.zeros((5, 3)),
                  'c_vals': np.zeros((5, 1))}
     moop.data['x_vals'][0, :] = np.asarray([0.0, 0.0, 0.0, 0.0])
-    moop.data['f_vals'][0, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][0, :] = moop.evaluateObjectives(
                                    np.asarray([0.0, 0.0, 0.0, 0.0]))
     moop.data['c_vals'][0, :] = moop.evaluateConstraints(
                                    np.asarray([0.0, 0.0, 0.0, 0.0]))
     moop.data['x_vals'][1, :] = np.asarray([1.0, 0.0, 0.0, 0.0])
-    moop.data['f_vals'][1, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][1, :] = moop.evaluateObjectives(
                                    np.asarray([1.0, 0.0, 0.0, 0.0]))
     moop.data['c_vals'][1, :] = moop.evaluateConstraints(
                                    np.asarray([1.0, 0.0, 0.0, 0.0]))
     moop.data['x_vals'][2, :] = np.asarray([0.0, 1.0, 0.0, 0.0])
-    moop.data['f_vals'][2, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][2, :] = moop.evaluateObjectives(
                                    np.asarray([0.0, 1.0, 0.0, 0.0]))
     moop.data['c_vals'][2, :] = moop.evaluateConstraints(
                                    np.asarray([0.0, 1.0, 0.0, 0.0]))
     moop.data['x_vals'][3, :] = np.asarray([0.0, 0.0, 1.0, 0.0])
-    moop.data['f_vals'][3, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][3, :] = moop.evaluateObjectives(
                                    np.asarray([0.0, 0.0, 1.0, 0.0]))
     moop.data['c_vals'][3, :] = moop.evaluateConstraints(
                                    np.asarray([0.0, 0.0, 1.0, 0.0]))
     moop.data['x_vals'][4, :] = np.asarray([0.0, 0.0, 0.0, 1.0])
-    moop.data['f_vals'][4, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][4, :] = moop.evaluateObjectives(
                                    np.asarray([0.0, 0.0, 0.0, 1.0]))
     moop.data['c_vals'][4, :] = moop.evaluateConstraints(
                                    np.asarray([0.0, 0.0, 0.0, 1.0]))
     moop.n_dat = 5
     soln = moop.getPF()
     assert (soln.shape[0] == 4)
 
@@ -1578,35 +1713,35 @@
     for i in range(3):
         moop.addAcquisition({'acquisition': UniformWeights})
     # Solve the MOOP and extract the final database with 6 iterations
     moop.data = {'x_vals': np.zeros((5, 4)),
                  'f_vals': np.zeros((5, 3)),
                  'c_vals': np.zeros((5, 1))}
     moop.data['x_vals'][0, :] = np.asarray([0.0, 0.0, 0.0, 0.0])
-    moop.data['f_vals'][0, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][0, :] = moop.evaluateObjectives(
                                    np.asarray([0.0, 0.0, 0.0, 0.0]))
     moop.data['c_vals'][0, :] = moop.evaluateConstraints(
                                    np.asarray([0.0, 0.0, 0.0, 0.0]))
     moop.data['x_vals'][1, :] = np.asarray([1.0, 0.0, 0.0, 0.0])
-    moop.data['f_vals'][1, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][1, :] = moop.evaluateObjectives(
                                    np.asarray([1.0, 0.0, 0.0, 0.0]))
     moop.data['c_vals'][1, :] = moop.evaluateConstraints(
                                    np.asarray([1.0, 0.0, 0.0, 0.0]))
     moop.data['x_vals'][2, :] = np.asarray([0.0, 1.0, 0.0, 0.0])
-    moop.data['f_vals'][2, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][2, :] = moop.evaluateObjectives(
                                    np.asarray([0.0, 1.0, 0.0, 0.0]))
     moop.data['c_vals'][2, :] = moop.evaluateConstraints(
                                    np.asarray([0.0, 1.0, 0.0, 0.0]))
     moop.data['x_vals'][3, :] = np.asarray([0.0, 0.0, 1.0, 0.0])
-    moop.data['f_vals'][3, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][3, :] = moop.evaluateObjectives(
                                    np.asarray([0.0, 0.0, 1.0, 0.0]))
     moop.data['c_vals'][3, :] = moop.evaluateConstraints(
                                    np.asarray([0.0, 0.0, 1.0, 0.0]))
     moop.data['x_vals'][4, :] = np.asarray([0.0, 0.0, 0.0, 1.0])
-    moop.data['f_vals'][4, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][4, :] = moop.evaluateObjectives(
                                    np.asarray([0.0, 0.0, 0.0, 1.0]))
     moop.data['c_vals'][4, :] = moop.evaluateConstraints(
                                    np.asarray([0.0, 0.0, 0.0, 1.0]))
     moop.n_dat = 5
     soln = moop.getObjectiveData()
     assert (soln['f_vals'].shape == (5, 3))
     # Create a toy problem with 4 design variables
@@ -1631,35 +1766,35 @@
     for i in range(3):
         moop.addAcquisition({'acquisition': UniformWeights})
     # Solve the MOOP and extract the final database with 6 iterations
     moop.data = {'x_vals': np.zeros((5, 4)),
                  'f_vals': np.zeros((5, 3)),
                  'c_vals': np.zeros((5, 1))}
     moop.data['x_vals'][0, :] = np.asarray([0.0, 0.0, 0.0, 0.0])
-    moop.data['f_vals'][0, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][0, :] = moop.evaluateObjectives(
                                    np.asarray([0.0, 0.0, 0.0, 0.0]))
     moop.data['c_vals'][0, :] = moop.evaluateConstraints(
                                    np.asarray([0.0, 0.0, 0.0, 0.0]))
     moop.data['x_vals'][1, :] = np.asarray([1.0, 0.0, 0.0, 0.0])
-    moop.data['f_vals'][1, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][1, :] = moop.evaluateObjectives(
                                    np.asarray([1.0, 0.0, 0.0, 0.0]))
     moop.data['c_vals'][1, :] = moop.evaluateConstraints(
                                    np.asarray([1.0, 0.0, 0.0, 0.0]))
     moop.data['x_vals'][2, :] = np.asarray([0.0, 1.0, 0.0, 0.0])
-    moop.data['f_vals'][2, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][2, :] = moop.evaluateObjectives(
                                    np.asarray([0.0, 1.0, 0.0, 0.0]))
     moop.data['c_vals'][2, :] = moop.evaluateConstraints(
                                    np.asarray([0.0, 1.0, 0.0, 0.0]))
     moop.data['x_vals'][3, :] = np.asarray([0.0, 0.0, 1.0, 0.0])
-    moop.data['f_vals'][3, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][3, :] = moop.evaluateObjectives(
                                    np.asarray([0.0, 0.0, 1.0, 0.0]))
     moop.data['c_vals'][3, :] = moop.evaluateConstraints(
                                    np.asarray([0.0, 0.0, 1.0, 0.0]))
     moop.data['x_vals'][4, :] = np.asarray([0.0, 0.0, 0.0, 1.0])
-    moop.data['f_vals'][4, :] = moop.evaluateSurrogates(
+    moop.data['f_vals'][4, :] = moop.evaluateObjectives(
                                    np.asarray([0.0, 0.0, 0.0, 1.0]))
     moop.data['c_vals'][4, :] = moop.evaluateConstraints(
                                    np.asarray([0.0, 0.0, 0.0, 1.0]))
     moop.n_dat = 5
     soln = moop.getObjectiveData()
     assert (soln.shape[0] == 5)
 
@@ -1987,14 +2122,15 @@
     test_pack_unpack_sim()
     test_MOOP_addObjective()
     test_MOOP_addConstraint()
     test_MOOP_addAcquisition()
     test_MOOP_getTypes()
     test_MOOP_evaluateSimulation()
     test_MOOP_evaluateSurrogates()
+    test_MOOP_evaluateObjectives()
     test_MOOP_evaluateConstraints()
     test_MOOP_addData()
     test_MOOP_iterate()
     test_MOOP_solve()
     test_MOOP_getPF()
     test_MOOP_getSimulationData()
     test_MOOP_getObjectiveData()
```

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_moop_embeddings.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_moop_embeddings.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_moop_grads.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_moop_grads.py`

 * *Files 0% similar despite different names*

```diff
@@ -450,15 +450,17 @@
     moop2.addObjective({'obj_func': f1})
     moop2.addObjective({'obj_func': f2})
     moop2.addConstraint({'constraint': c1})
     moop2.addConstraint({'constraint': c2})
     moop2.addAcquisition({'acquisition': FixedWeights})
     np.random.seed(0)
     moop2.solve(0)
+    np.random.seed(0)
     b1 = moop1.iterate(1)
+    np.random.seed(0)
     b2 = moop2.iterate(1)
     # Check that same solutions were found
     for x1, x2 in zip(b1, b2):
         assert (np.all(np.abs(x1[0] - x2[0]) < 0.1))
 
 
 if __name__ == "__main__":
```

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_obj_dtlz.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_obj_dtlz.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_obj_lib.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_obj_lib.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_random_search.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_random_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     # Initialize the problem dimensions
     n = 3
     o = 2
     lb = np.zeros(n)
     ub = np.ones(n)
     # Create the biobjective function
     def f(z): return np.asarray([-z[0] + z[1] + z[2], z[0] - z[1] + z[2]])
-    def L(z): return np.ones(2)
+    def L(z, sz=1): return f(z)
+    def S(z): return np.ones(2)
+    def SD(z): return np.zeros(2)
     def g(z): return np.ones((2, 3))
     # Create 2 acquisition functions targeting 2 "pure" solutions
     acqu1 = UniformWeights(o, lb, ub, {})
     acqu1.setTarget({}, lambda x: np.zeros(2), {})
     acqu1.weights[:] = 0.0
     acqu1.weights[0] = 1.0
     acqu2 = UniformWeights(o, lb, ub, {})
@@ -64,26 +66,25 @@
     with pytest.raises(ValueError):
         opt.setConstraints(lambda z1, z2: np.zeros(1))
     with pytest.raises(TypeError):
         opt.addAcquisition(5)
     # Add the correct objective and constraints
     opt.setObjective(f)
     opt.setConstraints(lambda z: np.asarray([0.1 - z[2], z[2] - 0.6]))
+    opt.setSimulation(S, SD)
     opt.setPenalty(L, g)
     opt.addAcquisition(acqu1, acqu2, acqu3)
     opt.setReset(lambda x: 100.0)
     # Try to solve with invalid inputs to test error handling
     with pytest.raises(TypeError):
         opt.solve(5)
     with pytest.raises(ValueError):
         opt.solve(np.zeros((3, n-1)))
     with pytest.raises(ValueError):
         opt.solve(np.zeros((4, n)))
-    with pytest.raises(ValueError):
-        opt.solve(-np.ones((3, n)))
     # Solve the surrogate problem with RandomSearch, starting from the centroid
     x = np.zeros((3, n))
     x[:] = 0.5
     (x1, x2, x3) = opt.solve(x)
     # Define the solution
     x1_soln = np.eye(n)[0]
     x1_soln[n-1] = 0.1
```

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_sims_dtlz.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_sims_dtlz.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_sims_simple.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_sims_simple.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_structs.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_structs.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_util.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_util.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_viz_without_dash.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_viz_without_dash.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/tests/unit_tests/test_weighted_sum.py` & `parmoo-0.3.0/parmoo/tests/unit_tests/test_weighted_sum.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,46 +27,58 @@
                        lambda x: np.zeros(3), {})
     with pytest.raises(ValueError):
         acqu.setTarget({'x_vals': np.ones((1, 4)), 'f_vals': np.ones((1, 1))},
                        lambda x: np.zeros(3), {})
     with pytest.raises(TypeError):
         acqu.setTarget({}, 4, {})
     with pytest.raises(ValueError):
-        acqu.setTarget({}, lambda x, y: np.zeros(3), {})
+        acqu.setTarget({}, lambda x, y, z: np.zeros(3), {})
     # Set a good target for future usage
     x0 = acqu.setTarget({}, lambda x: np.zeros(3), {})
     assert (abs(sum(acqu.weights) - 1.0) < 0.00000001)
     assert (np.all(x0[:] <= acqu.ub) and np.all(x0[:] >= acqu.lb))
     # Try some bad scalarizations to test error handling
     with pytest.raises(TypeError):
-        acqu.scalarize(5)
+        acqu.scalarize(5, 5, 5, 5)
     with pytest.raises(ValueError):
-        acqu.scalarize(np.ones(2))
+        acqu.scalarize(np.ones(2), np.ones(2), np.ones(2), np.ones(2))
     # Generate 3 random weight vector
     acqu1 = UniformWeights(3, np.zeros(4), np.ones(4), {})
     acqu1.setTarget({}, lambda x: np.zeros(3), {})
     acqu2 = UniformWeights(3, np.zeros(4), np.ones(4), {})
     acqu2.setTarget({}, lambda x: np.zeros(3), {})
     acqu3 = UniformWeights(3, np.zeros(4), np.ones(4), {})
     acqu3.setTarget({'x_vals': None, 'f_vals': None},
                     lambda x: np.zeros(3), {})
     # Check that the weights are all greater than 0
     assert (all(acqu1.weights[:] >= 0.0))
     assert (all(acqu2.weights[:] >= 0.0))
     assert (all(acqu3.weights[:] >= 0.0))
     # Use the scalarization function to check that the weights sum to 1
-    assert (np.abs(acqu1.scalarize(np.eye(3)[0])
-                   + acqu1.scalarize(np.eye(3)[1])
-                   + acqu1.scalarize(np.eye(3)[2]) - 1.0) < 0.00000001)
-    assert (np.abs(acqu2.scalarize(np.eye(3)[0])
-                   + acqu2.scalarize(np.eye(3)[1])
-                   + acqu2.scalarize(np.eye(3)[2]) - 1.0) < 0.00000001)
-    assert (np.abs(acqu3.scalarize(np.eye(3)[0])
-                   + acqu3.scalarize(np.eye(3)[1])
-                   + acqu3.scalarize(np.eye(3)[2]) - 1.0) < 0.00000001)
+    assert (np.abs(acqu1.scalarize(np.eye(3)[0], np.ones(2),
+                                   np.ones(2), np.ones(2))
+                   + acqu1.scalarize(np.eye(3)[1], np.ones(2),
+                                     np.ones(2), np.ones(2))
+                   + acqu1.scalarize(np.eye(3)[2], np.ones(2),
+                                     np.ones(2), np.ones(2)) - 1.0)
+            < 0.00000001)
+    assert (np.abs(acqu2.scalarize(np.eye(3)[0], np.ones(2),
+                                   np.ones(2), np.ones(2))
+                   + acqu2.scalarize(np.eye(3)[1], np.ones(2),
+                                     np.ones(2), np.ones(2))
+                   + acqu2.scalarize(np.eye(3)[2], np.ones(2),
+                                     np.ones(2), np.ones(2)) - 1.0)
+            < 0.00000001)
+    assert (np.abs(acqu3.scalarize(np.eye(3)[0], np.ones(2),
+                                   np.ones(2), np.ones(2))
+                   + acqu3.scalarize(np.eye(3)[1], np.ones(2),
+                                     np.ones(2), np.ones(2))
+                   + acqu3.scalarize(np.eye(3)[2], np.ones(2),
+                                     np.ones(2), np.ones(2)) - 1.0)
+            < 0.00000001)
     # Try some bad gradient scalarizations to test error handling
     with pytest.raises(TypeError):
         acqu.scalarizeGrad(5, np.zeros((3, 4))[0])
     with pytest.raises(ValueError):
         acqu.scalarizeGrad(np.ones(2), np.zeros((3, 4)))
     with pytest.raises(TypeError):
         acqu.scalarizeGrad(np.eye(3)[0], 5)
@@ -118,34 +130,39 @@
                        lambda x: np.zeros(3), {})
     with pytest.raises(ValueError):
         acqu.setTarget({'x_vals': np.ones((1, 4)), 'f_vals': np.ones((1, 1))},
                        lambda x: np.zeros(3), {})
     with pytest.raises(TypeError):
         acqu.setTarget({}, 4, {})
     with pytest.raises(ValueError):
-        acqu.setTarget({}, lambda x, y: np.zeros(3), {})
+        acqu.setTarget({}, lambda x, y, z: np.zeros(3), {})
     # Set some good targets
     x0 = acqu.setTarget({'x_vals': None, 'f_vals': None},
                         lambda x: np.zeros(3), {})
     assert (np.all(x0[:] <= acqu.ub) and np.all(x0[:] >= acqu.lb))
     x0 = acqu.setTarget({'x_vals': np.zeros((1, 4)),
                          'f_vals': np.zeros((1, 3)),
                          'c_vals': np.zeros((1, 1))},
                         lambda x: np.zeros(3), {})
     assert (np.all(x0[:] <= acqu.ub) and np.all(x0[:] >= acqu.lb))
     x0 = acqu.setTarget({}, lambda x: np.zeros(3), {})
     assert (np.all(x0[:] <= acqu.ub) and np.all(x0[:] >= acqu.lb))
     # Try some bad scalarizations to test error handling
     with pytest.raises(TypeError):
-        acqu.scalarize(5)
+        acqu.scalarize(5, 5, 5, 5)
     with pytest.raises(ValueError):
-        acqu.scalarize(np.ones(2))
+        acqu.scalarize(np.ones(2), np.ones(2), np.ones(2), np.ones(2))
     # Use the scalarization function to check that the weights sum to 1
-    assert (np.abs(acqu.scalarize(np.eye(3)[0]) + acqu.scalarize(np.eye(3)[1])
-                   + acqu.scalarize(np.eye(3)[2]) - 1.0) < 0.00000001)
+    assert (np.abs(acqu.scalarize(np.eye(3)[0], np.ones(2),
+                                  np.ones(2), np.ones(2))
+                   + acqu.scalarize(np.eye(3)[1], np.ones(2),
+                                    np.ones(2), np.ones(2))
+                   + acqu.scalarize(np.eye(3)[2], np.ones(2),
+                                    np.ones(2), np.ones(2)) - 1.0)
+            < 0.00000001)
     # Try some bad gradient scalarizations to test error handling
     with pytest.raises(TypeError):
         acqu.scalarizeGrad(5, np.zeros((3, 4))[0])
     with pytest.raises(ValueError):
         acqu.scalarizeGrad(np.ones(2), np.zeros((3, 4)))
     with pytest.raises(TypeError):
         acqu.scalarizeGrad(np.eye(3)[0], 5)
```

### Comparing `parmoo-0.2.2/parmoo/util.py` & `parmoo-0.3.0/parmoo/util.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/viz/dashboard.py` & `parmoo-0.3.0/parmoo/viz/dashboard.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/viz/graph.py` & `parmoo-0.3.0/parmoo/viz/graph.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/viz/plot.py` & `parmoo-0.3.0/parmoo/viz/plot.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo/viz/utilities.py` & `parmoo-0.3.0/parmoo/viz/utilities.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.2/parmoo.egg-info/PKG-INFO` & `parmoo-0.3.0/parmoo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: parmoo
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python library for parallel multiobjective simulation optimization
 Home-page: https://github.com/parmoo/parmoo
 Author: Tyler H. Chang, Stefan M. Wild, et al.
 Author-email: parmoo@mcs.anl.gov
 License: BSD 3-clause
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
@@ -37,9 +36,7 @@
 
 ParMOO also seeks to exploit structure in simulation optimization problems,
 by modeling simulations separately from surrogates.
 
 
 ParMOO is distributed under a BSD 3-clause license.
 
-
-
```

### Comparing `parmoo-0.2.2/parmoo.egg-info/SOURCES.txt` & `parmoo-0.3.0/parmoo.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 setup.py
 docs/Makefile
 docs/REQUIREMENTS.txt
 docs/about.rst
 docs/api.rst
 docs/conf.py
 docs/extras.rst
+docs/faqs.rst
 docs/how-to-write.rst
 docs/index.rst
 docs/install.rst
 docs/latex_index.rst
 docs/make.bat
 docs/quickstart.rst
 docs/refs.rst
@@ -50,26 +51,30 @@
 docs/modules/simulations.rst
 docs/modules/structs.rst
 docs/modules/surrogates.rst
 docs/modules/util.rst
 docs/modules/viz.rst
 docs/tutorials/basic-tutorials.rst
 docs/tutorials/libe-tutorial.rst
+docs/tutorials/local_method.rst
 examples/Makefile
-examples/Pareto Front.jpeg
 examples/advanced_ex.out
 examples/advanced_ex.py
 examples/checkpointing.out
 examples/checkpointing.py
 examples/libe_basic_ex.out
 examples/libe_basic_ex.py
+examples/local_method.csv
+examples/local_method.jpeg
+examples/local_method.py
 examples/named_var_ex.out
 examples/named_var_ex.py
 examples/precomputed_data.out
 examples/precomputed_data.py
+examples/quickstart.jpeg
 examples/quickstart.out
 examples/quickstart.py
 examples/unnamed_var_ex.out
 examples/unnamed_var_ex.py
 parmoo/__init__.py
 parmoo/moop.py
 parmoo/structs.py
@@ -132,14 +137,15 @@
 parmoo/tests/unit_tests/test_gaussian_proc.py
 parmoo/tests/unit_tests/test_gps_search.py
 parmoo/tests/unit_tests/test_latin_hypercube.py
 parmoo/tests/unit_tests/test_lbfgsb.py
 parmoo/tests/unit_tests/test_libe.py
 parmoo/tests/unit_tests/test_moop.py
 parmoo/tests/unit_tests/test_moop_embeddings.py
+parmoo/tests/unit_tests/test_moop_ev.py
 parmoo/tests/unit_tests/test_moop_grads.py
 parmoo/tests/unit_tests/test_obj_dtlz.py
 parmoo/tests/unit_tests/test_obj_lib.py
 parmoo/tests/unit_tests/test_random_search.py
 parmoo/tests/unit_tests/test_sims_dtlz.py
 parmoo/tests/unit_tests/test_sims_simple.py
 parmoo/tests/unit_tests/test_structs.py
```

### Comparing `parmoo-0.2.2/setup.py` & `parmoo-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     install_requires=["numpy", "scipy", "pyDOE", "pandas"],
 
     # If run tests through setup.py - downloads these but does not install
     tests_require=["pytest", "pytest-cov", "flake8"],
 
     extras_require={
-        'extras': ["libensemble", "plotly", "dash", "kaleido"],
+        'extras': ["libensemble==0.9.3", "plotly", "dash", "kaleido"],
         'docs': ["sphinx", "sphinxcontrib.bibtex", "sphinx_rtd_theme"]},
 
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
```

