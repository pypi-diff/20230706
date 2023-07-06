# Comparing `tmp/cf_xarray-0.8.2.tar.gz` & `tmp/cf_xarray-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf_xarray-0.8.2.tar", last modified: Fri Jun 23 21:37:38 2023, max compression
+gzip compressed data, was "cf_xarray-0.8.3.tar", last modified: Thu Jul  6 04:01:59 2023, max compression
```

## Comparing `cf_xarray-0.8.2.tar` & `cf_xarray-0.8.3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.191434 cf_xarray-0.8.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.179434 cf_xarray-0.8.2/.binder/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.binder/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.deepsource.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.179434 cf_xarray-0.8.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.179434 cf_xarray-0.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.github/workflows/parse_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.github/workflows/testpypi-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.github/workflows/upstream-dev-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.tributors
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-06-23 21:37:38.191434 cf_xarray-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.183434 cf_xarray-0.8.2/cf_xarray/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 21:37:37.000000 cf_xarray-0.8.2/cf_xarray/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)   100886 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/coding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    23849 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/options.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.183434 cf_xarray-0.8.2/cf_xarray/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/scripts/make_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/scripts/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/sgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.183434 cf_xarray-0.8.2/cf_xarray/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63574 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/tests/test_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/tests/test_coding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.183434 cf_xarray-0.8.2/cf_xarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-06-23 21:37:38.000000 cf_xarray-0.8.2/cf_xarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-23 21:37:38.000000 cf_xarray-0.8.2/cf_xarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:37:38.000000 cf_xarray-0.8.2/cf_xarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 21:37:38.000000 cf_xarray-0.8.2/cf_xarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 21:37:38.000000 cf_xarray-0.8.2/cf_xarray.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.183434 cf_xarray-0.8.2/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/ci/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/ci/environment-no-optional-deps.yml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/ci/upstream-dev-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.187435 cf_xarray-0.8.2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/2D_bounds_averaged.png
--rw-r--r--   0 runner    (1001) docker     (123)    62190 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/2D_bounds_error.png
--rw-r--r--   0 runner    (1001) docker     (123)    53236 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/2D_bounds_nonunique.png
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.187435 cf_xarray-0.8.2/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/_static/dataset-diagram-logo.tex
--rw-r--r--   0 runner    (1001) docker     (123)    48563 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/_static/full-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    33479 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    71840 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   130855 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/_static/rich-repr-example.png
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/bounds.md
--rw-r--r--   0 runner    (1001) docker     (123)    33785 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/cartopy_rotated_pole.png
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/coding.md
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/coord_axes.md
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/custom-criteria.md
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/dsg.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.187435 cf_xarray-0.8.2/doc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/examples/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/flags.md
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/geometry.md
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/grid_mappings.md
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/howtouse.md
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/parametricz.md
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/plotting.md
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/provenance.md
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/selecting.md
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/sgrid_ugrid.md
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/units.md
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/whats-new.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 21:37:38.191434 cf_xarray-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.460006 cf_xarray-0.8.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.448005 cf_xarray-0.8.3/.binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.binder/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.deepsource.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.448005 cf_xarray-0.8.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.448005 cf_xarray-0.8.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.github/workflows/parse_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.github/workflows/testpypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.github/workflows/upstream-dev-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.tributors
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-07-06 04:01:59.460006 cf_xarray-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.452005 cf_xarray-0.8.3/cf_xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 04:01:58.000000 cf_xarray-0.8.3/cf_xarray/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100886 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23849 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.452005 cf_xarray-0.8.3/cf_xarray/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/scripts/make_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/scripts/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/sgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.452005 cf_xarray-0.8.3/cf_xarray/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63717 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/tests/test_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/tests/test_coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.452005 cf_xarray-0.8.3/cf_xarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-07-06 04:01:59.000000 cf_xarray-0.8.3/cf_xarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-06 04:01:59.000000 cf_xarray-0.8.3/cf_xarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:01:59.000000 cf_xarray-0.8.3/cf_xarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 04:01:59.000000 cf_xarray-0.8.3/cf_xarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 04:01:59.000000 cf_xarray-0.8.3/cf_xarray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.452005 cf_xarray-0.8.3/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/ci/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/ci/environment-no-optional-deps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/ci/upstream-dev-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.460006 cf_xarray-0.8.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/2D_bounds_averaged.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62190 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/2D_bounds_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53236 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/2D_bounds_nonunique.png
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.460006 cf_xarray-0.8.3/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/_static/dataset-diagram-logo.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    48563 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/_static/full-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33479 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71840 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   130855 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/_static/rich-repr-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/bounds.md
+-rw-r--r--   0 runner    (1001) docker     (123)    33785 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/cartopy_rotated_pole.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/coding.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/coord_axes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/custom-criteria.md
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/dsg.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.460006 cf_xarray-0.8.3/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/examples/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/flags.md
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/geometry.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/grid_mappings.md
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/howtouse.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/parametricz.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/plotting.md
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/provenance.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/selecting.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/sgrid_ugrid.md
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/units.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/whats-new.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 04:01:59.460006 cf_xarray-0.8.3/setup.cfg
```

### Comparing `cf_xarray-0.8.2/.github/workflows/ci.yaml` & `cf_xarray-0.8.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/.github/workflows/parse_logs.py` & `cf_xarray-0.8.3/.github/workflows/parse_logs.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/.github/workflows/pypi.yaml` & `cf_xarray-0.8.3/.github/workflows/pypi.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         run: |
           python -m pip install --upgrade pip
           python -m pip install dist/cf_xarray*.whl
           python -m cf_xarray.scripts.print_versions
 
       - name: Publish package to TestPyPI
         if: github.event_name == 'push'
