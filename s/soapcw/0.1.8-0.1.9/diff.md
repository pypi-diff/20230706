# Comparing `tmp/soapcw-0.1.8.tar.gz` & `tmp/soapcw-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soapcw-0.1.8.tar", last modified: Wed Jul  5 17:11:50 2023, max compression
+gzip compressed data, was "soapcw-0.1.9.tar", last modified: Thu Jul  6 15:47:03 2023, max compression
```

## Comparing `soapcw-0.1.8.tar` & `soapcw-0.1.9.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:11:50.229467 soapcw-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-05 17:01:34.000000 soapcw-0.1.8/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     3508 2023-07-05 17:01:34.000000 soapcw-0.1.8/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-05 17:01:34.000000 soapcw-0.1.8/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-05 17:01:34.000000 soapcw-0.1.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-05 17:01:34.000000 soapcw-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2446 2023-07-05 17:11:50.229467 soapcw-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1377 2023-07-05 17:01:34.000000 soapcw-0.1.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:11:50.217466 soapcw-0.1.8/docs/
--rw-rw-rw-   0 root         (0) root         (0)      605 2023-07-05 17:01:34.000000 soapcw-0.1.8/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-05 17:01:34.000000 soapcw-0.1.8/docs/authors.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:11:50.218466 soapcw-0.1.8/docs/cnn_usage/
--rw-rw-rw-   0 root         (0) root         (0)     5902 2023-07-05 17:01:34.000000 soapcw-0.1.8/docs/cnn_usage/data_generation.rst
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-05 17:01:34.000000 soapcw-0.1.8/docs/cnn_usage/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5625 2023-07-05 17:01:34.000000 soapcw-0.1.8/docs/cnn_usage/train_model.rst
--rwxrwxrwx   0 root         (0) root         (0)     4930 2023-07-05 17:01:34.000000 soapcw-0.1.8/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-05 17:01:34.000000 soapcw-0.1.8/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-05 17:01:34.000000 soapcw-0.1.8/docs/history.rst
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-07-05 17:01:34.000000 soapcw-0.1.8/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-05 17:01:34.000000 soapcw-0.1.8/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-07-05 17:01:34.000000 soapcw-0.1.8/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:11:50.218466 soapcw-0.1.8/docs/pipeline_usage/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-05 17:01:34.000000 soapcw-0.1.8/docs/pipeline_usage/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     6633 2023-07-05 17:01:34.000000 soapcw-0.1.8/docs/pipeline_usage/run_pipeline.rst
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-05 17:01:34.000000 soapcw-0.1.8/docs/readme.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:11:50.218466 soapcw-0.1.8/docs/usage/
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-07-05 17:01:34.000000 soapcw-0.1.8/docs/usage/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:11:50.220466 soapcw-0.1.8/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 17:08:40.000000 soapcw-0.1.8/pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:11:50.220466 soapcw-0.1.8/pipeline/css/
--rw-rw-rw-   0 root         (0) root         (0)     3163 2023-07-05 17:01:34.000000 soapcw-0.1.8/pipeline/css/general.css
--rwxrwxrwx   0 root         (0) root         (0)     7001 2023-07-05 17:01:34.000000 soapcw-0.1.8/pipeline/make_dag_files_astro.py
--rwxrwxrwx   0 root         (0) root         (0)     6963 2023-07-05 17:01:34.000000 soapcw-0.1.8/pipeline/make_dag_files_lines.py
--rw-rw-rw-   0 root         (0) root         (0)    38283 2023-07-05 17:01:34.000000 soapcw-0.1.8/pipeline/make_html_page.py
--rwxrwxrwx   0 root         (0) root         (0)    37055 2023-07-05 17:01:34.000000 soapcw-0.1.8/pipeline/run_full_soap_astro.py
--rwxrwxrwx   0 root         (0) root         (0)    40172 2023-07-05 17:01:34.000000 soapcw-0.1.8/pipeline/run_full_soap_lines.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:11:50.220466 soapcw-0.1.8/pipeline/scripts/
--rw-rw-rw-   0 root         (0) root         (0)    18806 2023-07-05 17:01:34.000000 soapcw-0.1.8/pipeline/scripts/table_scripts.js
--rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-05 17:01:34.000000 soapcw-0.1.8/pipeline/soap_config_parser.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2023-07-05 17:11:50.230467 soapcw-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4209 2023-07-05 17:01:34.000000 soapcw-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:11:50.223466 soapcw-0.1.8/soapcw/
--rw-rw-rw-   0 root         (0) root         (0)      589 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:11:50.225467 soapcw-0.1.8/soapcw/cnn/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cnn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cnn/cnn_data_dag_gen.py
--rwxrwxrwx   0 root         (0) root         (0)    17946 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cnn/cnn_data_gen.py
--rw-rw-rw-   0 root         (0) root         (0)    12490 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cnn/generate_gaussian_train_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11006 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cnn/generate_test_data.py
--rw-rw-rw-   0 root         (0) root         (0)    20005 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cnn/generate_train_data.py
--rwxrwxrwx   0 root         (0) root         (0)     5822 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cnn/narrowband_sfts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:11:50.226467 soapcw-0.1.8/soapcw/cnn/pytorch/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cnn/pytorch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4307 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cnn/pytorch/load_models.py
--rw-rw-rw-   0 root         (0) root         (0)    15950 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cnn/pytorch/models.py
--rw-rw-rw-   0 root         (0) root         (0)    14308 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cnn/train_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:11:50.227467 soapcw-0.1.8/soapcw/cw/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cw/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42241 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cw/generate_data.py
--rw-rw-rw-   0 root         (0) root         (0)    19576 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cw/load_sfts.py
--rw-rw-rw-   0 root         (0) root         (0)     8660 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cw/make_sfts.py
--rw-rw-rw-   0 root         (0) root         (0)     9450 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cw/sft.py
--rw-rw-rw-   0 root         (0) root         (0)     8567 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cw/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/cw/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:11:50.228467 soapcw-0.1.8/soapcw/line_aware_stat/
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/line_aware_stat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11721 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/line_aware_stat/gen_lookup.pyx
--rw-rw-rw-   0 root         (0) root         (0)    38004 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/line_aware_stat/gen_lookup_python.py
--rwxrwxrwx   0 root         (0) root         (0)     6514 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/line_aware_stat/save_lookup.py
--rw-rw-rw-   0 root         (0) root         (0)     4237 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/soap_config_parser.py
--rw-r--r--   0 root         (0) root         (0)  2271838 2023-07-05 17:11:49.000000 soapcw-0.1.8/soapcw/soapcw.c
--rw-rw-rw-   0 root         (0) root         (0)    65928 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/soapcw.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:11:50.228467 soapcw-0.1.8/soapcw/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 17:08:40.000000 soapcw-0.1.8/soapcw/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2885 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/tools/plots.py
--rw-rw-rw-   0 root         (0) root         (0)     9044 2023-07-05 17:01:34.000000 soapcw-0.1.8/soapcw/tools/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:11:50.224466 soapcw-0.1.8/soapcw.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2446 2023-07-05 17:11:50.000000 soapcw-0.1.8/soapcw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1829 2023-07-05 17:11:50.000000 soapcw-0.1.8/soapcw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:11:50.000000 soapcw-0.1.8/soapcw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      484 2023-07-05 17:11:50.000000 soapcw-0.1.8/soapcw.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:11:50.000000 soapcw-0.1.8/soapcw.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-05 17:11:50.000000 soapcw-0.1.8/soapcw.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 17:11:50.000000 soapcw-0.1.8/soapcw.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:11:50.229467 soapcw-0.1.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)   445283 2023-07-05 17:01:34.000000 soapcw-0.1.8/tests/SNR_injections.ipynb
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-05 17:01:34.000000 soapcw-0.1.8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2023-07-05 17:01:34.000000 soapcw-0.1.8/tests/test_cwload.py
--rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-05 17:01:34.000000 soapcw-0.1.8/tests/test_line_aware_stat.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2023-07-05 17:01:34.000000 soapcw-0.1.8/tests/test_soap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.500949 soapcw-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-05 17:01:34.000000 soapcw-0.1.9/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3508 2023-07-05 17:01:34.000000 soapcw-0.1.9/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-05 17:01:34.000000 soapcw-0.1.9/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-05 17:01:34.000000 soapcw-0.1.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-05 17:01:34.000000 soapcw-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-07-06 15:47:03.500949 soapcw-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2023-07-06 15:28:59.000000 soapcw-0.1.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.487949 soapcw-0.1.9/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      605 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/authors.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.488949 soapcw-0.1.9/docs/cnn_usage/
+-rw-rw-rw-   0 root         (0) root         (0)     5902 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/cnn_usage/data_generation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/cnn_usage/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5625 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/cnn_usage/train_model.rst
+-rwxrwxrwx   0 root         (0) root         (0)     4930 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.488949 soapcw-0.1.9/docs/pipeline_usage/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/pipeline_usage/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6633 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/pipeline_usage/run_pipeline.rst
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/readme.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.488949 soapcw-0.1.9/docs/usage/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-07-05 17:01:34.000000 soapcw-0.1.9/docs/usage/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.489949 soapcw-0.1.9/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 15:44:48.000000 soapcw-0.1.9/pipeline/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.489949 soapcw-0.1.9/pipeline/css/
+-rw-rw-rw-   0 root         (0) root         (0)     3163 2023-07-05 17:01:34.000000 soapcw-0.1.9/pipeline/css/general.css
+-rwxrwxrwx   0 root         (0) root         (0)     7001 2023-07-05 17:01:34.000000 soapcw-0.1.9/pipeline/make_dag_files_astro.py
+-rwxrwxrwx   0 root         (0) root         (0)     6963 2023-07-05 17:01:34.000000 soapcw-0.1.9/pipeline/make_dag_files_lines.py
+-rw-rw-rw-   0 root         (0) root         (0)    38283 2023-07-05 17:01:34.000000 soapcw-0.1.9/pipeline/make_html_page.py
+-rwxrwxrwx   0 root         (0) root         (0)    37058 2023-07-06 15:04:52.000000 soapcw-0.1.9/pipeline/run_full_soap_astro.py
+-rwxrwxrwx   0 root         (0) root         (0)    40172 2023-07-05 17:01:34.000000 soapcw-0.1.9/pipeline/run_full_soap_lines.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.489949 soapcw-0.1.9/pipeline/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)    18806 2023-07-05 17:01:34.000000 soapcw-0.1.9/pipeline/scripts/table_scripts.js
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-05 17:01:34.000000 soapcw-0.1.9/pipeline/soap_config_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-06 15:47:03.501949 soapcw-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4209 2023-07-05 17:01:34.000000 soapcw-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.492949 soapcw-0.1.9/soapcw/
+-rw-rw-rw-   0 root         (0) root         (0)      589 2023-07-06 15:04:52.000000 soapcw-0.1.9/soapcw/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.494949 soapcw-0.1.9/soapcw/cnn/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/cnn_data_dag_gen.py
+-rwxrwxrwx   0 root         (0) root         (0)    17948 2023-07-06 15:04:52.000000 soapcw-0.1.9/soapcw/cnn/cnn_data_gen.py
+-rw-rw-rw-   0 root         (0) root         (0)    12490 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/generate_gaussian_train_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11006 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/generate_test_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    20005 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/generate_train_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     5822 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/narrowband_sfts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.495949 soapcw-0.1.9/soapcw/cnn/pytorch/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/pytorch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4307 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/pytorch/load_models.py
+-rw-rw-rw-   0 root         (0) root         (0)    15950 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cnn/pytorch/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    14625 2023-07-06 15:04:52.000000 soapcw-0.1.9/soapcw/cnn/train_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.497949 soapcw-0.1.9/soapcw/cw/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cw/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    43688 2023-07-06 14:43:01.000000 soapcw-0.1.9/soapcw/cw/generate_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    19576 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cw/load_sfts.py
+-rw-rw-rw-   0 root         (0) root         (0)     8660 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cw/make_sfts.py
+-rw-rw-rw-   0 root         (0) root         (0)     9450 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cw/sft.py
+-rw-rw-rw-   0 root         (0) root         (0)     8567 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cw/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/cw/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.498949 soapcw-0.1.9/soapcw/line_aware_stat/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/line_aware_stat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11721 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/line_aware_stat/gen_lookup.pyx
+-rw-rw-rw-   0 root         (0) root         (0)    38004 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/line_aware_stat/gen_lookup_python.py
+-rwxrwxrwx   0 root         (0) root         (0)     6514 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/line_aware_stat/save_lookup.py
+-rw-rw-rw-   0 root         (0) root         (0)     4237 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/soap_config_parser.py
+-rw-r--r--   0 root         (0) root         (0)  2271838 2023-07-06 15:47:02.000000 soapcw-0.1.9/soapcw/soapcw.c
+-rw-rw-rw-   0 root         (0) root         (0)    65928 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/soapcw.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.498949 soapcw-0.1.9/soapcw/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 15:44:48.000000 soapcw-0.1.9/soapcw/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/tools/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     9044 2023-07-05 17:01:34.000000 soapcw-0.1.9/soapcw/tools/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.493949 soapcw-0.1.9/soapcw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-07-06 15:47:03.000000 soapcw-0.1.9/soapcw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-07-06 15:47:03.000000 soapcw-0.1.9/soapcw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 15:47:03.000000 soapcw-0.1.9/soapcw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      484 2023-07-06 15:47:03.000000 soapcw-0.1.9/soapcw.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 15:47:03.000000 soapcw-0.1.9/soapcw.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-06 15:47:03.000000 soapcw-0.1.9/soapcw.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-06 15:47:03.000000 soapcw-0.1.9/soapcw.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:47:03.499949 soapcw-0.1.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)   445283 2023-07-05 17:01:34.000000 soapcw-0.1.9/tests/SNR_injections.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-05 17:01:34.000000 soapcw-0.1.9/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2023-07-05 17:01:34.000000 soapcw-0.1.9/tests/test_cwload.py
+-rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-05 17:01:34.000000 soapcw-0.1.9/tests/test_line_aware_stat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2023-07-05 17:01:34.000000 soapcw-0.1.9/tests/test_soap.py
```

### Comparing `soapcw-0.1.8/CONTRIBUTING.rst` & `soapcw-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/LICENSE` & `soapcw-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/PKG-INFO` & `soapcw-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soapcw
-Version: 0.1.8
+Version: 0.1.9
 Summary: SOAP is a rapid algorithm to search for continuous sources of gravitational waves, with a wider application to long duration narrowband signals.
 Home-page: https://git.ligo.org/joseph.bayley/soapcw
 Author: Joe Bayley
 Author-email: joseph.bayley@glasgow.ac.uk
 License: MIT license
 Download-URL: https://git.ligo.org/joseph.bayley/soapcw/-/archive/0.1.2/soapcw-0.1.2.tar.gz
 Keywords: soapcw,soap,gravitational waves,pulsars,neutron stars,continuous waves
