# Comparing `tmp/impose-0.4.1.tar.gz` & `tmp/impose-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose-0.4.1.tar", last modified: Fri Oct 14 06:35:24 2022, max compression
+gzip compressed data, was "impose-0.4.2.tar", last modified: Thu Jul  6 08:15:09 2023, max compression
```

## Comparing `impose-0.4.1.tar` & `impose-0.4.2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:35:24.268689 impose-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-10-14 06:34:55.000000 impose-0.4.1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-14 06:34:55.000000 impose-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-10-14 06:34:55.000000 impose-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-10-14 06:35:24.268689 impose-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-10-14 06:34:55.000000 impose-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:35:24.256689 impose-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-10-14 06:34:55.000000 impose-0.4.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     6434 2022-10-14 06:34:55.000000 impose-0.4.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:35:24.256689 impose-0.4.1/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)     2375 2022-10-14 06:34:55.000000 impose-0.4.1/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-14 06:34:55.000000 impose-0.4.1/docs/impose.bib
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-10-14 06:34:55.000000 impose-0.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-14 06:34:55.000000 impose-0.4.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-10-14 06:34:55.000000 impose-0.4.1/docs/sec_changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-10-14 06:34:55.000000 impose-0.4.1/docs/sec_getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-14 06:34:55.000000 impose-0.4.1/docs/sec_z_bib.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:35:24.260689 impose-0.4.1/impose/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-10-14 06:34:55.000000 impose-0.4.1/impose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-10-14 06:34:55.000000 impose-0.4.1/impose/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7035 2022-10-14 06:34:55.000000 impose-0.4.1/impose/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-14 06:35:03.000000 impose-0.4.1/impose/_version_save.py
--rw-r--r--   0 runner    (1001) docker     (121)     7783 2022-10-14 06:34:55.000000 impose-0.4.1/impose/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     9185 2022-10-14 06:34:55.000000 impose-0.4.1/impose/flblend.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:35:24.260689 impose-0.4.1/impose/formats/
--rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-10-14 06:34:55.000000 impose-0.4.1/impose/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-10-14 06:34:55.000000 impose-0.4.1/impose/formats/fmt_bf_generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     4635 2022-10-14 06:34:55.000000 impose-0.4.1/impose/formats/fmt_bm_bmlab.py
--rw-r--r--   0 runner    (1001) docker     (121)     3391 2022-10-14 06:34:55.000000 impose-0.4.1/impose/formats/fmt_fl_zeiss.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:35:24.260689 impose-0.4.1/impose/geometry/
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-10-14 06:34:55.000000 impose-0.4.1/impose/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-10-14 06:34:55.000000 impose-0.4.1/impose/geometry/mask.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:35:24.260689 impose-0.4.1/impose/geometry/shapes/
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-14 06:34:55.000000 impose-0.4.1/impose/geometry/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3249 2022-10-14 06:34:55.000000 impose-0.4.1/impose/geometry/shapes/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-10-14 06:34:55.000000 impose-0.4.1/impose/geometry/shapes/sh_circle.py
--rw-r--r--   0 runner    (1001) docker     (121)     5122 2022-10-14 06:34:55.000000 impose-0.4.1/impose/geometry/shapes/sh_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (121)     4187 2022-10-14 06:34:55.000000 impose-0.4.1/impose/geometry/shapes/sh_polygon.py
--rw-r--r--   0 runner    (1001) docker     (121)     4977 2022-10-14 06:34:55.000000 impose-0.4.1/impose/geometry/shapes/sh_rectangle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:35:24.260689 impose-0.4.1/impose/gui/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11665 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/collect.py
--rw-r--r--   0 runner    (1001) docker     (121)    10098 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/collect.ui
--rw-r--r--   0 runner    (1001) docker     (121)     4483 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/collect_pgrois.py
--rw-r--r--   0 runner    (1001) docker     (121)     5799 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/collect_shape_controls.py
--rw-r--r--   0 runner    (1001) docker     (121)     3806 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/collect_shape_controls.ui
--rw-r--r--   0 runner    (1001) docker     (121)    14077 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/colocalize.py
--rw-r--r--   0 runner    (1001) docker     (121)    15458 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/colocalize.ui
--rw-r--r--   0 runner    (1001) docker     (121)    10469 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/colocalize_pgrois.py
--rw-r--r--   0 runner    (1001) docker     (121)     4257 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/dlg_edit_circle.ui
--rw-r--r--   0 runner    (1001) docker     (121)     5564 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/dlg_edit_ellipse.ui
--rw-r--r--   0 runner    (1001) docker     (121)     2271 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/dlg_edit_polygon.ui
--rw-r--r--   0 runner    (1001) docker     (121)     5569 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/dlg_edit_rectangle.ui
--rw-r--r--   0 runner    (1001) docker     (121)     4446 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/dlg_edit_shape.py
--rw-r--r--   0 runner    (1001) docker     (121)     6413 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/main.ui
--rw-r--r--   0 runner    (1001) docker     (121)    10090 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/visualize.py
--rw-r--r--   0 runner    (1001) docker     (121)    11148 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/visualize.ui
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:35:24.260689 impose-0.4.1/impose/gui/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/widgets/simple_image_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     4585 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/widgets/simple_plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-10-14 06:34:55.000000 impose-0.4.1/impose/gui/widgets/wait_cursor.py
--rw-r--r--   0 runner    (1001) docker     (121)    11748 2022-10-14 06:34:55.000000 impose-0.4.1/impose/session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:35:24.264689 impose-0.4.1/impose/structure/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-10-14 06:34:55.000000 impose-0.4.1/impose/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7937 2022-10-14 06:34:55.000000 impose-0.4.1/impose/structure/composite.py
--rw-r--r--   0 runner    (1001) docker     (121)     2716 2022-10-14 06:34:55.000000 impose-0.4.1/impose/structure/composite_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     7235 2022-10-14 06:34:55.000000 impose-0.4.1/impose/structure/layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2942 2022-10-14 06:34:55.000000 impose-0.4.1/impose/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:35:24.260689 impose-0.4.1/impose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-10-14 06:35:24.000000 impose-0.4.1/impose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2591 2022-10-14 06:35:24.000000 impose-0.4.1/impose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-14 06:35:24.000000 impose-0.4.1/impose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-14 06:35:24.000000 impose-0.4.1/impose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-14 06:35:24.000000 impose-0.4.1/impose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-10-14 06:35:24.268689 impose-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-10-14 06:34:55.000000 impose-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:35:24.264689 impose-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-10-14 06:34:55.000000 impose-0.4.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:35:24.268689 impose-0.4.1/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (121)     4464 2022-10-14 06:34:55.000000 impose-0.4.1/tests/data/brillouin-invalid.h5
--rw-r--r--   0 runner    (1001) docker     (121)     7566 2022-10-14 06:34:55.000000 impose-0.4.1/tests/data/brillouin-wo-signature.impose-session
--rw-r--r--   0 runner    (1001) docker     (121)   118968 2022-10-14 06:34:55.000000 impose-0.4.1/tests/data/brillouin.h5
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-10-14 06:34:55.000000 impose-0.4.1/tests/data/brillouin.impose-composite
--rw-r--r--   0 runner    (1001) docker     (121)     7894 2022-10-14 06:34:55.000000 impose-0.4.1/tests/data/brillouin.impose-session
--rw-r--r--   0 runner    (1001) docker     (121)     6301 2022-10-14 06:34:55.000000 impose-0.4.1/tests/data/brillouin_cutout.impose-session
--rw-r--r--   0 runner    (1001) docker     (121)    99622 2022-10-14 06:34:55.000000 impose-0.4.1/tests/data/fmt_brillouin-h5_bmlab-session_2022.zip
--rw-r--r--   0 runner    (1001) docker     (121)   194328 2022-10-14 06:34:55.000000 impose-0.4.1/tests/data/fmt_brillouin-h5_bmlab-session_2022_2-rep.zip
--rw-r--r--   0 runner    (1001) docker     (121)   426967 2022-10-14 06:34:55.000000 impose-0.4.1/tests/data/fmt_brillouin-h5_bmlab-session_2022_water.zip
--rw-r--r--   0 runner    (1001) docker     (121)   881709 2022-10-14 06:34:55.000000 impose-0.4.1/tests/data/fmt_brillouin-h5_bmlab-session_2022_water_2-rep.zip
--rw-r--r--   0 runner    (1001) docker     (121)   333519 2022-10-14 06:34:55.000000 impose-0.4.1/tests/data/lsm-fish.zip
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-10-14 06:34:55.000000 impose-0.4.1/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-14 06:34:55.000000 impose-0.4.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3019 2022-10-14 06:34:55.000000 impose-0.4.1/tests/test_data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     3930 2022-10-14 06:34:55.000000 impose-0.4.1/tests/test_flblend.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-10-14 06:34:55.000000 impose-0.4.1/tests/test_fmt_czi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-10-14 06:34:55.000000 impose-0.4.1/tests/test_fmt_h5_brillouin_bmlab.py
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-10-14 06:34:55.000000 impose-0.4.1/tests/test_fmt_h5_brillouin_legacy.py
--rw-r--r--   0 runner    (1001) docker     (121)    12289 2022-10-14 06:34:55.000000 impose-0.4.1/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (121)     4069 2022-10-14 06:34:55.000000 impose-0.4.1/tests/test_gui_collect.py
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-10-14 06:34:55.000000 impose-0.4.1/tests/test_gui_colocalize.py
--rw-r--r--   0 runner    (1001) docker     (121)     9366 2022-10-14 06:34:55.000000 impose-0.4.1/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (121)     8281 2022-10-14 06:34:55.000000 impose-0.4.1/tests/test_structure_composite.py
--rw-r--r--   0 runner    (1001) docker     (121)     2252 2022-10-14 06:34:55.000000 impose-0.4.1/tests/test_structure_composite_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-10-14 06:34:55.000000 impose-0.4.1/tests/test_structure_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-10-14 06:34:55.000000 impose-0.4.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:15:09.687625 impose-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-06 08:14:24.000000 impose-0.4.2/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-06 08:14:24.000000 impose-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-06 08:14:24.000000 impose-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-06 08:15:09.687625 impose-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-06 08:14:24.000000 impose-0.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:15:09.675625 impose-0.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 08:14:24.000000 impose-0.4.2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-07-06 08:14:24.000000 impose-0.4.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:15:09.675625 impose-0.4.2/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-06 08:14:24.000000 impose-0.4.2/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-06 08:14:24.000000 impose-0.4.2/docs/impose.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-06 08:14:24.000000 impose-0.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-06 08:14:24.000000 impose-0.4.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-06 08:14:24.000000 impose-0.4.2/docs/sec_changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-06 08:14:24.000000 impose-0.4.2/docs/sec_getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 08:14:24.000000 impose-0.4.2/docs/sec_z_bib.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:15:09.675625 impose-0.4.2/impose/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-06 08:14:24.000000 impose-0.4.2/impose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-06 08:14:24.000000 impose-0.4.2/impose/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-07-06 08:14:24.000000 impose-0.4.2/impose/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-06 08:14:43.000000 impose-0.4.2/impose/_version_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-07-06 08:14:24.000000 impose-0.4.2/impose/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-07-06 08:14:24.000000 impose-0.4.2/impose/flblend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:15:09.675625 impose-0.4.2/impose/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-06 08:14:24.000000 impose-0.4.2/impose/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-06 08:14:24.000000 impose-0.4.2/impose/formats/fmt_bf_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-06 08:14:24.000000 impose-0.4.2/impose/formats/fmt_bm_bmlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-06 08:14:24.000000 impose-0.4.2/impose/formats/fmt_fl_zeiss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:15:09.679625 impose-0.4.2/impose/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-06 08:14:24.000000 impose-0.4.2/impose/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-06 08:14:24.000000 impose-0.4.2/impose/geometry/mask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:15:09.679625 impose-0.4.2/impose/geometry/shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 08:14:24.000000 impose-0.4.2/impose/geometry/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-06 08:14:24.000000 impose-0.4.2/impose/geometry/shapes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-06 08:14:24.000000 impose-0.4.2/impose/geometry/shapes/sh_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-06 08:14:24.000000 impose-0.4.2/impose/geometry/shapes/sh_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-06 08:14:24.000000 impose-0.4.2/impose/geometry/shapes/sh_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-06 08:14:24.000000 impose-0.4.2/impose/geometry/shapes/sh_rectangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:15:09.679625 impose-0.4.2/impose/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/collect.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/collect_pgrois.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/collect_shape_controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/collect_shape_controls.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    14077 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/colocalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/colocalize.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    10805 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/colocalize_pgrois.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/dlg_edit_circle.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/dlg_edit_ellipse.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/dlg_edit_polygon.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/dlg_edit_rectangle.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/dlg_edit_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/main.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/visualize.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:15:09.679625 impose-0.4.2/impose/gui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/widgets/simple_image_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/widgets/simple_plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-06 08:14:24.000000 impose-0.4.2/impose/gui/widgets/wait_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-07-06 08:14:24.000000 impose-0.4.2/impose/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:15:09.679625 impose-0.4.2/impose/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-06 08:14:24.000000 impose-0.4.2/impose/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-06 08:14:24.000000 impose-0.4.2/impose/structure/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-06 08:14:24.000000 impose-0.4.2/impose/structure/composite_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-06 08:14:24.000000 impose-0.4.2/impose/structure/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-06 08:14:24.000000 impose-0.4.2/impose/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:15:09.675625 impose-0.4.2/impose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-06 08:15:09.000000 impose-0.4.2/impose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-06 08:15:09.000000 impose-0.4.2/impose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 08:15:09.000000 impose-0.4.2/impose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-06 08:15:09.000000 impose-0.4.2/impose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 08:15:09.000000 impose-0.4.2/impose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-06 08:15:09.687625 impose-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-06 08:14:24.000000 impose-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:15:09.683625 impose-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-06 08:14:24.000000 impose-0.4.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:15:09.687625 impose-0.4.2/tests/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4464 2023-07-06 08:14:24.000000 impose-0.4.2/tests/data/brillouin-invalid.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-06 08:14:24.000000 impose-0.4.2/tests/data/brillouin-wo-signature.impose-session
+-rw-r--r--   0 runner    (1001) docker     (123)   118968 2023-07-06 08:14:24.000000 impose-0.4.2/tests/data/brillouin.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-06 08:14:24.000000 impose-0.4.2/tests/data/brillouin.impose-composite
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-06 08:14:24.000000 impose-0.4.2/tests/data/brillouin.impose-session
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-07-06 08:14:24.000000 impose-0.4.2/tests/data/brillouin_cutout.impose-session
+-rw-r--r--   0 runner    (1001) docker     (123)    99622 2023-07-06 08:14:24.000000 impose-0.4.2/tests/data/fmt_brillouin-h5_bmlab-session_2022.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   194328 2023-07-06 08:14:24.000000 impose-0.4.2/tests/data/fmt_brillouin-h5_bmlab-session_2022_2-rep.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   426967 2023-07-06 08:14:24.000000 impose-0.4.2/tests/data/fmt_brillouin-h5_bmlab-session_2022_water.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   881709 2023-07-06 08:14:24.000000 impose-0.4.2/tests/data/fmt_brillouin-h5_bmlab-session_2022_water_2-rep.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   333519 2023-07-06 08:14:24.000000 impose-0.4.2/tests/data/lsm-fish.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-06 08:14:24.000000 impose-0.4.2/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 08:14:24.000000 impose-0.4.2/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-06 08:14:24.000000 impose-0.4.2/tests/test_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-07-06 08:14:24.000000 impose-0.4.2/tests/test_flblend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-06 08:14:24.000000 impose-0.4.2/tests/test_fmt_czi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-06 08:14:24.000000 impose-0.4.2/tests/test_fmt_h5_brillouin_bmlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-06 08:14:24.000000 impose-0.4.2/tests/test_fmt_h5_brillouin_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-07-06 08:14:24.000000 impose-0.4.2/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-06 08:14:24.000000 impose-0.4.2/tests/test_gui_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-06 08:14:24.000000 impose-0.4.2/tests/test_gui_colocalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-07-06 08:14:24.000000 impose-0.4.2/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-07-06 08:14:24.000000 impose-0.4.2/tests/test_structure_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-06 08:14:24.000000 impose-0.4.2/tests/test_structure_composite_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-06 08:14:24.000000 impose-0.4.2/tests/test_structure_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-06 08:14:24.000000 impose-0.4.2/tests/test_util.py
```

### Comparing `impose-0.4.1/CHANGELOG` & `impose-0.4.2/CHANGELOG`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+0.4.2
+ - fix: workaround for TypeError when moving ROI with mouse
+ - ci: update badge and codecov
 0.4.1
  - fix: exception in Collect/Colocalize tab when using the sliders
    in the visualization panel (#51)
 0.4.0
  - fix: bump bmlab from 0.2.3 to 0.6.1 (file format changes) (#53)
 0.3.1
  - fix: bump bmlab from 0.1.10 to 0.2.3 (file format changes) (#49)
```

