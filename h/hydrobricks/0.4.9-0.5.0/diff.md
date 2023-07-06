# Comparing `tmp/hydrobricks-0.4.9.tar.gz` & `tmp/hydrobricks-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrobricks-0.4.9.tar", last modified: Wed Feb 15 09:09:02 2023, max compression
+gzip compressed data, was "hydrobricks-0.5.0.tar", last modified: Thu Jul  6 16:05:04 2023, max compression
```

## Comparing `hydrobricks-0.4.9.tar` & `hydrobricks-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:09:02.091725 hydrobricks-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-02-15 09:09:02.091725 hydrobricks-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:09:02.091725 hydrobricks-0.4.9/hydrobricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-02-15 09:09:02.000000 hydrobricks-0.4.9/hydrobricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-15 09:09:02.000000 hydrobricks-0.4.9/hydrobricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 09:09:02.000000 hydrobricks-0.4.9/hydrobricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 09:09:01.000000 hydrobricks-0.4.9/hydrobricks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-15 09:09:02.000000 hydrobricks-0.4.9/hydrobricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-15 09:09:02.000000 hydrobricks-0.4.9/hydrobricks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:09:02.087726 hydrobricks-0.4.9/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:09:02.087726 hydrobricks-0.4.9/python/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:09:02.091725 hydrobricks-0.4.9/python/src/hydrobricks/
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:09:02.091725 hydrobricks-0.4.9/python/src/hydrobricks/behaviours/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/behaviours/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/behaviours/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/behaviours/behaviour_land_cover_change.py
--rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/forcing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/hydro_units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:09:02.091725 hydrobricks-0.4.9/python/src/hydrobricks/models/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/models/socont.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:09:02.091725 hydrobricks-0.4.9/python/src/hydrobricks/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/preprocessing/catchment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/spotpy_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/python/src/hydrobricks/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 09:09:02.091725 hydrobricks-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-02-15 09:08:53.000000 hydrobricks-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:05:04.340725 hydrobricks-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 16:04:54.000000 hydrobricks-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-06 16:05:04.340725 hydrobricks-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-06 16:04:54.000000 hydrobricks-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:05:04.340725 hydrobricks-0.5.0/hydrobricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-06 16:05:04.000000 hydrobricks-0.5.0/hydrobricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-06 16:05:04.000000 hydrobricks-0.5.0/hydrobricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:05:04.000000 hydrobricks-0.5.0/hydrobricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:05:04.000000 hydrobricks-0.5.0/hydrobricks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 16:05:04.000000 hydrobricks-0.5.0/hydrobricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 16:05:04.000000 hydrobricks-0.5.0/hydrobricks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-06 16:04:54.000000 hydrobricks-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:05:04.336725 hydrobricks-0.5.0/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:05:04.336725 hydrobricks-0.5.0/python/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:05:04.340725 hydrobricks-0.5.0/python/src/hydrobricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:05:04.340725 hydrobricks-0.5.0/python/src/hydrobricks/behaviours/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/behaviours/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/behaviours/behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/behaviours/behaviour_land_cover_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/forcing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/hydro_units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:05:04.340725 hydrobricks-0.5.0/python/src/hydrobricks/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/models/socont.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18365 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:05:04.340725 hydrobricks-0.5.0/python/src/hydrobricks/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/preprocessing/catchment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/spotpy_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/python/src/hydrobricks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:05:04.340725 hydrobricks-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-06 16:04:55.000000 hydrobricks-0.5.0/setup.py
```

### Comparing `hydrobricks-0.4.9/LICENSE` & `hydrobricks-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.4.9/README.md` & `hydrobricks-0.5.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # hydrobricks
 
-> :warning: **This is a very preliminary code base that is not doing much yet...**
+> :warning: **hydrobricks is still in its very early stages and options are limited at this point...**
 
