# Comparing `tmp/swiftsimio-6.1.1.tar.gz` & `tmp/swiftsimio-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftsimio-6.1.1.tar", last modified: Mon Mar 13 10:47:15 2023, max compression
+gzip compressed data, was "swiftsimio-7.0.0.tar", last modified: Thu Jul  6 15:44:02 2023, max compression
```

## Comparing `swiftsimio-6.1.1.tar` & `swiftsimio-7.0.0.tar`

### file list

```diff
@@ -1,72 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:47:15.564420 swiftsimio-6.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-03-13 10:47:15.560420 swiftsimio-6.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 10:47:15.564420 swiftsimio-6.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:47:15.556420 swiftsimio-6.1.1/swiftsimio/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/__cite__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/accelerated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:47:15.556420 swiftsimio-6.1.1/swiftsimio/initial_conditions/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/initial_conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/initial_conditions/generate_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/masks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:47:15.556420 swiftsimio-6.1.1/swiftsimio/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:47:15.556420 swiftsimio-6.1.1/swiftsimio/metadata/cosmology/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/metadata/cosmology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/metadata/cosmology/cosmology_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:47:15.556420 swiftsimio-6.1.1/swiftsimio/metadata/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/metadata/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/metadata/metadata/metadata_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:47:15.556420 swiftsimio-6.1.1/swiftsimio/metadata/particle/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/metadata/particle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/metadata/particle/particle_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/metadata/particle/particle_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:47:15.560420 swiftsimio-6.1.1/swiftsimio/metadata/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/metadata/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/metadata/unit/unit_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/metadata/unit/unit_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:47:15.560420 swiftsimio-6.1.1/swiftsimio/metadata/writer/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/metadata/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/metadata/writer/required_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    35391 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/optional_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    51005 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/subset_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:47:15.560420 swiftsimio-6.1.1/swiftsimio/visualisation/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/projection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:47:15.560420 swiftsimio-6.1.1/swiftsimio/visualisation/projection_backends/
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/projection_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/projection_backends/fast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/projection_backends/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/projection_backends/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/projection_backends/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/projection_backends/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/projection_backends/renormalised.py
--rw-r--r--   0 runner    (1001) docker     (123)    15432 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/projection_backends/subsampled.py
--rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/projection_backends/subsampled_extreme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20777 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/smoothing_length_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/sphviewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:47:15.560420 swiftsimio-6.1.1/swiftsimio/visualisation/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/tools/cmaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    20354 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/visualisation/volume_render.py
--rw-r--r--   0 runner    (1001) docker     (123)    22898 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsimio/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 10:47:15.556420 swiftsimio-6.1.1/swiftsimio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-03-13 10:47:15.000000 swiftsimio-6.1.1/swiftsimio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-03-13 10:47:15.000000 swiftsimio-6.1.1/swiftsimio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 10:47:15.000000 swiftsimio-6.1.1/swiftsimio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 10:47:11.000000 swiftsimio-6.1.1/swiftsimio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-13 10:47:15.000000 swiftsimio-6.1.1/swiftsimio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-13 10:47:15.000000 swiftsimio-6.1.1/swiftsimio.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     5743 2023-03-13 10:46:29.000000 swiftsimio-6.1.1/swiftsnap
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-06 15:44:02.098849 swiftsimio-7.0.0/
+-rw-r--r--   0 jborrow    (501) staff       (20)    35147 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/COPYING
+-rw-r--r--   0 jborrow    (501) staff       (20)     7651 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/COPYING.LESSER
+-rw-r--r--   0 jborrow    (501) staff       (20)     4080 2023-07-06 15:44:02.098689 swiftsimio-7.0.0/PKG-INFO
+-rw-r--r--   0 jborrow    (501) staff       (20)     3244 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/README.md
+-rw-r--r--   0 jborrow    (501) staff       (20)     1049 2023-07-06 15:43:53.000000 swiftsimio-7.0.0/pyproject.toml
+-rw-r--r--   0 jborrow    (501) staff       (20)       38 2023-07-06 15:44:02.098894 swiftsimio-7.0.0/setup.cfg
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-06 15:44:02.094030 swiftsimio-7.0.0/swiftsimio/
+-rw-r--r--   0 jborrow    (501) staff       (20)      378 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/swiftsimio/__cite__.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     2864 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/__init__.py
+-rw-r--r--   0 jborrow    (501) staff       (20)       22 2023-07-06 15:43:30.000000 swiftsimio-7.0.0/swiftsimio/__version__.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    15983 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/accelerated.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     4713 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/conversions.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    13993 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/masks.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    35791 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/objects.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     1708 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/optional_packages.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    51005 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/reader.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     3590 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/swiftsimio/statistics.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    10236 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/subset_writer.py
+-rwxr-xr-x   0 jborrow    (501) staff       (20)     5779 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/swiftsnap.py
+-rw-r--r--   0 jborrow    (501) staff       (20)      800 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/swiftsimio/units.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    22898 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/writer.py
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-06 15:44:02.095209 swiftsimio-7.0.0/swiftsimio.egg-info/
+-rw-r--r--   0 jborrow    (501) staff       (20)     4080 2023-07-06 15:44:02.000000 swiftsimio-7.0.0/swiftsimio.egg-info/PKG-INFO
+-rw-r--r--   0 jborrow    (501) staff       (20)     1049 2023-07-06 15:44:02.000000 swiftsimio-7.0.0/swiftsimio.egg-info/SOURCES.txt
+-rw-r--r--   0 jborrow    (501) staff       (20)        1 2023-07-06 15:44:02.000000 swiftsimio-7.0.0/swiftsimio.egg-info/dependency_links.txt
+-rw-r--r--   0 jborrow    (501) staff       (20)       61 2023-07-06 15:44:02.000000 swiftsimio-7.0.0/swiftsimio.egg-info/entry_points.txt
+-rw-r--r--   0 jborrow    (501) staff       (20)       37 2023-07-06 15:44:02.000000 swiftsimio-7.0.0/swiftsimio.egg-info/requires.txt
+-rw-r--r--   0 jborrow    (501) staff       (20)       11 2023-07-06 15:44:02.000000 swiftsimio-7.0.0/swiftsimio.egg-info/top_level.txt
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-06 15:44:02.098271 swiftsimio-7.0.0/tests/
+-rw-r--r--   0 jborrow    (501) staff       (20)     2878 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_accelerated.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     1414 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/tests/test_chunked_read_ranges.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     1028 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/tests/test_conversions.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     1487 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_cosmo_array.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    23634 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_cosmo_array_attrs.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    11412 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_data.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     4502 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_extraparts.py
+-rw-r--r--   0 jborrow    (501) staff       (20)      259 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_helper.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     2640 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_mask.py
+-rw-r--r--   0 jborrow    (501) staff       (20)      897 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/tests/test_metadata.py
+-rw-r--r--   0 jborrow    (501) staff       (20)      436 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/tests/test_physical_conversion.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     2022 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_read_ic.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     3737 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_rotate_visualisations.py
+-rw-r--r--   0 jborrow    (501) staff       (20)      890 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/tests/test_rotation.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     2046 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/tests/test_smoothing_length_generation.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     1158 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/tests/test_vistools.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    14136 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_visualisation.py
```

### Comparing `swiftsimio-6.1.1/COPYING` & `swiftsimio-7.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `swiftsimio-6.1.1/COPYING.LESSER` & `swiftsimio-7.0.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `swiftsimio-6.1.1/PKG-INFO` & `swiftsimio-7.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,110 +1,113 @@
 Metadata-Version: 2.1
 Name: swiftsimio