### Comparing `impose-0.4.1/LICENSE` & `impose-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/PKG-INFO` & `impose-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impose
-Version: 0.4.1
+Version: 0.4.2
 Summary: Fit and superimpose shapes from different imaging modalities
 Home-page: https://github.com/GuckLab/impose
 Maintainer: Paul Müller
 Maintainer-email: dev@craban.de
 License: GPL v3
 Keywords: image analysis,biology,microscopy
 Platform: ALL
@@ -48,15 +48,15 @@
     python -m impose
 
 
 
 .. |impose| image:: https://raw.github.com/GuckLab/impose/master/docs/logo/impose.png
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/impose.svg
    :target: https://pypi.python.org/pypi/impose
-.. |Build Status| image:: https://img.shields.io/github/workflow/status/GuckLab/impose/Checks
+.. |Build Status| image:: https://img.shields.io/github/actions/workflow/status/GuckLab/impose/check.yml
    :target: https://github.com/GuckLab/impose/actions?query=workflow%3AChecks
 .. |Coverage Status| image:: https://img.shields.io/codecov/c/github/GuckLab/impose/master.svg
    :target: https://codecov.io/gh/GuckLab/impose
 .. |Docs Status| image:: https://readthedocs.org/projects/impose/badge/?version=latest
    :target: https://readthedocs.org/projects/impose/builds/