-Modular Hydrological Modelling Framework
+A modular hydrological modelling framework.
 
 [![DOI](https://zenodo.org/badge/301952016.svg)](https://zenodo.org/badge/latestdoi/301952016)
+[![GitHub release](https://img.shields.io/github/v/release/hydrobricks/hydrobricks)](https://github.com/hydrobricks/hydrobricks/releases)
+[![PyPI](https://img.shields.io/pypi/v/hydrobricks)](https://pypi.org/project/hydrobricks/)
+![Static Badge](https://img.shields.io/badge/python-%3E%3D3.8-blue)
 [![Core Tests Linux](https://github.com/hydrobricks/hydrobricks/actions/workflows/core-tests-linux.yml/badge.svg)](https://github.com/hydrobricks/hydrobricks/actions/workflows/core-tests-linux.yml)
 [![Python Wheels](https://github.com/hydrobricks/hydrobricks/actions/workflows/python-wheels.yml/badge.svg)](https://github.com/hydrobricks/hydrobricks/actions/workflows/python-wheels.yml)
-[![codecov](https://codecov.io/gh/hydrobricks/hydrobricks/branch/main/graph/badge.svg?token=G1PBSK8EG2)](https://codecov.io/gh/hydrobricks/hydrobricks)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/hydrobricks/hydrobricks/main.svg)](https://results.pre-commit.ci/latest/github/hydrobricks/hydrobricks/main)
 [![Core Doxygen](https://github.com/hydrobricks/hydrobricks/actions/workflows/core-doxygen.yml/badge.svg)](https://github.com/hydrobricks/hydrobricks/actions/workflows/core-doxygen.yml)
+[![Documentation Status](https://readthedocs.org/projects/hydrobricks/badge/?version=latest)](https://hydrobricks.readthedocs.io/en/latest/?badge=latest)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/hydrobricks/hydrobricks/main.svg)](https://results.pre-commit.ci/latest/github/hydrobricks/hydrobricks/main)
+[![Codecov](https://img.shields.io/codecov/c/github/hydrobricks/hydrobricks)](https://codecov.io/gh/hydrobricks/hydrobricks)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/639e5bb76690488f9aac5feb89722bfa)](https://www.codacy.com/gh/hydrobricks/hydrobricks/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=hydrobricks/hydrobricks&amp;utm_campaign=Badge_Grade)
 
+
 ## Install
 
 Wheels are available to install from PyPI (https://pypi.org/project/hydrobricks/)
 
 Install: ```pip install hydrobricks```
 
 ## Resources
-* **Documentation**: https://hydrobricks-doc.readthedocs.io/en/latest/
-* How to build: https://github.com/hydrobricks/hydrobricks/wiki
-* Code documentation of the core: https://hydrobricks.github.io/hydrobricks-doc-core/
+*   **Documentation**: https://hydrobricks.readthedocs.io/en/latest/
+*   How to build: https://github.com/hydrobricks/hydrobricks/wiki
+*   Code documentation of the core: https://hydrobricks.github.io/hydrobricks-doc-core/
```

### Comparing `hydrobricks-0.4.9/hydrobricks.egg-info/SOURCES.txt` & `hydrobricks-0.5.0/hydrobricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.4.9/pyproject.toml` & `hydrobricks-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = [
     "setuptools>=42",
     "wheel",
     "ninja",
-    "cmake>=3.12",
+    "cmake>=3.12"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 88
 
 [tool.isort]
@@ -32,39 +32,41 @@
 manylinux-s390x-image = "manylinux_2_28"
 manylinux-pypy_x86_64-image = "manylinux_2_28"
 manylinux-pypy_aarch64-image = "manylinux_2_28"
 build-verbosity = 3
 
 [tool.cibuildwheel.linux]
 before-build = [
+    "dnf update -y",
+    "dnf install epel-release -y",
+    "dnf install perl perl-core perl-IPC-Cmd perl-Digest-SHA -y",
     "rm -rf {project}/build/lib.*",
     "rm -rf {project}/build/temp.*",
     "rm -rf {project}/build/bdist.*",
-    "pip install conan",
+    "pip install conan==1.*",
     "pip show conan",
     "conan profile new default --detect --force",
     "conan remote add gitlab https://gitlab.com/api/v4/packages/conan --force",
     "conan profile update settings.compiler.libcxx=libstdc++11 default",
     "conan config set general.revisions_enabled=1",
-    "conan install . --build=missing",
+    "conan install . --build=missing -s build_type=Release -pr:b=default",
 ]
 
 [tool.cibuildwheel.windows]
 before-build = [
-    "pip install conan",
+    "pip install conan==1.*",
     "pip show conan",
     "conan profile new default --detect --force",
     "conan remote add gitlab https://gitlab.com/api/v4/packages/conan --force",
     "conan config set general.revisions_enabled=1",
-    "conan install . --build=missing",
-    #"conan install . --build=missing -s build_type=Debug",
+    "conan install . --build=missing -s build_type=Release -pr:b=default",
 ]
 
 [tool.cibuildwheel.macos]
 before-build = [
-    "pip install conan",
+    "pip install conan==1.*",
     "pip show conan",
     "conan profile new default --detect --force",
     "conan remote add gitlab https://gitlab.com/api/v4/packages/conan --force",
     "conan config set general.revisions_enabled=1",
-    "conan install . --build=missing",
+    "conan install . --build=missing -s build_type=Release -pr:b=default",
 ]
```

### Comparing `hydrobricks-0.4.9/python/src/hydrobricks/__init__.py` & `hydrobricks-0.5.0/python/src/hydrobricks/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.4.9/python/src/hydrobricks/behaviours/behaviour_land_cover_change.py` & `hydrobricks-0.5.0/python/src/hydrobricks/behaviours/behaviour_land_cover_change.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import _hydrobricks as _hb
-import pandas as pd
 import numpy as np
+import pandas as pd
 from hydrobricks import utils
 
 from .behaviour import Behaviour
 
 
 class BehaviourLandCoverChange(Behaviour):
     """Class for the land cover changes."""
```

### Comparing `hydrobricks-0.4.9/python/src/hydrobricks/forcing.py` & `hydrobricks-0.5.0/python/src/hydrobricks/forcing.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.4.9/python/src/hydrobricks/hydro_units.py` & `hydrobricks-0.5.0/python/src/hydrobricks/hydro_units.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.4.9/python/src/hydrobricks/models/model.py` & `hydrobricks-0.5.0/python/src/hydrobricks/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import importlib
 import os
 from abc import ABC, abstractmethod
 
 import _hydrobricks as _hb
 import HydroErr
-import pandas as pd
 from _hydrobricks import ModelHydro, SettingsModel
 from hydrobricks import utils
 
 
 class Model(ABC):
     """Base class for the models"""
 
@@ -130,15 +129,16 @@
         except RuntimeError:
             print("A runtime exception occurred.")
         except TypeError:
             print("A type error exception occurred.")
         except Exception:
             print("An exception occurred.")
 
-    def cleanup(self):
+    @staticmethod
+    def cleanup():
         _hb.close_log()
 
     def initialize_state_variables(self, parameters, forcing=None):
         """
         Run the model and save the state variables as initial values.
 
         Parameters
```

### Comparing `hydrobricks-0.4.9/python/src/hydrobricks/models/socont.py` & `hydrobricks-0.5.0/python/src/hydrobricks/models/socont.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,96 +27,95 @@
             raise Exception(f'Socont model initialization raised an exception: {err}')
 
     def generate_parameters(self):
         ps = ParameterSet()
 
         ps.define_parameter(
             component='snow_rain_transition', name='transition_start', unit='°C',
-            min_value=-5, max_value=5, default_value=0, mandatory=False)
+            aliases=['prec_t_start'], min_value=-2, max_value=2, default_value=0,
+            mandatory=False)
 
         ps.define_parameter(
             component='snow_rain_transition', name='transition_end', unit='°C',
-            min_value=-5, max_value=5, default_value=2, mandatory=False)
+            aliases=['prec_t_end'], min_value=0, max_value=4, default_value=2,
+            mandatory=False)
 
         ps.define_parameter(
             component='snowpack', name='degree_day_factor', unit='mm/d/°C',
             aliases=['a_snow'], min_value=1, max_value=12, mandatory=True)
 
         ps.define_parameter(
             component='snowpack', name='melting_temperature', unit='°C',
-            min_value=0, max_value=5, default_value=0, mandatory=False)
+            aliases=['melt_t_snow'], min_value=0, max_value=5, default_value=0,
+            mandatory=False)
 
         i_glacier = 0
         has_glacier = False
         for cover_type, cover_name in zip(self.land_cover_types, self.land_cover_names):
             if cover_type == 'glacier':
                 has_glacier = True
                 aliases = ['a_ice']
-                if self.land_cover_types.count('glacier') == 1:
-                    ps.define_constraint('a_snow', '<', aliases[0])
-                elif self.land_cover_types.count('glacier') > 1:
+                if self.land_cover_types.count('glacier') > 1:
                     i_glacier += 1
                     aliases = [f'a_ice_{cover_name.replace("-", "_")}',
-                               f'a_ice_{i_glacier}', f'a_ice{i_glacier}']
+                               f'a_ice_{i_glacier}']
+
+                ps.define_constraint('a_snow', '<', aliases[0])
+                ps.define_constraint('k_snow', '<', 'k_ice')
 
                 ps.define_parameter(
                     component=cover_name, name='degree_day_factor',
                     unit='mm/d/°C', aliases=aliases, min_value=5, max_value=20,
                     mandatory=True)
 
                 ps.define_parameter(
                     component=cover_name, name='melting_temperature',
-                    unit='°C', min_value=0, max_value=5, default_value=0,
-                    mandatory=False)
+                    unit='°C', aliases=['melt_t_ice'], min_value=0, max_value=5,
+                    default_value=0, mandatory=False)
 
         if has_glacier:
             ps.define_parameter(
-                component='glacier-area-rain-snowmelt-storage', name='response_factor',
-                unit='1/t', aliases=['k_snow'], min_value=0, max_value=1,
+                component='glacier_area_rain_snowmelt_storage', name='response_factor',
+                unit='1/d', aliases=['k_snow'], min_value=0.05, max_value=0.25,
                 mandatory=True)
 
             ps.define_parameter(
-                component='glacier-area-icemelt-storage', name='response_factor',
-                unit='1/t', aliases=['k_ice'], min_value=0, max_value=1,
+                component='glacier_area_icemelt_storage', name='response_factor',
+                unit='1/d', aliases=['k_ice'], min_value=0.05, max_value=1,
                 mandatory=True)
 
         if self.surface_runoff == 'socont_runoff':
             ps.define_parameter(
-                component='surface-runoff', name='runoff_coefficient', unit='m^(4/3)/s',
+                component='surface_runoff', name='runoff_coefficient', unit='m^(4/3)/s',
                 aliases=['beta'], min_value=100, max_value=30000, mandatory=True)
             ps.define_parameter(
-                component='surface-runoff', name='slope', unit='°',
+                component='surface_runoff', name='slope', unit='°',
                 aliases=['J'], min_value=0, max_value=90, mandatory=True)
         elif self.surface_runoff == 'linear_storage':
             ps.define_parameter(
-                component='surface-runoff', name='response_factor', unit='1/t',
-                aliases=['k_quick'], min_value=0, max_value=1, mandatory=True)
+                component='surface_runoff', name='response_factor', unit='1/d',
+                aliases=['k_quick'], min_value=0.05, max_value=1, mandatory=True)
 
         ps.define_parameter(
-            component='slow-reservoir', name='capacity', unit='mm', aliases=['A'],
-            min_value=0, max_value=3000, mandatory=True)
-
-        if self.soil_storage_nb == 1:
-            ps.define_parameter(
-                component='slow-reservoir', name='response_factor', unit='1/t',
-                aliases=['k_slow'], min_value=0, max_value=1, mandatory=True)
+            component='slow_reservoir', name='capacity', unit='mm', aliases=['A'],
+            min_value=10, max_value=3000, mandatory=True)
 
-        elif self.soil_storage_nb == 2:
-            ps.define_parameter(
-                component='slow-reservoir', name='response_factor', unit='1/t',
-                aliases=['k_slow_1', 'k_slow1'], min_value=0, max_value=1,
-                mandatory=True)
+        ps.define_parameter(
+            component='slow_reservoir', name='response_factor', unit='1/d',
+            aliases=['k_slow', 'k_slow_1', 'k_slow1'], min_value=0.001, max_value=1,
+            mandatory=True)
 
+        if self.soil_storage_nb == 2:
             ps.define_parameter(
-                component='slow-reservoir', name='percolation_rate', unit='mm/d',
+                component='slow_reservoir', name='percolation_rate', unit='mm/d',
                 aliases=['percol'], min_value=0, max_value=10, mandatory=True)
 
             ps.define_parameter(
-                component='slow-reservoir-2', name='response_factor', unit='1/t',
-                aliases=['k_slow_2', 'k_slow2'], min_value=0, max_value=1,
+                component='slow_reservoir_2', name='response_factor', unit='1/d',
+                aliases=['k_slow_2', 'k_slow2'], min_value=0.001, max_value=1,
                 mandatory=True)
 
             if self.surface_runoff == 'linear_storage':
                 ps.define_constraint('k_slow_1', '<', 'k_quick')
                 ps.define_constraint('k_slow_2', '<', 'k_quick')
             ps.define_constraint('k_slow_2', '<', 'k_slow_1')
```

### Comparing `hydrobricks-0.4.9/python/src/hydrobricks/parameters.py` & `hydrobricks-0.5.0/python/src/hydrobricks/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         """
         Define a parameter by setting its properties.
 
         Parameters
         ----------
         component : str
             The component (brick) name to which the parameter refer (e.g., snowpack,
-            glacier, surface-runoff).
+            glacier, surface_runoff).
         name : str
             The name of the parameter in the C++ code of hydrobricks (e.g.,
             degree_day_factor, response_factor).
         unit : str
             The unit of the parameter.
         aliases : list
             Aliases to the parameter name, such as names used in other implementations
@@ -201,15 +201,15 @@
             min_value = row['min']
             max_value = row['max']
             value = row['value']
 
             if value is None:
                 return False
 
-            if type(min_value) != list:
+            if not isinstance(min_value, list):
                 if max_value is not None and value > max_value:
                     return False
                 if min_value is not None and value < min_value:
                     return False
             else:
                 assert isinstance(max_value, list)
                 assert isinstance(value, list)
@@ -226,15 +226,15 @@
         Set the parameter values.
 
         Parameters
         ----------
         values : dict
             The values must be provided as a dictionary with the parameter name with the
             related component or one of its aliases as the key.
-            Example: {'k': 32, 'A': 300} or {'slow-reservoir:capacity': 300}
+            Example: {'k': 32, 'A': 300} or {'slow_reservoir:capacity': 300}
         check_range : bool
             Check that the parameter value falls into the allowed range.
         allow_adapt : bool
             Allow the parameter values to be adapted to enforce defined constraints
             (e.g.: min, max).
         """
         for key in values:
@@ -480,15 +480,15 @@
                 raise Exception(f'The alias "{alias}" already exists. '
                                 f'It must be unique.')
 
     def _check_value_range(self, index, key, value, allow_adapt=False):
         max_value = self.parameters.loc[index, 'max']
         min_value = self.parameters.loc[index, 'min']
 
-        if type(min_value) != list:
+        if not isinstance(min_value, list):
             if max_value is not None and value > max_value:
                 if allow_adapt:
                     return max_value
                 raise Exception(f'The value {value} for the parameter "{key}" is above '
                                 f'the maximum threshold ({max_value}).')
             if min_value is not None and value < min_value:
                 if allow_adapt:
```

### Comparing `hydrobricks-0.4.9/python/src/hydrobricks/plotting.py` & `hydrobricks-0.5.0/python/src/hydrobricks/plotting.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.4.9/python/src/hydrobricks/preprocessing/catchment.py` & `hydrobricks-0.5.0/python/src/hydrobricks/preprocessing/catchment.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.4.9/python/src/hydrobricks/spotpy_setup.py` & `hydrobricks-0.5.0/python/src/hydrobricks/spotpy_setup.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.4.9/python/src/hydrobricks/time_series.py` & `hydrobricks-0.5.0/python/src/hydrobricks/time_series.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from datetime import datetime
-
 import pandas as pd
 from hydrobricks import utils
 
 
 class TimeSeries:
     """Class for generic time series data"""
 
@@ -27,15 +25,15 @@
             Format of the time
         content : dict
             Type of data and column name containing the data.
             Example: {'precipitation': 'Precipitation (mm)'}
         """
         file_content = pd.read_csv(
             path, parse_dates=[column_time],
-            date_parser=lambda x: datetime.strptime(x, time_format))
+            date_format=time_format)
 
         self.time = file_content[column_time]
 
         for col in content:
             self.data_name.append(col)
             self.data_raw.append(file_content[content[col]].to_numpy())
             self.data_spatialized.append(None)
```

### Comparing `hydrobricks-0.4.9/python/src/hydrobricks/utils.py` & `hydrobricks-0.5.0/python/src/hydrobricks/utils.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.4.9/setup.py` & `hydrobricks-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 
 class CMakeBuild(build_ext):
     def build_extension(self, ext):
         # To build the extension in debug mode.
         # self.debug = True
 
+        skip_conan = os.environ.get("SKIP_CONAN", 0)
+
         ext_dir = os.path.abspath(os.path.dirname(self.get_ext_fullpath(ext.name)))
 
         # Required for auto-detection & inclusion of auxiliary "native" libs
         if not ext_dir.endswith(os.path.sep):
             ext_dir += os.path.sep
 
         debug = int(os.environ.get("DEBUG", 0)) if self.debug is None else self.debug
@@ -97,28 +99,31 @@
             if hasattr(self, "parallel") and self.parallel:
                 build_args += [f"-j{self.parallel}"]
 
         build_temp = os.path.join(self.build_temp, ext.name)
         if not os.path.exists(build_temp):
             os.makedirs(build_temp)
 
+        if not skip_conan:
+            subprocess.check_call(["conan", "install", ext.source_dir, "-s", "build_type=Release",
+                                   "--build=missing", "-pr:b=default"], cwd=build_temp)
         subprocess.check_call(["cmake", ext.source_dir] + cmake_args, cwd=build_temp)
         subprocess.check_call(["cmake", "--build", "."] + build_args, cwd=build_temp)
 
 
 # Read the contents of the README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "python" / "README.md").read_text()
 
 # Setup
 setup(
     name="hydrobricks",
-    version="0.4.9",
+    version="0.5.0",
     author="Pascal Horton",
-    author_email="pascal.horton@giub.unibe",
+    author_email="pascal.horton@unibe.ch",
     description="A modular hydrological modelling framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     ext_modules=[CMakeExtension("_hydrobricks")],
     cmdclass={"build_ext": CMakeBuild},
     packages=['hydrobricks', 'hydrobricks.models', 'hydrobricks.preprocessing',
               'hydrobricks.behaviours'],
```

