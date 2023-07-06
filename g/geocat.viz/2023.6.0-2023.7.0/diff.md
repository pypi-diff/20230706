# Comparing `tmp/geocat.viz-2023.6.0.tar.gz` & `tmp/geocat.viz-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocat.viz-2023.6.0.tar", last modified: Fri Jun  2 04:18:53 2023, max compression
+gzip compressed data, was "geocat.viz-2023.7.0.tar", last modified: Thu Jul  6 21:14:58 2023, max compression
```

## Comparing `geocat.viz-2023.6.0.tar` & `geocat.viz-2023.7.0.tar`

### file list

```diff
@@ -1,74 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.931011 geocat.viz-2023.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.935011 geocat.viz-2023.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/.github/ISSUE_TEMPLATE/plot-type-request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.935011 geocat.viz-2023.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/.github/workflows/upstream-examples-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/INSTALLATION.md
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.935011 geocat.viz-2023.6.0/build_envs/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/build_envs/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/build_envs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/build_envs/upstream-dev-environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.935011 geocat.viz-2023.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.935011 geocat.viz-2023.6.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.931011 geocat.viz-2023.6.0/docs/_static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.935011 geocat.viz-2023.6.0/docs/_static/images/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/images/icons/code.svg
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/images/icons/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/images/icons/notpublic.svg
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/images/icons/public.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/docs/_static/images/logos/
--rw-r--r--   0 runner    (1001) docker     (123)   171533 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/images/logos/GeoCAT_long.svg
--rw-r--r--   0 runner    (1001) docker     (123)   291776 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/images/logos/GeoCAT_nsf.svg
--rw-r--r--   0 runner    (1001) docker     (123)   180376 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/images/logos/GeoCAT_square.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/images/logos/nsf.png
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.931011 geocat.viz-2023.6.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/docs/internal_api/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/internal_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/docs/user_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/docs/user_api/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.931011 geocat.viz-2023.6.0/gallery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/gallery/util/
--rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/gallery/util/add_height_from_pressure_axis.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.935011 geocat.viz-2023.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/src/geocat/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/src/geocat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/src/geocat/viz/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/src/geocat/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30354 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/src/geocat/viz/taylor.py
--rw-r--r--   0 runner    (1001) docker     (123)    62471 2023-06-02 04:18:41.000000 geocat.viz-2023.6.0/src/geocat/viz/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:18:53.939011 geocat.viz-2023.6.0/src/geocat.viz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-02 04:18:53.000000 geocat.viz-2023.6.0/src/geocat.viz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-02 04:18:53.000000 geocat.viz-2023.6.0/src/geocat.viz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 04:18:53.000000 geocat.viz-2023.6.0/src/geocat.viz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 04:18:53.000000 geocat.viz-2023.6.0/src/geocat.viz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-02 04:18:53.000000 geocat.viz-2023.6.0/src/geocat.viz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 04:18:53.000000 geocat.viz-2023.6.0/src/geocat.viz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.839025 geocat.viz-2023.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.827024 geocat.viz-2023.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.831025 geocat.viz-2023.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/.github/ISSUE_TEMPLATE/plot-type-request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.831025 geocat.viz-2023.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-06 21:14:58.839025 geocat.viz-2023.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.831025 geocat.viz-2023.7.0/build_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/build_envs/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/build_envs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/build_envs/upstream-dev-environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.831025 geocat.viz-2023.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.831025 geocat.viz-2023.7.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.827024 geocat.viz-2023.7.0/docs/_static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.831025 geocat.viz-2023.7.0/docs/_static/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/images/icons/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/images/icons/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/images/icons/electric_bolt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/images/icons/handshake.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/images/icons/menu_book.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/images/icons/notpublic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/images/icons/public.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/images/icons/science.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/images/icons/tips.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.835025 geocat.viz-2023.7.0/docs/_static/images/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)   171533 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/images/logos/GeoCAT_long.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   291776 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/images/logos/GeoCAT_nsf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   180376 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/images/logos/GeoCAT_square.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/images/logos/nsf.png
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.835025 geocat.viz-2023.7.0/docs/_static/thumbnails/
+-rw-r--r--   0 runner    (1001) docker     (123)   120452 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/thumbnails/add_height_from_pressure_axis.png
+-rw-r--r--   0 runner    (1001) docker     (123)   122204 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/thumbnails/add_lat_lon_gridlines.png
+-rw-r--r--   0 runner    (1001) docker     (123)   212135 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/thumbnails/add_lat_lon_ticklabels.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35504 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/thumbnails/add_major_minor_ticks.png
+-rw-r--r--   0 runner    (1001) docker     (123)   159700 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/thumbnails/add_right_hand_axis.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_static/thumbnails/set_tick_direction_spine_visibility.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.827024 geocat.viz-2023.7.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.835025 geocat.viz-2023.7.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.835025 geocat.viz-2023.7.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   163435 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/examples/add_height_from_pressure_axis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   168202 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/examples/add_lat_lon_gridlines.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   286260 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/examples/add_lat_lon_ticklabels.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    49604 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/examples/add_major_minor_ticks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   215927 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/examples/add_right_hand_axis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/examples/set_tick_direction_spine_visibility.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/gallery.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/getting-started.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.835025 geocat.viz-2023.7.0/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/getting_started/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/getting_started/quick-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.835025 geocat.viz-2023.7.0/docs/internal_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/internal_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/support.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.835025 geocat.viz-2023.7.0/docs/user_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/docs/user_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-06 21:14:58.839025 geocat.viz-2023.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.827024 geocat.viz-2023.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.835025 geocat.viz-2023.7.0/src/geocat/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/src/geocat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.839025 geocat.viz-2023.7.0/src/geocat/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/src/geocat/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30354 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/src/geocat/viz/taylor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63172 2023-07-06 21:14:46.000000 geocat.viz-2023.7.0/src/geocat/viz/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:14:58.839025 geocat.viz-2023.7.0/src/geocat.viz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-06 21:14:58.000000 geocat.viz-2023.7.0/src/geocat.viz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-06 21:14:58.000000 geocat.viz-2023.7.0/src/geocat.viz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:14:58.000000 geocat.viz-2023.7.0/src/geocat.viz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:14:58.000000 geocat.viz-2023.7.0/src/geocat.viz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-06 21:14:58.000000 geocat.viz-2023.7.0/src/geocat.viz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 21:14:58.000000 geocat.viz-2023.7.0/src/geocat.viz.egg-info/top_level.txt
```

### Comparing `geocat.viz-2023.6.0/.github/workflows/ci.yml` & `geocat.viz-2023.7.0/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         with:
           activate-environment: geocat_viz_build
           channel-priority: strict
           python-version: ${{ matrix.python-version }}
           channels: conda-forge
           environment-file: build_envs/environment.yml
 
