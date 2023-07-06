# Comparing `tmp/pyhalo-0.2.8.tar.gz` & `tmp/pyhalo-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhalo-0.2.8.tar", last modified: Wed Jun 14 15:40:38 2023, max compression
+gzip compressed data, was "pyhalo-0.2.9.tar", last modified: Thu Jul  6 18:53:44 2023, max compression
```

## Comparing `pyhalo-0.2.8.tar` & `pyhalo-0.2.9.tar`

### file list

```diff
@@ -1,132 +1,141 @@
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.738269 pyhalo-0.2.8/
--rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.8/AUTHORS.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.8/CONTRIBUTING.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.8/HISTORY.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.8/LICENSE
--rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.8/MANIFEST.in
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-06-14 15:40:38.737576 pyhalo-0.2.8/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     2034 2023-05-29 07:26:56.000000 pyhalo-0.2.8/README.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.529179 pyhalo-0.2.8/docs/
--rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/Makefile
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/authors.rst
--rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.8/docs/conf.py
--rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/contributing.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/history.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/index.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/installation.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/make.bat
--rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/readme.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.8/docs/usage.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.545109 pyhalo-0.2.8/pyHalo/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.554355 pyhalo-0.2.8/pyHalo/Cosmology/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-08-15 00:50:13.000000 pyhalo-0.2.8/pyHalo/Cosmology/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4768 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Cosmology/cosmology.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9394 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Cosmology/geometry.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.558920 pyhalo-0.2.8/pyHalo/Halos/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.565753 pyhalo-0.2.8/pyHalo/Halos/HaloModels/
--rw-r--r--   0 danielgilman   (501) staff       (20)     2920 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/NFW.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1515 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/PTMass.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4967 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/PsuedoJaffe.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4684 2023-06-06 17:00:07.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/TNFW.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5544 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/TNFWemulator.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9969 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/ULDM.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-11-11 08:37:06.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1575 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/gaussian.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4561 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/generalized_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5615 2023-05-18 16:09:33.000000 pyhalo-0.2.8/pyHalo/Halos/HaloModels/powerlaw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-02-20 20:53:15.000000 pyhalo-0.2.8/pyHalo/Halos/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8462 2023-06-10 17:05:16.000000 pyhalo-0.2.8/pyHalo/Halos/concentration.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5631 2023-06-06 15:53:41.000000 pyhalo-0.2.8/pyHalo/Halos/halo_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    16076 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/lens_cosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9941 2023-06-10 01:21:15.000000 pyhalo-0.2.8/pyHalo/Halos/tidal_truncation.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2142 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Halos/util.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.571260 pyhalo-0.2.8/pyHalo/Rendering/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.576717 pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1873 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/delta_function.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     7019 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/density_peaks.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    10149 2023-06-10 17:27:13.000000 pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/mass_function_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2285 2023-06-09 20:28:33.000000 pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/stucker.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      883 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/util.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.580167 pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      361 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2440 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/correlated.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4339 2023-05-29 07:26:42.000000 pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4696 2023-05-29 07:26:42.000000 pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/uniform.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.8/pyHalo/Rendering/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8837 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/correlated_structure.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5268 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/halo_population.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4605 2023-05-29 07:26:42.000000 pyhalo-0.2.8/pyHalo/Rendering/line_of_sight.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3205 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/rendering_class_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5991 2023-06-06 21:19:38.000000 pyhalo-0.2.8/pyHalo/Rendering/subhalos.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3487 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/Rendering/two_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      157 2023-06-14 15:39:35.000000 pyhalo-0.2.8/pyHalo/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3061 2023-06-09 21:04:32.000000 pyhalo-0.2.8/pyHalo/concentration_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/defaults.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3872 2023-06-13 07:05:17.000000 pyhalo-0.2.8/pyHalo/mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8338 2023-06-10 16:58:29.000000 pyhalo-0.2.8/pyHalo/plotting_routines.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    55312 2023-06-13 19:50:28.000000 pyhalo-0.2.8/pyHalo/preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/pyhalo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-18 15:44:57.000000 pyhalo-0.2.8/pyHalo/realization_extensions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    36340 2023-06-06 19:11:00.000000 pyhalo-0.2.8/pyHalo/single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1448 2023-06-09 21:04:32.000000 pyhalo-0.2.8/pyHalo/truncation_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    14271 2023-05-28 04:22:20.000000 pyhalo-0.2.8/pyHalo/utilities.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.552416 pyhalo-0.2.8/pyHalo.egg-info/
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-06-14 15:40:38.000000 pyhalo-0.2.8/pyHalo.egg-info/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     4043 2023-06-14 15:40:38.000000 pyhalo-0.2.8/pyHalo.egg-info/SOURCES.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-06-14 15:40:38.000000 pyhalo-0.2.8/pyHalo.egg-info/dependency_links.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-06-14 15:40:38.000000 pyhalo-0.2.8/pyHalo.egg-info/entry_points.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.8/pyHalo.egg-info/not-zip-safe
--rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-06-14 15:40:38.000000 pyhalo-0.2.8/pyHalo.egg-info/requires.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)       13 2023-06-14 15:40:38.000000 pyhalo-0.2.8/pyHalo.egg-info/top_level.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-06-14 15:40:10.000000 pyhalo-0.2.8/pyproject.toml
--rw-r--r--   0 danielgilman   (501) staff       (20)       38 2023-06-14 15:40:38.738460 pyhalo-0.2.8/setup.cfg
--rw-r--r--   0 danielgilman   (501) staff       (20)     1639 2023-05-24 16:05:34.000000 pyhalo-0.2.8/setup.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.628376 pyhalo-0.2.8/tests/
--rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.8/tests/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1858 2023-06-10 01:03:10.000000 pyhalo-0.2.8/tests/test_concentration_models.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.638108 pyhalo-0.2.8/tests/test_cosmology/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.8/tests/test_cosmology/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_cosmology/test_cone_geometry.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_cosmology/test_cosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_cosmology/test_cylinder_geometry.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.718651 pyhalo-0.2.8/tests/test_halos/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.8/tests/test_halos/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2832 2023-05-28 04:43:27.000000 pyhalo-0.2.8/tests/test_halos/test_adiabatic_tides.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_halos/test_concentrations.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_halos/test_gaussian.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     6011 2023-05-18 16:13:37.000000 pyhalo-0.2.8/tests/test_halos/test_general_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_halos/test_lenscosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_halos/test_nfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_halos/test_pjaffe.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_halos/test_point_mass.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4304 2023-05-18 16:13:19.000000 pyhalo-0.2.8/tests/test_halos/test_powerlaw_profile.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3319 2023-06-06 21:39:37.000000 pyhalo-0.2.8/tests/test_halos/test_tnfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3517 2023-05-29 07:26:42.000000 pyhalo-0.2.8/tests/test_halos/test_truncation.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_halos/test_uldm.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_halos/test_util.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      917 2023-06-10 17:50:52.000000 pyhalo-0.2.8/tests/test_mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1153 2023-06-10 17:27:13.000000 pyhalo-0.2.8/tests/test_plotting.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3384 2023-06-10 01:27:42.000000 pyhalo-0.2.8/tests/test_preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_pyhalo_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_realization_extensions.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.724126 pyhalo-0.2.8/tests/test_rendering/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.8/tests/test_rendering/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_2halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_los.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.728980 pyhalo-0.2.8/tests/test_rendering/test_mass_functions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_mass_functions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_mass_functions/test_base_functions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_mass_functions/test_delta_function.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    10932 2023-06-09 19:49:01.000000 pyhalo-0.2.8/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3776 2023-06-09 22:32:59.000000 pyhalo-0.2.8/tests/test_rendering/test_mass_functions/test_stucker.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_population.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-06-14 15:40:38.735653 pyhalo-0.2.8/tests/test_rendering/test_spatial_distribution/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_spatial_distribution/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_spatial_distribution/test_correlated.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2484 2023-05-29 07:26:42.000000 pyhalo-0.2.8/tests/test_rendering/test_spatial_distribution/test_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_rendering/test_spatial_distribution/test_uniform.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-29 07:23:17.000000 pyhalo-0.2.8/tests/test_rendering/test_subhalos.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-18 15:44:57.000000 pyhalo-0.2.8/tests/test_single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3429 2023-05-29 07:26:42.000000 pyhalo-0.2.8/tests/test_utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.140563 pyhalo-0.2.9/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.9/AUTHORS.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.9/HISTORY.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.9/LICENSE
+-rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.9/MANIFEST.in
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-07-06 18:53:44.140264 pyhalo-0.2.9/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2034 2023-05-29 07:26:56.000000 pyhalo-0.2.9/README.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.070818 pyhalo-0.2.9/docs/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.9/docs/Makefile
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.9/docs/authors.rst
+-rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.9/docs/conf.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.9/docs/contributing.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.9/docs/history.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.9/docs/index.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.9/docs/installation.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.9/docs/make.bat
+-rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.9/docs/readme.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.9/docs/usage.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.079958 pyhalo-0.2.9/pyHalo/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.084410 pyhalo-0.2.9/pyHalo/Cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-08-15 00:50:13.000000 pyhalo-0.2.9/pyHalo/Cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4768 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Cosmology/cosmology.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9394 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Cosmology/geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.086079 pyhalo-0.2.9/pyHalo/GalacticusInterface/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-06-22 15:04:36.000000 pyhalo-0.2.9/pyHalo/GalacticusInterface/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4653 2023-07-02 18:08:40.000000 pyhalo-0.2.9/pyHalo/GalacticusInterface/param_file.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8263 2023-06-22 15:17:06.000000 pyhalo-0.2.9/pyHalo/GalacticusInterface/read_output.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.089897 pyhalo-0.2.9/pyHalo/Halos/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.097731 pyhalo-0.2.9/pyHalo/Halos/HaloModels/
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2917 2023-07-06 18:52:36.000000 pyhalo-0.2.9/pyHalo/Halos/HaloModels/NFW.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1515 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Halos/HaloModels/PTMass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4967 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Halos/HaloModels/PsuedoJaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4638 2023-07-06 18:52:36.000000 pyhalo-0.2.9/pyHalo/Halos/HaloModels/TNFW.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5544 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Halos/HaloModels/TNFWemulator.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9969 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Halos/HaloModels/ULDM.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-11-11 08:37:06.000000 pyhalo-0.2.9/pyHalo/Halos/HaloModels/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1575 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Halos/HaloModels/gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4561 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Halos/HaloModels/generalized_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5615 2023-05-18 16:09:33.000000 pyhalo-0.2.9/pyHalo/Halos/HaloModels/powerlaw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-02-20 20:53:15.000000 pyhalo-0.2.9/pyHalo/Halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8462 2023-06-10 17:05:16.000000 pyhalo-0.2.9/pyHalo/Halos/concentration.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.099622 pyhalo-0.2.9/pyHalo/Halos/galacticus_truncation/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:52:36.000000 pyhalo-0.2.9/pyHalo/Halos/galacticus_truncation/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4308 2023-07-06 18:52:36.000000 pyhalo-0.2.9/pyHalo/Halos/galacticus_truncation/interp_mass_loss.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)   101480 2023-07-06 18:52:36.000000 pyhalo-0.2.9/pyHalo/Halos/galacticus_truncation/tabulated_mass_loss.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5631 2023-06-06 15:53:41.000000 pyhalo-0.2.9/pyHalo/Halos/halo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16535 2023-07-06 18:52:36.000000 pyhalo-0.2.9/pyHalo/Halos/lens_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    12156 2023-07-06 18:52:36.000000 pyhalo-0.2.9/pyHalo/Halos/tidal_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2144 2023-07-06 18:52:36.000000 pyhalo-0.2.9/pyHalo/Halos/util.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.104808 pyhalo-0.2.9/pyHalo/Rendering/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.108854 pyhalo-0.2.9/pyHalo/Rendering/MassFunctions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.9/pyHalo/Rendering/MassFunctions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1873 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Rendering/MassFunctions/delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     7019 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Rendering/MassFunctions/density_peaks.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    10149 2023-06-10 17:27:13.000000 pyhalo-0.2.9/pyHalo/Rendering/MassFunctions/mass_function_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2285 2023-06-09 20:28:33.000000 pyhalo-0.2.9/pyHalo/Rendering/MassFunctions/stucker.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      883 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Rendering/MassFunctions/util.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.111451 pyhalo-0.2.9/pyHalo/Rendering/SpatialDistributions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.9/pyHalo/Rendering/SpatialDistributions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      361 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Rendering/SpatialDistributions/base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2440 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Rendering/SpatialDistributions/correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4676 2023-07-06 18:52:36.000000 pyhalo-0.2.9/pyHalo/Rendering/SpatialDistributions/nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4696 2023-05-29 07:26:42.000000 pyhalo-0.2.9/pyHalo/Rendering/SpatialDistributions/uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.9/pyHalo/Rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8837 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Rendering/correlated_structure.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5268 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Rendering/halo_population.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4605 2023-05-29 07:26:42.000000 pyhalo-0.2.9/pyHalo/Rendering/line_of_sight.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3205 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Rendering/rendering_class_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5991 2023-06-06 21:19:38.000000 pyhalo-0.2.9/pyHalo/Rendering/subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3487 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/Rendering/two_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      157 2023-06-14 15:39:35.000000 pyhalo-0.2.9/pyHalo/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3061 2023-06-09 21:04:32.000000 pyhalo-0.2.9/pyHalo/concentration_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/defaults.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3872 2023-06-13 07:05:17.000000 pyhalo-0.2.9/pyHalo/mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    13592 2023-07-06 18:52:36.000000 pyhalo-0.2.9/pyHalo/plotting_routines.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    55723 2023-07-06 18:52:36.000000 pyhalo-0.2.9/pyHalo/preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/pyhalo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-18 15:44:57.000000 pyhalo-0.2.9/pyHalo/realization_extensions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    36340 2023-07-06 15:22:58.000000 pyhalo-0.2.9/pyHalo/single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1422 2023-07-06 18:52:36.000000 pyhalo-0.2.9/pyHalo/truncation_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    13033 2023-07-06 18:52:36.000000 pyhalo-0.2.9/pyHalo/utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.083114 pyhalo-0.2.9/pyHalo.egg-info/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-07-06 18:53:44.000000 pyhalo-0.2.9/pyHalo.egg-info/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4372 2023-07-06 18:53:44.000000 pyhalo-0.2.9/pyHalo.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-07-06 18:53:44.000000 pyhalo-0.2.9/pyHalo.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-07-06 18:53:44.000000 pyhalo-0.2.9/pyHalo.egg-info/entry_points.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.9/pyHalo.egg-info/not-zip-safe
+-rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-07-06 18:53:44.000000 pyhalo-0.2.9/pyHalo.egg-info/requires.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       13 2023-07-06 18:53:44.000000 pyhalo-0.2.9/pyHalo.egg-info/top_level.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-07-06 18:52:58.000000 pyhalo-0.2.9/pyproject.toml
+-rw-r--r--   0 danielgilman   (501) staff       (20)       38 2023-07-06 18:53:44.140658 pyhalo-0.2.9/setup.cfg
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1639 2023-07-06 18:53:29.000000 pyhalo-0.2.9/setup.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.119876 pyhalo-0.2.9/tests/
+-rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.9/tests/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1858 2023-06-10 01:03:10.000000 pyhalo-0.2.9/tests/test_concentration_models.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.122871 pyhalo-0.2.9/tests/test_cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.9/tests/test_cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_cosmology/test_cone_geometry.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_cosmology/test_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_cosmology/test_cylinder_geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.132505 pyhalo-0.2.9/tests/test_halos/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.9/tests/test_halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2832 2023-05-28 04:43:27.000000 pyhalo-0.2.9/tests/test_halos/test_adiabatic_tides.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_halos/test_concentrations.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2456 2023-07-06 18:52:36.000000 pyhalo-0.2.9/tests/test_halos/test_galacticus_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_halos/test_gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     6011 2023-05-18 16:13:37.000000 pyhalo-0.2.9/tests/test_halos/test_general_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3159 2023-07-06 18:52:36.000000 pyhalo-0.2.9/tests/test_halos/test_lenscosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_halos/test_nfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_halos/test_pjaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_halos/test_point_mass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4304 2023-05-18 16:13:19.000000 pyhalo-0.2.9/tests/test_halos/test_powerlaw_profile.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3319 2023-06-06 21:39:37.000000 pyhalo-0.2.9/tests/test_halos/test_tnfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3517 2023-05-29 07:26:42.000000 pyhalo-0.2.9/tests/test_halos/test_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_halos/test_uldm.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_halos/test_util.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      917 2023-06-10 17:50:52.000000 pyhalo-0.2.9/tests/test_mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1468 2023-07-06 18:52:36.000000 pyhalo-0.2.9/tests/test_plotting.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3674 2023-07-06 18:52:36.000000 pyhalo-0.2.9/tests/test_preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_pyhalo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_realization_extensions.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.134802 pyhalo-0.2.9/tests/test_rendering/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.9/tests/test_rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_rendering/test_2halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_rendering/test_los.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.137410 pyhalo-0.2.9/tests/test_rendering/test_mass_functions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_rendering/test_mass_functions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_rendering/test_mass_functions/test_base_functions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_rendering/test_mass_functions/test_delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    10932 2023-06-09 19:49:01.000000 pyhalo-0.2.9/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3776 2023-06-09 22:32:59.000000 pyhalo-0.2.9/tests/test_rendering/test_mass_functions/test_stucker.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_rendering/test_population.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-07-06 18:53:44.139749 pyhalo-0.2.9/tests/test_rendering/test_spatial_distribution/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_rendering/test_spatial_distribution/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_rendering/test_spatial_distribution/test_correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2484 2023-05-29 07:26:42.000000 pyhalo-0.2.9/tests/test_rendering/test_spatial_distribution/test_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_rendering/test_spatial_distribution/test_uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-29 07:23:17.000000 pyhalo-0.2.9/tests/test_rendering/test_subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-18 15:44:57.000000 pyhalo-0.2.9/tests/test_single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4038 2023-07-06 18:52:36.000000 pyhalo-0.2.9/tests/test_utilities.py
```

### Comparing `pyhalo-0.2.8/CONTRIBUTING.rst` & `pyhalo-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/LICENSE` & `pyhalo-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/PKG-INFO` & `pyhalo-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.2.8/README.rst` & `pyhalo-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/docs/Makefile` & `pyhalo-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/docs/conf.py` & `pyhalo-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/docs/installation.rst` & `pyhalo-0.2.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/docs/make.bat` & `pyhalo-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Cosmology/cosmology.py` & `pyhalo-0.2.9/pyHalo/Cosmology/cosmology.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Cosmology/geometry.py` & `pyhalo-0.2.9/pyHalo/Cosmology/geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Halos/HaloModels/NFW.py` & `pyhalo-0.2.9/pyHalo/Halos/HaloModels/NFW.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,22 +42,19 @@
     def lenstronomy_params(self):
         """
         See documentation in base class (Halos/halo_base.py)
         """
 
         (concentration) = self.profile_args
         Rs_angle, theta_Rs = self._lens_cosmo.nfw_physical2angle(self.mass, concentration, self.z)
