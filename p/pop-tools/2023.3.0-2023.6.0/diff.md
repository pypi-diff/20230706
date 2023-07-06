# Comparing `tmp/pop-tools-2023.3.0.tar.gz` & `tmp/pop-tools-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-tools-2023.3.0.tar", last modified: Sat Mar  4 03:00:21 2023, max compression
+gzip compressed data, was "pop-tools-2023.6.0.tar", last modified: Thu Jul  6 02:03:53 2023, max compression
```

## Comparing `pop-tools-2023.3.0.tar` & `pop-tools-2023.6.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:00:21.288098 pop-tools-2023.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:00:21.276098 pop-tools-2023.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:00:21.276098 pop-tools-2023.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/.github/workflows/cancel-duplicate-runs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/.github/workflows/ci-upstream-dev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/.prettierrc.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-03-04 03:00:21.288098 pop-tools-2023.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:00:21.276098 pop-tools-2023.3.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/ci/environment-upstream-dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:00:21.276098 pop-tools-2023.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:00:21.272098 pop-tools-2023.3.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:00:21.276098 pop-tools-2023.3.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/_static/css/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:00:21.276098 pop-tools-2023.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:00:21.284098 pop-tools-2023.3.0/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   152639 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/examples/CloseHeatBudget_POP2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   190740 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/examples/POP_Grid.png
--rw-r--r--   0 runner    (1001) docker     (123)  1459143 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/examples/cesm-cmip-cf-xarray.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/examples/eos.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/examples/get-model-grid.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/examples/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/examples/lateral-fill-idealized.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/examples/lateral-fill-model-grid.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (123)  2586453 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/examples/pop_div_curl_xr_xgcm_metrics_compare.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/examples/region-mask.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/examples/sample-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/examples/xgcm-transform.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   234827 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/examples/xoak-example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:00:21.284098 pop-tools-2023.3.0/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/images/nsf.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/docs/source/install.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:00:21.284098 pop-tools-2023.3.0/pop_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/data_registry.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/eos.py
--rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)    15823 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:00:21.288098 pop-tools-2023.3.0/pop_tools/input_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/input_templates/gx1v6_vert_grid
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/input_templates/gx1v7_vert_grid
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/input_templates/gx3v5_vert_grid
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/input_templates/gx3v7_vert_grid
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/input_templates/tx0.1v2_vert_grid
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/input_templates/tx0.1v3_vert_grid
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/input_templates/tx1v1_vert_grid
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/inputdata_registry.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/pop_grid_definitions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/region_mask_definitions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/region_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pop_tools/xgcm_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:00:21.288098 pop-tools-2023.3.0/pop_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-03-04 03:00:21.000000 pop-tools-2023.3.0/pop_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-04 03:00:21.000000 pop-tools-2023.3.0/pop_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 03:00:21.000000 pop-tools-2023.3.0/pop_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 03:00:21.000000 pop-tools-2023.3.0/pop_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-04 03:00:21.000000 pop-tools-2023.3.0/pop_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-04 03:00:21.000000 pop-tools-2023.3.0/pop_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-04 03:00:21.288098 pop-tools-2023.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-03-04 03:00:11.000000 pop-tools-2023.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:03:53.748012 pop-tools-2023.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:03:53.740013 pop-tools-2023.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:03:53.740013 pop-tools-2023.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/.github/workflows/cancel-duplicate-runs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/.github/workflows/ci-upstream-dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/.prettierrc.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-06 02:03:53.748012 pop-tools-2023.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:03:53.740013 pop-tools-2023.6.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/ci/environment-upstream-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:03:53.740013 pop-tools-2023.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:03:53.736013 pop-tools-2023.6.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:03:53.740013 pop-tools-2023.6.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/_static/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:03:53.740013 pop-tools-2023.6.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:03:53.744012 pop-tools-2023.6.0/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   153094 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/examples/CloseHeatBudget_POP2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   190740 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/examples/POP_Grid.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1459143 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/examples/cesm-cmip-cf-xarray.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/examples/eos.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/examples/get-model-grid.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/examples/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/examples/lateral-fill-idealized.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/examples/lateral-fill-model-grid.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2586453 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/examples/pop_div_curl_xr_xgcm_metrics_compare.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/examples/region-mask.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/examples/sample-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/examples/xgcm-transform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   234827 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/examples/xoak-example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:03:53.744012 pop-tools-2023.6.0/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/images/nsf.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/docs/source/install.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:03:53.744012 pop-tools-2023.6.0/pop_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/data_registry.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/eos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15798 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:03:53.748012 pop-tools-2023.6.0/pop_tools/input_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/input_templates/gx1v6_vert_grid
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/input_templates/gx1v7_vert_grid
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/input_templates/gx3v5_vert_grid
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/input_templates/gx3v7_vert_grid
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/input_templates/tx0.1v2_vert_grid
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/input_templates/tx0.1v3_vert_grid
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/input_templates/tx1v1_vert_grid
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/inputdata_registry.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/pop_grid_definitions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/region_mask_definitions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/region_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pop_tools/xgcm_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:03:53.748012 pop-tools-2023.6.0/pop_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-06 02:03:53.000000 pop-tools-2023.6.0/pop_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-06 02:03:53.000000 pop-tools-2023.6.0/pop_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 02:03:53.000000 pop-tools-2023.6.0/pop_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 02:03:53.000000 pop-tools-2023.6.0/pop_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 02:03:53.000000 pop-tools-2023.6.0/pop_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 02:03:53.000000 pop-tools-2023.6.0/pop_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-06 02:03:53.748012 pop-tools-2023.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-06 02:03:41.000000 pop-tools-2023.6.0/setup.py
```

### Comparing `pop-tools-2023.3.0/.github/workflows/ci-upstream-dev.yaml` & `pop-tools-2023.6.0/.github/workflows/ci-upstream-dev.yaml`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/.github/workflows/pypi.yml` & `pop-tools-2023.6.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/.gitignore` & `pop-tools-2023.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/.pre-commit-config.yaml` & `pop-tools-2023.6.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -11,22 +11,22 @@
       - id: check-json
       - id: check-yaml
       - id: double-quote-string-fixer
       - id: debug-statements
       - id: mixed-line-ending
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.8.0
     hooks:
       - id: pyupgrade
         args:
           - '--py37-plus'
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black-jupyter
 
   - repo: https://github.com/keewis/blackdoc
     rev: v0.3.8
     hooks:
       - id: blackdoc
@@ -37,10 +37,10 @@
       - id: flake8
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.4
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
```