```

### Comparing `soapcw-0.1.8/README.rst` & `soapcw-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/docs/Makefile` & `soapcw-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/docs/cnn_usage/data_generation.rst` & `soapcw-0.1.9/docs/cnn_usage/data_generation.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/docs/cnn_usage/train_model.rst` & `soapcw-0.1.9/docs/cnn_usage/train_model.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/docs/conf.py` & `soapcw-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/docs/index.rst` & `soapcw-0.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/docs/installation.rst` & `soapcw-0.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/docs/make.bat` & `soapcw-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/docs/pipeline_usage/run_pipeline.rst` & `soapcw-0.1.9/docs/pipeline_usage/run_pipeline.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/pipeline/css/general.css` & `soapcw-0.1.9/pipeline/css/general.css`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/pipeline/make_dag_files_astro.py` & `soapcw-0.1.9/pipeline/make_dag_files_astro.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/pipeline/make_dag_files_lines.py` & `soapcw-0.1.9/pipeline/make_dag_files_lines.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/pipeline/make_html_page.py` & `soapcw-0.1.9/pipeline/make_html_page.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/pipeline/run_full_soap_astro.py` & `soapcw-0.1.9/pipeline/run_full_soap_astro.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,22 +129,22 @@
                                         config["transitionmatrix"]["det2_prob"])
 
     # run soap search using the two detector line aware statistic (one detector in gaps)
 
     if len(getattr(sft,"det_names")) == 2:
         # SOAP using SNR based statistic
         if config["lookuptable"]["lookup_type"] == "power":
-            soaprun = soap.two_detector(tr,sft.H1.downsamp_summed_norm_sft_power[:,ind_start:ind_end],sft.L1.downsamp_summed_norm_sft_power[:,ind_start:ind_end],lookup_file_2det=lookup_2,lookup_file_1det=lookup_1)
+            soaprun = soap.two_detector(tr,sft.H1.downsamp_summed_norm_sft_power[:,ind_start:ind_end],sft.L1.downsamp_summed_norm_sft_power[:,ind_start:ind_end],lookup_table_2det=lookup_2,lookup_table_1det=lookup_1)
         elif config["lookuptable"]["lookup_type"] == "amplitude":
             # SOAP using amplitude statistics
             # get the ratio of duty cycle and noise floor of the two detectors (used if using amplitude based statistic_
             fractions = 1./(sft.L1.summed_dutycycle*sft.H1.summed_rng_med/(sft.H1.summed_dutycycle*sft.L1.summed_rng_med))
             # where there is no data (i.e. nans) set the detectors to equal sensitivity
             fractions[np.isnan(fractions)] = 1
-            soaprun = soap.two_detector(tr,sft.H1.downsamp_summed_norm_sft_power[:,ind_start:ind_end],sft.L1.downsamp_summed_norm_sft_power[:,ind_start:ind_end],lookup_file_2det=lookup_2,fractions = fractions)
+            soaprun = soap.two_detector(tr,sft.H1.downsamp_summed_norm_sft_power[:,ind_start:ind_end],sft.L1.downsamp_summed_norm_sft_power[:,ind_start:ind_end],lookup_table_2det=lookup_2,fractions = fractions)
 
     else:
         raise Exception(f"Only runs for two detectors currently, you have: {getattr(sft, 'det_names')}")
 
     return soaprun
 
 def load_sft_band(config, filenames, minfreq, maxfreq, tmin, tmax, verbose = False):
```