-        uses: pypa/gh-action-pypi-publish@v1.8.6
+        uses: pypa/gh-action-pypi-publish@v1.8.7
         with:
           password: ${{ secrets.TESTPYPI_TOKEN }}
           repository_url: https://test.pypi.org/legacy/
           verbose: true
 
 
   upload-to-pypi:
@@ -92,10 +92,10 @@
 
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: releases
           path: dist
       - name: Publish package to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.6
+        uses: pypa/gh-action-pypi-publish@v1.8.7
         with:
           verbose: true
```

### Comparing `cf_xarray-0.8.2/.github/workflows/testpypi-release.yaml` & `cf_xarray-0.8.3/.github/workflows/testpypi-release.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/.github/workflows/upstream-dev-ci.yaml` & `cf_xarray-0.8.3/.github/workflows/upstream-dev-ci.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/.gitignore` & `cf_xarray-0.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/.pre-commit-config.yaml` & `cf_xarray-0.8.3/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ci:
     autoupdate_schedule: quarterly
 
 repos:
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
+  - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: 'v0.0.260'
+    rev: 'v0.0.276'
     hooks:
       - id: ruff
         args: ["--fix"]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
@@ -57,10 +57,10 @@
 
   - repo: https://github.com/citation-file-format/cff-converter-python
     rev: "44e8fc9"
     hooks:
     - id: validate-cff
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.2
+    rev: v0.13
     hooks:
       - id: validate-pyproject