### Comparing `pop-tools-2023.3.0/CHANGELOG.md` & `pop-tools-2023.6.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/CONTRIBUTING.md` & `pop-tools-2023.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/LICENSE` & `pop-tools-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/PKG-INFO` & `pop-tools-2023.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-tools
-Version: 2023.3.0
+Version: 2023.6.0
 Summary: POP2-CESM tools
 Home-page: https://github.com/NCAR/pop-tools
 Maintainer: Matthew Long
 Maintainer-email: mclong@ucar.edu
 License: Apache Software License 2.0
 Project-URL: Documentation, https://pop-tools.readthedocs.io
 Project-URL: Source, https://github.com/NCAR/pop-tools
```

### Comparing `pop-tools-2023.3.0/README.md` & `pop-tools-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/Makefile` & `pop-tools-2023.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/make.bat` & `pop-tools-2023.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/source/api.rst` & `pop-tools-2023.6.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/source/conf.py` & `pop-tools-2023.6.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/source/examples/CloseHeatBudget_POP2.ipynb` & `pop-tools-2023.6.0/docs/source/examples/CloseHeatBudget_POP2.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993386243386243%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'In this notebook, we are going to use xgcm with metrics "*

 * *            'to demonstrate budget closure for the 0.1 degree horizontal resolution version of '*

 * *            'POP2. Note that the lower resolution has more parameterizations and therefore does '*

 * *            'not close following this notebook. This notebook was contributed by [Anna-Lena '*

 * *            "Deppenmeier](https://github.com/ALDepp).\\n')], delete: [2]}}, 16: {'source': "*

 * *            '{insert: [(1, "< […]*