-      - name: Install geocat-comp
+      - name: Install geocat-viz
         run: |
           python -m pip install . --no-deps
 
       - name: conda list
         run: |
           conda list
```

### Comparing `geocat.viz-2023.6.0/.github/workflows/pypi.yaml` & `geocat.viz-2023.7.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/.pre-commit-config.yaml` & `geocat.viz-2023.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/CONTRIBUTING.md` & `geocat.viz-2023.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/LICENSE` & `geocat.viz-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/PKG-INFO` & `geocat.viz-2023.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocat.viz
-Version: 2023.6.0
+Version: 2023.7.0
 Summary: GeoCAT-viz is vizualization component of the GeoCAT project and
 Home-page: https://geocat-viz.readthedocs.io
 Author: GeoCAT Team
 Author-email: geocat@ucar.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `geocat.viz-2023.6.0/README.md` & `geocat.viz-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/build_envs/upstream-dev-environment.yml` & `geocat.viz-2023.7.0/build_envs/upstream-dev-environment.yml`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   - fiona
   - geocat-viz
   - cartopy
   - geographiclib
   - jupyter
   - jupyterlab
   - make
-  - matplotlib<3.6
+  - matplotlib
   - metpy
   - mock
   - myst-nb
   - nbsphinx
   - netcdf4
   - pillow
   - pint
@@ -28,7 +28,8 @@
   - sphinx-gallery
   - sphinx_rtd_theme
   - sphinx-design
   - sphinx-book-theme
   - wrf-python
   - xarray<=2023.02.0 # pinned as per issue #98
   - pre-commit