```

### Comparing `cf_xarray-0.8.2/.tributors` & `cf_xarray-0.8.3/.tributors`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/CITATION.cff` & `cf_xarray-0.8.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/LICENSE` & `cf_xarray-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/PKG-INFO` & `cf_xarray-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf_xarray
-Version: 0.8.2
+Version: 0.8.3
 Summary: A convenience wrapper for using CF attributes on xarray objects
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cf_xarray-0.8.2/README.rst` & `cf_xarray-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/accessor.py` & `cf_xarray-0.8.3/cf_xarray/accessor.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/coding.py` & `cf_xarray-0.8.3/cf_xarray/coding.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/criteria.py` & `cf_xarray-0.8.3/cf_xarray/criteria.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/datasets.py` & `cf_xarray-0.8.3/cf_xarray/datasets.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/formatting.py` & `cf_xarray-0.8.3/cf_xarray/formatting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import warnings
 from functools import partial
 from typing import Dict, Hashable, Iterable, List
 
+import numpy as np
+
 STAR = " * "
 TAB = len(STAR) * " "
 
 try:
     from rich.table import Table
 except ImportError:
     Table = None  # type: ignore
@@ -143,14 +145,29 @@
             text = "".join(textgen)
             return Panel(f"[color(241)]{text.rstrip()}[/color(241)]", **kwargs)  # type: ignore
     else:
         text = "".join(textgen)
         return title + ":\n" + text
 
 
+def find_set_bits(mask, value, repeated_masks):
+    bitpos = np.arange(8)[::-1]
+    if mask not in repeated_masks:
+        if value == 0:
+            return [-1]
+        elif value is not None:
+            return [int(np.log2(value))]
+        else:
+            return [int(np.log2(mask))]
+    else:
+        allset = bitpos[np.unpackbits(np.uint8(mask)) == 1]
+        setbits = bitpos[np.unpackbits(np.uint8(mask & value)) == 1]
+        return [b if abs(b) in setbits else -b for b in allset]
+
+
 def _format_flags(accessor, rich):
     from .accessor import create_flag_dict
 
     try:
         flag_dict = create_flag_dict(accessor._obj)
     except ValueError:
         return _print_rows(
@@ -161,51 +178,69 @@
     repeated_masks = {m for m in masks if masks.count(m) > 1}
     excl_flags = [f for f, (m, v) in flag_dict.items() if m in repeated_masks]
     # indep_flags = [
     #     f
     #     for f, (m, _) in flag_dict.items()
     #     if m is not None and m not in repeated_masks
     # ]
+    bit_text = []
+    value_text = []
+    for key, (mask, value) in flag_dict.items():
+        if mask is None:
+            bit_text.append("✗" if rich else "")
+            value_text.append(str(value))
+            continue
+        bits = find_set_bits(mask, value, repeated_masks)
+        bitstring = ["."] * 8
+        if bits == [-1]:
+            continue
+        else:
+            for b in bits:
+                bitstring[abs(b)] = _format_cf_name("1" if b >= 0 else "0", rich)
+        text = "".join(bitstring[::-1])
+        value_text.append(
+            f"{mask} & {value}"
+            if key in excl_flags and value is not None
+            else str(mask)
+        )
+        bit_text.append(text if rich else f" / Bit: {text}")
+
     if rich:
         from rich import box
         from rich.table import Table
 
         table = Table(
             box=box.SIMPLE,
             width=None,
             title_justify="left",
             padding=(0, 2),
             header_style="bold color(244)",
         )
 
         table.add_column("Meaning", justify="left")
         table.add_column("Value", justify="right")
-        table.add_column("Bit?", justify="center")
+        table.add_column("Bits", justify="center")
 
-        for key, (mask, value) in flag_dict.items():
+        for val, bit, (key, (mask, value)) in zip(
+            value_text, bit_text, flag_dict.items()
+        ):
             table.add_row(
                 _format_cf_name(key, rich),
-                str(value) if key in excl_flags else str(mask),
-                "✗" if key in excl_flags else "✓",
+                val,
+                bit,
             )
 
         return table
 
     else:
-        rows = [
-            f"{TAB}{_format_cf_name(key, rich)}: " f"{_format_varname(value, rich)}"
-            for key, (mask, value) in flag_dict.items()
-            if key in excl_flags
-        ]
-
-        rows += [
-            f"{TAB}{_format_cf_name(key, rich)}: " f"Bit {_format_varname(mask, rich)}"
-            for key, (mask, value) in flag_dict.items()
-            if key not in excl_flags
-        ]
+        rows = []
+        for val, bit, (key, (mask, value)) in zip(
+            value_text, bit_text, flag_dict.items()
+        ):
+            rows.append(f"{TAB}{_format_cf_name(key, rich)}: {TAB} {val} {bit}")
         return _print_rows("Flag Meanings", rows, rich)
 
 
 def _format_dsg_roles(accessor, dims, rich):
     from .criteria import _DSG_ROLES
 
     yield make_text_section(
```