```

### Comparing `impose-0.4.1/README.rst` & `impose-0.4.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,14 @@
     python -m impose
 
 
 
 .. |impose| image:: https://raw.github.com/GuckLab/impose/master/docs/logo/impose.png
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/impose.svg
    :target: https://pypi.python.org/pypi/impose
-.. |Build Status| image:: https://img.shields.io/github/workflow/status/GuckLab/impose/Checks
+.. |Build Status| image:: https://img.shields.io/github/actions/workflow/status/GuckLab/impose/check.yml
    :target: https://github.com/GuckLab/impose/actions?query=workflow%3AChecks
 .. |Coverage Status| image:: https://img.shields.io/codecov/c/github/GuckLab/impose/master.svg
    :target: https://codecov.io/gh/GuckLab/impose
 .. |Docs Status| image:: https://readthedocs.org/projects/impose/badge/?version=latest
    :target: https://readthedocs.org/projects/impose/builds/
```

### Comparing `impose-0.4.1/docs/conf.py` & `impose-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/docs/extensions/github_changelog.py` & `impose-0.4.2/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/docs/index.rst` & `impose-0.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/docs/sec_getting_started.rst` & `impose-0.4.2/docs/sec_getting_started.rst`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/__main__.py` & `impose-0.4.2/impose/__main__.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/_version.py` & `impose-0.4.2/impose/_version.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/data.py` & `impose-0.4.2/impose/data.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/flblend.py` & `impose-0.4.2/impose/flblend.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/formats/__init__.py` & `impose-0.4.2/impose/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/formats/fmt_bf_generic.py` & `impose-0.4.2/impose/formats/fmt_bf_generic.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/formats/fmt_bm_bmlab.py` & `impose-0.4.2/impose/formats/fmt_bm_bmlab.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/formats/fmt_fl_zeiss.py` & `impose-0.4.2/impose/formats/fmt_fl_zeiss.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/geometry/__init__.py` & `impose-0.4.2/impose/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/geometry/mask.py` & `impose-0.4.2/impose/geometry/mask.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/geometry/shapes/base.py` & `impose-0.4.2/impose/geometry/shapes/base.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/geometry/shapes/sh_circle.py` & `impose-0.4.2/impose/geometry/shapes/sh_circle.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/geometry/shapes/sh_ellipse.py` & `impose-0.4.2/impose/geometry/shapes/sh_ellipse.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/geometry/shapes/sh_polygon.py` & `impose-0.4.2/impose/geometry/shapes/sh_polygon.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/geometry/shapes/sh_rectangle.py` & `impose-0.4.2/impose/geometry/shapes/sh_rectangle.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/collect.py` & `impose-0.4.2/impose/gui/collect.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/collect.ui` & `impose-0.4.2/impose/gui/collect.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/collect_pgrois.py` & `impose-0.4.2/impose/gui/collect_pgrois.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/collect_shape_controls.py` & `impose-0.4.2/impose/gui/collect_shape_controls.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/collect_shape_controls.ui` & `impose-0.4.2/impose/gui/collect_shape_controls.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/colocalize.py` & `impose-0.4.2/impose/gui/colocalize.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/colocalize.ui` & `impose-0.4.2/impose/gui/colocalize.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/colocalize_pgrois.py` & `impose-0.4.2/impose/gui/colocalize_pgrois.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+import logging
+import traceback
+
 import numpy as np
 from PyQt6 import QtCore
 import pyqtgraph as pg
 from pyqtgraph import functions as fn
 
 from ..geometry import pg_roi_to_impose_shape
 from ..geometry.shapes import rotate_around_point
 from ..structure import StructureComposite
 
 
+logger = logging.getLogger(__name__)
+
+
 class StructureCompositeGroupedROIs(QtCore.QObject):
     structure_changed = QtCore.pyqtSignal()
 
     def __init__(self, image_view):
         """A list of ROIs that can be moved and rotated together"""
         # We have to subclass from QObject, otherwise signals and
         # slots won't work.
@@ -48,15 +54,16 @@
         roi.sigRegionChangeStarted.connect(self.on_change_started)
         roi.sigRegionChangeFinished.connect(self.on_change_finished)
         roi.sigRegionChanged.connect(self.on_change_finished)
         roi.setAcceptedMouseButtons(
             QtCore.Qt.MouseButton.LeftButton)  # allow clicking
         roi.sigClicked.connect(self.update_structure_geometry)
         self.rois.append(roi)
-        self._initial_states.append(roi.saveState())
+        rstate = roi.saveState()
+        self._initial_states.append(rstate)
 
         # Add rotation handles where appropriate
         if isinstance(roi, pg.RectROI):
             roi.addRotateHandle([1, 0], [0.5, 0.5])
         elif isinstance(roi, pg.CircleROI):
             # Add rotate handle for circles, because rotating a
             # circle rotates everything around it in colocalize.
@@ -93,42 +100,44 @@
         return tr
 
     @QtCore.pyqtSlot(object)
     def on_change_finished(self, roi):
         try:
             old_state = self._initial_states[self.rois.index(roi)]
         except ValueError:
-            old_state = {"angle": None, "pos": None}
-        new_state = roi.saveState()
-        # compute the transform from old_state to new_state
-        if old_state["angle"] != new_state["angle"]:
-            rotate_center = self._rotation_center
-            rotate_angle = new_state["angle"] - old_state["angle"]
-            translate = None
+            logger.error(f"Could not find roi {roi} in initial states!")
+            logger.error(traceback.format_exc())
         else:
-            rotate_angle = None
-            rotate_center = None
-            if old_state["pos"] != new_state["pos"]:
-                translate = np.array(
-                    new_state["pos"]) - np.array(old_state["pos"])
-            else:
+            new_state = roi.saveState()
+            # compute the transform from old_state to new_state
+            if old_state["angle"] != new_state["angle"]:
+                rotate_center = self._rotation_center
+                rotate_angle = new_state["angle"] - old_state["angle"]
                 translate = None
-        for ii, rr in enumerate(self.rois):
-            if rr is not roi:
-                rr.blockSignals(True)
-                rr.setState(self._initial_states[ii])
-                # transform the geometry
-                if rotate_angle is not None:
-                    tr = fn.invertQTransform(self._scene_transforms[ii])
-                    center = tr.map(rotate_center)
-                    rr.setAngle(angle=rr.state["angle"] + rotate_angle,
-                                centerLocal=center)
-                elif translate is not None:
-                    rr.translate(translate, snap=False)
-                rr.blockSignals(False)
+            else:
+                rotate_angle = None
+                rotate_center = None
+                if old_state["pos"] != new_state["pos"]:
+                    translate = np.array(
+                        new_state["pos"]) - np.array(old_state["pos"])
+                else:
+                    translate = None
+            for ii, rr in enumerate(self.rois):
+                if rr is not roi:
+                    rr.blockSignals(True)
+                    rr.setState(self._initial_states[ii])
+                    # transform the geometry
+                    if rotate_angle is not None:
+                        tr = fn.invertQTransform(self._scene_transforms[ii])
+                        center = tr.map(rotate_center)
+                        rr.setAngle(angle=rr.state["angle"] + rotate_angle,
+                                    centerLocal=center)
+                    elif translate is not None:
+                        rr.translate(translate, snap=False)
+                    rr.blockSignals(False)
         self.update_structure_geometry()
 
     @QtCore.pyqtSlot(object)
     def on_change_started(self, roi):
         self._initial_states.clear()
         self._initial_states += [r.saveState() for r in self.rois]
         # determine scene rotation center
@@ -139,14 +148,15 @@
         self._scene_transforms += [r.sceneTransform() for r in self.rois]
         self.active_roi = roi
         for sl, _, rr in self._structur_layer_rois:
             if roi is rr:
                 self.active_structure_layer = sl
                 break
         else:
+            logger.error(traceback.format_exc())
             raise ValueError("Could not find active structure!")
 
     def set_structure_composite(self, cs, vis):
         """Visualize a specific structure composite"""
         assert isinstance(cs, StructureComposite)
         # remove all ROIs and structure information
         self.clear()
```