+  - geocat-datafiles # for examples/tests
```

### Comparing `geocat.viz-2023.6.0/docs/Makefile` & `geocat.viz-2023.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/docs/_static/images/icons/code.svg` & `geocat.viz-2023.7.0/docs/_static/images/icons/code.svg`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/docs/_static/images/icons/notpublic.svg` & `geocat.viz-2023.7.0/docs/_static/images/icons/notpublic.svg`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/docs/_static/images/icons/public.svg` & `geocat.viz-2023.7.0/docs/_static/images/icons/public.svg`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/docs/_static/images/logos/GeoCAT_long.svg` & `geocat.viz-2023.7.0/docs/_static/images/logos/GeoCAT_long.svg`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/docs/_static/images/logos/GeoCAT_nsf.svg` & `geocat.viz-2023.7.0/docs/_static/images/logos/GeoCAT_nsf.svg`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/docs/_static/images/logos/GeoCAT_square.svg` & `geocat.viz-2023.7.0/docs/_static/images/logos/GeoCAT_square.svg`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/docs/_static/images/logos/nsf.png` & `geocat.viz-2023.7.0/docs/_static/images/logos/nsf.png`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/docs/_templates/autosummary/class.rst` & `geocat.viz-2023.7.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/docs/api.rst` & `geocat.viz-2023.7.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/docs/citation.rst` & `geocat.viz-2023.7.0/docs/citation.rst`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/docs/conf.py` & `geocat.viz-2023.7.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -315,18 +315,56 @@
 #html_search_scorer = 'scorer.js'
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = 'geocat-vizdoc'
 
 autodoc_typehints = 'none'
 
+
+# custom scripts for making a gallery of examples notebooks
+# note: this method only supports a single gallery
+def update_gallery(app: Sphinx):
+    """Update the gallery of examples notebooks."""
+
+    LOGGER.info("creating gallery...")
+
+    notebooks = yaml.safe_load(
+        pathlib.Path(app.srcdir, "gallery.yml").read_bytes())
+
+    items = [
+        f"""
+         .. grid-item-card::
+            :text-align: center
+            :link: {item['path']}
+
+            .. image:: {item['thumbnail']}
+                :alt: {item['title']}
+            +++
+            {item['title']}
+            """ for item in notebooks
+    ]
+
+    items_md = indent(dedent("\n".join(items)), prefix="    ")
+    markdown = f"""
+.. grid:: 1 2 3 3
+    :gutter: 2
+
+    {items_md}
+    """
+
+    pathlib.Path(app.srcdir, "notebook-examples.txt").write_text(markdown)
+
+    LOGGER.info("gallery created")
+
+
 # turn off notebook execution
 # set to "auto" for default behavior
 nb_execution_mode = "off"
 
 # generate warning for all invalid links
 #nitpicky = True
 
 
 # Allow for changes to be made to the css in the theme_overrides file
 def setup(app):
     app.add_css_file('theme_overrides.css')
+    app.connect("builder-inited", update_gallery)
```

### Comparing `geocat.viz-2023.6.0/docs/index.rst` & `geocat.viz-2023.7.0/docs/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,32 @@
 The GeoCAT-viz repo contains tools to help plot data, including convenience and plotting functions that are used
 to facilitate plotting geosciences data with Matplotlib, Cartopy, and possibly other Python ecosystem
 plotting packages.
 
 .. grid:: 1 1 2 2
     :gutter: 2
 
+    .. grid-item-card:: Getting Started
+        :class-title: custom-title
+        :class-body: custom-body
+        :img-top: _static/images/icons/tips.svg
+        :link: getting-started
+        :link-type: doc
+
+        A good place to start for new users
+
+    .. grid-item-card::  Examples
+        :class-title: custom-title
+        :class-body: custom-body
+        :img-top: _static/images/icons/science.svg
+        :link: examples
+        :link-type: doc
+
+        A gallery of examples using GeoCAT-viz
+
     .. grid-item-card::  Installation
         :class-title: custom-title
         :class-body: custom-body
         :img-top: _static/images/icons/download.svg
         :link: installation
         :link-type: doc
```

### Comparing `geocat.viz-2023.6.0/docs/installation.rst` & `geocat.viz-2023.7.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/docs/make.bat` & `geocat.viz-2023.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/docs/release-notes.rst` & `geocat.viz-2023.7.0/docs/release-notes.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 .. currentmodule:: geocat.viz
 
 .. _release:
 Release Notes
 =============
 
+v2023.07.0 (July 6, 2023)
+-------------------------
+
+Matplotlib unpinned and an examples gallery added.
+
+Bug Fixes
+^^^^^^^^^^^^
+* Matplotlib unpinned by `Katelyn Fitzgerald`_ in (:pr:`134`)
+
+Documentation
+^^^^^^^^^^^^^
+* Examples gallery with usage examples of `add_height_from_pressure_axis()`, `add_lat_lon_gridlines()`, and `add_lat_lon_ticklabels()` added by `Julia Kent`_ in (:pr:`133`)
+* More examples including `set_tick_direction_spine_visibility()`, `add_right_hand_axis()`, `add_major_minor_ticks()` added by y `Julia Kent`_ in (:pr:`135`)
+
 v2023.06.0 (Jun 1, 2023)
 -------------------------
 
 Function and keyword argument names have been adjusted to follow consistent formatting and style, and one bug fix.
 
 Deprecations
 ^^^^^^^^^^^^