### Comparing `cf_xarray-0.8.2/cf_xarray/geometry.py` & `cf_xarray-0.8.3/cf_xarray/geometry.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/helpers.py` & `cf_xarray-0.8.3/cf_xarray/helpers.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/options.py` & `cf_xarray-0.8.3/cf_xarray/options.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/scripts/make_doc.py` & `cf_xarray-0.8.3/cf_xarray/scripts/make_doc.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/sgrid.py` & `cf_xarray-0.8.3/cf_xarray/sgrid.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/tests/__init__.py` & `cf_xarray-0.8.3/cf_xarray/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/tests/test_accessor.py` & `cf_xarray-0.8.3/cf_xarray/tests/test_accessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1844,20 +1844,21 @@
         actual = flag_excl.cf.isin(["flag_ERR"])
         assert not actual.any()
 
     def test_flag_errors(self) -> None:
         with pytest.raises(ValueError):
             flag_mix.cf == "ERR"
 
-        flag_excl.attrs.pop("flag_values")
+        flag_ex = flag_excl.copy()
+        flag_ex.attrs.pop("flag_values")
         with pytest.raises(ValueError):
-            flag_excl.cf.isin(["flag_1"])
+            flag_ex.cf.isin(["flag_1"])
 
         with pytest.raises(ValueError):
-            flag_excl.cf == "flag_1"
+            flag_ex.cf == "flag_1"
 
         with pytest.raises(ValueError):
             basin.cf == "arctic_ocean"
 
         ds = xr.Dataset({"basin": basin})
         with pytest.raises(ValueError):
             ds.cf.isin(["atlantic_ocean"])
@@ -1951,14 +1952,17 @@
 @requires_rich
 @pytest.mark.parametrize(
     "obj, contains",
     (
         [airds.air, "Coordinates"],
         [popds, "Data Variables"],
         [basin, "Flag Variable"],
+        [flag_mix, "Flag Variable"],
+        [flag_indep, "Flag Variable"],
+        [flag_excl, "Flag Variable"],
         [dsg, "Discrete Sampling Geometry"],
     ),
 )
 def test_rich_repr(obj, contains):
     from rich.console import Console
 
     console = Console()