-Version: 6.1.1
+Version: 7.0.0
 Summary: SWIFTsim (swift.dur.ac.uk) i/o routines for python.
-Home-page: https://github.com/swiftsim/swiftsimio
-Author: Josh Borrow
-Author-email: joshua.borrow@durham.ac.uk
-License: UNKNOWN
-Description: SWIFTsimIO
-        ==========
-        
-        ![Build Status](https://github.com/swiftsim/swiftsimio/actions/workflows/pytest.yml/badge.svg)
-        [![Documentation Status](https://readthedocs.org/projects/swiftsimio/badge/?version=latest)](https://swiftsimio.readthedocs.io/en/latest/?badge=latest)
-        [![JOSS Status](https://joss.theoj.org/papers/e85c85f49b99389d98f9b6d81f090331/status.svg)](https://joss.theoj.org/papers/e85c85f49b99389d98f9b6d81f090331)
-        
-        
-        The SWIFT astrophysical simulation code (http://swift.dur.ac.uk) is used
-        widely. There exists many ways of reading the data from SWIFT, which outputs
-        HDF5 files. These range from reading directly using `h5py` to using a complex
-        system such as `yt`; however these either are unsatisfactory (e.g. a lack of
-        unit information in reading HDF5), or too complex for most use-cases. 
-        `swiftsimio` provides an object-oriented API to read (dynamically) data
-        from SWIFT.
-        
-        Full documentation is available at [ReadTheDocs](http://swiftsimio.readthedocs.org).
-        
-        Getting set up with `swiftsimio` is easy; it (by design) has very few
-        requirements. There are a number of optional packages that you can install
-        to make the experience better and these are recommended.
-        
-        
-        Requirements
-        ------------
-        
-        This requires `python` `v3.8.0` or higher. Unfortunately it is not
-        possible to support `swiftsimio` on versions of python lower than this.
-        It is important that you upgrade if you are still a `python2` user.
-        
-        ### Python packages
-        
-        
-        + `numpy`, required for the core numerical routines.
-        + `h5py`, required to read data from the SWIFT HDF5 output files.
-        + `unyt`, required for symbolic unit calculations (depends on sympy`).
-        
-        ### Optional packages
-        
-        
-        + `numba`, highly recommended should you wish to use the in-built visualisation
-          tools.
-        + `scipy`, required if you wish to generate smoothing lengths for particle types
-          that do not store this variable in the snapshots (e.g. dark matter)
-        + `tqdm`, required for progress bars for some long-running tasks. If not installed
-          no progress bar will be shown.
-        + `py-sphviewer`, if you wish to use our integration with this visualisation
-          code.
-        
-        
-        Installing
-        ----------
-        
-        `swiftsimio` can be installed using the python packaging manager, `pip`,
-        or any other packaging manager that you wish to use:
-        
-        `pip install swiftsimio`
-        
-        
-        Citing
-        ------
-        
-        Please cite `swiftsimio` using the JOSS [paper](https://joss.theoj.org/papers/10.21105/joss.02430):
-        
-        ```bibtex
-        @article{Borrow2020,
-          doi = {10.21105/joss.02430},
-          url = {https://doi.org/10.21105/joss.02430},
-          year = {2020},
-          publisher = {The Open Journal},
-          volume = {5},
-          number = {52},
-          pages = {2430},
-          author = {Josh Borrow and Alexei Borrisov},
-          title = {swiftsimio: A Python library for reading SWIFT data},
-          journal = {Journal of Open Source Software}
-        }
-        ```
-        
-        If you use any of the subsampled projection backends, we ask that you cite our
-        relevant SPHERIC [paper](https://arxiv.org/abs/2106.05281). Note that citing
-        the arXiv version here is recommended as the ADS cannot track conference
-        proceedings well.
-        
-        ```bibtex
-        @article{Borrow2021
-          title={Projecting SPH Particles in Adaptive Environments}, 
-          author={Josh Borrow and Ashley J. Kelly},
-          year={2021},
-          eprint={2106.05281},
-          archivePrefix={arXiv},
-          primaryClass={astro-ph.GA}
-        }
-        ```
-        
-Platform: UNKNOWN
+Author-email: Josh Borrow <joshua.borrow@durham.ac.uk>
+Project-URL: Homepage, https://github.com/SWIFTSIM/swiftsimio
+Project-URL: Bug Tracker, https://github.com/SWIFTSIM/swiftsimio/issues
+Project-URL: Documentation, https://swiftsimio.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.8.0
 Description-Content-Type: text/markdown
+License-File: COPYING
+License-File: COPYING.LESSER
+
+SWIFTsimIO
+==========
+
+![Build Status](https://github.com/swiftsim/swiftsimio/actions/workflows/pytest.yml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/swiftsimio/badge/?version=latest)](https://swiftsimio.readthedocs.io/en/latest/?badge=latest)
+[![JOSS Status](https://joss.theoj.org/papers/e85c85f49b99389d98f9b6d81f090331/status.svg)](https://joss.theoj.org/papers/e85c85f49b99389d98f9b6d81f090331)
+
+
+The SWIFT astrophysical simulation code (http://swift.dur.ac.uk) is used
+widely. There exists many ways of reading the data from SWIFT, which outputs
+HDF5 files. These range from reading directly using `h5py` to using a complex
+system such as `yt`; however these either are unsatisfactory (e.g. a lack of
+unit information in reading HDF5), or too complex for most use-cases. 
+`swiftsimio` provides an object-oriented API to read (dynamically) data
+from SWIFT.
+
+Full documentation is available at [ReadTheDocs](http://swiftsimio.readthedocs.org).
+
+Getting set up with `swiftsimio` is easy; it (by design) has very few
+requirements. There are a number of optional packages that you can install
+to make the experience better and these are recommended.
+
+
+Requirements
+------------
+
+This requires `python` `v3.8.0` or higher. Unfortunately it is not
+possible to support `swiftsimio` on versions of python lower than this.
+It is important that you upgrade if you are still a `python2` user.
+
+### Python packages
+
+
++ `numpy`, required for the core numerical routines.
++ `h5py`, required to read data from the SWIFT HDF5 output files.
++ `unyt`, required for symbolic unit calculations (depends on sympy`).
+
+### Optional packages
+
+
++ `numba`, highly recommended should you wish to use the in-built visualisation
+  tools.
++ `scipy`, required if you wish to generate smoothing lengths for particle types
+  that do not store this variable in the snapshots (e.g. dark matter)
++ `tqdm`, required for progress bars for some long-running tasks. If not installed
+  no progress bar will be shown.
++ `py-sphviewer`, if you wish to use our integration with this visualisation
+  code.
+
+
+Installing
+----------
+
+`swiftsimio` can be installed using the python packaging manager, `pip`,
+or any other packaging manager that you wish to use:
+
+`pip install swiftsimio`
+
+
+Citing
+------
+
+Please cite `swiftsimio` using the JOSS [paper](https://joss.theoj.org/papers/10.21105/joss.02430):
+
+```bibtex
+@article{Borrow2020,
+  doi = {10.21105/joss.02430},
+  url = {https://doi.org/10.21105/joss.02430},
+  year = {2020},
+  publisher = {The Open Journal},
+  volume = {5},
+  number = {52},
+  pages = {2430},
+  author = {Josh Borrow and Alexei Borrisov},
+  title = {swiftsimio: A Python library for reading SWIFT data},
+  journal = {Journal of Open Source Software}
+}
+```
+
+If you use any of the subsampled projection backends, we ask that you cite our
+relevant SPHERIC [paper](https://arxiv.org/abs/2106.05281). Note that citing
+the arXiv version here is recommended as the ADS cannot track conference
+proceedings well.
+
+```bibtex
+@article{Borrow2021
+  title={Projecting SPH Particles in Adaptive Environments}, 
+  author={Josh Borrow and Ashley J. Kelly},
+  year={2021},
+  eprint={2106.05281},
+  archivePrefix={arXiv},
+  primaryClass={astro-ph.GA}
+}
+```
```

### Comparing `swiftsimio-6.1.1/README.md` & `swiftsimio-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `swiftsimio-6.1.1/swiftsimio/__init__.py` & `swiftsimio-7.0.0/swiftsimio/__init__.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-6.1.1/swiftsimio/accelerated.py` & `swiftsimio-7.0.0/swiftsimio/accelerated.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-6.1.1/swiftsimio/conversions.py` & `swiftsimio-7.0.0/swiftsimio/conversions.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-6.1.1/swiftsimio/masks.py` & `swiftsimio-7.0.0/swiftsimio/masks.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-6.1.1/swiftsimio/objects.py` & `swiftsimio-7.0.0/swiftsimio/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -733,19 +733,30 @@
             obj = super().__new__(
                 cls,
                 input_array,
                 units=units,
                 registry=registry,
                 dtype=dtype,
                 bypass_validation=bypass_validation,
+                name=name,
+            )
+        except TypeError:
+            # Older versions of unyt (before input_units was deprecated)
+            obj = super().__new__(
+                cls,
+                input_array,
+                units=units,
+                registry=registry,
+                dtype=dtype,
+                bypass_validation=bypass_validation,
                 input_units=input_units,
                 name=name,
             )
         except TypeError:
-            # Older versions of unyt
+            # Even older versions of unyt (before name was added)
             obj = super().__new__(
                 cls,
                 input_array,
                 units=units,
                 registry=registry,
                 dtype=dtype,
                 bypass_validation=bypass_validation,
```

### Comparing `swiftsimio-6.1.1/swiftsimio/optional_packages.py` & `swiftsimio-7.0.0/swiftsimio/optional_packages.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Imports of optional packages.
 
 This includes:
 
 + tqdm: progress bars
 + scipy.spatial: KDTrees
-+ sphviewer: visualisation
 + numba/cuda: visualisation
 """
 
 # TQDM
 try:
     from tqdm import tqdm
 
@@ -26,24 +25,14 @@
 
     TREE_AVAILABLE = True
 except (ImportError, ModuleNotFoundError):
     KDTree = None
     TREE_AVAILABLE = False
 
 
-# Py-sphviewer
-try:
-    import sphviewer as viewer
-
-    SPHVIEWER_AVAILABLE = True
-except (ImportError, ModuleNotFoundError):
-    viewer = None
-    SPHVIEWER_AVAILABLE = False
-
-
 # Astropy
 try:
     import astropy
 
     ASTROPY_AVAILABLE = True
 except (ImportError, ModuleNotFoundError):
     astropy = None
```

### Comparing `swiftsimio-6.1.1/swiftsimio/reader.py` & `swiftsimio-7.0.0/swiftsimio/reader.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-6.1.1/swiftsimio/statistics.py` & `swiftsimio-7.0.0/swiftsimio/statistics.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-6.1.1/swiftsimio/subset_writer.py` & `swiftsimio-7.0.0/swiftsimio/subset_writer.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-6.1.1/swiftsimio/units.py` & `swiftsimio-7.0.0/swiftsimio/units.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-6.1.1/swiftsimio/writer.py` & `swiftsimio-7.0.0/swiftsimio/writer.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-6.1.1/swiftsimio.egg-info/PKG-INFO` & `swiftsimio-7.0.0/swiftsimio.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,110 +1,113 @@
 Metadata-Version: 2.1
 Name: swiftsimio
-Version: 6.1.1
+Version: 7.0.0
 Summary: SWIFTsim (swift.dur.ac.uk) i/o routines for python.
-Home-page: https://github.com/swiftsim/swiftsimio
-Author: Josh Borrow
-Author-email: joshua.borrow@durham.ac.uk
-License: UNKNOWN
-Description: SWIFTsimIO
-        ==========
-        
-        ![Build Status](https://github.com/swiftsim/swiftsimio/actions/workflows/pytest.yml/badge.svg)
-        [![Documentation Status](https://readthedocs.org/projects/swiftsimio/badge/?version=latest)](https://swiftsimio.readthedocs.io/en/latest/?badge=latest)
-        [![JOSS Status](https://joss.theoj.org/papers/e85c85f49b99389d98f9b6d81f090331/status.svg)](https://joss.theoj.org/papers/e85c85f49b99389d98f9b6d81f090331)
-        
-        
-        The SWIFT astrophysical simulation code (http://swift.dur.ac.uk) is used
-        widely. There exists many ways of reading the data from SWIFT, which outputs
-        HDF5 files. These range from reading directly using `h5py` to using a complex
-        system such as `yt`; however these either are unsatisfactory (e.g. a lack of
-        unit information in reading HDF5), or too complex for most use-cases. 
-        `swiftsimio` provides an object-oriented API to read (dynamically) data
-        from SWIFT.
-        
-        Full documentation is available at [ReadTheDocs](http://swiftsimio.readthedocs.org).
-        
-        Getting set up with `swiftsimio` is easy; it (by design) has very few
-        requirements. There are a number of optional packages that you can install
-        to make the experience better and these are recommended.
-        
-        
-        Requirements
-        ------------
-        
-        This requires `python` `v3.8.0` or higher. Unfortunately it is not
-        possible to support `swiftsimio` on versions of python lower than this.
-        It is important that you upgrade if you are still a `python2` user.
-        
-        ### Python packages
-        
-        
-        + `numpy`, required for the core numerical routines.
-        + `h5py`, required to read data from the SWIFT HDF5 output files.
-        + `unyt`, required for symbolic unit calculations (depends on sympy`).
-        
-        ### Optional packages
-        
-        
-        + `numba`, highly recommended should you wish to use the in-built visualisation
-          tools.
-        + `scipy`, required if you wish to generate smoothing lengths for particle types
-          that do not store this variable in the snapshots (e.g. dark matter)
-        + `tqdm`, required for progress bars for some long-running tasks. If not installed
-          no progress bar will be shown.
-        + `py-sphviewer`, if you wish to use our integration with this visualisation
-          code.
-        
-        
-        Installing
-        ----------
-        
-        `swiftsimio` can be installed using the python packaging manager, `pip`,
-        or any other packaging manager that you wish to use:
-        
-        `pip install swiftsimio`
-        
-        
-        Citing
-        ------
-        
-        Please cite `swiftsimio` using the JOSS [paper](https://joss.theoj.org/papers/10.21105/joss.02430):
-        
-        ```bibtex
-        @article{Borrow2020,
-          doi = {10.21105/joss.02430},
-          url = {https://doi.org/10.21105/joss.02430},
-          year = {2020},
-          publisher = {The Open Journal},
-          volume = {5},
-          number = {52},
-          pages = {2430},
-          author = {Josh Borrow and Alexei Borrisov},
-          title = {swiftsimio: A Python library for reading SWIFT data},
-          journal = {Journal of Open Source Software}
-        }
-        ```
-        
-        If you use any of the subsampled projection backends, we ask that you cite our
-        relevant SPHERIC [paper](https://arxiv.org/abs/2106.05281). Note that citing
-        the arXiv version here is recommended as the ADS cannot track conference
-        proceedings well.
-        
-        ```bibtex
-        @article{Borrow2021
-          title={Projecting SPH Particles in Adaptive Environments}, 
-          author={Josh Borrow and Ashley J. Kelly},
-          year={2021},
-          eprint={2106.05281},
-          archivePrefix={arXiv},
-          primaryClass={astro-ph.GA}
-        }
-        ```
-        
-Platform: UNKNOWN
+Author-email: Josh Borrow <joshua.borrow@durham.ac.uk>
+Project-URL: Homepage, https://github.com/SWIFTSIM/swiftsimio
+Project-URL: Bug Tracker, https://github.com/SWIFTSIM/swiftsimio/issues
+Project-URL: Documentation, https://swiftsimio.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.8.0
 Description-Content-Type: text/markdown
+License-File: COPYING
+License-File: COPYING.LESSER
+
+SWIFTsimIO
+==========
+
+![Build Status](https://github.com/swiftsim/swiftsimio/actions/workflows/pytest.yml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/swiftsimio/badge/?version=latest)](https://swiftsimio.readthedocs.io/en/latest/?badge=latest)
+[![JOSS Status](https://joss.theoj.org/papers/e85c85f49b99389d98f9b6d81f090331/status.svg)](https://joss.theoj.org/papers/e85c85f49b99389d98f9b6d81f090331)
+
+
+The SWIFT astrophysical simulation code (http://swift.dur.ac.uk) is used
+widely. There exists many ways of reading the data from SWIFT, which outputs
+HDF5 files. These range from reading directly using `h5py` to using a complex
+system such as `yt`; however these either are unsatisfactory (e.g. a lack of
+unit information in reading HDF5), or too complex for most use-cases. 
+`swiftsimio` provides an object-oriented API to read (dynamically) data
+from SWIFT.
+
+Full documentation is available at [ReadTheDocs](http://swiftsimio.readthedocs.org).
+
+Getting set up with `swiftsimio` is easy; it (by design) has very few
+requirements. There are a number of optional packages that you can install
+to make the experience better and these are recommended.
+
+
+Requirements
+------------
+
+This requires `python` `v3.8.0` or higher. Unfortunately it is not
+possible to support `swiftsimio` on versions of python lower than this.
+It is important that you upgrade if you are still a `python2` user.
+
+### Python packages
+
+
++ `numpy`, required for the core numerical routines.
++ `h5py`, required to read data from the SWIFT HDF5 output files.
++ `unyt`, required for symbolic unit calculations (depends on sympy`).
+
+### Optional packages
+
+
++ `numba`, highly recommended should you wish to use the in-built visualisation
+  tools.
++ `scipy`, required if you wish to generate smoothing lengths for particle types
+  that do not store this variable in the snapshots (e.g. dark matter)
++ `tqdm`, required for progress bars for some long-running tasks. If not installed
+  no progress bar will be shown.
++ `py-sphviewer`, if you wish to use our integration with this visualisation
+  code.
+
+
+Installing
+----------
+
+`swiftsimio` can be installed using the python packaging manager, `pip`,
+or any other packaging manager that you wish to use:
+
+`pip install swiftsimio`
+
+
+Citing
+------
+
+Please cite `swiftsimio` using the JOSS [paper](https://joss.theoj.org/papers/10.21105/joss.02430):
+
+```bibtex
+@article{Borrow2020,
+  doi = {10.21105/joss.02430},
+  url = {https://doi.org/10.21105/joss.02430},
+  year = {2020},
+  publisher = {The Open Journal},
+  volume = {5},
+  number = {52},
+  pages = {2430},
+  author = {Josh Borrow and Alexei Borrisov},
+  title = {swiftsimio: A Python library for reading SWIFT data},
+  journal = {Journal of Open Source Software}
+}
+```
+
+If you use any of the subsampled projection backends, we ask that you cite our
+relevant SPHERIC [paper](https://arxiv.org/abs/2106.05281). Note that citing
+the arXiv version here is recommended as the ADS cannot track conference
+proceedings well.
+
+```bibtex
+@article{Borrow2021
+  title={Projecting SPH Particles in Adaptive Environments}, 
+  author={Josh Borrow and Ashley J. Kelly},
+  year={2021},
+  eprint={2106.05281},
+  archivePrefix={arXiv},
+  primaryClass={astro-ph.GA}
+}
+```
```

### Comparing `swiftsimio-6.1.1/swiftsnap` & `swiftsimio-7.0.0/swiftsimio/swiftsnap.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,16 @@
     action="store_true",
     help=(
         "Print out just the scale factor of the snapshots and exit. "
         "Useful if you want to use these values in a shell script."
     ),
 )
 
-if __name__ == "__main__":
+
+def swiftsnap():
     import swiftsimio as sw
     import unyt
 
     from swiftsimio.metadata.particle import particle_name_underscores
     from textwrap import wrap
 
     args = parser.parse_args()
@@ -185,7 +186,11 @@
             )
         except:
             pass
 
         for name, scheme in data.subgrid_scheme.items():
             if name != "NamedColumns":
                 print(f"{name.replace('Model', 'model')}: {decode(scheme)}")
+
+
+if __name__ == "__main__":
+    swiftsnap()
```