```

### Comparing `geocat.viz-2023.6.0/docs/support.rst` & `geocat.viz-2023.7.0/docs/support.rst`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/docs/user_api/index.rst` & `geocat.viz-2023.7.0/docs/user_api/index.rst`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/setup.cfg` & `geocat.viz-2023.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/src/geocat/viz/taylor.py` & `geocat.viz-2023.7.0/src/geocat/viz/taylor.py`

 * *Files identical despite different names*

### Comparing `geocat.viz-2023.6.0/src/geocat/viz/util.py` & `geocat.viz-2023.7.0/src/geocat/viz/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,17 @@
         Set False to turn off left spine of the axes.
 
     right_spine_visible : bool
         Set False to turn off right spine.
 
     Examples
     --------
-    All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+     See this example notebook: :doc:`../../examples/set_tick_direction_spine_visibility`.
+
+     More in-depth plotting examples that utilize this function are in the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
     - `NCL_box_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Boxplots/NCL_box_2.html?highlight=set_tick_direction_spine_visibility>`_
     """
 
     ax.tick_params(direction=tick_direction, axis='both', which='both')
     ax.spines['top'].set_visible(top_spine_visible)
     ax.spines['bottom'].set_visible(bottom_spine_visible)
@@ -126,15 +128,17 @@
     Returns
     -------
     gl : :class:`cartopy.mpl.gridliner.Gridliner`
         A Cartopy GridLiner object.
 
     Examples
     --------
-    All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+    See this example notebook: :doc:`../../examples/add_lat_lon_gridlines`.
+
+    More in-depth plotting examples that utilize this function are in the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
     - `NCL_native_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_native_1.html?highlight=add_lat_lon_gridlines>`_
 
     - `NCL_native_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/MapProjections/NCL_native_2.html?highlight=add_lat_lon_gridlines>`_
     """
 
     # Draw gridlines
@@ -193,15 +197,17 @@
     Returns
     -------
     axRHS : :class:`matplotlib.axes._subplots.AxesSubplot`, :class:`cartopy.mpl.geoaxes.GeoAxesSubplot`
         The created right-hand axis
 
     Examples
     --------
-    All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+    See this example notebook: :doc:`../../examples/add_right_hand_axis`.
+
+    More in-depth plotting examples that utilize this function are in the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
     - `NCL_coneff_8.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_coneff_8.html?highlight=add_right_hand_axis>`_
     """
 
     axRHS = ax.twinx()
     if label is not None:
         axRHS.set_ylabel(ylabel=label,
@@ -262,15 +268,17 @@
     See ALso
     --------
     Related NCL Functions:
         `gsn_csm_pres_hgt <https://www.ncl.ucar.edu/Document/Graphics/Interfaces/gsn_csm_pres_hgt.shtml>`_,
 
     Examples
     --------
-    All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+    See this example notebook: :doc:`../../examples/add_height_from_pressure_axis`.
+
+    More in-depth plotting examples that utilize this function are in the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
     - `NCL_conOncon_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_conOncon_1.html?highlight=add_height_from_pressure_axis>`_
 
     - `NCL_h_lat_6.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_h_lat_6.html?highlight=add_height_from_pressure_axis>`_
 
     - `NCL_h_lat_7.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_h_lat_7.html?highlight=add_height_from_pressure_axis>`_
 
@@ -331,15 +339,17 @@
         Set True to get 0 E / O W or False to get 0 only.
 
     dateline_direction_label : bool
         Set True to get 180 E / 180 W or False to get 180 only.
 
     Examples
     --------
-    All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+    See this example notebook: :doc:`../../examples/add_lat_lon_ticklabels`.
+
+    More in-depth plotting examples that utilize this function are in the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
     - `NCL_ce_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_ce_1.html?highlight=add_lat_lon_ticklabels>`_
 
     - `NCL_ce_3_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_ce_3_2.html?highlight=add_lat_lon_ticklabels>`_
 
     - `NCL_conOncon_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Contours/NCL_conOncon_2.html?highlight=add_lat_lon_ticklabels>`_
     """