### Comparing `impose-0.4.1/impose/gui/dlg_edit_circle.ui` & `impose-0.4.2/impose/gui/dlg_edit_circle.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/dlg_edit_ellipse.ui` & `impose-0.4.2/impose/gui/dlg_edit_ellipse.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/dlg_edit_polygon.ui` & `impose-0.4.2/impose/gui/dlg_edit_polygon.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/dlg_edit_rectangle.ui` & `impose-0.4.2/impose/gui/dlg_edit_rectangle.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/dlg_edit_shape.py` & `impose-0.4.2/impose/gui/dlg_edit_shape.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/main.py` & `impose-0.4.2/impose/gui/main.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/main.ui` & `impose-0.4.2/impose/gui/main.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/visualize.py` & `impose-0.4.2/impose/gui/visualize.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/visualize.ui` & `impose-0.4.2/impose/gui/visualize.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/widgets/simple_image_view.py` & `impose-0.4.2/impose/gui/widgets/simple_image_view.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/widgets/simple_plot_widget.py` & `impose-0.4.2/impose/gui/widgets/simple_plot_widget.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/gui/widgets/wait_cursor.py` & `impose-0.4.2/impose/gui/widgets/wait_cursor.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/session.py` & `impose-0.4.2/impose/session.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/structure/composite.py` & `impose-0.4.2/impose/structure/composite.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/structure/composite_stack.py` & `impose-0.4.2/impose/structure/composite_stack.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/structure/layer.py` & `impose-0.4.2/impose/structure/layer.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose/util.py` & `impose-0.4.2/impose/util.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/impose.egg-info/PKG-INFO` & `impose-0.4.2/impose.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impose
-Version: 0.4.1
+Version: 0.4.2
 Summary: Fit and superimpose shapes from different imaging modalities
 Home-page: https://github.com/GuckLab/impose
 Maintainer: Paul Müller
 Maintainer-email: dev@craban.de
 License: GPL v3
 Keywords: image analysis,biology,microscopy
 Platform: ALL