### Comparing `soapcw-0.1.8/pipeline/run_full_soap_lines.py` & `soapcw-0.1.9/pipeline/run_full_soap_lines.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/pipeline/scripts/table_scripts.js` & `soapcw-0.1.9/pipeline/scripts/table_scripts.js`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/pipeline/soap_config_parser.py` & `soapcw-0.1.9/pipeline/soap_config_parser.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/setup.cfg` & `soapcw-0.1.9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [bumpversion]
 current_version = 0.1.8
+new_version = 0.1.9
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
 
@@ -17,15 +18,15 @@
 [flake8]
 exclude = docs
 
 [aliases]
 
 [metadata]
 name = soapcw
-version = 0.1.8
+version = 0.1.9
 
 [options]
 packages = soapcw, pipeline
 
 [options.entry_points]
 console_scripts = 
 	soapcw-make-dag-files-lines = pipeline.make_dag_files_lines:main
```

### Comparing `soapcw-0.1.8/setup.py` & `soapcw-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/__init__.py` & `soapcw-0.1.9/soapcw/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import
 """Top-level package for soapcw."""
 
 __author__ = """Joe Bayley"""
 __email__ = 'joseph.bayley@glasgow.ac.uk'
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 from .soapcw import single_detector, two_detector, three_detector, single_detector_gaps
 from .tools import tools, plots
 from .cnn import __init__
 from .line_aware_stat import __init__
 from .cw import __init__
 from . import soap_config_parser