```

### Comparing `cf_xarray-0.8.2/cf_xarray/tests/test_coding.py` & `cf_xarray-0.8.3/cf_xarray/tests/test_coding.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/tests/test_geometry.py` & `cf_xarray-0.8.3/cf_xarray/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/tests/test_helpers.py` & `cf_xarray-0.8.3/cf_xarray/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/tests/test_scripts.py` & `cf_xarray-0.8.3/cf_xarray/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/tests/test_units.py` & `cf_xarray-0.8.3/cf_xarray/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/units.py` & `cf_xarray-0.8.3/cf_xarray/units.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray/utils.py` & `cf_xarray-0.8.3/cf_xarray/utils.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/cf_xarray.egg-info/PKG-INFO` & `cf_xarray-0.8.3/cf_xarray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-xarray
-Version: 0.8.2
+Version: 0.8.3
 Summary: A convenience wrapper for using CF attributes on xarray objects
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cf_xarray-0.8.2/cf_xarray.egg-info/SOURCES.txt` & `cf_xarray-0.8.3/cf_xarray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/2D_bounds_averaged.png` & `cf_xarray-0.8.3/doc/2D_bounds_averaged.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/2D_bounds_error.png` & `cf_xarray-0.8.3/doc/2D_bounds_error.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/2D_bounds_nonunique.png` & `cf_xarray-0.8.3/doc/2D_bounds_nonunique.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/Makefile` & `cf_xarray-0.8.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/_static/dataset-diagram-logo.tex` & `cf_xarray-0.8.3/doc/_static/dataset-diagram-logo.tex`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/_static/full-logo.png` & `cf_xarray-0.8.3/doc/_static/full-logo.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/_static/logo.png` & `cf_xarray-0.8.3/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/_static/logo.svg` & `cf_xarray-0.8.3/doc/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/_static/rich-repr-example.png` & `cf_xarray-0.8.3/doc/_static/rich-repr-example.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/api.rst` & `cf_xarray-0.8.3/doc/api.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/bounds.md` & `cf_xarray-0.8.3/doc/bounds.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/cartopy_rotated_pole.png` & `cf_xarray-0.8.3/doc/cartopy_rotated_pole.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/coding.md` & `cf_xarray-0.8.3/doc/coding.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/conf.py` & `cf_xarray-0.8.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/contributing.rst` & `cf_xarray-0.8.3/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/coord_axes.md` & `cf_xarray-0.8.3/doc/coord_axes.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/custom-criteria.md` & `cf_xarray-0.8.3/doc/custom-criteria.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/dsg.md` & `cf_xarray-0.8.3/doc/dsg.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/examples/introduction.ipynb` & `cf_xarray-0.8.3/doc/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/flags.md` & `cf_xarray-0.8.3/doc/flags.md`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 ```{code-cell}
 from cf_xarray.datasets import flag_indep
 
 flag_indep
 ```
 
 ```{code-cell}
-flag_indep.cf.is_flag_variable
+flag_indep.cf
 ```
 
 ```{code-cell}
 flag_indep.cf == "flag_1"
 ```
 
 And `isin`
@@ -99,13 +99,13 @@
 ```{code-cell}
 from cf_xarray.datasets import flag_mix
 
 flag_mix
 ```
 
 ```{code-cell}
-flag_mix.cf.is_flag_variable
+flag_mix.cf
 ```
 
 ```{code-cell}
 flag_mix.cf == 'flag_4'
 ```
```

### Comparing `cf_xarray-0.8.2/doc/grid_mappings.md` & `cf_xarray-0.8.3/doc/grid_mappings.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/howtouse.md` & `cf_xarray-0.8.3/doc/howtouse.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/index.rst` & `cf_xarray-0.8.3/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/make.bat` & `cf_xarray-0.8.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/parametricz.md` & `cf_xarray-0.8.3/doc/parametricz.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/plotting.md` & `cf_xarray-0.8.3/doc/plotting.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/provenance.md` & `cf_xarray-0.8.3/doc/provenance.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/quickstart.md` & `cf_xarray-0.8.3/doc/quickstart.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/roadmap.rst` & `cf_xarray-0.8.3/doc/roadmap.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/selecting.md` & `cf_xarray-0.8.3/doc/selecting.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/sgrid_ugrid.md` & `cf_xarray-0.8.3/doc/sgrid_ugrid.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/units.md` & `cf_xarray-0.8.3/doc/units.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.2/doc/whats-new.rst` & `cf_xarray-0.8.3/doc/whats-new.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 .. currentmodule:: xarray
 
 What's New
 ----------
 
+v0.8.2 (July 05, 2023)
+======================
+- Better reprs for flag masks. By `Deepak Cherian`_.
+
 v0.8.2 (June 23, 2023)
 ======================
 - Support for flag masks. By `Clément Haëck`_ and `Deepak Cherian`_.
 
 v0.8.1 (May 9, 2023)
 ====================
 - Stop bundling the standard name table and use ``pooch`` (new optional dependency) to download when needed.
```

### Comparing `cf_xarray-0.8.2/pyproject.toml` & `cf_xarray-0.8.3/pyproject.toml`

 * *Files identical despite different names*

