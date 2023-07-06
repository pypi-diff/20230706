# Comparing `tmp/cellfinder-core-0.4.1.tar.gz` & `tmp/cellfinder-core-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellfinder-core-0.4.1.tar", last modified: Thu Jun 22 14:26:27 2023, max compression
+gzip compressed data, was "cellfinder-core-0.5.0.tar", last modified: Thu Jul  6 11:10:40 2023, max compression
```

## Comparing `cellfinder-core-0.4.1.tar` & `cellfinder-core-0.5.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.415090 cellfinder-core-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.423091 cellfinder-core-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/.github/workflows/test_numba_off.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.427091 cellfinder-core-0.4.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/benchmarks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/benchmarks/detect_and_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/benchmarks/filter_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/benchmarks/filter_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.415090 cellfinder-core-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.427091 cellfinder-core-0.4.1/src/cellfinder_core/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.431091 cellfinder-core-0.4.1/src/cellfinder_core/classify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/classify/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/classify/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)    15384 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/classify/cube_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/classify/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/classify/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.431091 cellfinder-core-0.4.1/src/cellfinder_core/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/config/cellfinder.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.431091 cellfinder-core-0.4.1/src/cellfinder_core/detect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/detect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.431091 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.435091 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/plane/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/plane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/plane/classical_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/plane/plane_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/plane/tile_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/setup_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.435091 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/ball_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/structure_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/structure_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/volume_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.439091 cellfinder-core-0.4.1/src/cellfinder_core/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/download/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/download/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/download/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/src/cellfinder_core/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/IO.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/array_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/prep.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/source_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/tiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/src/cellfinder_core/train/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/train/train_yml.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.427091 cellfinder-core-0.4.1/src/cellfinder_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-06-22 14:26:25.000000 cellfinder-core-0.4.1/src/cellfinder_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-22 14:26:27.000000 cellfinder-core-0.4.1/src/cellfinder_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:26:25.000000 cellfinder-core-0.4.1/src/cellfinder_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 14:26:25.000000 cellfinder-core-0.4.1/src/cellfinder_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-22 14:26:25.000000 cellfinder-core-0.4.1/src/cellfinder_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 14:26:25.000000 cellfinder-core-0.4.1/src/cellfinder_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/tests/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_integration/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_integration/test_detection_structure_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_integration/test_train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/tests/tests/test_unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/test_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.419091 cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/test_filters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/test_structure_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/test_image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/test_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/test_tools_general.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.259268 cellfinder-core-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.271268 cellfinder-core-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/.github/workflows/test_numba_off.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13398 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12361 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.271268 cellfinder-core-0.5.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/benchmarks/detect_and_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/benchmarks/filter_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/benchmarks/filter_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.263268 cellfinder-core-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.271268 cellfinder-core-0.5.0/src/cellfinder_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.279268 cellfinder-core-0.5.0/src/cellfinder_core/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/classify/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/classify/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/classify/cube_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/classify/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/classify/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.279268 cellfinder-core-0.5.0/src/cellfinder_core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/config/cellfinder.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.279268 cellfinder-core-0.5.0/src/cellfinder_core/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/detect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.279268 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.279268 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/plane/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/plane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/plane/classical_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/plane/plane_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/plane/tile_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/setup_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.283268 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/ball_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/structure_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/structure_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/volume_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.283268 cellfinder-core-0.5.0/src/cellfinder_core/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/download/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/download/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/download/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/src/cellfinder_core/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/array_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/source_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/tiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/src/cellfinder_core/train/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/train/train_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.275268 cellfinder-core-0.5.0/src/cellfinder_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13398 2023-07-06 11:10:38.000000 cellfinder-core-0.5.0/src/cellfinder_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-06 11:10:40.000000 cellfinder-core-0.5.0/src/cellfinder_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:10:38.000000 cellfinder-core-0.5.0/src/cellfinder_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-06 11:10:38.000000 cellfinder-core-0.5.0/src/cellfinder_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-06 11:10:38.000000 cellfinder-core-0.5.0/src/cellfinder_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 11:10:38.000000 cellfinder-core-0.5.0/src/cellfinder_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/tests/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_integration/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_integration/test_detection_structure_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_integration/test_train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/tests/tests/test_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/tests/tests/test_unit/test_detect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_detect/test_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.267268 cellfinder-core-0.5.0/tests/tests/test_unit/test_detect/test_filters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/test_structure_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/test_image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/test_tools_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tox.ini
```

### Comparing `cellfinder-core-0.4.1/.codecov.yml` & `cellfinder-core-0.5.0/.codecov.yml`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/.github/workflows/test_and_deploy.yml` & `cellfinder-core-0.5.0/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/.github/workflows/test_numba_off.yml` & `cellfinder-core-0.5.0/.github/workflows/test_numba_off.yml`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/.gitignore` & `cellfinder-core-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/CHANGELOG.md` & `cellfinder-core-0.5.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/LICENSE` & `cellfinder-core-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/PKG-INFO` & `cellfinder-core-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellfinder-core
-Version: 0.4.1
+Version: 0.5.0
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
 Project-URL: Homepage, https://brainglobe.info/cellfinder
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder-core
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder-core/issues
 Project-URL: Documentation, https://docs.brainglobe.info/cellfinder
 Classifier: Development Status :: 3 - Alpha