```

### Comparing `soapcw-0.1.8/soapcw/cnn/cnn_data_dag_gen.py` & `soapcw-0.1.9/soapcw/cnn/cnn_data_dag_gen.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/cnn/cnn_data_gen.py` & `soapcw-0.1.9/soapcw/cnn/cnn_data_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     # set the transition matrix as likely to be in the same bin in each detector and slightyl more probable to go straight (mostly so it goest straight through gaps)
     #tr = soap.tools.transition_matrix_2d_5(1.0000001,1.000001,1e400,1e400,log=True)
     tr = soap.tools.transition_matrix_2d(1.00000001,1e400,1e400)
 
 
     if "stats" in save_options:
         # run two detector search using the line aware statistic
-        viterbi = soap.two_detector(tr,datah,datal,lookup_file_2det=lookup_2,lookup_file_1det=lookup_1)
+        viterbi = soap.two_detector(tr,datah,datal,lookup_table_2det=lookup_2,lookup_table_1det=lookup_1)
 
     roll_track_sub = viterbi.vit_track - np.roll(viterbi.vit_track, 1)
     if np.any(np.abs(roll_track_sub[3:-3]) > 3):
         print("diff of track >1")
         print(viterbi.vit_track)
         sys.exit()
```

### Comparing `soapcw-0.1.8/soapcw/cnn/generate_gaussian_train_data.py` & `soapcw-0.1.9/soapcw/cnn/generate_gaussian_train_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/cnn/generate_test_data.py` & `soapcw-0.1.9/soapcw/cnn/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/cnn/generate_train_data.py` & `soapcw-0.1.9/soapcw/cnn/generate_train_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/cnn/narrowband_sfts.py` & `soapcw-0.1.9/soapcw/cnn/narrowband_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/cnn/pytorch/load_models.py` & `soapcw-0.1.9/soapcw/cnn/pytorch/load_models.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/cnn/pytorch/models.py` & `soapcw-0.1.9/soapcw/cnn/pytorch/models.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/cnn/train_model.py` & `soapcw-0.1.9/soapcw/cnn/train_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,17 +96,19 @@
 
         if self.nfile_load != "all":
             self.noise_filenames = self.noise_filenames[:self.nfile_load]
             self.signal_filenames = self.signal_filenames[:self.nfile_load]
 
 
 def train_batch(model, optimiser, loss_fn, batch_data, batch_labels, model_type="spectrogram", train=True, device="cpu"):