@@ -48,15 +48,15 @@
     python -m impose
 
 
 
 .. |impose| image:: https://raw.github.com/GuckLab/impose/master/docs/logo/impose.png
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/impose.svg
    :target: https://pypi.python.org/pypi/impose
-.. |Build Status| image:: https://img.shields.io/github/workflow/status/GuckLab/impose/Checks
+.. |Build Status| image:: https://img.shields.io/github/actions/workflow/status/GuckLab/impose/check.yml
    :target: https://github.com/GuckLab/impose/actions?query=workflow%3AChecks
 .. |Coverage Status| image:: https://img.shields.io/codecov/c/github/GuckLab/impose/master.svg
    :target: https://codecov.io/gh/GuckLab/impose
 .. |Docs Status| image:: https://readthedocs.org/projects/impose/badge/?version=latest
    :target: https://readthedocs.org/projects/impose/builds/
```

### Comparing `impose-0.4.1/impose.egg-info/SOURCES.txt` & `impose-0.4.2/impose.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/setup.py` & `impose-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/conftest.py` & `impose-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/data/brillouin-invalid.h5` & `impose-0.4.2/tests/data/brillouin-invalid.h5`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/data/brillouin-wo-signature.impose-session` & `impose-0.4.2/tests/data/brillouin-wo-signature.impose-session`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/data/brillouin.h5` & `impose-0.4.2/tests/data/brillouin.h5`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/data/brillouin.impose-composite` & `impose-0.4.2/tests/data/brillouin.impose-composite`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/data/brillouin.impose-session` & `impose-0.4.2/tests/data/brillouin.impose-session`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/data/brillouin_cutout.impose-session` & `impose-0.4.2/tests/data/brillouin_cutout.impose-session`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/data/fmt_brillouin-h5_bmlab-session_2022.zip` & `impose-0.4.2/tests/data/fmt_brillouin-h5_bmlab-session_2022.zip`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/data/fmt_brillouin-h5_bmlab-session_2022_2-rep.zip` & `impose-0.4.2/tests/data/fmt_brillouin-h5_bmlab-session_2022_2-rep.zip`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/data/fmt_brillouin-h5_bmlab-session_2022_water.zip` & `impose-0.4.2/tests/data/fmt_brillouin-h5_bmlab-session_2022_water.zip`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/data/fmt_brillouin-h5_bmlab-session_2022_water_2-rep.zip` & `impose-0.4.2/tests/data/fmt_brillouin-h5_bmlab-session_2022_water_2-rep.zip`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/data/lsm-fish.zip` & `impose-0.4.2/tests/data/lsm-fish.zip`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/test_data_source.py` & `impose-0.4.2/tests/test_data_source.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/test_flblend.py` & `impose-0.4.2/tests/test_flblend.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/test_fmt_czi.py` & `impose-0.4.2/tests/test_fmt_czi.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/test_fmt_h5_brillouin_bmlab.py` & `impose-0.4.2/tests/test_fmt_h5_brillouin_bmlab.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/test_fmt_h5_brillouin_legacy.py` & `impose-0.4.2/tests/test_fmt_h5_brillouin_legacy.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/test_geometry.py` & `impose-0.4.2/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/test_gui_collect.py` & `impose-0.4.2/tests/test_gui_collect.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/test_gui_colocalize.py` & `impose-0.4.2/tests/test_gui_colocalize.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/test_session.py` & `impose-0.4.2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/test_structure_composite.py` & `impose-0.4.2/tests/test_structure_composite.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/test_structure_composite_stack.py` & `impose-0.4.2/tests/test_structure_composite_stack.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/test_structure_layer.py` & `impose-0.4.2/tests/test_structure_layer.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.1/tests/test_util.py` & `impose-0.4.2/tests/test_util.py`

 * *Files identical despite different names*