@@ -27,15 +27,15 @@
 [![Wheel](https://img.shields.io/pypi/wheel/cellfinder-core.svg)](https://pypi.org/project/cellfinder-core)
 [![Development Status](https://img.shields.io/pypi/status/cellfinder-core.svg)](https://github.com/brainglobe/cellfinder-core)
 [![Tests](https://img.shields.io/github/workflow/status/brainglobe/cellfinder-core/tests)](https://github.com/brainglobe/cellfinder-core/actions)
 [![codecov](https://codecov.io/gh/brainglobe/cellfinder-core/branch/main/graph/badge.svg?token=nx1lhNI7ox)](https://codecov.io/gh/brainglobe/cellfinder-core)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://docs.brainglobe.info/cellfinder/contributing)
+[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://brainglobe.info/developers/index.html)
 [![Twitter](https://img.shields.io/twitter/follow/brain_globe?style=social)](https://twitter.com/brain_globe)
 
 # cellfinder-core
 Standalone cellfinder cell detection algorithm
 
 This package implements the cell detection algorithm from
 [Tyson, Rousseau & Niedworok et al. (2021)](https://doi.org/10.1371/journal.pcbi.1009074)
@@ -69,14 +69,26 @@
 ```bash
 pip install cellfinder-napari
 ```
 
 N.B. To speed up cellfinder, you need CUDA & cuDNN installed. Instructions
 [here](https://brainglobe.info/documentation/general/gpu.html).
 
+#### Conda Install
+Linux and MacOS users can also install `cellfinder-core` from `conda-forge`, by running
+```sh
+conda install -c conda-forge cellfinder-core
+```
+
+Windows users can also use the command above to install `cellfinder-core`, however `tensorflow` (one of `cellfinder-core`'s core dependencies) is not available so will not be included.
+Consequentially, `cellfinder-core` will be usable - you will get `PackageNotFound` errors when attempting to import.
+To rectify this, Windows users _must_ [manually install `tensorflow`](#manual-tensorflow-installations) (and ensure their Python interpreter can see this install) for `cellfinder-core` to work.
+Please refer to the [`tensorflow` install page](https://www.tensorflow.org/install) for further guidance.
+Whether `tensorflow` is installed before or after `conda install`ing `cellfinder-core` shouldn't matter, so long as `tensorflow` is visible to the Python interpreter.
+
 ### Usage
 Before using cellfinder-core, it may be useful to take a look at the
 [paper](https://doi.org/10.1371/journal.pcbi.1009074) which
 outlines the algorithm.
 
 The API is not yet fully documented. For an idea of what the parameters do,
 see the documentation for the cellfinder whole-brain microscopy image analysis
@@ -95,45 +107,45 @@
 background_array = tifffile.imread("/path/to/background_image.tif")
 
 voxel_sizes = [5, 2, 2] # in microns
 detected_cells = cellfinder_run(signal_array,background_array,voxel_sizes)
 ```
 
 The output is a list of
-[imlib Cell objects](https://github.com/adamltyson/imlib/blob/51ec5a8053e738776ceaa8d44e531b3c4b0e29d8/imlib/cells/cells.py#L15).
+[brainglobe-utils Cell objects](https://github.com/brainglobe/brainglobe-utils/blob/044a735049c1323466d277f9df1c3abad8b2bb8d/brainglobe_utils/cells/cells.py#L19)
 Each `Cell` has a centroid coordinate, and a type:
 
 ```python
 print(detected_cells[0])
 # Cell: x: 132, y: 308, z: 10, type: 2
 ```
 
 Cell type 2 is a "real" cell, and Cell type 1 is a "rejected" object (i.e.
 not classified as a cell):
 
 ```python
-from imlib.cells.cells import Cell
+from brainglobe_utils.cells.cells import Cell
 print(Cell.CELL)
 # 2
 
 print(Cell.NO_CELL)
 # 1
 ```
 
 #### Saving the results
 If you want to save the detected cells for use in other BrainGlobe software (e.g. the
-[cellfinder napari plugin](https://docs.brainglobe.info/cellfinder-napari/introduction)),
+[cellfinder napari plugin](https://brainglobe.info/documentation/cellfinder/user-guide/napari-plugin/index.html)),
 you can save in the cellfinder XML standard:
 ```python
-from imlib.IO.cells import save_cells
+from brainglobe_utils.IO.cells import save_cells
 save_cells(detected_cells, "/path/to/cells.xml")
 ```
 You can load these back with:
 ```python
-from imlib.IO.cells import get_cells
+from brainglobe_utils.IO.cells import get_cells
 cells = get_cells("/path/to/cells.xml")
 ```
 
 
 #### Using dask for lazy loading
 `cellfinder-core` supports most array-like objects. Using
 [Dask arrays](https://docs.dask.org/en/latest/array.html) allows for lazy
@@ -229,15 +241,16 @@
         network_depth,
     )
 ```
 #### Training the network
 The training data needed are matched pairs (signal & background) of small
 (usually 50 x 50 x 100um) images centered on the coordinate of candidate cells.
 These can be generated however you like, but I recommend using the
-[Napari plugin](https://docs.brainglobe.info/cellfinder-napari/user-guide/training-data-generation).
+[Napari plugin](https://brainglobe.
+info/documentation/cellfinder/user-guide/napari-plugin/training-data-generation.html).
 
 `cellfinder-core` comes with a 50-layer ResNet trained on ~100,000 data points
 from serial two-photon microscopy images of mouse brains
 (available [here](https://gin.g-node.org/cellfinder/training_data)).
 
 Training the network is likely simpler using the
 [command-line interface](https://brainglobe.info/documentation/cellfinder/user-guide/command-line/training/index.html)
@@ -315,9 +328,9 @@
 ---
 ## Citing cellfinder
 If you find this plugin useful, and use it in your research, please cite the paper outlining the cell detection algorithm:
 > Tyson, A. L., Rousseau, C. V., Niedworok, C. J., Keshavarzi, S., Tsitoura, C., Cossell, L., Strom, M. and Margrie, T. W. (2021) “A deep learning algorithm for 3D cell detection in whole mouse brain image datasets’ PLOS Computational Biology, 17(5), e1009074
 [https://doi.org/10.1371/journal.pcbi.1009074](https://doi.org/10.1371/journal.pcbi.1009074)
 
 **If you use this, or any other tools in the brainglobe suite, please
- [let us know](mailto:code@adamltyson.com?subject=cellfinder-core), and
+ [let us know](mailto:hello@brainglobe.info?subject=cellfinder-core), and
  we'd be happy to promote your paper/talk etc.**
```

### Comparing `cellfinder-core-0.4.1/README.md` & `cellfinder-core-0.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![Wheel](https://img.shields.io/pypi/wheel/cellfinder-core.svg)](https://pypi.org/project/cellfinder-core)
 [![Development Status](https://img.shields.io/pypi/status/cellfinder-core.svg)](https://github.com/brainglobe/cellfinder-core)
 [![Tests](https://img.shields.io/github/workflow/status/brainglobe/cellfinder-core/tests)](https://github.com/brainglobe/cellfinder-core/actions)
 [![codecov](https://codecov.io/gh/brainglobe/cellfinder-core/branch/main/graph/badge.svg?token=nx1lhNI7ox)](https://codecov.io/gh/brainglobe/cellfinder-core)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://docs.brainglobe.info/cellfinder/contributing)
+[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://brainglobe.info/developers/index.html)
 [![Twitter](https://img.shields.io/twitter/follow/brain_globe?style=social)](https://twitter.com/brain_globe)
 
 # cellfinder-core
 Standalone cellfinder cell detection algorithm
 
 This package implements the cell detection algorithm from
 [Tyson, Rousseau & Niedworok et al. (2021)](https://doi.org/10.1371/journal.pcbi.1009074)
@@ -46,14 +46,26 @@
 ```bash
 pip install cellfinder-napari
 ```
 
 N.B. To speed up cellfinder, you need CUDA & cuDNN installed. Instructions
 [here](https://brainglobe.info/documentation/general/gpu.html).
 
+#### Conda Install
+Linux and MacOS users can also install `cellfinder-core` from `conda-forge`, by running
+```sh
+conda install -c conda-forge cellfinder-core
+```
+
+Windows users can also use the command above to install `cellfinder-core`, however `tensorflow` (one of `cellfinder-core`'s core dependencies) is not available so will not be included.
+Consequentially, `cellfinder-core` will be usable - you will get `PackageNotFound` errors when attempting to import.
+To rectify this, Windows users _must_ [manually install `tensorflow`](#manual-tensorflow-installations) (and ensure their Python interpreter can see this install) for `cellfinder-core` to work.
+Please refer to the [`tensorflow` install page](https://www.tensorflow.org/install) for further guidance.
+Whether `tensorflow` is installed before or after `conda install`ing `cellfinder-core` shouldn't matter, so long as `tensorflow` is visible to the Python interpreter.
+
 ### Usage
 Before using cellfinder-core, it may be useful to take a look at the
 [paper](https://doi.org/10.1371/journal.pcbi.1009074) which
 outlines the algorithm.
 
 The API is not yet fully documented. For an idea of what the parameters do,
 see the documentation for the cellfinder whole-brain microscopy image analysis
@@ -72,45 +84,45 @@
 background_array = tifffile.imread("/path/to/background_image.tif")
 
 voxel_sizes = [5, 2, 2] # in microns
 detected_cells = cellfinder_run(signal_array,background_array,voxel_sizes)
 ```
 
 The output is a list of
-[imlib Cell objects](https://github.com/adamltyson/imlib/blob/51ec5a8053e738776ceaa8d44e531b3c4b0e29d8/imlib/cells/cells.py#L15).
+[brainglobe-utils Cell objects](https://github.com/brainglobe/brainglobe-utils/blob/044a735049c1323466d277f9df1c3abad8b2bb8d/brainglobe_utils/cells/cells.py#L19)
 Each `Cell` has a centroid coordinate, and a type:
 
 ```python
 print(detected_cells[0])
 # Cell: x: 132, y: 308, z: 10, type: 2
 ```
 
 Cell type 2 is a "real" cell, and Cell type 1 is a "rejected" object (i.e.
 not classified as a cell):
 
 ```python
-from imlib.cells.cells import Cell
+from brainglobe_utils.cells.cells import Cell
 print(Cell.CELL)
 # 2
 
 print(Cell.NO_CELL)
 # 1
 ```
 
 #### Saving the results
 If you want to save the detected cells for use in other BrainGlobe software (e.g. the
-[cellfinder napari plugin](https://docs.brainglobe.info/cellfinder-napari/introduction)),
+[cellfinder napari plugin](https://brainglobe.info/documentation/cellfinder/user-guide/napari-plugin/index.html)),
 you can save in the cellfinder XML standard:
 ```python
-from imlib.IO.cells import save_cells
+from brainglobe_utils.IO.cells import save_cells
 save_cells(detected_cells, "/path/to/cells.xml")
 ```
 You can load these back with:
 ```python
-from imlib.IO.cells import get_cells
+from brainglobe_utils.IO.cells import get_cells
 cells = get_cells("/path/to/cells.xml")
 ```
 
 
 #### Using dask for lazy loading
 `cellfinder-core` supports most array-like objects. Using
 [Dask arrays](https://docs.dask.org/en/latest/array.html) allows for lazy
@@ -206,15 +218,16 @@
         network_depth,
     )
 ```
 #### Training the network
 The training data needed are matched pairs (signal & background) of small
 (usually 50 x 50 x 100um) images centered on the coordinate of candidate cells.
 These can be generated however you like, but I recommend using the
-[Napari plugin](https://docs.brainglobe.info/cellfinder-napari/user-guide/training-data-generation).
+[Napari plugin](https://brainglobe.
+info/documentation/cellfinder/user-guide/napari-plugin/training-data-generation.html).
 
 `cellfinder-core` comes with a 50-layer ResNet trained on ~100,000 data points
 from serial two-photon microscopy images of mouse brains
 (available [here](https://gin.g-node.org/cellfinder/training_data)).
 
 Training the network is likely simpler using the
 [command-line interface](https://brainglobe.info/documentation/cellfinder/user-guide/command-line/training/index.html)
@@ -292,9 +305,9 @@
 ---
 ## Citing cellfinder
 If you find this plugin useful, and use it in your research, please cite the paper outlining the cell detection algorithm:
 > Tyson, A. L., Rousseau, C. V., Niedworok, C. J., Keshavarzi, S., Tsitoura, C., Cossell, L., Strom, M. and Margrie, T. W. (2021) “A deep learning algorithm for 3D cell detection in whole mouse brain image datasets’ PLOS Computational Biology, 17(5), e1009074
 [https://doi.org/10.1371/journal.pcbi.1009074](https://doi.org/10.1371/journal.pcbi.1009074)
 
 **If you use this, or any other tools in the brainglobe suite, please
- [let us know](mailto:code@adamltyson.com?subject=cellfinder-core), and
+ [let us know](mailto:hello@brainglobe.info?subject=cellfinder-core), and
  we'd be happy to promote your paper/talk etc.**
```

### Comparing `cellfinder-core-0.4.1/benchmarks/README.md` & `cellfinder-core-0.5.0/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/benchmarks/detect_and_classify.py` & `cellfinder-core-0.5.0/benchmarks/detect_and_classify.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/benchmarks/filter_2d.py` & `cellfinder-core-0.5.0/benchmarks/filter_2d.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/benchmarks/filter_3d.py` & `cellfinder-core-0.5.0/benchmarks/filter_3d.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/pyproject.toml` & `cellfinder-core-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Image Recognition",
 ]
 requires-python = ">=3.8"
 dependencies = [
     "dask[array]",
     "fancylog>=0.0.7",
-    "imlib>=0.0.26",
+    "brainglobe-utils",
     "natsort",
     "numba",
     "numpy",
     "scikit-image",
     "scikit-learn",
     # See https://github.com/brainglobe/cellfinder-core/issues/103 for < 2.12.0 pin
     "tensorflow-macos>=2.5.0,<2.12.0; platform_system=='Darwin' and platform_machine=='arm64'",
@@ -103,16 +103,32 @@
 select = ["I", "E", "F"]
 fix = true
 
 [tool.ruff.isort]
 known-first-party = ["cellfinder_core"]
 
 [tool.mypy]
-python_version = "3.8"
+
+[[tool.mypy.overrides]]
+module = [
+    "fancylog.*",
+    "brainglobe_utils.*",
+    "natsort.*",
+    "numba.*",
+    "tensorflow.*",
+    "tifffile.*",
+    "pyinstrument.*",
+    "pytest.*",
+    "scipy.*",
+    "skimage.*",
+    "sklearn.*",
+]
+ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = [
     "cellfinder_core.detect.*",
+    "cellfinder_core.classify.*"
 ]
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_calls = true
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/classify/augment.py` & `cellfinder-core-0.5.0/src/cellfinder_core/classify/augment.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+from typing import List, Tuple
+
 import numpy as np
 from scipy.ndimage import rotate, zoom
 
 from cellfinder_core.tools.tools import (
     all_elements_equal,
     random_bool,
     random_probability,
     random_sign,
 )
 
 all_axes = np.array((0, 1, 2))
 
 
-def augment(augmentation_parameters, image, scale_back=True):
+def augment(
+    augmentation_parameters: "AugmentationParameters",
+    image: np.ndarray,
+    scale_back: bool = True,
+) -> np.ndarray:
     pixel_sizes = image.shape
     min_pixel_size = min(pixel_sizes)
     relative_pixel_sizes = []
     for pixel_size in pixel_sizes:
         relative_pixel_sizes.append(pixel_size / min_pixel_size)
 
     image, normalised_pixel_sizes = rescale_to_isotropic(
@@ -46,15 +52,19 @@
             relative_pixel_sizes,
             normalised_pixel_sizes,
             augmentation_parameters.interpolation_order,
         )
     return image
 
 
-def rescale_to_isotropic(image, relative_pixel_sizes, interpolation_order):
+def rescale_to_isotropic(
+    image: np.ndarray,
+    relative_pixel_sizes: List[float],
+    interpolation_order: int,
+) -> Tuple[np.ndarray, List[float]]:
     if not all_elements_equal(relative_pixel_sizes):
         min_pixel_size = min(relative_pixel_sizes)
         normalised_pixel_sizes = []
         for pixel_size in relative_pixel_sizes:
             normalised_pixel_sizes.append(
                 round(pixel_size / min_pixel_size, 2)
             )
@@ -62,43 +72,52 @@
         image = zoom(image, normalised_pixel_sizes, order=interpolation_order)
     else:
         normalised_pixel_sizes = relative_pixel_sizes
     return image, normalised_pixel_sizes
 
 
 def rescale_to_original_size(
-    image, relative_pixel_sizes, normalised_pixel_sizes, interpolation_order
-):
+    image: np.ndarray,
+    relative_pixel_sizes: List[float],
+    normalised_pixel_sizes: List[float],
+    interpolation_order: int,
+) -> np.ndarray:
     if not all_elements_equal(relative_pixel_sizes):
         inverse_pixel_sizes = []
         for pixel_size in normalised_pixel_sizes:
             inverse_pixel_sizes.append(round(1 / pixel_size, 2))
 
         image = zoom(image, inverse_pixel_sizes, order=interpolation_order)
     return image
 
 
-def flip_image(image, axes_to_flip):
+def flip_image(image: np.ndarray, axes_to_flip: List[int]) -> np.ndarray:
     for axis in axes_to_flip:
         image = np.flip(image, axis)
     return image
 
 
-def translate_image(image, translate_axes, random_translate_multipliers):
+def translate_image(
+    image: np.ndarray,
+    translate_axes: List[int],
+    random_translate_multipliers: List[float],
+) -> np.ndarray:
     pixel_shifts = []
     for idx, axis in enumerate(translate_axes):
         pixel_shifts.append(
             int(round(random_translate_multipliers[idx] * image.shape[axis]))
         )
 
     image = np.roll(image, pixel_shifts, axis=translate_axes)
     return image
 
 
-def rotate_image(image, rotation_angles):
+def rotate_image(
+    image: np.ndarray, rotation_angles: List[float]
+) -> np.ndarray:
     for axis, angle in enumerate(rotation_angles):
         if angle != 0:
             rotate_axes = all_axes[all_axes != axis]
             image = rotate(
                 image, angle, axes=rotate_axes, reshape=False, mode="constant"
             )
     return image
@@ -114,59 +133,63 @@
 #     return image
 
 
 class AugmentationParameters:
     # precomputed, so both channels are treated identically
     def __init__(
         self,
-        flip_axis,
-        translate,
-        rotate_max_axes,
-        interpolation_order,
-        augment_likelihood,
+        flip_axis: Tuple[int, int, int],
+        translate: Tuple[float, float, float],
+        rotate_max_axes: Tuple[float, float, float],
+        interpolation_order: int,
+        augment_likelihood: float,
     ):
         # this is a clumsy way of passing parameters to the augment function
         self.flip_axis = flip_axis
         self.translate = translate
         self.rotate_max_axes = rotate_max_axes
         self.interpolation_order = interpolation_order
 
         self.augment_likelihood = augment_likelihood
 
-        self.axes_to_flip = None
-        self.translate_axes = None
-        self.random_translate_multipliers = None
-        self.rotation_angles = None
+        self.axes_to_flip: List[int] = []
+        self.translate_axes: List[int] = []
+        self.random_translate_multipliers: List[float] = []
+        self.rotation_angles: List[float] = []
 
         if flip_axis:
             self.get_flip_parameters(flip_axis)
         if translate:
             self.get_translation_parameters(translate)
         if rotate_max_axes:
             self.get_rotation_parameters(rotate_max_axes)
 
-    def get_flip_parameters(self, flip_axis):
+    def get_flip_parameters(self, flip_axis: Tuple[int, int, int]) -> None:
         self.axes_to_flip = []
         for axis in all_axes:
             if axis in flip_axis:
                 if random_bool(likelihood=self.augment_likelihood):
                     self.axes_to_flip.append(axis)
 
-    def get_translation_parameters(self, translate):
+    def get_translation_parameters(
+        self, translate: Tuple[float, float, float]
+    ) -> None:
         self.translate_axes = []
         self.random_translate_multipliers = []
         for axis, translate_mag in enumerate(translate):
             if translate_mag > 0:
                 if random_bool(likelihood=self.augment_likelihood):
                     self.translate_axes.append(axis)
                     self.random_translate_multipliers.append(
                         random_sign() * random_probability() * translate_mag
                     )
 
-    def get_rotation_parameters(self, rotate_max_axes):
+    def get_rotation_parameters(
+        self, rotate_max_axes: Tuple[float, float, float]
+    ) -> None:
         self.rotation_angles = []
         for max_rotation in rotate_max_axes:
             if random_bool(likelihood=self.augment_likelihood):
                 angle = int(
                     round(
                         -max_rotation + 2 * random_probability() * max_rotation
                     )
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/classify/classify.py` & `cellfinder-core-0.5.0/src/cellfinder_core/classify/classify.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from typing import Callable, List, Optional
+import os
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import numpy as np
-from imlib.general.system import get_num_processes
+from brainglobe_utils.cells.cells import Cell
+from brainglobe_utils.general.system import get_num_processes
 from tensorflow import keras
 
 from cellfinder_core import logger, types
 from cellfinder_core.classify.cube_generator import CubeGeneratorFromFile
 from cellfinder_core.classify.tools import get_model
-from cellfinder_core.train.train_yml import models
+from cellfinder_core.train.train_yml import depth_type, models
 
 
 def main(
-    points,
+    points: List[Cell],
     signal_array: types.array,
     background_array: types.array,
     n_free_cpus: int,
-    voxel_sizes,
-    network_voxel_sizes,
-    batch_size,
-    cube_height,
-    cube_width,
-    cube_depth,
-    trained_model,
-    model_weights,
-    network_depth,
-    max_workers=3,
+    voxel_sizes: Tuple[int, int, int],
+    network_voxel_sizes: Tuple[int, int, int],
+    batch_size: int,
+    cube_height: int,
+    cube_width: int,
+    cube_depth: int,
+    trained_model: Optional[os.PathLike],
+    model_weights: Optional[os.PathLike],
+    network_depth: depth_type,
+    max_workers: int = 3,
     *,
     callback: Optional[Callable[[int], None]] = None,
 ) -> List:
     """
     Parameters
     ----------
     callback : Callable[int], optional
@@ -89,12 +91,14 @@
         cell.type = predictions[idx] + 1
         points_list.append(cell)
 
     return points_list
 
 
 class BatchEndCallback(keras.callbacks.Callback):
-    def __init__(self, callback):
+    def __init__(self, callback: Callable[[int], None]):
         self._callback = callback
 
-    def on_predict_batch_end(self, batch, logs=None):
+    def on_predict_batch_end(
+        self, batch: int, logs: Optional[Dict[str, Any]] = None
+    ) -> None:
         self._callback(batch)
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/classify/cube_generator.py` & `cellfinder-core-0.5.0/src/cellfinder_core/classify/cube_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from pathlib import Path
 from random import shuffle
-from typing import Optional, Tuple
+from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import tensorflow as tf
-from imlib.cells.cells import group_cells_by_z
-from imlib.general.numerical import is_even
+from brainglobe_utils.cells.cells import Cell, group_cells_by_z
+from brainglobe_utils.general.numerical import is_even
 from scipy.ndimage import zoom
 from skimage.io import imread
 from tensorflow.keras.utils import Sequence
 
 from cellfinder_core import types
 from cellfinder_core.classify.augment import AugmentationParameters, augment
 
@@ -30,35 +31,35 @@
     """
 
     # TODO: shuffle within (and maybe between) batches
     # TODO: limit workers based on RAM
 
     def __init__(
         self,
-        points,
+        points: List[Cell],
         signal_array: types.array,
         background_array: types.array,
-        voxel_sizes,
-        network_voxel_sizes,
-        batch_size: Optional[int] = 16,
-        cube_width: Optional[int] = 50,
-        cube_height: Optional[int] = 50,
-        cube_depth: Optional[int] = 20,
-        channels: Optional[int] = 2,  # No other option currently
-        classes: Optional[int] = 2,
-        extract: Optional[bool] = False,
-        train: Optional[bool] = False,
-        augment: Optional[bool] = False,
-        augment_likelihood: Optional[float] = 0.1,
+        voxel_sizes: Tuple[int, int, int],
+        network_voxel_sizes: Tuple[int, int, int],
+        batch_size: int = 16,
+        cube_width: int = 50,
+        cube_height: int = 50,
+        cube_depth: int = 20,
+        channels: int = 2,  # No other option currently
+        classes: int = 2,
+        extract: bool = False,
+        train: bool = False,
+        augment: bool = False,
+        augment_likelihood: float = 0.1,
         flip_axis: Tuple[int, int, int] = (0, 1, 2),
         rotate_max_axes: Tuple[float, float, float] = (1, 1, 1),  # degrees
         # scale=[0.5, 2],  # min, max
         translate: Tuple[float, float, float] = (0.05, 0.05, 0.05),
-        shuffle: Optional[bool] = False,
-        interpolation_order: Optional[int] = 2,
+        shuffle: bool = False,
+        interpolation_order: int = 2,
     ):
         self.points = points
         self.signal_array = signal_array
         self.background_array = background_array
         self.batch_size = batch_size
         self.axis_2_pixel_um = float(voxel_sizes[2])
         self.axis_1_pixel_um = float(voxel_sizes[1])
@@ -83,41 +84,41 @@
         # self.scale = scale
         self.translate = translate
         self.shuffle = shuffle
         self.interpolation_order = interpolation_order
 
         self.scale_cubes = False
 
-        self.rescaling_factor_axis_2 = 1
-        self.rescaling_factor_axis_1 = 1
-        self.rescaled_cube_width = self.cube_width
-        self.rescaled_cube_height = self.cube_height
+        self.rescaling_factor_axis_2: float = 1
+        self.rescaling_factor_axis_1: float = 1
+        self.rescaled_cube_width: float = self.cube_width
+        self.rescaled_cube_height: float = self.cube_height
 
         self.__check_image_sizes()
         self.__get_image_size()
         self.__check_z_scaling()
         self.__check_in_plane_scaling()
         self.__remove_outlier_points()
         self.__get_batches()
         if shuffle:
             self.on_epoch_end()
 
-    def __check_image_sizes(self):
+    def __check_image_sizes(self) -> None:
         if len(self.signal_array) != len(self.background_array):
             raise ValueError(
                 f"Number of signal images ({len(self.signal_array)}) does not "
                 f"match the number of background images "
                 f"({len(self.background_array)}"
             )
 
-    def __get_image_size(self):
+    def __get_image_size(self) -> None:
         self.image_z_size = len(self.signal_array)
         self.image_height, self.image_width = self.signal_array[0].shape
 
-    def __check_in_plane_scaling(self):
+    def __check_in_plane_scaling(self) -> None:
         if self.axis_2_pixel_um != self.network_axis_2_pixel_um:
             self.rescaling_factor_axis_2 = (
                 self.network_axis_2_pixel_um / self.axis_2_pixel_um
             )
             self.rescaled_cube_width = (
                 self.cube_width * self.rescaling_factor_axis_2
             )
@@ -127,15 +128,15 @@
                 self.network_axis_1_pixel_um / self.axis_1_pixel_um
             )
             self.rescaled_cube_height = (
                 self.cube_height * self.rescaling_factor_axis_1
             )
             self.scale_cubes = True
 
-    def __check_z_scaling(self):
+    def __check_z_scaling(self) -> None:
         if self.axis_0_pixel_um != self.network_axis_0_pixel_um:
             plane_scaling_factor = (
                 self.network_axis_0_pixel_um / self.axis_0_pixel_um
             )
             self.num_planes_needed_for_cube = round(
                 self.cube_depth * plane_scaling_factor
             )
@@ -146,69 +147,67 @@
             raise StackSizeError(
                 f"The number of planes provided ({self.image_z_size}) "
                 "is not sufficient for any cubes to be extracted "
                 f"(need at least {self.num_planes_needed_for_cube}). "
                 "Please check the input data"
             )
 
-    def __remove_outlier_points(self):
+    def __remove_outlier_points(self) -> None:
         """
         Remove points that won't get extracted (i.e too close to the edge)
         """
         self.points = [
             point for point in self.points if self.extractable(point)
         ]
 
-    def extractable(self, point):
+    def extractable(self, point: Cell) -> bool:
         x0, x1, y0, y1, z0, z1 = self.__get_boundaries()
-        if (
-            point.z < z0
-            or point.z > z1
-            or point.x < x0
-            or point.x > x1
-            or point.y < y0
-            or point.y > y1
-        ):
-            return False
-        else:
-            return True
+        return (
+            x0 <= point.x <= x1 and y0 <= point.y <= y1 and z0 <= point.z <= z1
+        )
 
-    def __get_boundaries(self):
+    def __get_boundaries(self) -> Tuple[int, int, int, int, int, int]:
         x0 = int(round((self.cube_width / 2) * self.rescaling_factor_axis_2))
         x1 = int(round(self.image_width - x0))
 
         y0 = int(round((self.cube_height / 2) * self.rescaling_factor_axis_1))
         y1 = int(round(self.image_height - y0))
 
         z0 = int(round(self.num_planes_needed_for_cube / 2))
         z1 = self.image_z_size - z0
         return x0, x1, y0, y1, z0, z1
 
-    def __get_batches(self):
+    def __get_batches(self) -> None:
         self.points_groups = group_cells_by_z(self.points)
         # TODO: add optional shuffling of each group here
         self.batches = []
         for centre_plane in self.points_groups.keys():
             points_per_plane = self.points_groups[centre_plane]
             for i in range(0, len(points_per_plane), self.batch_size):
                 self.batches.append(points_per_plane[i : i + self.batch_size])
 
         self.ordered_points = []
         for batch in self.batches:
             for cell in batch:
                 self.ordered_points.append(cell)
 
-    def __len__(self):
+    def __len__(self) -> int:
         """
         Number of batches
         :return: Number of batches per epoch
         """
         return len(self.batches)
 
-    def __getitem__(self, index):
+    def __getitem__(
+        self, index: int
+    ) -> Union[
+        np.ndarray,
+        Tuple[np.ndarray, List[Dict[str, float]]],
+        Tuple[np.ndarray, Dict],
+    ]:
         """
         Generates a single batch of cubes
         :param index:
         :return:
         """
         if not self.batches:
             raise IndexError("Empty batch. Were any cells detected?")
@@ -227,27 +226,32 @@
             return images, batch_labels
         elif self.extract:
             batch_info = self.__get_batch_dict(cell_batch)
             return images, batch_info
         else:
             return images
 
-    def __get_stacks(self, index):
+    def __get_stacks(self, index: int) -> Tuple[np.ndarray, np.ndarray]:
         centre_plane = self.batches[index][0].z
 
         min_plane, max_plane = get_cube_depth_min_max(
             centre_plane, self.num_planes_needed_for_cube
         )
 
         signal_stack = np.array(self.signal_array[min_plane:max_plane])
         background_stack = np.array(self.background_array[min_plane:max_plane])
 
         return signal_stack, background_stack
 
-    def __generate_cubes(self, cell_batch, signal_stack, background_stack):
+    def __generate_cubes(
+        self,
+        cell_batch: List[Cell],
+        signal_stack: np.ndarray,
+        background_stack: np.ndarray,
+    ) -> np.ndarray:
         number_images = len(cell_batch)
         images = np.empty(
             (
                 (number_images,)
                 + (self.cube_height, self.cube_width, self.cube_depth)
                 + (self.channels,)
             )
@@ -257,31 +261,38 @@
             images = self.__populate_array_with_cubes(
                 images, idx, cell, signal_stack, background_stack
             )
 
         return images
 
     def __populate_array_with_cubes(
-        self, images, idx, cell, signal_stack, background_stack
-    ):
+        self,
+        images: np.ndarray,
+        idx: int,
+        cell: Cell,
+        signal_stack: np.ndarray,
+        background_stack: np.ndarray,
+    ) -> np.ndarray:
         if self.augment:
             self.augmentation_parameters = AugmentationParameters(
                 self.flip_axis,
                 self.translate,
                 self.rotate_max_axes,
                 self.interpolation_order,
                 self.augment_likelihood,
             )
         images[idx, :, :, :, 0] = self.__get_oriented_image(cell, signal_stack)
         images[idx, :, :, :, 1] = self.__get_oriented_image(
             cell, background_stack
         )
         return images
 
-    def __get_oriented_image(self, cell, image_stack):
+    def __get_oriented_image(
+        self, cell: Cell, image_stack: np.ndarray
+    ) -> np.ndarray:
         x0 = int(round(cell.x - (self.rescaled_cube_width / 2)))
         x1 = int(x0 + self.rescaled_cube_width)
         y0 = int(round(cell.y - (self.rescaled_cube_height / 2)))
         y1 = int(y0 + self.rescaled_cube_height)
         image = image_stack[:, y0:y1, x0:x1]
         image = np.moveaxis(image, 0, 2)
 
@@ -290,26 +301,27 @@
             image = augment(
                 self.augmentation_parameters, image, scale_back=False
             )
 
         pixel_scalings = [
             self.cube_height / image.shape[0],
             self.cube_width / image.shape[1],
-            self.cube_depth / image.shape[2],
+            self.cube_depth / image.shape[2],  # type: ignore[misc]
+            # Not sure why mypy thinks .shape[2] is out of bounds above?
         ]
 
         # TODO: ensure this is always the correct size
         image = zoom(image, pixel_scalings, order=self.interpolation_order)
         return image
 
     @staticmethod
-    def __get_batch_dict(cell_batch):
+    def __get_batch_dict(cell_batch: List[Cell]) -> List[Dict[str, float]]:
         return [cell.to_dict() for cell in cell_batch]
 
-    def on_epoch_end(self):
+    def on_epoch_end(self) -> None:
         """
         Shuffle data for each epoch
         :return: Shuffled indexes
         """
         shuffle(self.batches)
 
 
@@ -320,30 +332,30 @@
 
     If augment=True, each augmentation selected has a 50/50 chance of being
     applied to each cube
     """
 
     def __init__(
         self,
-        signal_list,
-        background_list,
-        labels=None,  # only if training or validating
-        batch_size=16,
-        shape=(50, 50, 20),
-        channels=2,
-        classes=2,
-        shuffle=False,
-        augment=False,
-        augment_likelihood=0.1,
-        flip_axis=[0, 1, 2],
-        rotate_max_axes=[45, 45, 45],  # degrees
+        signal_list: List[Union[str, Path]],
+        background_list: List[Union[str, Path]],
+        labels: Optional[List[int]] = None,  # only if training or validating
+        batch_size: int = 16,
+        shape: Tuple[int, int, int] = (50, 50, 20),
+        channels: int = 2,
+        classes: int = 2,
+        shuffle: bool = False,
+        augment: bool = False,
+        augment_likelihood: float = 0.1,
+        flip_axis: Tuple[int, int, int] = (0, 1, 2),
+        rotate_max_axes: Tuple[int, int, int] = (45, 45, 45),  # degrees
         # scale=[0.5, 2],  # min, max
-        translate=[0.2, 0.2, 0.2],
-        train=False,  # also return labels
-        interpolation_order=2,
+        translate: Tuple[float, float, float] = (0.2, 0.2, 0.2),
+        train: bool = False,  # also return labels
+        interpolation_order: int = 2,
     ):
         self.im_shape = shape
         self.batch_size = batch_size
         self.labels = labels
         self.signal_list = signal_list
         self.background_list = background_list
         self.channels = channels
@@ -358,30 +370,36 @@
         self.interpolation_order = interpolation_order
         self.indexes = np.arange(len(self.signal_list))
         if shuffle:
             self.on_epoch_end()
 
     # TODO: implement scale and shear
 
-    def on_epoch_end(self):
+    def on_epoch_end(self) -> None:
         """
         Shuffle data for each epoch
         :return: Shuffled indexes
         """
         self.indexes = np.arange(len(self.signal_list))
         np.random.shuffle(self.indexes)
 
-    def __len__(self):
+    def __len__(self) -> int:
         """
         Number of batches
         :return: Number of batches per epoch
         """
         return int(np.ceil(len(self.signal_list) / self.batch_size))
 
-    def __getitem__(self, index):
+    def __getitem__(
+        self, index: int
+    ) -> Union[
+        np.ndarray,
+        Tuple[np.ndarray, List[Dict[str, float]]],
+        Tuple[np.ndarray, Dict],
+    ]:
         """
         Generates a single batch of cubes
         :param index:
         :return:
         """
         # Generate indexes of the batch
         start_index = index * self.batch_size
@@ -390,62 +408,72 @@
 
         # Get data corresponding to batch
         list_signal_tmp = [self.signal_list[k] for k in indexes]
         list_background_tmp = [self.background_list[k] for k in indexes]
 
         images = self.__generate_cubes(list_signal_tmp, list_background_tmp)
 
-        if self.train:
+        if self.train and self.labels is not None:
             batch_labels = [self.labels[k] for k in indexes]
             batch_labels = tf.keras.utils.to_categorical(
                 batch_labels, num_classes=self.classes
             )
             return images, batch_labels
         else:
             return images
 
-    def __generate_cubes(self, list_signal_tmp, list_background_tmp):
+    def __generate_cubes(
+        self,
+        list_signal_tmp: List[Union[str, Path]],
+        list_background_tmp: List[Union[str, Path]],
+    ) -> np.ndarray:
         number_images = len(list_signal_tmp)
         images = np.empty(
             ((number_images,) + self.im_shape + (self.channels,))
         )
 
         for idx, signal_im in enumerate(list_signal_tmp):
             background_im = list_background_tmp[idx]
             images = self.__populate_array_with_cubes(
                 images, idx, signal_im, background_im
             )
 
         return images.astype(np.float16)
 
     def __populate_array_with_cubes(
-        self, images, idx, signal_im, background_im
-    ):
+        self,
+        images: np.ndarray,
+        idx: int,
+        signal_im: Union[str, Path],
+        background_im: Union[str, Path],
+    ) -> np.ndarray:
         if self.augment:
             self.augmentation_parameters = AugmentationParameters(
                 self.flip_axis,
                 self.translate,
                 self.rotate_max_axes,
                 self.interpolation_order,
                 self.augment_likelihood,
             )
         images[idx, :, :, :, 0] = self.__get_oriented_image(signal_im)
         images[idx, :, :, :, 1] = self.__get_oriented_image(background_im)
 
         return images
 
-    def __get_oriented_image(self, image_path):
+    def __get_oriented_image(self, image_path: Union[str, Path]) -> np.ndarray:
         # if paths are pathlib objs, skimage only reads one plane
         image = np.moveaxis(imread(image_path), 0, 2)
         if self.augment:
             image = augment(self.augmentation_parameters, image)
         return image
 
 
-def get_cube_depth_min_max(centre_plane, num_planes_needed_for_cube):
+def get_cube_depth_min_max(
+    centre_plane: int, num_planes_needed_for_cube: int
+) -> Tuple[int, int]:
     half_cube_depth = num_planes_needed_for_cube // 2
     min_plane = centre_plane - half_cube_depth
 
     if is_even(num_planes_needed_for_cube):
         # WARNING: not centered because even
         max_plane = centre_plane + half_cube_depth
     else:
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/classify/resnet.py` & `cellfinder-core-0.5.0/src/cellfinder_core/classify/resnet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from typing import Dict, List, Literal, Tuple, Union
+from typing import Callable, Dict, List, Literal, Optional, Tuple, Union
 
+from tensorflow import Tensor
 from tensorflow.keras import Model
 from tensorflow.keras.initializers import Initializer
 from tensorflow.keras.layers import (
     Activation,
     Add,
     BatchNormalization,
     Conv3D,
     Dense,
     GlobalAveragePooling3D,
     Input,
     MaxPooling3D,
     ZeroPadding3D,
 )
-from tensorflow.keras.optimizers import Adam
+from tensorflow.keras.optimizers import Adam, Optimizer
 
 #####################################################################
 # Define the types of ResNet
 
 layer_type = Literal[
     "18-layer", "34-layer", "50-layer", "101-layer", "152-layer"
 ]
@@ -39,22 +40,22 @@
 }
 #####################################################################
 
 
 def build_model(
     shape: Tuple[int, int, int, int] = (50, 50, 20, 2),
     network_depth: layer_type = "18-layer",
-    optimizer=None,
+    optimizer: Optional[Optimizer] = None,
     learning_rate: float = 0.0005,  # higher rates don't always converge
-    loss="categorical_crossentropy",
-    metrics=["accuracy"],
+    loss: str = "categorical_crossentropy",
+    metrics: List[str] = ["accuracy"],
     number_classes: int = 2,
     axis: int = 3,
     starting_features: int = 64,
-    classification_activation="softmax",
+    classification_activation: str = "softmax",
 ) -> Model:
     blocks, bottleneck = get_resnet_blocks_and_bottleneck(network_depth)
 
     inputs = Input(shape)
     x = non_residual_block(inputs, starting_features, axis=axis)
 
     features = starting_features
@@ -83,56 +84,45 @@
     if optimizer is None:
         optimizer = Adam(learning_rate=learning_rate)
 
     model.compile(optimizer, loss=loss, metrics=metrics)
     return model
 
 
-def get_resnet_blocks_and_bottleneck(network_depth: layer_type):
+def get_resnet_blocks_and_bottleneck(
+    network_depth: layer_type,
+) -> Tuple[List[int], bool]:
     """
     Parses dicts, and returns how many resnet blocks are in each unit, along
     with whether they are bottlneck blocks or not
 
     :param network_depth:
     :return:
     """
     blocks = resnet_unit_blocks[network_depth]
     bottleneck = network_residual_bottleneck[network_depth]
     return blocks, bottleneck
 
 
 def non_residual_block(
-    inputs,
-    starting_features,
-    conv_kernel=(7, 7, 3),
-    strides=(2, 2, 2),
-    padding=3,
-    max_pool_size=(3, 3, 2),
-    activation="relu",
-    use_bias=False,
-    bn_epsilon=1e-5,
-    pooling_padding="same",
-    axis=3,
-):
+    inputs: Tensor,
+    starting_features: int,
+    conv_kernel: Tuple[int, int, int] = (7, 7, 3),
+    strides: Tuple[int, int, int] = (2, 2, 2),
+    padding: int = 3,
+    max_pool_size: Tuple[int, int, int] = (3, 3, 2),
+    activation: str = "relu",
+    use_bias: bool = False,
+    bn_epsilon: float = 1e-5,
+    pooling_padding: str = "same",
+    axis: int = 3,
+) -> Tensor:
     """
-     Non-residual unit from He et al. (2015). Corresponds to "conv1" and the
+    Non-residual unit from He et al. (2015). Corresponds to "conv1" and the
     max pool.
-
-    :param inputs:
-    :param starting_features:
-    :param conv_kernel:
-    :param strides:
-    :param padding:
-    :param max_pool_size:
-    :param activation:
-    :param use_bias:
-    :param bn_epsilon:
-    :param pooling_padding:
-    :param axis:
-    :return:
     """
 
     x = ZeroPadding3D(padding=padding, name="conv1_padding")(inputs)
     x = Conv3D(
         starting_features,
         conv_kernel,
         strides=strides,
@@ -148,26 +138,26 @@
         name="max_pool",
     )(x)
 
     return x
 
 
 def residual_block(
-    output_features,
-    resnet_unit_id,
-    block_id,
-    conv_kernel=(3, 3, 3),
-    bottleneck_conv_kernel=(1, 1, 1),
-    bottleneck=False,
-    activation="relu",
-    use_bias=False,
-    kernel_initializer="he_normal",
-    bn_epsilon=1e-5,
-    axis=3,
-):
+    output_features: Tensor,
+    resnet_unit_id: int,
+    block_id: int,
+    conv_kernel: Tuple[int, int, int] = (3, 3, 3),
+    bottleneck_conv_kernel: Tuple[int, int, int] = (1, 1, 1),
+    bottleneck: int = False,
+    activation: str = "relu",
+    use_bias: bool = False,
+    kernel_initializer: str = "he_normal",
+    bn_epsilon: float = 1e-5,
+    axis: int = 3,
+) -> Callable[[Tensor], Tensor]:
     """
     Residual unit from He et al. (2015)
 
 
     :param int output_features: How many output features
     :param int resnet_unit_id: Which resnet unit
     (e.g. 0 is conv2_x, 1 is conv3_x)
@@ -184,15 +174,15 @@
     :param axis:
     :return:
     """
 
     stride = get_stride(resnet_unit_id, block_id)
     resnet_unit_label = resnet_unit_id + 2
 
-    def f(x):
+    def f(x: Tensor) -> Tensor:
         if bottleneck:
             y = Conv3D(
                 output_features,
                 bottleneck_conv_kernel,
                 strides=stride,
                 use_bias=use_bias,
                 name=f"resunit{resnet_unit_label}_block{block_id}_conv_a",
@@ -292,24 +282,24 @@
 
         return y
 
     return f
 
 
 def get_shortcut(
-    inputs,
+    inputs: Tensor,
     resnet_unit_label: int,
     block_id: int,
     features: int,
     stride: int,
     use_bias: bool = False,
     kernel_initializer: Union[str, Initializer] = "he_normal",
     bn_epsilon: float = 1e-5,
     axis: int = 3,
-):
+) -> Tensor:
     """
     Create shortcut. For none-bottleneck residual units, this is just the
     identity. Otherwise, the input is reshaped to match the output of the
     bottleneck unit
 
     :param inputs: Input to the residual unit
     :param int resnet_unit_label: Which resnet unit (i.e. 2 is conv2_x)
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/classify/tools.py` & `cellfinder-core-0.5.0/src/cellfinder_core/classify/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import os
-from typing import Optional
+from typing import List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import tensorflow as tf
+from tensorflow.keras import Model
 
 from cellfinder_core import logger
-from cellfinder_core.classify.resnet import build_model
+from cellfinder_core.classify.resnet import build_model, layer_type
 
 
 def get_model(
     existing_model: Optional[os.PathLike] = None,
     model_weights: Optional[os.PathLike] = None,
-    network_depth=None,
-    learning_rate=0.0001,
-    inference=False,
-    continue_training=False,
-):
+    network_depth: Optional[layer_type] = None,
+    learning_rate: float = 0.0001,
+    inference: bool = False,
+    continue_training: bool = False,
+) -> Model:
     """
     Returns the correct model based on the arguments passed
     :param existing_model: An existing, trained model. This is returned if it
     exists
     :param model_weights: This file is used to set the model weights if it
     exists
     :param network_depth: This defines the type of model to be created if
@@ -28,15 +29,15 @@
     :param inference: If True, will ensure that a trained model exists. E.g.
     by using the default one
     :param continue_training: If True, will ensure that a trained model
     exists. E.g. by using the default one
     :return: A tf.keras model
 
     """
-    if existing_model is not None:
+    if existing_model is not None or network_depth is None:
         logger.debug(f"Loading model: {existing_model}")
         return tf.keras.models.load_model(existing_model)
     else:
         logger.debug(f"Creating a new instance of model: {network_depth}")
         model = build_model(
             network_depth=network_depth, learning_rate=learning_rate
         )
@@ -46,15 +47,17 @@
             )
             if model_weights is None:
                 raise IOError("`model_weights` must be provided")
             model.load_weights(model_weights)
         return model
 
 
-def make_lists(tiff_files, train=True):
+def make_lists(
+    tiff_files: Sequence, train: bool = True
+) -> Union[Tuple[List, List], Tuple[List, List, np.ndarray]]:
     signal_list = []
     background_list = []
     if train:
         labels = []
 
     for group in tiff_files:
         for image in group:
@@ -63,11 +66,10 @@
             if train:
                 if image.label == "no_cell":
                     labels.append(0)
                 elif image.label == "cell":
                     labels.append(1)
 
     if train:
-        labels = np.array(labels)
-        return signal_list, background_list, labels
+        return signal_list, background_list, np.array(labels)
     else:
         return signal_list, background_list
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/detect/detect.py` & `cellfinder-core-0.5.0/src/cellfinder_core/detect/detect.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import multiprocessing
 from datetime import datetime
 from queue import Queue
 from threading import Lock
 from typing import Callable, List, Optional, Sequence, Tuple, TypeVar
 
 import numpy as np
-from imlib.cells.cells import Cell
-from imlib.general.system import get_num_processes
+from brainglobe_utils.cells.cells import Cell
+from brainglobe_utils.general.system import get_num_processes
 
 from cellfinder_core import logger, types
 from cellfinder_core.detect.filters.plane import TileProcessor
 from cellfinder_core.detect.filters.setup_filters import setup_tile_filtering
 from cellfinder_core.detect.filters.volume.volume_filter import VolumeFilter
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/plane/classical_filter.py` & `cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/plane/classical_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/plane/plane_filter.py` & `cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/plane/plane_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/plane/tile_walker.py` & `cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/plane/tile_walker.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/setup_filters.py` & `cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/setup_filters.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/ball_filter.py` & `cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/ball_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/structure_detection.py` & `cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/structure_detection.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/structure_splitting.py` & `cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/structure_splitting.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/volume_filter.py` & `cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/volume_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 import os
 from queue import Queue
 from threading import Lock
 from typing import Any, Callable, List, Optional, Tuple
 
 import numpy as np
-from imlib.cells.cells import Cell
+from brainglobe_utils.cells.cells import Cell
 from tifffile import tifffile
 from tqdm import tqdm
 
 from cellfinder_core import logger
 from cellfinder_core.detect.filters.setup_filters import (
     get_ball_filter,
     get_cell_detector,
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/download/cli.py` & `cellfinder-core-0.5.0/src/cellfinder_core/download/cli.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/download/download.py` & `cellfinder-core-0.5.0/src/cellfinder_core/download/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import shutil
 import tarfile
 import urllib.request
 
-from imlib.general.config import get_config_obj
-from imlib.general.system import disk_free_gb
+from brainglobe_utils.general.config import get_config_obj
+from brainglobe_utils.general.system import disk_free_gb
 
 from cellfinder_core.tools.source_files import (
     source_config_cellfinder,
     source_custom_config_cellfinder,
 )
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/download/models.py` & `cellfinder-core-0.5.0/src/cellfinder_core/download/models.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/main.py` & `cellfinder-core-0.5.0/src/cellfinder_core/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 N.B imports are within functions to prevent tensorflow being imported before
 it's warnings are silenced
 """
 import os
-from typing import Callable, Optional, Tuple
+from typing import Callable, List, Optional, Tuple
 
 import numpy as np
-from imlib.general.logging import suppress_specific_logs
+from brainglobe_utils.general.logging import suppress_specific_logs
 
 from cellfinder_core import logger
 from cellfinder_core.download.models import model_type
 from cellfinder_core.train.train_yml import depth_type
 
 tf_suppress_log_messages = [
     "multiprocessing can interact badly with TensorFlow"
@@ -41,15 +41,15 @@
     cube_height: int = 50,
     cube_depth: int = 20,
     network_depth: depth_type = "50",
     *,
     detect_callback: Optional[Callable[[int], None]] = None,
     classify_callback: Optional[Callable[[int], None]] = None,
     detect_finished_callback: Optional[Callable[[list], None]] = None,
-):
+) -> List:
     """
     Parameters
     ----------
     detect_callback : Callable[int], optional
         Called every time a plane has finished being processed during the
         detection stage. Called with the plane number that has finished.
     classify_callback : Callable[int], optional
@@ -109,15 +109,15 @@
             callback=classify_callback,
         )
     else:
         logger.info("No candidates, skipping classification")
     return points
 
 
-def suppress_tf_logging(tf_suppress_log_messages):
+def suppress_tf_logging(tf_suppress_log_messages: List[str]) -> None:
     """
     Prevents many lines of logs such as:
     "2019-10-24 16:54:41.363978: I tensorflow/stream_executor/platform/default
     /dso_loader.cc:44] Successfully opened dynamic library libcuda.so.1"
     """
     os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/tools/IO.py` & `cellfinder-core-0.5.0/src/cellfinder_core/tools/IO.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import glob
 import os
 from typing import Tuple
 
 import numpy as np
+from brainglobe_utils.general.system import get_sorted_file_paths
 from dask import array as da
 from dask import delayed
-from imlib.general.system import get_sorted_file_paths
 from tifffile import TiffFile, imread
 
 
 def get_tiff_meta(
     path: str,
 ) -> Tuple[Tuple[int, int], np.dtype]:
     with TiffFile(path) as tfile:
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/tools/array_operations.py` & `cellfinder-core-0.5.0/src/cellfinder_core/tools/array_operations.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/tools/geometry.py` & `cellfinder-core-0.5.0/src/cellfinder_core/tools/geometry.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/tools/image_processing.py` & `cellfinder-core-0.5.0/src/cellfinder_core/tools/image_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from imlib.general.numerical import is_even
+from brainglobe_utils.general.numerical import is_even
 
 
 def crop_center_2d(img, crop_x=None, crop_y=None):
     """
     Crops the centre of a 2D image, and returns a smaller array. If the desired
     dimension is larger than the original dimension, nothing is changed.
     :param img: 2D input image
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/tools/prep.py` & `cellfinder-core-0.5.0/src/cellfinder_core/tools/prep.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ==================
 Functions to prepare files and directories needed for other functions
 """
 import os
 from pathlib import Path
 from typing import Optional
 
-from imlib.general.config import get_config_obj
-from imlib.general.system import get_num_processes
+from brainglobe_utils.general.config import get_config_obj
+from brainglobe_utils.general.system import get_num_processes
 
 import cellfinder_core.tools.tf as tf_tools
 from cellfinder_core import logger
 from cellfinder_core.download import models as model_download
 from cellfinder_core.download.download import amend_cfg
 from cellfinder_core.tools.source_files import source_custom_config_cellfinder
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/tools/system.py` & `cellfinder-core-0.5.0/src/cellfinder_core/tools/system.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from imlib.general.exceptions import CommandLineInputError
+from brainglobe_utils.general.exceptions import CommandLineInputError
 
 
 def get_subdirectories(directory, names_only=False):
     """
     Return all subdirectories in a given directory
     :param directory:
     :param names_only: If true, dont return paths, but the names
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/tools/tf.py` & `cellfinder-core-0.5.0/src/cellfinder_core/tools/tf.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/tools/tiff.py` & `cellfinder-core-0.5.0/src/cellfinder_core/tools/tiff.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from os import listdir
 from os.path import isfile, join
 
 import natsort
-from imlib.cells.cells import Cell, UntypedCell
+from brainglobe_utils.cells.cells import Cell, UntypedCell
 
 
 class TiffList(object):
     """This class represents list of tiff files. These tiff files are the
      output from the cell extractor plugin
     and are used as training and classification data.
     """
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/tools/tools.py` & `cellfinder-core-0.5.0/src/cellfinder_core/tools/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from random import getrandbits, uniform
+from typing import Optional
 
 import numpy as np
 from natsort import natsorted
 
 
 def get_max_possible_value(obj_in: np.ndarray) -> int:
     """
@@ -123,15 +124,15 @@
     :param list_a: Any list
     :param list_b: Any other list
     :return: True if lists have shared elements
     """
     return any({*list_a} & {*list_b})
 
 
-def random_bool(likelihood=None):
+def random_bool(likelihood: Optional[float] = None) -> bool:
     """
     Return a random boolean (True/False). If "likelihood" is not None, this
     is biased.
     :param likelihood: Only return True if a random number in the range (0,1)
     is greater than this. Default: None.
     :return: Random (or biased) boolean
     """
@@ -140,33 +141,33 @@
     else:
         if uniform(0, 1) > likelihood:
             return True
         else:
             return False
 
 
-def random_sign():
+def random_sign() -> int:
     """
     Returns a random sign (-1 or 1) with a 50/50 chance of each.
     :return: Random sign (-1 or 1)
     """
     if random_bool():
         return 1
     else:
         return -1
 
 
-def random_probability():
+def random_probability() -> float:
     """
     Return a random probability in the range (0, 1)
     :return: Random probability in the range (0, 1)
     """
     return uniform(0, 1)
 
 
-def all_elements_equal(x):
+def all_elements_equal(x) -> bool:
     """
     Return True is all the elements in a series are equal
     :param x: Series of values (e.g. list or numpy array)
     :return: True if all elements are equal, False otherwise.
     """
     return len(set(x)) <= 1
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core/train/train_yml.py` & `cellfinder-core-0.5.0/src/cellfinder_core/train/train_yml.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,42 +12,46 @@
 from argparse import (
     ArgumentDefaultsHelpFormatter,
     ArgumentParser,
     ArgumentTypeError,
 )
 from datetime import datetime
 from pathlib import Path
-from typing import Literal
+from typing import Dict, Literal
 
+from brainglobe_utils.general.numerical import (
+    check_positive_float,
+    check_positive_int,
+)
+from brainglobe_utils.general.system import ensure_directory_exists
+from brainglobe_utils.IO.cells import find_relevant_tiffs
+from brainglobe_utils.IO.yaml import read_yaml_section
 from fancylog import fancylog
-from imlib.general.numerical import check_positive_float, check_positive_int
-from imlib.general.system import ensure_directory_exists
-from imlib.IO.cells import find_relevant_tiffs
-from imlib.IO.yaml import read_yaml_section
 from sklearn.model_selection import train_test_split
 
 import cellfinder_core as program_for_log
 from cellfinder_core import logger
+from cellfinder_core.classify.resnet import layer_type
 from cellfinder_core.tools.prep import DEFAULT_INSTALL_PATH
 
 tf_suppress_log_messages = [
     "sample_weight modes were coerced from",
     "multiprocessing can interact badly with TensorFlow",
 ]
 
-models = {
+depth_type = Literal["18", "34", "50", "101", "152"]
+
+models: Dict[depth_type, layer_type] = {
     "18": "18-layer",
     "34": "34-layer",
     "50": "50-layer",
     "101": "101-layer",
     "152": "152-layer",
 }
 
-depth_type = Literal["18", "34", "50", "101", "152"]
-
 
 def valid_model_depth(depth):
     """
     Ensures a correct existing_model is chosen
     :param value: Input value
     :param models: Dict of allowed models
     :return: Input value, if it corresponds to a valid existing_model
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core.egg-info/PKG-INFO` & `cellfinder-core-0.5.0/src/cellfinder_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellfinder-core
-Version: 0.4.1
+Version: 0.5.0
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
 Project-URL: Homepage, https://brainglobe.info/cellfinder
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder-core
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder-core/issues
 Project-URL: Documentation, https://docs.brainglobe.info/cellfinder
 Classifier: Development Status :: 3 - Alpha
@@ -27,15 +27,15 @@
 [![Wheel](https://img.shields.io/pypi/wheel/cellfinder-core.svg)](https://pypi.org/project/cellfinder-core)
 [![Development Status](https://img.shields.io/pypi/status/cellfinder-core.svg)](https://github.com/brainglobe/cellfinder-core)
 [![Tests](https://img.shields.io/github/workflow/status/brainglobe/cellfinder-core/tests)](https://github.com/brainglobe/cellfinder-core/actions)
 [![codecov](https://codecov.io/gh/brainglobe/cellfinder-core/branch/main/graph/badge.svg?token=nx1lhNI7ox)](https://codecov.io/gh/brainglobe/cellfinder-core)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://docs.brainglobe.info/cellfinder/contributing)
+[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://brainglobe.info/developers/index.html)
 [![Twitter](https://img.shields.io/twitter/follow/brain_globe?style=social)](https://twitter.com/brain_globe)
 
 # cellfinder-core
 Standalone cellfinder cell detection algorithm
 
 This package implements the cell detection algorithm from
 [Tyson, Rousseau & Niedworok et al. (2021)](https://doi.org/10.1371/journal.pcbi.1009074)
@@ -69,14 +69,26 @@
 ```bash
 pip install cellfinder-napari
 ```
 
 N.B. To speed up cellfinder, you need CUDA & cuDNN installed. Instructions
 [here](https://brainglobe.info/documentation/general/gpu.html).
 
+#### Conda Install
+Linux and MacOS users can also install `cellfinder-core` from `conda-forge`, by running
+```sh
+conda install -c conda-forge cellfinder-core
+```
+
+Windows users can also use the command above to install `cellfinder-core`, however `tensorflow` (one of `cellfinder-core`'s core dependencies) is not available so will not be included.
+Consequentially, `cellfinder-core` will be usable - you will get `PackageNotFound` errors when attempting to import.
+To rectify this, Windows users _must_ [manually install `tensorflow`](#manual-tensorflow-installations) (and ensure their Python interpreter can see this install) for `cellfinder-core` to work.
+Please refer to the [`tensorflow` install page](https://www.tensorflow.org/install) for further guidance.
+Whether `tensorflow` is installed before or after `conda install`ing `cellfinder-core` shouldn't matter, so long as `tensorflow` is visible to the Python interpreter.
+
 ### Usage
 Before using cellfinder-core, it may be useful to take a look at the
 [paper](https://doi.org/10.1371/journal.pcbi.1009074) which
 outlines the algorithm.
 
 The API is not yet fully documented. For an idea of what the parameters do,
 see the documentation for the cellfinder whole-brain microscopy image analysis
@@ -95,45 +107,45 @@
 background_array = tifffile.imread("/path/to/background_image.tif")
 
 voxel_sizes = [5, 2, 2] # in microns
 detected_cells = cellfinder_run(signal_array,background_array,voxel_sizes)
 ```
 
 The output is a list of
-[imlib Cell objects](https://github.com/adamltyson/imlib/blob/51ec5a8053e738776ceaa8d44e531b3c4b0e29d8/imlib/cells/cells.py#L15).
+[brainglobe-utils Cell objects](https://github.com/brainglobe/brainglobe-utils/blob/044a735049c1323466d277f9df1c3abad8b2bb8d/brainglobe_utils/cells/cells.py#L19)
 Each `Cell` has a centroid coordinate, and a type:
 
 ```python
 print(detected_cells[0])
 # Cell: x: 132, y: 308, z: 10, type: 2
 ```
 
 Cell type 2 is a "real" cell, and Cell type 1 is a "rejected" object (i.e.
 not classified as a cell):
 
 ```python
-from imlib.cells.cells import Cell
+from brainglobe_utils.cells.cells import Cell
 print(Cell.CELL)
 # 2
 
 print(Cell.NO_CELL)
 # 1
 ```
 
 #### Saving the results
 If you want to save the detected cells for use in other BrainGlobe software (e.g. the
-[cellfinder napari plugin](https://docs.brainglobe.info/cellfinder-napari/introduction)),
+[cellfinder napari plugin](https://brainglobe.info/documentation/cellfinder/user-guide/napari-plugin/index.html)),
 you can save in the cellfinder XML standard:
 ```python
-from imlib.IO.cells import save_cells
+from brainglobe_utils.IO.cells import save_cells
 save_cells(detected_cells, "/path/to/cells.xml")
 ```
 You can load these back with:
 ```python
-from imlib.IO.cells import get_cells
+from brainglobe_utils.IO.cells import get_cells
 cells = get_cells("/path/to/cells.xml")
 ```
 
 
 #### Using dask for lazy loading
 `cellfinder-core` supports most array-like objects. Using
 [Dask arrays](https://docs.dask.org/en/latest/array.html) allows for lazy
@@ -229,15 +241,16 @@
         network_depth,
     )
 ```
 #### Training the network
 The training data needed are matched pairs (signal & background) of small
 (usually 50 x 50 x 100um) images centered on the coordinate of candidate cells.
 These can be generated however you like, but I recommend using the
-[Napari plugin](https://docs.brainglobe.info/cellfinder-napari/user-guide/training-data-generation).
+[Napari plugin](https://brainglobe.
+info/documentation/cellfinder/user-guide/napari-plugin/training-data-generation.html).
 
 `cellfinder-core` comes with a 50-layer ResNet trained on ~100,000 data points
 from serial two-photon microscopy images of mouse brains
 (available [here](https://gin.g-node.org/cellfinder/training_data)).
 
 Training the network is likely simpler using the
 [command-line interface](https://brainglobe.info/documentation/cellfinder/user-guide/command-line/training/index.html)
@@ -315,9 +328,9 @@
 ---
 ## Citing cellfinder
 If you find this plugin useful, and use it in your research, please cite the paper outlining the cell detection algorithm:
 > Tyson, A. L., Rousseau, C. V., Niedworok, C. J., Keshavarzi, S., Tsitoura, C., Cossell, L., Strom, M. and Margrie, T. W. (2021) “A deep learning algorithm for 3D cell detection in whole mouse brain image datasets’ PLOS Computational Biology, 17(5), e1009074
 [https://doi.org/10.1371/journal.pcbi.1009074](https://doi.org/10.1371/journal.pcbi.1009074)
 
 **If you use this, or any other tools in the brainglobe suite, please
- [let us know](mailto:code@adamltyson.com?subject=cellfinder-core), and
+ [let us know](mailto:hello@brainglobe.info?subject=cellfinder-core), and
  we'd be happy to promote your paper/talk etc.**
```

### Comparing `cellfinder-core-0.4.1/src/cellfinder_core.egg-info/SOURCES.txt` & `cellfinder-core-0.5.0/src/cellfinder_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/tests/tests/conftest.py` & `cellfinder-core-0.5.0/tests/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/tests/tests/test_integration/test_detection.py` & `cellfinder-core-0.5.0/tests/tests/test_integration/test_detection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from math import isclose
 
-import imlib.IO.cells as cell_io
+import brainglobe_utils.IO.cells as cell_io
 import numpy as np
 import pytest
-from imlib.general.system import get_num_processes
+from brainglobe_utils.general.system import get_num_processes
 
 from cellfinder_core.main import main
 from cellfinder_core.tools.IO import read_with_dask
 
 data_dir = os.path.join(
     os.getcwd(), "tests", "data", "integration", "detection"
 )
```

### Comparing `cellfinder-core-0.4.1/tests/tests/test_integration/test_detection_structure_splitting.py` & `cellfinder-core-0.5.0/tests/tests/test_integration/test_detection_structure_splitting.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/tests/tests/test_integration/test_train.py` & `cellfinder-core-0.5.0/tests/tests/test_integration/test_train.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/test_detect.py` & `cellfinder-core-0.5.0/tests/tests/test_unit/test_detect/test_detect.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/test_structure_detection.py` & `cellfinder-core-0.5.0/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/test_structure_detection.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/test_image_processing.py` & `cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/test_image_processing.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/test_system.py` & `cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/test_system.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from math import isclose
 from pathlib import Path
 
 import pytest
-from imlib.general.exceptions import CommandLineInputError
-from imlib.general.system import ensure_directory_exists
+from brainglobe_utils.general.exceptions import CommandLineInputError
+from brainglobe_utils.general.system import ensure_directory_exists
 
 import cellfinder_core.tools.system as system
 
 data_dir = Path("tests", "data")
 background_im_dir = os.path.join(data_dir, "background")
```

### Comparing `cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/test_tools_general.py` & `cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/test_tools_general.py`

 * *Files identical despite different names*