-    model.train(train)
     if train:
+        model.train()
         optimiser.zero_grad()
+    else:
+        model.eval()
 
     if model_type in ["spectrogram", "vitmapspectrogram"]:
         output = model(torch.Tensor(batch_data[0]).to(device))
         loss = loss_fn(output, batch_labels.to(device).to(torch.float32))
         if train:
             loss.backward()
             optimiser.step()
@@ -127,15 +129,18 @@
         train (bool, optional): _description_. Defaults to True.
         device (str, optional): _description_. Defaults to "cpu".
         n_train_multi_size (int, optional): number of times to split up the time axis, 3 with split into N/1, N/2 and N/3. Defaults to 2.
 
     Returns:
         _type_: _description_
     """
-    model.train(train)
+    if train:
+        model.train()
+    else:
+        model.eval()
 
     nsize = batch_data[0].size(-1)
     
     total_loss = []
 
     for i in range(n_train_multi_size):
         seglen = int(nsize/(i+1))
@@ -281,15 +286,18 @@
                 print(f"batch_time: {batch_time}")
 
         print(f"mean_batch_time: {np.mean(batch_times)}")
         
         with torch.no_grad():
             val_losses = []
             for i, (batch_data, batch_labels) in enumerate(validation_dataset):
-                vloss = train_batch(model, optimiser, loss_fn, batch_data, batch_labels, train=False, device=device)    
+                if n_train_multi_size is not None:
+                    vloss = train_multi_batch(model, optimiser, loss_fn, batch_data, batch_labels, train=False, device=device, n_train_multi_size=n_train_multi_size)
+                else:
+                    vloss = train_batch(model, optimiser, loss_fn, batch_data, batch_labels, train=False, device=device)    
                 val_losses.append(vloss)
                 if i > 10:
                     break
         
         mloss = np.mean(losses)
         mvloss = np.mean(val_losses)
         all_losses.extend(losses)
```

### Comparing `soapcw-0.1.8/soapcw/cw/generate_data.py` & `soapcw-0.1.9/soapcw/cw/generate_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import timeit
 import lal
 import lalpulsar
 from lalpulsar import simulateCW
 from scipy.special import fresnel
 import scipy.stats as st
 import time
+from astropy.time import Time
 import os
 import copy
 import subprocess
 from .sft import SFT
 from .timeseries import TimeSeries
 from .tools import download_ephemeris_file, LAL_EPHEMERIS_URL
 
@@ -63,24 +64,51 @@
         self.f     = f
         self.tref = None
         
         self.gaps = False
         self.snr = snr
         self.edat = None
         self.antenna_pattern = True
+        self.baryinputs = {}
+        self.siteinfo = {}
+        self.earth = lalpulsar.EarthState()
+        self.emit = lalpulsar.EmissionTime()
         
     def param_check(self):
         
         for i,v in enumerate(params[:-2]):
             if np.isnan(v):
                 raise Exception("parameter {} is not a valid value".format(params_names[i]))
                 
         if self.tref is None:
             print("No reference time: Pulsar referece time same as sft start time")
             self.tref = self.tstart
+
+        
+    def get_baryinput(self, detector):
+        """
+        Load in the baryinputs prior to running
+        """
+        baryinput = lalpulsar.BarycenterInput()
+        if detector == 'SSB':
+            # set up the for reference frame at center of earth                                                                              
+            baryinput.site.location[0] = 0./lal.C_SI
+            baryinput.site.location[1] = 0./lal.C_SI
+            baryinput.site.location[2] = 0./lal.C_SI
+        else:
+            # get the information on specified detector                                                                                      
+            # set up the barycenter for given detector    
+            siteinfo = lalpulsar.GetSiteInfo(detector)   
+            self.siteinfo[detector] = siteinfo                                                                             
+            baryinput.site = siteinfo
+            baryinput.site.location[0] = baryinput.site.location[0]/lal.C_SI
+            baryinput.site.location[1] = baryinput.site.location[1]/lal.C_SI
+            baryinput.site.location[2] = baryinput.site.location[2]/lal.C_SI
+
+        return baryinput
         
         
     def detector_velocity(self,edat,epoch,detector):
         '''                                                                                                                                  
         get the three dimensional velocity of the earth                                                                                      
         args                                                                                                                                 
         --------                                                                                                                             
@@ -89,50 +117,32 @@
         detector : the detector i.e. 'H1'                                                                                                    
                                                                                                                                          
         returns                                                                                                                              
         --------                                                                                                                             
         emit.vDetector : velocity of detector at arrival time (epoch) in cartesian coords                                                    
         '''
 
-        # initialise the barycenter structure                                                                                                
-        baryinput = lalpulsar.BarycenterInput()
-
-        # dividing the positions by the speed of light                                                                                       
-        if detector == 'SSB':
-            # set up the for reference frame at center of earth                                                                              
-            baryinput.site.location[0] = 0./lal.C_SI
-            baryinput.site.location[1] = 0./lal.C_SI
-            baryinput.site.location[2] = 0./lal.C_SI
-        else:
-            # get the information on specified detector                                                                                      
-            det = lalpulsar.GetSiteInfo(detector)
-            # set up the barycenter for given detector                                                                                       
-            baryinput.site = det
-            baryinput.site.location[0] = baryinput.site.location[0]/lal.C_SI
-            baryinput.site.location[1] = baryinput.site.location[1]/lal.C_SI
-            baryinput.site.location[2] = baryinput.site.location[2]/lal.C_SI
+        # initialise the barycenter structure   
+        if detector not in self.baryinputs.keys():
+             self.baryinputs[detector] = self.get_baryinput(detector)                                                                                             
 
         # distance to the source in [s^-1]                                                                                                   
-        baryinput.dInv = 0.0
+        self.baryinputs[detector].dInv = 0.0
 
         # source right ascension and declination in radians                                                                                  
-        baryinput.alpha = 0.0
-        baryinput.delta = 0.0
-
-        earth = lalpulsar.EarthState()
-
-        emit = lalpulsar.EmissionTime()
+        self.baryinputs[detector].alpha = 0.0
+        self.baryinputs[detector].delta = 0.0
 
         # finds position and orientation of the earth at arrival time (epoch) for earth state and ephemerus data                             
-        lalpulsar.BarycenterEarth(earth,epoch,edat)
+        lalpulsar.BarycenterEarth(self.earth,epoch,edat)
 
         # transforms arrival time (epoch) into pulse emission time                                                                           
-        lalpulsar.Barycenter(emit,baryinput,earth)
+        lalpulsar.Barycenter(self.emit,self.baryinputs[detector],self.earth)
 
-        return emit.vDetector
+        return self.emit.vDetector
 
     def get_detector_velocities(self,epochs: np.array,det: str,edat = None):
         """
         get the velocities of the detector
         args
         -------------
         epochs: array or list