@@ -394,15 +404,17 @@
         An argument passed to SymmetricalLogLocator if the yaxis scale is
         `symlog`. Defines the range (-x, x), within which the plot is
         linear. This avoids having the plot go to infinity around zero.
         Defaults to 2.
 
     Examples
     --------
-    All usage examples are within the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
+    See this example notebook: :doc:`../../examples/add_major_minor_ticks`.
+
+    More in-depth plotting examples that utilize this function are in the GeoCAT-Examples Gallery. To see more usage cases, search the function on the `website <https://geocat-examples.readthedocs.io/en/latest/index.html>`_.
 
     - `NCL_bar_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Bar/NCL_bar_2.html?highlight=add_major_minor_ticks>`_
 
     - `NCL_box_2.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Boxplots/NCL_box_2.html?highlight=add_major_minor_ticks>`_
 
     - `NCL_scatter_1.py <https://geocat-examples.readthedocs.io/en/latest/gallery/Scatter/NCL_scatter_1.html?highlight=add_major_minor_ticks>`_
     """
```

### Comparing `geocat.viz-2023.6.0/src/geocat.viz.egg-info/PKG-INFO` & `geocat.viz-2023.7.0/src/geocat.viz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocat.viz
-Version: 2023.6.0
+Version: 2023.7.0
 Summary: GeoCAT-viz is vizualization component of the GeoCAT project and
 Home-page: https://geocat-viz.readthedocs.io
 Author: GeoCAT Team
 Author-email: geocat@ucar.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `geocat.viz-2023.6.0/src/geocat.viz.egg-info/SOURCES.txt` & `geocat.viz-2023.7.0/src/geocat.viz.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -9,42 +9,61 @@
 pyproject.toml
 setup.cfg
 setup.py
 .github/ISSUE_TEMPLATE/plot-type-request.md
 .github/workflows/ci.yml
 .github/workflows/pre-commit.yml
 .github/workflows/pypi.yaml
-.github/workflows/upstream-examples-ci.yml
 build_envs/docs.yml
 build_envs/environment.yml
 build_envs/upstream-dev-environment.yml
 docs/Makefile
 docs/api.rst
 docs/citation.rst
 docs/conf.py
 docs/examples.rst
+docs/gallery.yml
+docs/getting-started.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/release-notes.rst
 docs/support.rst
 docs/_static/style.css
 docs/_static/theme_overrides.css
 docs/_static/images/icons/code.svg
 docs/_static/images/icons/download.svg
+docs/_static/images/icons/electric_bolt.svg
+docs/_static/images/icons/handshake.svg
+docs/_static/images/icons/menu_book.svg
 docs/_static/images/icons/notpublic.svg
 docs/_static/images/icons/public.svg
+docs/_static/images/icons/science.svg
+docs/_static/images/icons/tips.svg
 docs/_static/images/logos/GeoCAT_long.svg
 docs/_static/images/logos/GeoCAT_nsf.svg
 docs/_static/images/logos/GeoCAT_square.svg
 docs/_static/images/logos/nsf.png
+docs/_static/thumbnails/add_height_from_pressure_axis.png
+docs/_static/thumbnails/add_lat_lon_gridlines.png
+docs/_static/thumbnails/add_lat_lon_ticklabels.png
+docs/_static/thumbnails/add_major_minor_ticks.png
+docs/_static/thumbnails/add_right_hand_axis.png
+docs/_static/thumbnails/set_tick_direction_spine_visibility.png
 docs/_templates/autosummary/class.rst
+docs/examples/add_height_from_pressure_axis.ipynb
+docs/examples/add_lat_lon_gridlines.ipynb
+docs/examples/add_lat_lon_ticklabels.ipynb
+docs/examples/add_major_minor_ticks.ipynb
+docs/examples/add_right_hand_axis.ipynb
+docs/examples/set_tick_direction_spine_visibility.ipynb
+docs/getting_started/overview.rst
+docs/getting_started/quick-install.rst
 docs/internal_api/index.rst
 docs/user_api/index.rst
-gallery/util/add_height_from_pressure_axis.ipynb
 src/geocat/__init__.py
 src/geocat.viz.egg-info/PKG-INFO
 src/geocat.viz.egg-info/SOURCES.txt
 src/geocat.viz.egg-info/dependency_links.txt
 src/geocat.viz.egg-info/not-zip-safe
 src/geocat.viz.egg-info/requires.txt
 src/geocat.viz.egg-info/top_level.txt
```