```diff
@@ -2,15 +2,15 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Calculate POP2 heat budget using xgcm\n",
                 "\n",
-                "In this notebook, we are going to use xgcm with metrics to demonstrate budget closure. This notebook was contributed by [Anna-Lena Deppenmeier](https://github.com/ALDepp).\n",
+                "In this notebook, we are going to use xgcm with metrics to demonstrate budget closure for the 0.1 degree horizontal resolution version of POP2. Note that the lower resolution has more parameterizations and therefore does not close following this notebook. This notebook was contributed by [Anna-Lena Deppenmeier](https://github.com/ALDepp).\n",
                 "\n",
                 "\n",
                 "This is an image of the POP output structure on the horizontal B-grid courtesy of [Yassir Eddebbar](https://github.com/Eddebbar).\n",
                 "\n",
                 "<img src=\"POP_Grid.png\" alt=\"Drawing\" style=\"width: 800px;\"/>"
             ]
         },
@@ -743,15 +743,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### i) Total heat advection\n",
-                "<p style='text-align: justify;'> We use grid.diff and multiply and divide by the volumes ourselves is the way POP outputs the fluxes. It performs a division by the cell area before saving the terms, which would not be accounted for if we used grid.derivative. Note that we also multiply by dsxgcm.VOL.values and then divide by dsxgcm.VOL. This is due to the same issue, there is a mis-alignment in the grid in this output term that xgcm would not like, and we are getting around it this way. This might be specific to POP and it should likely be possible to use grid.derivative for other models.</p>"
+                "<p style='text-align: justify;'> We use grid.diff and multiply and divide by the volumes ourselves is the way POP outputs the fluxes. It performs a division by the cell area before saving the terms, which would not be accounted for if we used grid.derivative. Note that we also multiply by dsxgcm.VOL.values and then divide by dsxgcm.VOL. This is due to the same issue, there is a mis-alignment in the grid in this output term that xgcm would not like, and we are getting around it this way. This might be specific to POP and it should likely be possible to use grid.derivative for other models. The variables used here are online accumulated transports as output by the model. If you calculate according to udT/dx etc you will have the transport from the mean fields, and miss the eddy contribution below the timescale of your averaging operator (e.g. monthly for monthly output).</p>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {},
             "outputs": [],
```

### Comparing `pop-tools-2023.3.0/docs/source/examples/POP_Grid.png` & `pop-tools-2023.6.0/docs/source/examples/POP_Grid.png`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/source/examples/cesm-cmip-cf-xarray.ipynb` & `pop-tools-2023.6.0/docs/source/examples/cesm-cmip-cf-xarray.ipynb`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/source/examples/eos.ipynb` & `pop-tools-2023.6.0/docs/source/examples/eos.ipynb`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/source/examples/get-model-grid.ipynb` & `pop-tools-2023.6.0/docs/source/examples/get-model-grid.ipynb`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/source/examples/lateral-fill-idealized.ipynb` & `pop-tools-2023.6.0/docs/source/examples/lateral-fill-idealized.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998697916666667%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(6, 'valid_points = np.ones(z_orig.shape, dtype=bool)\\n')], "*

 * *            'delete: [6]}}}'}*

```diff
@@ -46,15 +46,15 @@
             "source": [
                 "dx, dy = 0.05, 0.05\n",
                 "\n",
                 "y, x = np.mgrid[slice(1 - dy, 3 + dy, dy), slice(1 - dx, 5 + dx, dx)]\n",
                 "\n",
                 "z_orig = np.sin(x) ** 10 + np.cos(10 + y * x) * np.cos(x)\n",
                 "\n",
-                "valid_points = np.ones(z_orig.shape, dtype=np.bool)\n",
+                "valid_points = np.ones(z_orig.shape, dtype=bool)\n",
                 "valid_points = np.where(y < 0.5 * np.sin(5 * x) + 1.5, False, valid_points)\n",
                 "\n",
                 "z_orig = np.where(~valid_points, np.nan, z_orig)\n",
                 "z_orig[0, :] = np.nan\n",
                 "\n",
                 "\n",
                 "cb = plt.pcolormesh(z_orig, vmin=-1, vmax=2.0)\n",
```