@@ -183,14 +193,34 @@
             self.tref = epochs[0]
 
         timeDiff = epochs - self.tref
         fhat = self.f[0] + timeDiff*self.f[1]
         
         return fhat * (1 + vDotn_c)
 
+    def gps_to_gmst_rad(self, epochs):
+        """ Taken amd vectorised from LAL code,  https://lscsoft.docs.ligo.org/lalsuite/lal/_x_l_a_l_sidereal_time_8c_source.html#l00062
+        !!!!!!!!!! will definitely need updating !!!!!!!!!!!!!!!
+        """
+        #print("using custom GMST code taken from LAL")
+        as_time = Time(epochs, format="gps", scale="utc")
+        # keep track of larger part
+        t_hi = (as_time.jd - 2451545.0)/36525.0
+        # keep track of nanosecond part separately
+        t_lo = (as_time.gps % 1e-9)/(1e9 * 36525.0 * 86400.0)
+        t = t_hi + t_lo
+        
+        sidereal_time = (-6.2e-6 * t + 0.093104) * t * t + 67310.54841
+        sidereal_time += 8640184.812866 * t_lo
+        sidereal_time += 3155760000.0 * t_lo
+        sidereal_time += 8640184.812866 * t_hi
+        sidereal_time += 3155760000.0 * t_hi
+        
+        return sidereal_time * np.pi / 43200.0
+
     def av_antenna(self,alpha,delta,det,tstart,nsft,tsft,antenna=True,use_lal=False,average = True):
         """
         Calculates the time averages of the antenna patterns
         args
         ----------
         alpha: float
             right ascension
@@ -216,18 +246,21 @@
 
         # this is not the source polarisation, that will be used later
         psi = 0.0
 
         if not antenna:
             return np.array([[1,1,1]])
         else:
-            detr = lalpulsar.GetSiteInfo(det)
+            if det not in self.siteinfo.keys():
+                self.baryinputs[det] = self.get_baryinput(det)  
+            #detr = lalpulsar.GetSiteInfo(det)
             epochs = np.arange(tstart,tstart+tsft*nsft,tsft) + 0.5*tsft
-            gmst_rad = [lal.GreenwichMeanSiderealTime(i) for i in epochs]
-            am = [lal.ComputeDetAMResponse(detr.response, alpha, delta, 0.0, i) for i in gmst_rad]
+            #gmst_rad = [lal.GreenwichMeanSiderealTime(i) for i in epochs]
+            gmst_rad = self.gps_to_gmst_rad(epochs)
+            am = [lal.ComputeDetAMResponse(self.siteinfo[det].response, alpha, delta, 0.0, i) for i in gmst_rad]
             fraczeta = (1./np.sin(det_params[det]["zeta"]))
             cos2psi = np.cos(2*psi)
             sin2psi = np.sin(2*psi)
             #A,B,C = 0,0,0
             ABC = []
             for i in range(len(epochs)):
                 av,bv = 0,0
```

### Comparing `soapcw-0.1.8/soapcw/cw/load_sfts.py` & `soapcw-0.1.9/soapcw/cw/load_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/cw/make_sfts.py` & `soapcw-0.1.9/soapcw/cw/make_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/cw/sft.py` & `soapcw-0.1.9/soapcw/cw/sft.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/cw/timeseries.py` & `soapcw-0.1.9/soapcw/cw/timeseries.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/cw/tools.py` & `soapcw-0.1.9/soapcw/cw/tools.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/line_aware_stat/gen_lookup.pyx` & `soapcw-0.1.9/soapcw/line_aware_stat/gen_lookup.pyx`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/line_aware_stat/gen_lookup_python.py` & `soapcw-0.1.9/soapcw/line_aware_stat/gen_lookup_python.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/line_aware_stat/save_lookup.py` & `soapcw-0.1.9/soapcw/line_aware_stat/save_lookup.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/soap_config_parser.py` & `soapcw-0.1.9/soapcw/soap_config_parser.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/soapcw.c` & `soapcw-0.1.9/soapcw/soapcw.c`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/soapcw.pyx` & `soapcw-0.1.9/soapcw/soapcw.pyx`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/tools/plots.py` & `soapcw-0.1.9/soapcw/tools/plots.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw/tools/tools.py` & `soapcw-0.1.9/soapcw/tools/tools.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/soapcw.egg-info/PKG-INFO` & `soapcw-0.1.9/soapcw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soapcw
-Version: 0.1.8
+Version: 0.1.9
 Summary: SOAP is a rapid algorithm to search for continuous sources of gravitational waves, with a wider application to long duration narrowband signals.
 Home-page: https://git.ligo.org/joseph.bayley/soapcw
 Author: Joe Bayley
 Author-email: joseph.bayley@glasgow.ac.uk
 License: MIT license
 Download-URL: https://git.ligo.org/joseph.bayley/soapcw/-/archive/0.1.2/soapcw-0.1.2.tar.gz
 Keywords: soapcw,soap,gravitational waves,pulsars,neutron stars,continuous waves
```

### Comparing `soapcw-0.1.8/soapcw.egg-info/SOURCES.txt` & `soapcw-0.1.9/soapcw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/tests/SNR_injections.ipynb` & `soapcw-0.1.9/tests/SNR_injections.ipynb`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/tests/test_cwload.py` & `soapcw-0.1.9/tests/test_cwload.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/tests/test_line_aware_stat.py` & `soapcw-0.1.9/tests/test_line_aware_stat.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.8/tests/test_soap.py` & `soapcw-0.1.9/tests/test_soap.py`

 * *Files identical despite different names*