-
         x, y = np.round(self.x, 4), np.round(self.y, 4)
         Rs_angle = np.round(Rs_angle, 10)
         theta_Rs = np.round(theta_Rs, 10)
-
         kwargs = [{'alpha_Rs': self._rescale_norm * theta_Rs, 'Rs': Rs_angle,
                   'center_x': x, 'center_y': y}]
-
         return kwargs, None
 
     @property
     def c(self):
         """
         Computes the halo concentration (once)
         """
```

### Comparing `pyhalo-0.2.8/pyHalo/Halos/HaloModels/PTMass.py` & `pyhalo-0.2.9/pyHalo/Halos/HaloModels/PTMass.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Halos/HaloModels/PsuedoJaffe.py` & `pyhalo-0.2.9/pyHalo/Halos/HaloModels/PsuedoJaffe.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Halos/HaloModels/TNFW.py` & `pyhalo-0.2.9/pyHalo/Halos/HaloModels/TNFW.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pyHalo.Halos.halo_base import Halo
 from lenstronomy.LensModel.Profiles.tnfw import TNFW as TNFWLenstronomy
 import numpy as np
+from pyHalo.Halos.util import tnfw_mass_fraction
 
 class TNFWFieldHalo(Halo):
 
     """
     The base class for a truncated NFW halo
     """
     def __init__(self, mass, x, y, r3d, z,
@@ -90,31 +91,14 @@
         if not hasattr(self, '_profile_args'):
 
             truncation_radius_kpc = self._truncation_class.truncation_radius_halo(self)
             self._profile_args = (self.c, truncation_radius_kpc)
 
         return self._profile_args
 
-    @property
-    def bound_mass(self):
-        """
-        Computes the mass inside the virial radius (with truncation effects included)
-        :return: the mass inside r = c * r_s
-        """
-        prof = TNFWLenstronomy()
-        kwargs_profile = self.lenstronomy_params[0][0]
-        alpha_rs = kwargs_profile['alpha_Rs']
-        rs = kwargs_profile['Rs']
-        r_trunc = kwargs_profile['r_trunc']
-        r = self.c * rs
-        rho0 = prof.alpha2rho0(alpha_rs, rs)
-        mass_3d = prof.mass_3d(r, rs, rho0, r_trunc)
-        mass_3d_infall = prof.mass_3d(r, rs, rho0, 1000*rs)
-        return (mass_3d / mass_3d_infall) * self.mass
-
 
 class TNFWSubhalo(TNFWFieldHalo):
     """
     Defines a truncated NFW halo that is a subhalo of the host dark matter halo
     """
 
     @property
@@ -138,7 +122,21 @@
         """
         if not hasattr(self, '_params_physical'):
             [concentration, rt] = self.profile_args
             rhos, rs, r200 = self._lens_cosmo.NFW_params_physical(self.mass, concentration, self.z_eval)
             self._params_physical = {'rhos': rhos, 'rs': rs, 'r200': r200, 'r_trunc_kpc': rt}
 
         return self._params_physical
+
+    @property
+    def bound_mass(self):
+        """
+        Computes the mass inside the virial radius (with truncation effects included)
+        :return: the mass inside r = c * r_s
+        """
+        if hasattr(self, '_kwargs_lenstronomy'):
+            tau = self._kwargs_lenstronomy[0]['r_trunc'] / self._kwargs_lenstronomy[0]['Rs']
+        else:
+            params_physical = self.params_physical
+            tau = params_physical['r_trunc_kpc'] / params_physical['rs']
+        f = tnfw_mass_fraction(tau, self.c)
+        return f * self.mass
```

### Comparing `pyhalo-0.2.8/pyHalo/Halos/HaloModels/TNFWemulator.py` & `pyhalo-0.2.9/pyHalo/Halos/HaloModels/TNFWemulator.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Halos/HaloModels/ULDM.py` & `pyhalo-0.2.9/pyHalo/Halos/HaloModels/ULDM.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Halos/HaloModels/gaussian.py` & `pyhalo-0.2.9/pyHalo/Halos/HaloModels/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Halos/HaloModels/generalized_nfw.py` & `pyhalo-0.2.9/pyHalo/Halos/HaloModels/generalized_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Halos/HaloModels/powerlaw.py` & `pyhalo-0.2.9/pyHalo/Halos/HaloModels/powerlaw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Halos/concentration.py` & `pyhalo-0.2.9/pyHalo/Halos/concentration.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Halos/halo_base.py` & `pyhalo-0.2.9/pyHalo/Halos/halo_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Halos/lens_cosmo.py` & `pyhalo-0.2.9/pyHalo/Halos/lens_cosmo.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,26 @@
 from scipy.optimize import minimize
 from scipy.special import erfc
 from lenstronomy.Cosmo.nfw_param import NFWParam
 import astropy.units as un
 from colossus.lss.bias import twoHaloTerm
 from scipy.integrate import quad
 
+
 class LensCosmo(object):
 
     def __init__(self, z_lens=None, z_source=None, cosmology=None):
+        """
 
+        This class performs calcuations relevant for certain halo mass profiles and lensing-related quantities for a
+        given lens/source redshift and cosmology
+        :param z_lens: deflector redshift
+        :param z_source: source redshift
+        :param cosmology: and instance of the Cosmology class (see pyhalo.Cosmology.cosmology.py)
+        """
         if cosmology is None:
             from pyHalo.Cosmology.cosmology import Cosmology
             cosmology = Cosmology()
 
         self.cosmo = cosmology
         self._arcsec = 2 * numpy.pi / 360 / 3600
         self.h = self.cosmo.h
@@ -70,21 +78,22 @@
 
         h = self.cosmo.h
         M_h = M * h
         r_h = r * h
         rho_2h = twoHaloTerm(r_h, M_h, z, mdef=mdef) / self.cosmo._colossus_cosmo.rho_m(z)
         return rho_2h
 
-    def nfw_physical2angle(self, m, c, z):
+    def nfw_physical2angle(self, m, c, z, no_interp=False):
         """
         converts the physical mass and concentration parameter of an NFW profile into the lensing quantities
         updates lenstronomy implementation with arbitrary redshift
 
         :param m: mass enclosed 200 rho_crit in units of M_sun (physical units, meaning no little h)
         :param c: NFW concentration parameter (r200/r_s)
+        :param no_interp: bool; compute NFW params with interpolation
         :return: Rs_angle (angle at scale radius) (in units of arcsec), alpha_Rs (observed bending angle at the scale radius
         """
         dd = self.cosmo.D_A_z(z)
         rho0, Rs, r200 = self.nfwParam_physical(m, c, z)
         Rs_angle = Rs / dd / self._arcsec  # Rs in arcsec
         alpha_Rs = rho0 * (4 * Rs ** 2 * (1 + numpy.log(1. / 2.)))
         sigma_crit = self.get_sigma_crit_lensing(z, self.z_source)
```

### Comparing `pyhalo-0.2.8/pyHalo/Halos/tidal_truncation.py` & `pyhalo-0.2.9/pyHalo/Halos/tidal_truncation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import numpy as np
-import pickle
 from pyHalo.Halos.concentration import ConcentrationDiemerJoyce
-from scipy.interpolate import RegularGridInterpolator
 from pyHalo.Halos.util import tau_mf_interpolation
 from colossus.lss import peaks
 from colossus.halo import splashback
-
+from pyHalo.Halos.galacticus_truncation.interp_mass_loss import InterpGalacticus
 
 class TruncationSplashBack(object):
 
     def __init__(self, lens_cosmo):
         """
         This computes the splashback radius of a halo as the truncation radius (appropriate for field halos)
         See Diemer (2020)
@@ -118,15 +116,15 @@
     """
     An example of the type of class we want to create and implement in pyHalo
     """
 
     def __init__(self, lens_cosmo, log_m_host, z_host, mass_loss_interp):
         """
 
-        :param lens_cosmo: an instacee of the LensCosmo class
+        :param lens_cosmo: an instance of the LensCosmo class
         :param log_m_host: the host halo mass
         :param z_host: the redshift of the host halo
         :param mass_loss_interp: an instance of RegularGridInterpolator
         The interpolator should take as input a point
         (log10(concentration), log10(r_pericenter), c_host) and return the
         asymptotic final bound mass divided by the infall mass
         """
@@ -190,16 +188,16 @@
         return mass_loss
 
     def _make_params_in_bounds_tau_evaluate(self, point):
         """
         This routine makes sure the arguments for the initerpolation are inside the domain of the function.
         """
         (log10c, log10mass_loss_fraction) = point
-        log10c = max(self._min_c, log10c)
-        log10c = min(self._max_c, log10c)
+        log10c = max(np.log10(self._min_c), log10c)
+        log10c = min(np.log10(self._max_c), log10c)
         log10mass_loss_fraction = max(-1.5, log10mass_loss_fraction)
         log10mass_loss_fraction = min(-0.01, log10mass_loss_fraction)
         return (log10c, log10mass_loss_fraction)
 
 class TruncateMeanDensity(object):
 
     def __init__(self, lens_cosmo, median_rt_over_rs=2.0, c_power=3.0):
@@ -237,7 +235,66 @@
         :param c_actual:
         :param r_peri:
         :return:
         """
         rt_over_rs = self._norm * (c_actual / c_median) ** self._cpower * (r_peri / 0.5)
         _, rs, _ = self.lens_cosmo.NFW_params_physical(halo_mass, c_actual, halo_redshift)
         return rs * rt_over_rs
+
+class TruncationGalacticus(object):
+
+    def __init__(self, lens_cosmo, c_host):
+        """
+
+        :param lens_cosmo:
+        """
+
+        self._chost = c_host
+        self._lens_cosmo = lens_cosmo
+        self._mass_loss_interp = InterpGalacticus()
+        self._tau_mf_interpolation = tau_mf_interpolation()
+
+    @staticmethod
+    def _make_params_in_bounds_tau_evaluate(point):
+        """
+        This routine makes sure the arguments for the interpolation are inside the domain of the function.
+        """
+        min_c, max_c = np.log10(1.0), np.log10(10 ** 2.7)
+        (log10c, log10mass_loss_fraction) = point
+        log10c = max(min_c, log10c)
+        log10c = min(max_c, log10c)
+        log10mass_loss_fraction = max(-3.0, log10mass_loss_fraction)
+        log10mass_loss_fraction = min(-0.001, log10mass_loss_fraction)
+        return (log10c, log10mass_loss_fraction)
+
+    def truncation_radius_halo(self, halo):
+
+        """
+        Thiis method computess the truncation radius using the class attributes of an instance of Halo
+        :param halo: an instance of halo
+        :return: the truncation radius in physical kpc
+        """
+
+        return self.truncation_radius(halo.mass, halo.c,
+                                      halo.time_since_infall, self._chost, halo.z)
+
+    def truncation_radius(self, halo_mass, infall_concentration,
+                          time_since_infall, chost, z_eval_angles):
+        """
+
+        :param halo_mass:
+        :param infall_concentration:
+        :param time_since_infall:
+        :param chost:
+        :param z_eval_angles:
+        :return:
+        """
+        log10c = np.log10(infall_concentration)
+        log10mbound_over_minfall = self._mass_loss_interp(log10c, time_since_infall, chost)
+        point = self._make_params_in_bounds_tau_evaluate((log10c, log10mbound_over_minfall))
+        log10tau = float(self._tau_mf_interpolation(point))
+        tau = 10 ** log10tau
+        _, rs, _ = self._lens_cosmo.NFW_params_physical(halo_mass,
+                                                        infall_concentration,
+                                                        z_eval_angles)
+        return tau * rs
+
```

### Comparing `pyhalo-0.2.8/pyHalo/Halos/util.py` & `pyhalo-0.2.9/pyHalo/Halos/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,19 @@
 def tau_mf_interpolation():
 
     """
     This function interpolates solutions for the truncation radius of a truncated NFW profile given the concentration
     and final bound mass
     :return: an instance of RegularGridInterpolator that returns (r_t / r_s) given a final mass and concentration
     """
-    N = 50
-    tau = np.logspace(-1., 2., N)
+    N = 80
+    tau = np.logspace(-2., 2.3, N)
     log10_c = np.linspace(0, 2.7, N)
     # mass_fraction_1d = np.logspace(-1.45, -0.02, N)
-    mass_fraction_1d = np.logspace(-1.5, np.log10(0.999), N)
+    mass_fraction_1d = np.logspace(-3.0, np.log10(0.9999), N)
     log10tau_2d = np.zeros((N, N))
 
     # This computes the value of tau that correponds to each pair of (concentration, mass_loss)
     for i, log10con_i in enumerate(log10_c):
         log10final_mass = np.log10(tnfw_mass_fraction(tau, 10**log10con_i))
         mfinterp = interp1d(log10final_mass, np.log10(tau), bounds_error=False, fill_value='extrapolate')
         for j, mass_j in enumerate(mass_fraction_1d):
```

### Comparing `pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/delta_function.py` & `pyhalo-0.2.9/pyHalo/Rendering/MassFunctions/delta_function.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/density_peaks.py` & `pyhalo-0.2.9/pyHalo/Rendering/MassFunctions/density_peaks.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/mass_function_base.py` & `pyhalo-0.2.9/pyHalo/Rendering/MassFunctions/mass_function_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/stucker.py` & `pyhalo-0.2.9/pyHalo/Rendering/MassFunctions/stucker.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Rendering/MassFunctions/util.py` & `pyhalo-0.2.9/pyHalo/Rendering/MassFunctions/util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/correlated.py` & `pyhalo-0.2.9/pyHalo/Rendering/SpatialDistributions/correlated.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/nfw.py` & `pyhalo-0.2.9/pyHalo/Rendering/SpatialDistributions/nfw.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,27 +31,30 @@
         self._x3dmax = r_200_arcsec / rs_arcsec
         self._rcore_arcsec = r_core_arcsec
         self._cnfw_profile = CNFW()
         self._arcsec_to_kpc = arcsec_to_kpc
         super(ProjectedNFW, self).__init__()
 
     @classmethod
-    def from_Mhost(cls, m_host, zlens, rmax2d_arcsec, r_core_units_rs, lens_cosmo):
+    def from_Mhost(cls, m_host, zlens, rmax2d_arcsec, r_core_units_rs, lens_cosmo, c_host=None):
         """
 
-        :param m_host:
-        :param zlens:
-        :param rmax2d_arcsec:
-        :param r_core_units_rs:
-        :param lens_cosmo:
+        :param m_host: host halo mass
+        :param zlens: the deflector redshift
+        :param rmax2d_arcsec: the maximum radius in projection to rendering subhalos
+        :param r_core_units_rs: the core size in units rs of a cored nfw profile (subhalos are distributed
+        following a cored nfw profile)
+        :param lens_cosmo: an instance of LensCosmo
+        :param c_host: host halo concentration
         :return:
         """
-        c_model = ConcentrationDiemerJoyce(lens_cosmo)
-        c = c_model.nfw_concentration(m_host, zlens)
-        _, rs_mpc, r_200_mpc = lens_cosmo.nfwParam_physical(m_host, c, zlens)
+        if c_host is None:
+            c_model = ConcentrationDiemerJoyce(lens_cosmo)
+            c_host = c_model.nfw_concentration(m_host, zlens)
+        _, rs_mpc, r_200_mpc = lens_cosmo.nfwParam_physical(m_host, c_host, zlens)
         arcsec_to_kpc = lens_cosmo.cosmo.kpc_proper_per_asec(zlens)
         rs_arcsec = rs_mpc * 1000 / arcsec_to_kpc
         r_200_arcsec = r_200_mpc * 1000 / arcsec_to_kpc
         r_core_arcsec = r_core_units_rs * rs_arcsec
         return ProjectedNFW(rmax2d_arcsec, rs_arcsec, r_core_arcsec, r_200_arcsec, arcsec_to_kpc)
 
     def draw(self, N, z_plane=None):
```

### Comparing `pyhalo-0.2.8/pyHalo/Rendering/SpatialDistributions/uniform.py` & `pyhalo-0.2.9/pyHalo/Rendering/SpatialDistributions/uniform.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Rendering/correlated_structure.py` & `pyhalo-0.2.9/pyHalo/Rendering/correlated_structure.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Rendering/halo_population.py` & `pyhalo-0.2.9/pyHalo/Rendering/halo_population.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Rendering/line_of_sight.py` & `pyhalo-0.2.9/pyHalo/Rendering/line_of_sight.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Rendering/rendering_class_base.py` & `pyhalo-0.2.9/pyHalo/Rendering/rendering_class_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Rendering/subhalos.py` & `pyhalo-0.2.9/pyHalo/Rendering/subhalos.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/Rendering/two_halo.py` & `pyhalo-0.2.9/pyHalo/Rendering/two_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/concentration_models.py` & `pyhalo-0.2.9/pyHalo/concentration_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/defaults.py` & `pyhalo-0.2.9/pyHalo/defaults.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/mass_function_models.py` & `pyhalo-0.2.9/pyHalo/mass_function_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/preset_models.py` & `pyhalo-0.2.9/pyHalo/preset_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,21 +116,24 @@
     model_subhalos, kwargs_mc_subs = preset_concentration_models(concentration_model_subhalos,
                                                                  kwargs_concentration_model_subhalos)
     concentration_model_subhalos = model_subhalos(**kwargs_mc_subs)
 
     model_fieldhalos, kwargs_mc_field = preset_concentration_models(concentration_model_fieldhalos,
                                                                     kwargs_concentration_model_fieldhalos)
     concentration_model_fieldhalos = model_fieldhalos(**kwargs_mc_field)
+    c_host = concentration_model_fieldhalos.nfw_concentration(10 ** log_m_host, z_lens)
 
     # SET THE TRUNCATION RADIUS FOR SUBHALOS AND FIELD HALOS
     kwargs_truncation_model_subhalos['lens_cosmo'] = pyhalo.lens_cosmo
     kwargs_truncation_model_fieldhalos['lens_cosmo'] = pyhalo.lens_cosmo
 
     model_subhalos, kwargs_trunc_subs = truncation_models(truncation_model_subhalos)
     kwargs_trunc_subs.update(kwargs_truncation_model_subhalos)
+    if truncation_model_subhalos == 'TRUNCATION_GALACTICUS':
+        kwargs_trunc_subs['c_host'] = c_host
     truncation_model_subhalos = model_subhalos(**kwargs_trunc_subs)
 
     model_fieldhalos, kwargs_trunc_field = truncation_models(truncation_model_fieldhalos)
     kwargs_trunc_field.update(kwargs_truncation_model_fieldhalos)
     truncation_model_fieldhalos = model_fieldhalos(**kwargs_trunc_field)
 
     # NOW THAT THE CLASSES ARE SPECIFIED, WE SORT THE KEYWORD ARGUMENTS AND CLASSES INTO LISTS
@@ -147,15 +150,15 @@
                        'log_mhigh': log_mhigh,
                   'LOS_normalization': LOS_normalization,
                        'm_pivot': 10 ** 8,
                        'delta_power_law_index': delta_power_law_index,
                        'log_m_host': log_m_host}
     kwargs_mass_function_list = [kwargs_subhalos, kwargs_los]
     spatial_distribution_class_list = [subhalo_spatial_distribution, fieldhalo_spatial_distribution]
-    kwargs_subhalos_spatial = {'m_host': 10 ** log_m_host, 'zlens': z_lens,
+    kwargs_subhalos_spatial = {'m_host': 10 ** log_m_host, 'zlens': z_lens, 'c_host': c_host,
                                'rmax2d_arcsec': cone_opening_angle_arcsec / 2, 'r_core_units_rs': r_tidal,
                                'lens_cosmo': pyhalo.lens_cosmo}
     kwargs_los_spatial = {'cone_opening_angle': cone_opening_angle_arcsec, 'geometry': geometry}
     kwargs_spatial_distribution_list = [kwargs_subhalos_spatial, kwargs_los_spatial]
 
     if two_halo_contribution:
         population_model_list += ['TWO_HALO']
@@ -261,21 +264,24 @@
     model_fieldhalos, kwargs_mc_field = preset_concentration_models(concentration_model_fieldhalos,
                                                                     kwargs_concentration_model_fieldhalos)
     kwargs_mc_field['cosmo'] = pyhalo.astropy_cosmo
     kwargs_mc_field['log_mc'] = log_mc
     concentration_model_CDM = preset_concentration_models('DIEMERJOYCE19')[0]
     kwargs_mc_field['concentration_cdm_class'] = concentration_model_CDM
     concentration_model_fieldhalos = model_fieldhalos(**kwargs_mc_field)
+    c_host = concentration_model_fieldhalos.nfw_concentration(10 ** log_m_host, z_lens)
 
     # SET THE TRUNCATION RADIUS FOR SUBHALOS AND FIELD HALOS
     kwargs_truncation_model_subhalos['lens_cosmo'] = pyhalo.lens_cosmo
     kwargs_truncation_model_fieldhalos['lens_cosmo'] = pyhalo.lens_cosmo
 
     model_subhalos, kwargs_trunc_subs = truncation_models(truncation_model_subhalos)
     kwargs_trunc_subs.update(kwargs_truncation_model_subhalos)
+    if truncation_model_subhalos == 'TRUNCATION_GALACTICUS':
+        kwargs_trunc_subs['c_host'] = c_host
     kwargs_trunc_subs['lens_cosmo'] = pyhalo.lens_cosmo
     truncation_model_subhalos = model_subhalos(**kwargs_trunc_subs)
 
     model_fieldhalos, kwargs_trunc_field = truncation_models(truncation_model_fieldhalos)
     kwargs_trunc_field.update(kwargs_truncation_model_fieldhalos)
     kwargs_trunc_field['lens_cosmo'] = pyhalo.lens_cosmo
     truncation_model_fieldhalos = model_fieldhalos(**kwargs_trunc_field)
@@ -297,15 +303,16 @@
                   'log_mhigh': log_mhigh,
                   'LOS_normalization': LOS_normalization,
                   'm_pivot': 10 ** 8,
                   'log_m_host': log_m_host,
                   'delta_power_law_index': 0.0})
     kwargs_mass_function_list = [kwargs_mass_function_subhalos, kwargs_mass_function_fieldhalos, kwargs_mass_function_fieldhalos]
     spatial_distribution_class_list = [subhalo_spatial_distribution, fieldhalo_spatial_distribution, fieldhalo_spatial_distribution]
-    kwargs_subhalos_spatial = {'m_host': 10 ** log_m_host, 'zlens': z_lens,
+
+    kwargs_subhalos_spatial = {'m_host': 10 ** log_m_host, 'zlens': z_lens, 'c_host': c_host,
                                'rmax2d_arcsec': cone_opening_angle_arcsec / 2, 'r_core_units_rs': r_tidal,
                                'lens_cosmo': pyhalo.lens_cosmo}
     kwargs_los_spatial = {'cone_opening_angle': cone_opening_angle_arcsec, 'geometry': geometry}
     kwargs_spatial_distribution_list = [kwargs_subhalos_spatial, kwargs_los_spatial, kwargs_los_spatial]
 
     kwargs_halo_model = {'truncation_model_subhalos': truncation_model_subhalos,
                          'concentration_model_subhalos': concentration_model_subhalos,
@@ -468,15 +475,14 @@
                   'log_m_host': log_m_host, 'r_tidal': r_tidal, 'LOS_normalization': LOS_normalization,
                   'geometry_type': geometry_type, 'kwargs_cosmo': kwargs_cosmo,
                   'mdef_subhalos': 'ULDM', 'mdef_field_halos': 'ULDM',
                   'kwargs_density_profile': kwargs_density_profile
                   }
 
     uldm_no_fluctuations = WDM(**kwargs_wdm)
-
     if flucs: # add fluctuations to realization
         ext = RealizationExtensions(uldm_no_fluctuations)
         lambda_dB = de_broglie_wavelength(log10_m_uldm, velocity_scale) # de Broglie wavelength in kpc
 
         if flucs_args=={}:
             raise Exception('Must specify fluctuation arguments, see realization_extensions.add_ULDM_fluctuations')
 
@@ -672,15 +678,15 @@
                   'log_m_host': log_m_host, 'r_tidal': r_tidal, 'LOS_normalization': LOS_normalization,
                   'geometry_type': geometry_type, 'kwargs_cosmo': kwargs_cosmo,
                   'kwargs_density_profile': kwargs_density_profile
                   }
     return WDM(**kwargs_wdm)
 
 def WDMGeneral(z_lens, z_source, log_mc, dlogT_dlogk, sigma_sub=0.025, log_mlow=6., log_mhigh=10.,
-        truncation_model_subhalos='TRUNCATION_MEAN_DENSITY', kwargs_truncation_model_subhalos={},
+        truncation_model_subhalos='TRUNCATION_GALACTICUS', kwargs_truncation_model_subhalos={},
         truncation_model_fieldhalos='SPLASHBACK', kwargs_truncation_model_fieldhalos={},
         shmf_log_slope=-1.9, cone_opening_angle_arcsec=6., log_m_host=13.3, r_tidal=0.25,
         LOS_normalization=1.0, geometry_type='DOUBLE_CONE', kwargs_cosmo=None,
         mdef_subhalos='TNFW', mdef_field_halos='TNFW', kwargs_density_profile={}):
 
     """
     This preset model implements a generalized treatment of warm dark matter, or any theory that produces a cutoff in
@@ -730,25 +736,14 @@
     subhalo_spatial_distribution = ProjectedNFW
     fieldhalo_spatial_distribution = LensConeUniform
 
     kwargs_model_dlogT_dlogk = {'dlogT_dlogk': dlogT_dlogk}
     mass_function_model_subhalos, kwargs_mfunc_subs = preset_mass_function_models('STUCKER_SHMF', kwargs_model_dlogT_dlogk)
     mass_function_model_fieldhalos, kwargs_mfunc_field = preset_mass_function_models('STUCKER', kwargs_model_dlogT_dlogk)
 
-    # SET THE TRUNCATION RADIUS FOR SUBHALOS AND FIELD HALOS
-    model_subhalos, kwargs_truncation_model_subhalos = truncation_models(truncation_model_subhalos,
-                                                                         kwargs_truncation_model_subhalos)
-    kwargs_truncation_model_subhalos['lens_cosmo'] = pyhalo.lens_cosmo
-    truncation_model_subhalos = model_subhalos(**kwargs_truncation_model_subhalos)
-
-    model_fieldhalos, kwargs_truncation_model_fieldhalos = truncation_models(truncation_model_fieldhalos,
-                                                                             kwargs_truncation_model_fieldhalos)
-    kwargs_truncation_model_fieldhalos['lens_cosmo'] = pyhalo.lens_cosmo
-    truncation_model_fieldhalos = model_fieldhalos(**kwargs_truncation_model_fieldhalos)
-
     # SET THE CONCENTRATION-MASS RELATION FOR SUBHALOS AND FIELD HALOS
     concentration_model = 'FROM_FORMATION_HISTORY'
     model_subhalos, kwargs_concentration_model_subhalos = preset_concentration_models(concentration_model,
                                                                                       kwargs_model_dlogT_dlogk)
     concentration_model_CDM = preset_concentration_models('DIEMERJOYCE19')[0]
     kwargs_concentration_model_subhalos['concentration_cdm_class'] = concentration_model_CDM
     kwargs_concentration_model_subhalos['cosmo'] = pyhalo.astropy_cosmo
@@ -758,14 +753,26 @@
     model_fieldhalos, kwargs_concentration_model_fieldhalos = preset_concentration_models(concentration_model,
                                                                                           kwargs_model_dlogT_dlogk)
     kwargs_concentration_model_fieldhalos['concentration_cdm_class'] = concentration_model_CDM
     kwargs_concentration_model_fieldhalos['cosmo'] = pyhalo.astropy_cosmo
     kwargs_concentration_model_fieldhalos['log_mc'] = log_mc
     concentration_model_fieldhalos = model_fieldhalos(**kwargs_concentration_model_fieldhalos)
 
+    # SET THE TRUNCATION RADIUS FOR SUBHALOS AND FIELD HALOS
+    model_subhalos, kwargs_truncation_model_subhalos = truncation_models(truncation_model_subhalos)
+    kwargs_truncation_model_subhalos['lens_cosmo'] = pyhalo.lens_cosmo
+    c_host = concentration_model_fieldhalos.nfw_concentration(10 ** log_m_host, z_lens)
+    if truncation_model_subhalos == 'TRUNCATION_GALACTICUS':
+        kwargs_truncation_model_subhalos['c_host'] = c_host
+    truncation_model_subhalos = model_subhalos(**kwargs_truncation_model_subhalos)
+
+    model_fieldhalos, kwargs_truncation_model_fieldhalos = truncation_models(truncation_model_fieldhalos)
+    kwargs_truncation_model_fieldhalos['lens_cosmo'] = pyhalo.lens_cosmo
+    truncation_model_fieldhalos = model_fieldhalos(**kwargs_truncation_model_fieldhalos)
+
     # NOW THAT THE CLASSES ARE SPECIFIED, WE SORT THE KEYWORD ARGUMENTS AND CLASSES INTO LISTS
     population_model_list = ['SUBHALOS', 'LINE_OF_SIGHT', 'TWO_HALO']
 
     mass_function_class_list = [mass_function_model_subhalos,
                                 mass_function_model_fieldhalos,
                                 mass_function_model_fieldhalos]
     kwargs_mfunc_subs.update({'log_mlow': log_mlow,
```

### Comparing `pyhalo-0.2.8/pyHalo/pyhalo.py` & `pyhalo-0.2.9/pyHalo/pyhalo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/realization_extensions.py` & `pyhalo-0.2.9/pyHalo/realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/single_realization.py` & `pyhalo-0.2.9/pyHalo/single_realization.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/pyHalo/utilities.py` & `pyhalo-0.2.9/pyHalo/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -237,38 +237,16 @@
     :param rein: Einstein radius in kpc
     :param de_Broglie_wavelength: de Broglie wavelength of axion in kpc
     '''
     l = LensCosmo(z_lens,z_source)
     sigma_crit = l.get_sigma_crit_lensing(z_lens, z_source) * (1e-3) ** 2
     ds = delta_sigma(m, z_lens, rein, de_Broglie_wavelength)
     delta_kappa = ds / sigma_crit
-
     return delta_kappa
 
-def delta_sigmaNFW(z_lens, m, rein, de_Broglie_wavelength):
-    '''
-    Returns standard deviation of the density fluctuations in projection normalized by the projected
-    density of the host halo
-
-    :param z_lens,z_source: lens and source redshifts
-    :param m: main deflector halo mass in M_solar
-    :param rein: Einstein radius in kpc
-    :param de_Broglie_wavelength: de Broglie wavelength of axion in kpc
-    '''
-
-    cosmo = Cosmology()
-    l = LensCosmo(z_lens, 2.0, cosmo)
-    model, _ = preset_concentration_models('DIEMERJOYCE19')
-    cmodel = model(cosmo.astropy, scatter=False)
-    c = cmodel.nfw_concentration(m, z_lens)
-    rhos, rs, _ = l.NFW_params_physical(m, c, z_lens)
-    kappa_host = projected_squared_density(rein, rhos, rs, c) ** 0.5
-    ds = delta_sigma(m, z_lens, rein, de_Broglie_wavelength)
-    return ds/kappa_host
-
 def delta_sigma(m, z, rein, de_Broglie_wavelength):
     """
     Returns the mean ULDM fluctuation ampltiude of the host dark matter halo in units M_sun/kpc^2
     :param m:
     :param z:
     :param rein:
     :param de_Broglie_wavelength:
@@ -312,30 +290,18 @@
     :param c:
     :return:
     """
     G = 4.3e-6  # kpc/solMass * (km/sec)**2
     prefactor = 4 * np.pi * G * rhos ** 2 * rs ** 2
     density_at_r = rhos / (x * (1 + x) ** 2)
     _integrand = lambda x: (np.log(1 + x) - x / (1 + x)) / (x * (1 + x) ** 2) / x ** 2
-
     x = np.linspace(x, c, 150)
     y = _integrand(x)
     return np.sqrt(prefactor * simps(y, x) / density_at_r)
 
-def nfw_velocity_dispersion_fromfit(m):
-    """
-    The velocity dispersion of an NFW profile with mass m calibrated from a power law fit for halos
-    between 10^6 and 10^10 at z=0
-    :param m: halo mass in M_sun
-    :return: the velocity dispersion inside rs
-    """
-    coeffs = [0.31575757, -1.74259129]
-    log_vrms = coeffs[0] * np.log10(m) + coeffs[1]
-    return 10 ** log_vrms
-
 class MinHaloMassULDM(object):
 
     def __init__(self, log10_m_uldm, astropy_instance, log_mlow):
         """
         This class implements the minimum halo mass for ultra-light dark matter, given the particle mass and a cosmology
 
         The call method returns the maximum of log_mlow, and the resulting minimum ULDM halo mass to ensure that one does
```

### Comparing `pyhalo-0.2.8/pyHalo.egg-info/PKG-INFO` & `pyhalo-0.2.9/pyHalo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.2.8/pyHalo.egg-info/SOURCES.txt` & `pyhalo-0.2.9/pyHalo.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 pyHalo.egg-info/entry_points.txt
 pyHalo.egg-info/not-zip-safe
 pyHalo.egg-info/requires.txt
 pyHalo.egg-info/top_level.txt
 pyHalo/Cosmology/__init__.py
 pyHalo/Cosmology/cosmology.py
 pyHalo/Cosmology/geometry.py
+pyHalo/GalacticusInterface/__init__.py
+pyHalo/GalacticusInterface/param_file.py
+pyHalo/GalacticusInterface/read_output.py
 pyHalo/Halos/__init__.py
 pyHalo/Halos/concentration.py
 pyHalo/Halos/halo_base.py
 pyHalo/Halos/lens_cosmo.py
 pyHalo/Halos/tidal_truncation.py
 pyHalo/Halos/util.py
 pyHalo/Halos/HaloModels/NFW.py
@@ -49,14 +52,17 @@
 pyHalo/Halos/HaloModels/TNFW.py
 pyHalo/Halos/HaloModels/TNFWemulator.py
 pyHalo/Halos/HaloModels/ULDM.py
 pyHalo/Halos/HaloModels/__init__.py
 pyHalo/Halos/HaloModels/gaussian.py
 pyHalo/Halos/HaloModels/generalized_nfw.py
 pyHalo/Halos/HaloModels/powerlaw.py
+pyHalo/Halos/galacticus_truncation/__init__.py
+pyHalo/Halos/galacticus_truncation/interp_mass_loss.py
+pyHalo/Halos/galacticus_truncation/tabulated_mass_loss.py
 pyHalo/Rendering/__init__.py
 pyHalo/Rendering/correlated_structure.py
 pyHalo/Rendering/halo_population.py
 pyHalo/Rendering/line_of_sight.py
 pyHalo/Rendering/rendering_class_base.py
 pyHalo/Rendering/subhalos.py
 pyHalo/Rendering/two_halo.py
@@ -94,14 +100,15 @@
 tests/test_cosmology/__init__.py
 tests/test_cosmology/test_cone_geometry.py
 tests/test_cosmology/test_cosmo.py
 tests/test_cosmology/test_cylinder_geometry.py
 tests/test_halos/__init__.py
 tests/test_halos/test_adiabatic_tides.py
 tests/test_halos/test_concentrations.py
+tests/test_halos/test_galacticus_truncation.py
 tests/test_halos/test_gaussian.py
 tests/test_halos/test_general_nfw.py
 tests/test_halos/test_lenscosmo.py
 tests/test_halos/test_nfw_halo.py
 tests/test_halos/test_pjaffe.py
 tests/test_halos/test_point_mass.py
 tests/test_halos/test_powerlaw_profile.py
```

### Comparing `pyhalo-0.2.8/pyproject.toml` & `pyhalo-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyhalo"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="Daniel Gilman", email="daniel.gilman@utoronto.ca" },
 ]
 description = "A python package for generating populations of dark matter halos"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pyhalo-0.2.8/setup.py` & `pyhalo-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 setup_requirements = [ ]
 
 test_requirements = [ ]
 
 setup(
     author="Daniel Gilman",
-    version='0.2.1',
+    version='0.2.9',
     author_email='daniel.gilman@utoronto.ca',
     classifiers=[
         'Development Status :: 5 - Stable',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3.4',
```

### Comparing `pyhalo-0.2.8/tests/test_concentration_models.py` & `pyhalo-0.2.9/tests/test_concentration_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_cosmology/test_cone_geometry.py` & `pyhalo-0.2.9/tests/test_cosmology/test_cone_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_cosmology/test_cosmo.py` & `pyhalo-0.2.9/tests/test_cosmology/test_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_cosmology/test_cylinder_geometry.py` & `pyhalo-0.2.9/tests/test_cosmology/test_cylinder_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_halos/test_adiabatic_tides.py` & `pyhalo-0.2.9/tests/test_halos/test_adiabatic_tides.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_halos/test_concentrations.py` & `pyhalo-0.2.9/tests/test_halos/test_concentrations.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_halos/test_gaussian.py` & `pyhalo-0.2.9/tests/test_halos/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_halos/test_general_nfw.py` & `pyhalo-0.2.9/tests/test_halos/test_general_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_halos/test_lenscosmo.py` & `pyhalo-0.2.9/tests/test_halos/test_lenscosmo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import numpy.testing as npt
-from pyHalo.Cosmology.cosmology import Cosmology
 from pyHalo.Halos.lens_cosmo import LensCosmo
 import numpy as np
 import pytest
 from astropy.cosmology import FlatLambdaCDM
 from astropy.constants import G, c
-from pyHalo.Halos.concentration import ConcentrationDiemerJoyce
 import astropy.units as un
-from pyHalo.Halos.HaloModels.NFW import NFWSubhhalo, NFWFieldHalo
 from pyHalo.Cosmology.cosmology import Cosmology
 from lenstronomy.Cosmo.lens_cosmo import LensCosmo as LensCosmoLenstronomy
-from pyHalo.Halos.HaloModels.generalized_nfw import GeneralNFWSubhalo
+
 
 class TestLensCosmo(object):
 
     def setup_method(self):
 
         kwargs_cosmo = {'Om0': 0.2}
         self.cosmo = Cosmology(cosmo_kwargs=kwargs_cosmo)
```

### Comparing `pyhalo-0.2.8/tests/test_halos/test_nfw_halo.py` & `pyhalo-0.2.9/tests/test_halos/test_nfw_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_halos/test_pjaffe.py` & `pyhalo-0.2.9/tests/test_halos/test_pjaffe.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_halos/test_point_mass.py` & `pyhalo-0.2.9/tests/test_halos/test_point_mass.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_halos/test_powerlaw_profile.py` & `pyhalo-0.2.9/tests/test_halos/test_powerlaw_profile.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_halos/test_tnfw_halo.py` & `pyhalo-0.2.9/tests/test_halos/test_tnfw_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_halos/test_truncation.py` & `pyhalo-0.2.9/tests/test_halos/test_truncation.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_halos/test_uldm.py` & `pyhalo-0.2.9/tests/test_halos/test_uldm.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_halos/test_util.py` & `pyhalo-0.2.9/tests/test_halos/test_util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_mass_function_models.py` & `pyhalo-0.2.9/tests/test_mass_function_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_plotting.py` & `pyhalo-0.2.9/tests/test_plotting.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 import numpy.testing as npt
 import pytest
 from pyHalo.preset_models import CDM
-from pyHalo.plotting_routines import plot_subhalo_bound_mass, \
-    plot_subhalo_mass_functon, plot_concentration_mass_relation, plot_halo_mass_function
+from pyHalo.plotting_routines import *
 
 class TestPlottingRoutines(object):
 
     def setup_method(self):
         self.realization = CDM(0.5, 1.5, sigma_sub=0.025, LOS_normalization=0.0)
 
+    def test_spatial_distribution(self):
+        plot_subhalo_spatial_distribution(self.realization)
+
     def test_mass_function_plot(self):
 
         plot_subhalo_mass_functon(self.realization)
         plot_subhalo_mass_functon(self.realization, bound_mass_function=True)
         plot_halo_mass_function(self.realization, z_eval=0.5)
         plot_halo_mass_function(self.realization, z_eval=None)
         plot_halo_mass_function(self.realization, z_eval=[0.5, 0.6])
 
     def test_bound_mass_function_plot(self):
 
         plot_subhalo_bound_mass(self.realization)
+        plot_bound_mass_histogram(self.realization)
+        plot_subhalo_concentration_versus_bound_mass(self.realization)
 
     def test_plot_mc_relation(self):
 
         plot_concentration_mass_relation(self.realization, z_eval='z_lens')
         plot_concentration_mass_relation(self.realization, z_eval=0.5)
         plot_concentration_mass_relation(self.realization, z_eval=[0.4, 0.6])
 
+    def test_truncation_radius_plot(self):
+
+        plot_truncation_radius_histogram(self.realization, subhalos_only=False)
+        plot_truncation_radius_histogram(self.realization, subhalos_only=True)
+
 
 if __name__ == '__main__':
      pytest.main()
```

### Comparing `pyhalo-0.2.8/tests/test_preset_models.py` & `pyhalo-0.2.9/tests/test_preset_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,20 +8,26 @@
 
     def test_CDM(self):
 
         cdm = CDM(0.5, 1.5)
         _ = cdm.lensing_quantities()
         _ = preset_model_from_name('CDM')
 
+        cdm = CDM(0.5, 1.5,
+                  truncation_model_subhalos='TRUNCATION_GALACTICUS')
+
     def test_WDM(self):
 
         wdm = WDM(0.5, 1.5, 8.0)
         _ = wdm.lensing_quantities()
         _ = preset_model_from_name('WDM')
 
+        _ = WDM(0.5, 1.5, 8.0,
+                  truncation_model_subhalos='TRUNCATION_GALACTICUS')
+
     def test_ULDM(self):
 
         flucs_shape = 'ring'
         flucs_args = {'angle': 0.0, 'rmin': 0.9, 'rmax': 1.1}
         uldm = ULDM(0.5, 1.5, -21, flucs_shape=flucs_shape, flucs_args=flucs_args)
         _ = uldm.lensing_quantities()
         _ = preset_model_from_name('ULDM')
@@ -42,14 +48,16 @@
         _ = preset_model_from_name('WDM_mixed')
 
     def test_WDM_general(self):
         func = preset_model_from_name('WDMGeneral')
         wdm = func(0.5, 1.5, 7.7, 2.0)
         _ = wdm.lensing_quantities()
 
+        wdm = func(0.5, 1.5, 7.7, 2.0, truncation_model_subhalos='TRUNCATION_GALACTICUS')
+
     def test_CDM_emulator(self):
 
         def emulator_input_callable(*args, **kwargs):
             subhalo_infall_masses = np.array([10**7,10**8])
             subhalo_x_kpc = np.array([1.0, 1.0])
             subhalo_y_kpc = np.array([1.0, 1.0])
             subhalo_final_bound_masses = subhalo_infall_masses / 2
```

### Comparing `pyhalo-0.2.8/tests/test_pyhalo_base.py` & `pyhalo-0.2.9/tests/test_pyhalo_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_realization_extensions.py` & `pyhalo-0.2.9/tests/test_realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_rendering/test_2halo.py` & `pyhalo-0.2.9/tests/test_rendering/test_2halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_rendering/test_los.py` & `pyhalo-0.2.9/tests/test_rendering/test_los.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_rendering/test_mass_functions/test_base_functions.py` & `pyhalo-0.2.9/tests/test_rendering/test_mass_functions/test_base_functions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_rendering/test_mass_functions/test_delta_function.py` & `pyhalo-0.2.9/tests/test_rendering/test_mass_functions/test_delta_function.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_rendering/test_mass_functions/test_sheth_tormen.py` & `pyhalo-0.2.9/tests/test_rendering/test_mass_functions/test_sheth_tormen.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_rendering/test_mass_functions/test_stucker.py` & `pyhalo-0.2.9/tests/test_rendering/test_mass_functions/test_stucker.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_rendering/test_population.py` & `pyhalo-0.2.9/tests/test_rendering/test_population.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_rendering/test_spatial_distribution/test_correlated.py` & `pyhalo-0.2.9/tests/test_rendering/test_spatial_distribution/test_correlated.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_rendering/test_spatial_distribution/test_nfw.py` & `pyhalo-0.2.9/tests/test_rendering/test_spatial_distribution/test_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_rendering/test_spatial_distribution/test_uniform.py` & `pyhalo-0.2.9/tests/test_rendering/test_spatial_distribution/test_uniform.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_rendering/test_subhalos.py` & `pyhalo-0.2.9/tests/test_rendering/test_subhalos.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_single_realization.py` & `pyhalo-0.2.9/tests/test_single_realization.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.8/tests/test_utilities.py` & `pyhalo-0.2.9/tests/test_utilities.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from lenstronomy.LensModel.lens_model import LensModel
 import numpy.testing as npt
 import numpy as np
 from pyHalo.utilities import interpolate_ray_paths, de_broglie_wavelength, delta_sigma, ITSampling, \
-    inverse_transform_sampling, inverse_transform_sampling_from_cdf
+    inverse_transform_sampling, delta_kappa, nfw_velocity_dispersion
 from pyHalo.Cosmology.cosmology import Cosmology
+from pyHalo.Halos.lens_cosmo import LensCosmo
 import pytest
 
 class TestUtilities(object):
 
     def test_interp_ray_paths(self):
 
         cosmo = Cosmology()
@@ -43,19 +44,32 @@
     def test_uldm_functions(self):
 
         log10_m_uldm=-22 # log(eV)
         v=200 # km/s
         z_lens,z_source=0.5,1.5
         m=1e13 #M_solar
         rein=6. #kpc
-
+        lens_cosmo = LensCosmo(z_lens, z_source)
         lambda_dB = de_broglie_wavelength(log10_m_uldm,v)
         npt.assert_almost_equal(lambda_dB,0.6)
-        delta_kappa = delta_sigma(m,z_lens,rein,lambda_dB)
-        npt.assert_almost_equal(delta_kappa/80837585.696, 1, 2)
+        delta_s = delta_sigma(m,z_lens,rein,lambda_dB)
+        npt.assert_almost_equal(delta_s/80837585.696, 1, 2)
+        dk = delta_kappa(z_lens, z_source, 10 ** 13.0, rein, lambda_dB)
+        sigma_crit = lens_cosmo.get_sigma_crit_lensing(z_lens, z_source) * (1e-3) ** 2
+        npt.assert_almost_equal(delta_s, dk * sigma_crit)
+
+    def test_nfw_velocity_dispersion(self):
+
+        lens_comso = LensCosmo(0.5, 1.5)
+        m = 10**8
+        z = 0.5
+        c = 15.0
+        rhos, rs, _ = lens_comso.NFW_params_physical(m, c, z)
+        vdis1 = nfw_velocity_dispersion(rhos, rs, c)
+        npt.assert_almost_equal(vdis1/6.34, 1.0, 2)
 
     def test_inverse_transform_sampling(self):
 
         mu = 2.0
         sigma = 1.5
         func = lambda x: np.exp(-0.5 * (x - mu) ** 2 / sigma**2)
         x = np.linspace(mu - 5*sigma, mu + 5*sigma, 1000)
```