### Comparing `pop-tools-2023.3.0/docs/source/examples/lateral-fill-model-grid.ipynb` & `pop-tools-2023.6.0/docs/source/examples/lateral-fill-model-grid.ipynb`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/source/examples/pop_div_curl_xr_xgcm_metrics_compare.ipynb` & `pop-tools-2023.6.0/docs/source/examples/pop_div_curl_xr_xgcm_metrics_compare.ipynb`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/source/examples/region-mask.ipynb` & `pop-tools-2023.6.0/docs/source/examples/region-mask.ipynb`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/source/examples/sample-data.ipynb` & `pop-tools-2023.6.0/docs/source/examples/sample-data.ipynb`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/source/examples/xgcm-transform.ipynb` & `pop-tools-2023.6.0/docs/source/examples/xgcm-transform.ipynb`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/source/examples/xoak-example.ipynb` & `pop-tools-2023.6.0/docs/source/examples/xoak-example.ipynb`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/source/images/nsf.png` & `pop-tools-2023.6.0/docs/source/images/nsf.png`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/source/index.md` & `pop-tools-2023.6.0/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/docs/source/install.md` & `pop-tools-2023.6.0/docs/source/install.md`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools/__init__.py` & `pop-tools-2023.6.0/pop_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools/calc.py` & `pop-tools-2023.6.0/pop_tools/calc.py`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools/data_registry.txt` & `pop-tools-2023.6.0/pop_tools/data_registry.txt`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools/datasets.py` & `pop-tools-2023.6.0/pop_tools/datasets.py`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools/eos.py` & `pop-tools-2023.6.0/pop_tools/eos.py`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools/fill.py` & `pop-tools-2023.6.0/pop_tools/fill.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 
     return da_out
 
 
 def lateral_fill_np_array(
     var, isvalid_mask, ltripole=False, tol=1.0e-4, use_sor=False, rc=1.8, max_iter=10000
 ):
-
     """Perform lateral fill on numpy.array
 
     Parameters [NB defaults set redundantly with lateral_fill above to allow this
                 function to be called directly for numpy arrays]
     ----------
 
     var : numpy.array
```

### Comparing `pop-tools-2023.3.0/pop_tools/grid.py` & `pop-tools-2023.6.0/pop_tools/grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 input_templates_dir = pkg_resources.resource_filename('pop_tools', 'input_templates')
 
 with open(grid_def_file) as f:
     grid_defs = yaml.safe_load(f)
 
 
 def fetch(self, fname, processor=None, downloader=None):
-
     """
     This is a modified version of Pooch.fetch() method. This modification is necessary
     due to the fact that on Cheyenne/Casper path to the local data storage folder points
     to a folder (CESMDATAROOT: /glade/p/cesmdata/cseg), and this is not a location that
     we have permissions to write to.
 
     Parameters
@@ -135,22 +134,22 @@
     nlon = grid_attrs['lateral_dims'][1]
 
     # read horizontal grid
     horiz_grid_fname = INPUTDATA.fetch(grid_attrs['horiz_grid_fname'], downloader=downloader)
     grid_file_data = np.fromfile(horiz_grid_fname, dtype='>f8', count=-1)
     grid_file_data = grid_file_data.reshape((7, nlat, nlon))
 
-    ULAT = grid_file_data[0, :, :].astype(np.float)
-    ULONG = grid_file_data[1, :, :].astype(np.float)
-    HTN = grid_file_data[2, :, :].astype(np.float)
-    HTE = grid_file_data[3, :, :].astype(np.float)
+    ULAT = grid_file_data[0, :, :].astype(float)
+    ULONG = grid_file_data[1, :, :].astype(float)
+    HTN = grid_file_data[2, :, :].astype(float)
+    HTE = grid_file_data[3, :, :].astype(float)
 
     # compute TLAT, TLONG
-    TLAT = np.empty((nlat, nlon), dtype=np.float)
-    TLONG = np.empty((nlat, nlon), dtype=np.float)
+    TLAT = np.empty((nlat, nlon), dtype=float)
+    TLONG = np.empty((nlat, nlon), dtype=float)
     _compute_TLAT_TLONG(ULAT, ULONG, TLAT, TLONG, nlat, nlon)
 
     # generate DXT, DYT
     # DXT[i,j] = (HTN[i,j] + HTN[i,j−1])/2
     DXT = np.empty((nlat, nlon))
     DXT[1:, :] = 0.5 * (HTN[: nlat - 1, :] + HTN[1:, :])
     # DXT[0, :] = 0.5 * (2 * HTN[0, :] - HTN[1, :] + HTN[0, :])
@@ -435,16 +434,16 @@
     TLONG[0, :] = TLONG[1, :] - (TLONG[2, :] - TLONG[1, :])
 
 
 def _compute_corners(ULAT, ULONG):
     """Compute grid corners."""
 
     nlat, nlon = ULAT.shape
-    corner_lat = np.empty((nlat, nlon, 4), dtype=np.float)
-    corner_lon = np.empty((nlat, nlon, 4), dtype=np.float)
+    corner_lat = np.empty((nlat, nlon, 4), dtype=float)
+    corner_lon = np.empty((nlat, nlon, 4), dtype=float)
 
     # NE corner
     corner_lat[:, :, 0] = ULAT
     corner_lon[:, :, 0] = ULONG
 
     # NW corner (copy from NE corner of column to the left, assume zonal periodic bc)
     corner_lat[:, :, 1] = np.roll(corner_lat[:, :, 0], 1, axis=1)
```

### Comparing `pop-tools-2023.3.0/pop_tools/input_templates/gx1v6_vert_grid` & `pop-tools-2023.6.0/pop_tools/input_templates/gx1v6_vert_grid`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools/input_templates/gx1v7_vert_grid` & `pop-tools-2023.6.0/pop_tools/input_templates/gx1v7_vert_grid`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools/input_templates/gx3v5_vert_grid` & `pop-tools-2023.6.0/pop_tools/input_templates/gx3v5_vert_grid`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools/input_templates/gx3v7_vert_grid` & `pop-tools-2023.6.0/pop_tools/input_templates/gx3v7_vert_grid`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools/input_templates/tx0.1v2_vert_grid` & `pop-tools-2023.6.0/pop_tools/input_templates/tx0.1v2_vert_grid`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools/input_templates/tx0.1v3_vert_grid` & `pop-tools-2023.6.0/pop_tools/input_templates/tx0.1v3_vert_grid`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools/input_templates/tx1v1_vert_grid` & `pop-tools-2023.6.0/pop_tools/input_templates/tx1v1_vert_grid`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools/inputdata_registry.txt` & `pop-tools-2023.6.0/pop_tools/inputdata_registry.txt`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools/pop_grid_definitions.yaml` & `pop-tools-2023.6.0/pop_tools/pop_grid_definitions.yaml`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools/region_mask_definitions.yaml` & `pop-tools-2023.6.0/pop_tools/region_mask_definitions.yaml`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools/region_masks.py` & `pop-tools-2023.6.0/pop_tools/region_masks.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,24 +73,21 @@
         attrs={'mask_name': mask_name},
     )
 
     not_land = np.where(ds.KMT > 0, 1, 0)
 
     # loop over region names
     for i, (region_name, crit_list) in enumerate(region_defs.items()):
-
         # loop over list of criteria groups
         mask = np.zeros((nlat, nlon), dtype=bool)
         for crit in crit_list:
-
             mask_and = np.ones((nlat, nlon), dtype=bool)
 
             # loop over each criterion
             for crit_type, crit_dict in crit.items():
-
                 # apply bounds or match
                 if crit_type == 'bounds':
                     for field, bounds in crit_dict.items():
                         if bounds[0] > bounds[1]:
                             mask_and = (bounds[0] <= ds[field]) | (
                                 ds[field] <= bounds[1]
                             ) & mask_and
```

### Comparing `pop-tools-2023.3.0/pop_tools/xgcm_util.py` & `pop-tools-2023.6.0/pop_tools/xgcm_util.py`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/pop_tools.egg-info/PKG-INFO` & `pop-tools-2023.6.0/pop_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-tools
-Version: 2023.3.0
+Version: 2023.6.0
 Summary: POP2-CESM tools
 Home-page: https://github.com/NCAR/pop-tools
 Maintainer: Matthew Long
 Maintainer-email: mclong@ucar.edu
 License: Apache Software License 2.0
 Project-URL: Documentation, https://pop-tools.readthedocs.io
 Project-URL: Source, https://github.com/NCAR/pop-tools
```

### Comparing `pop-tools-2023.3.0/pop_tools.egg-info/SOURCES.txt` & `pop-tools-2023.6.0/pop_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/setup.cfg` & `pop-tools-2023.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pop-tools-2023.3.0/setup.py` & `pop-tools-2023.6.0/setup.py`

 * *Files identical despite different names*

