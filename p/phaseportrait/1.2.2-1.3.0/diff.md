# Comparing `tmp/phaseportrait-1.2.2.tar.gz` & `tmp/phaseportrait-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phaseportrait-1.2.2.tar", last modified: Wed Apr 19 19:17:12 2023, max compression
+gzip compressed data, was "phaseportrait-1.3.0.tar", last modified: Thu Jul  6 16:16:00 2023, max compression
```

## Comparing `phaseportrait-1.2.2.tar` & `phaseportrait-1.3.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:17:12.145978 phaseportrait-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-04-19 19:17:12.145978 phaseportrait-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/README_no_imgs.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:17:12.129977 phaseportrait-1.2.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:17:12.137977 phaseportrait-1.2.2/examples/api_examples/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/examples/api_examples/phaseportrait2d_example.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:17:12.141978 phaseportrait-1.2.2/phaseportrait/
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/Cobweb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/Map1D.py
--rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/PhasePortrait2D.py
--rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/PhasePortrait3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/PhasePortraitManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/Trajectories2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/Trajectories3D.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:17:12.141978 phaseportrait-1.2.2/phaseportrait/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:17:12.141978 phaseportrait-1.2.2/phaseportrait/generators_base/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/generators_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/generators_base/generator_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:17:12.141978 phaseportrait-1.2.2/phaseportrait/maps/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/maps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/maps/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:17:12.145978 phaseportrait-1.2.2/phaseportrait/nullclines/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/nullclines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/nullclines/nullclines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:17:12.145978 phaseportrait-1.2.2/phaseportrait/sliders/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/sliders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/sliders/sliders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:17:12.145978 phaseportrait-1.2.2/phaseportrait/streamlines/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/streamlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/streamlines/size_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/streamlines/streamlines_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/streamlines/velocity_color_gradient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:17:12.145978 phaseportrait-1.2.2/phaseportrait/trajectories/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/trajectories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/trajectories/rungekutta.py
--rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/trajectories/trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:17:12.145978 phaseportrait-1.2.2/phaseportrait/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/utils/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/phaseportrait/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:17:12.141978 phaseportrait-1.2.2/phaseportrait.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-04-19 19:17:12.000000 phaseportrait-1.2.2/phaseportrait.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-19 19:17:12.000000 phaseportrait-1.2.2/phaseportrait.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:17:12.000000 phaseportrait-1.2.2/phaseportrait.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 19:17:12.000000 phaseportrait-1.2.2/phaseportrait.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 19:17:12.000000 phaseportrait-1.2.2/phaseportrait.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 19:17:12.149978 phaseportrait-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-19 19:17:00.000000 phaseportrait-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:15:59.996407 phaseportrait-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-06 16:15:59.996407 phaseportrait-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/README_no_imgs.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:15:59.988407 phaseportrait-1.3.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:15:59.992407 phaseportrait-1.3.0/examples/api_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/examples/api_examples/phaseportrait2d_example.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:15:59.992407 phaseportrait-1.3.0/phaseportrait/
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/Cobweb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/Map1D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/PhasePortrait2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/PhasePortrait3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/PhasePortraitManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/Trajectories2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/Trajectories3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:15:59.992407 phaseportrait-1.3.0/phaseportrait/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:15:59.992407 phaseportrait-1.3.0/phaseportrait/generators_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/generators_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/generators_base/generator_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:15:59.992407 phaseportrait-1.3.0/phaseportrait/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/maps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/maps/map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:15:59.996407 phaseportrait-1.3.0/phaseportrait/nullclines/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/nullclines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/nullclines/nullclines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:15:59.996407 phaseportrait-1.3.0/phaseportrait/sliders/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/sliders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/sliders/sliders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:15:59.996407 phaseportrait-1.3.0/phaseportrait/streamlines/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/streamlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/streamlines/size_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14067 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/streamlines/streamlines_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/streamlines/velocity_color_gradient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:15:59.996407 phaseportrait-1.3.0/phaseportrait/trajectories/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/trajectories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/trajectories/rungekutta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/trajectories/trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:15:59.996407 phaseportrait-1.3.0/phaseportrait/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/utils/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/phaseportrait/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:15:59.992407 phaseportrait-1.3.0/phaseportrait.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-06 16:15:59.000000 phaseportrait-1.3.0/phaseportrait.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-06 16:15:59.000000 phaseportrait-1.3.0/phaseportrait.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:15:59.000000 phaseportrait-1.3.0/phaseportrait.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 16:15:59.000000 phaseportrait-1.3.0/phaseportrait.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 16:15:59.000000 phaseportrait-1.3.0/phaseportrait.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 16:15:59.996407 phaseportrait-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-06 16:15:43.000000 phaseportrait-1.3.0/setup.py
```

### Comparing `phaseportrait-1.2.2/LICENSE` & `phaseportrait-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/PKG-INFO` & `phaseportrait-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phaseportrait
-Version: 1.2.2
+Version: 1.3.0
 Summary: A python package for visualizing non-linear dynamics and chaos. (2D phase portraits, 3D chaotic trajectories, Maps, Cobweb plots...)
 Author-email: Víctor Loras <vhloras@gmail.com>, Unai Lería <unaileria@gmail.com>
 Maintainer-email: Víctor Loras <vhloras@gmail.com>, Unai Lería <unaileria@gmail.com>
 License: MIT license
 Project-URL: Documentation, https://phaseportrait.github.io/
 Project-URL: GitHub, https://github.com/phaseportrait/phaseportrait
 Project-URL: GUI, https://github.com/phaseportrait/phaseportrait-gui
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phaseportrait Version: 1.2.2 Summary: A python
+Metadata-Version: 2.1 Name: phaseportrait Version: 1.3.0 Summary: A python
 package for visualizing non-linear dynamics and chaos. (2D phase portraits, 3D
 chaotic trajectories, Maps, Cobweb plots...) Author-email: VÃ­ctor Loras
 gmail.com>, Unai LerÃ­a
 gmail.com> Maintainer-email: VÃ­ctor Loras
 gmail.com>, Unai LerÃ­a
 gmail.com> License: MIT license Project-URL: Documentation, https://
 phaseportrait.github.io/ Project-URL: GitHub, https://github.com/phaseportrait/
```

### Comparing `phaseportrait-1.2.2/README.md` & `phaseportrait-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/README_no_imgs.md` & `phaseportrait-1.3.0/README_no_imgs.md`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/phaseportrait/Cobweb.py` & `phaseportrait-1.3.0/phaseportrait/Cobweb.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/phaseportrait/Map1D.py` & `phaseportrait-1.3.0/phaseportrait/Map1D.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/phaseportrait/PhasePortrait2D.py` & `phaseportrait-1.3.0/phaseportrait/PhasePortrait2D.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/phaseportrait/PhasePortrait3D.py` & `phaseportrait-1.3.0/phaseportrait/PhasePortrait3D.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/phaseportrait/PhasePortraitManager.py` & `phaseportrait-1.3.0/phaseportrait/PhasePortraitManager.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/phaseportrait/Trajectories2D.py` & `phaseportrait-1.3.0/phaseportrait/Trajectories2D.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,33 +55,37 @@
             'Z': figZ,
         }
         self.ax = {
             'Z': axZ,
         }
 
 
-    def _plot_lines(self, val, vel, val_init, *, cnorm=None):
-        label = f"({','.join(tuple(map(str, val_init)))})"
-
+    def _plot_lines(self, val, vel, val_init, *, color=None, cnorm=None):
         val_ = val.T.reshape(-1, 1, 2)
         segments = np.concatenate([val_[:-1], val_[1:]], axis=1)
 
-        vel_ = np.sqrt(np.sum(np.square(vel), axis=0))
-        if cnorm is None:
-            cnorm = Normalize(vel_.min(), vel_.max())
-        C = plt.get_cmap(self.color)(cnorm(vel_))
+        if color is None:
+            vel_ = np.sqrt(np.sum(np.square(vel), axis=0))
+            if cnorm is None:
+                cnorm = Normalize(vel_.min(), vel_.max())
+            C = plt.get_cmap(self.color)(cnorm(vel_))
+        else:
+            C = color
         
-        linez = LineCollection(segments[:,:,(0,1)], linewidth=self.size, color=C, label=label)
+        linez = LineCollection(segments[:,:,(0,1)], linewidth=self.size, color=C)
         self.ax['Z'].add_collection(linez)
-        self.ax['Z'].plot([val_init[0],val[0,0]], [val_init[1], val[1,0]], '-', linewidth=self.size, color=C[0], zorder=-1)
+        if isinstance(C, list):
+            C = C[0]
+        self.ax['Z'].plot([val_init[0],val[0,0]], [val_init[1], val[1,0]], '-', linewidth=self.size, color=C, zorder=-1)
         # self.ax['Z'].plot(val[0,1:], val[1,1:], label=f"({','.join(tuple(map(str, val_init)))})")
 
 
     def _scatter_start_point(self, val_init):
-        self.ax['Z'].scatter(val_init[0], val_init[1], s=self.size+1, c=[0])
+        label = f"({','.join(tuple(map(str, val_init)))})"
+        self.ax['Z'].scatter(val_init[0], val_init[1], s=self.size*2, label=label)
 
 
     def _scatter_trajectory(self, val, color, cmap):
         self.ax['Z'].scatter(val[0,:], val[1,:], s=self.size, c=color, cmap=cmap)
 
 
     def _prepare_plot(self, grid=False):
```

### Comparing `phaseportrait-1.2.2/phaseportrait/Trajectories3D.py` & `phaseportrait-1.3.0/phaseportrait/Trajectories3D.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,55 +67,58 @@
             'X': axX,
             'Y': axY,
             'Z': axZ,
             '3d': ax3d
         }
 
 
-    def _plot_lines(self, val, vel, val_init, *, cnorm=None):
-        label = f"({','.join(tuple(map(str, val_init)))})"
-
+    def _plot_lines(self, val, vel, val_init, *, color=None, cnorm=None):
         val_ = val.T.reshape(-1, 1, 3)
         segments = np.concatenate([val_[:-1], val_[1:]], axis=1)
 
-        vel_ = np.sqrt(np.sum(np.square(vel), axis=0))
-        if cnorm is None:
-            cnorm = Normalize(vel_.min(), vel_.max())
-        C = plt.get_cmap(self.color)(cnorm(vel_))
-        line3d = Line3DCollection(segments, linewidth=self.size, color=C, label=label)
-        linex = LineCollection(segments[:,:,(1,2)], linewidth=self.size, color=C, label=label)
-        liney = LineCollection(segments[:,:,(0,2)], linewidth=self.size, color=C, label=label)
-        linez = LineCollection(segments[:,:,(0,1)], linewidth=self.size, color=C, label=label)
+        if color is None:
+            vel_ = np.sqrt(np.sum(np.square(vel), axis=0))
+            if cnorm is None:
+                cnorm = Normalize(vel_.min(), vel_.max())
+            C = plt.get_cmap(self.color)(cnorm(vel_))
+        else:
+            C = color
+        line3d = Line3DCollection(segments, linewidth=self.size, color=C)
+        linex = LineCollection(segments[:,:,(1,2)], linewidth=self.size, color=C)
+        liney = LineCollection(segments[:,:,(0,2)], linewidth=self.size, color=C)
+        linez = LineCollection(segments[:,:,(0,1)], linewidth=self.size, color=C)
 
         
 
         self.ax['3d'].add_collection(line3d)
         self.ax['X'].add_collection(linex)
         self.ax['Y'].add_collection(liney)
         self.ax['Z'].add_collection(linez)
 
 
-
-        self.ax['3d'].plot(*[[val_init[i],val[i,0]] for i in range(3)], '-', linewidth=self.size, color=C[0])
-        self.ax['X'].plot([val_init[1],val[1,0]], [val_init[2], val[2,0]], '-', linewidth=self.size, color=C[0], zorder=-1)
-        self.ax['Y'].plot([val_init[0],val[0,0]], [val_init[2], val[2,0]], '-', linewidth=self.size, color=C[0], zorder=-1)
-        self.ax['Z'].plot([val_init[0],val[0,0]], [val_init[1], val[1,0]], '-', linewidth=self.size, color=C[0], zorder=-1)
+        if isinstance(C, list): 
+            C = C[0]
+        self.ax['3d'].plot(*[[val_init[i],val[i,0]] for i in range(3)], '-', linewidth=self.size, color=C)
+        self.ax['X'].plot([val_init[1],val[1,0]], [val_init[2], val[2,0]], '-', linewidth=self.size, color=C, zorder=-1)
+        self.ax['Y'].plot([val_init[0],val[0,0]], [val_init[2], val[2,0]], '-', linewidth=self.size, color=C, zorder=-1)
+        self.ax['Z'].plot([val_init[0],val[0,0]], [val_init[1], val[1,0]], '-', linewidth=self.size, color=C, zorder=-1)
         self._update_3d_lims()
 
     def _update_3d_lims(self):
         self.ax['3d'].set_xlim(self.ax['Y'].get_xlim())
         self.ax['3d'].set_ylim(self.ax['Z'].get_xlim())
         self.ax['3d'].set_zlim(self.ax['X'].get_ylim())
 
 
     def _scatter_start_point(self, val_init):
-        self.ax['3d'].scatter3D(*val_init, s=self.size*2, c=[0])
-        self.ax['X'].scatter(val_init[1], val_init[2], s=self.size*2, c=[0])
-        self.ax['Y'].scatter(val_init[0], val_init[2], s=self.size*2, c=[0])
-        self.ax['Z'].scatter(val_init[0], val_init[1], s=self.size*2, c=[0])
+        label = f"({','.join(tuple(map(str, val_init)))})"
+        self.ax['3d'].scatter3D(*val_init, s=self.size*2, label=label)
+        self.ax['X'].scatter(val_init[1], val_init[2], s=self.size*2, label=label)
+        self.ax['Y'].scatter(val_init[0], val_init[2], s=self.size*2, label=label)
+        self.ax['Z'].scatter(val_init[0], val_init[1], s=self.size*2, label=label)
 
 
     def _scatter_trajectory(self, val, color, cmap):
         self.ax['3d'].scatter3D(*val, s=self.size, c=color, cmap=cmap)
         self.ax['X'].scatter(val[1,:], val[2,:], s=self.size, c=color, cmap=cmap)
         self.ax['Y'].scatter(val[0,:], val[2,:], s=self.size, c=color, cmap=cmap)
         self.ax['Z'].scatter(val[0,:], val[1,:], s=self.size, c=color, cmap=cmap)
```

### Comparing `phaseportrait-1.2.2/phaseportrait/exceptions/exceptions.py` & `phaseportrait-1.3.0/phaseportrait/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/phaseportrait/generators_base/generator_base.py` & `phaseportrait-1.3.0/phaseportrait/generators_base/generator_base.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/phaseportrait/maps/map.py` & `phaseportrait-1.3.0/phaseportrait/maps/map.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/phaseportrait/nullclines/nullclines.py` & `phaseportrait-1.3.0/phaseportrait/nullclines/nullclines.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/phaseportrait/sliders/sliders.py` & `phaseportrait-1.3.0/phaseportrait/sliders/sliders.py`

 * *Files 20% similar despite different names*

```diff
@@ -64,24 +64,40 @@
         
         Arguments
         ---------
         value : float
             New value for the parameter of the slider
         """
         
-        try:
-            self.portrait.ax.cla()
-        except:
-            for ax in self.portrait.ax.values():
-                ax.cla()
+        ax = self.portrait.ax 
+        if isinstance(ax, dict):
+            legend = {}
+            for k in ax.keys():
+                legend.update({k: ax[k].get_legend()})
+            
+        else:
+            legend = ax.get_legend()
+            
+        if isinstance(ax, dict):
+            for k in ax.keys():
+                ax[k].cla()
+        else:
+            ax.cla()
+
         self.value = value
 
         if 'Cobweb' in self.portrait._name_:
             self.portrait.update_dF_args()
 
+        if isinstance(ax, dict):
+            for k in ax.keys():
+                ax[k].legend_ = legend[k]
+        else:
+            ax.legend_ = legend
+        
         self.portrait.plot()
         
     def update_slider_ends(self, valmin, valmax):
         """
         Updates slider min and max values
 
         Parameters
```

### Comparing `phaseportrait-1.2.2/phaseportrait/streamlines/size_gradient.py` & `phaseportrait-1.3.0/phaseportrait/streamlines/size_gradient.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/phaseportrait/streamlines/streamlines_base.py` & `phaseportrait-1.3.0/phaseportrait/streamlines/streamlines_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,28 +21,40 @@
         elif odeint_method == "rungekutta3":
             self._integration_method = self._runge_kutta_3rd_odeint
         else:
             raise NameError(f"Integration method {odeint_method} is not in [scipy, euler or rungekutta3]")
     
     def _makeStreamline(self, y0):
         """
-        Compute a streamline extending in both directions from the given point. Using Euler integrator.
+        Compute a streamline extending in both directions from the given point.
         """
-        *s, svelocity = self._makeHalfStreamline(y0, 1)  # forwards
-        *r, rvelocity = self._makeHalfStreamline(y0, -1)  # backwards
-
-        for _r in r:
-            _r.reverse()
-        rvelocity.reverse()
-
+        
+        s, svelocity, i_f = self._makeHalfStreamline(y0, 1)  # forwards
+        r, rvelocity, i_b = self._makeHalfStreamline(y0, -1)  # backwards
+        
         speed = self._speed(y0)
-        if np.isnan(speed).any() or np.isinf(speed).any():
+        
+        if np.isnan(speed).any() or np.isinf(speed).any() or i_b==0 or i_f==0:
             return None
+        
+        svelocity = svelocity[:i_f]
+        rvelocity_flip = np.flip(rvelocity[:i_b])
+        
+        speed = np.sqrt(np.sum(np.square(speed)))
+        
+        
+        if not np.isclose(svelocity[0], speed, rtol=100).all() or not np.isclose(rvelocity[0], speed, rtol=100).all():
+            return None
+        
+        s = s[:i_f]
+        r = np.flip(r[:i_b],0)
 
-        return *[r[i] + [y0[i]] + s[i] for i in range(len(y0))],  rvelocity + [np.sqrt(np.sum(np.square(speed)))] + svelocity
+        if not np.isclose(s[0], y0, rtol=100).all() or not np.isclose(r[0], y0, rtol=100).all():
+            return None
+        return np.concatenate((r, [y0], s), 0), np.concatenate((rvelocity_flip, [speed], svelocity))
     
     def _speed_2d_no_polar(self, y0, *args, **kargs):
         return np.array(self.dF(*y0, **self.dF_args))
     
     def _speed_2d_polar(self, y0, *args, **kargs):
         R, Theta = np.sqrt(np.sum(np.square(y0))), np.arctan2(y0[1], y0[0])
         dR, dTheta = self.dF(R, Theta, **self.dF_args)
@@ -65,23 +77,23 @@
         """
         Computes speed in given coordinates
         """
         ...
 
 
     def _scipy_odeint(self, coords, sign, deltat):
-        return integrate.odeint(self._speed, coords, [0.1*i*sign*deltat for i in range(4)])[-1]
+        return integrate.odeint(self._speed, coords, sign * np.arange(1,5)*0.2*deltat)[-1]
     
     def _euler_odeint(self, coords, sign, deltat):
         return coords + self._speed(coords) * deltat * sign
     
     def _runge_kutta_3rd_odeint(self, coords, sign, deltat):
         k1 = self._speed(coords)
-        k2 = self._speed(coords + sign*deltat*1/4*k1)
-        k3 = self._speed(coords + sign*deltat*(-1*k1 + 2*k2))
+        k2 = self._speed(coords + sign * deltat*1/4*k1)
+        k3 = self._speed(coords + sign * deltat*(-1*k1 + 2*k2))
         return coords + sign * deltat * ((k1+k3)/6 + 2/3*k2)
     
     def _integration_method(self, coords, sign, deltat):
         """Function responsible to integrate the function the given delta time
         """
         ...
 
@@ -94,64 +106,67 @@
         # coords_mask_position = np.asarray(np.rint((coords-self.range_min)/self.delta_coords), int)
         coords_mask_position = self.get_masked_coordinates(*coords)
 
         # Set prev_coords_mask_position to actual position so backwards trajectory can, at least, start
         prev_coords_mask_position = coords_mask_position.copy()
 
         # Save arrays
-        s = [[] for i in range(self.dimension)]
-        svelocity = []
+        s = np.zeros((int(self.maxLen / 2), self.dimension))
+        # s = [[] for i in range(self.dimension)]
+        svelocity = np.zeros((int(self.maxLen / 2)))
 
         i = 0
-        persistency = 0
+        persistency = 20
+        _speed = self._speed(coords)
 
         while (self.range_min < coords).all() and (coords < self.range_max).all():
-            if i > self.maxLen / 2:
+            if i >= int(self.maxLen / 2):
                 break
-            i += 1
+            
 
             coords_mask_position = self.get_masked_coordinates(*coords)
 
             # If mask is False there is not trajectory there yet.
             if not self.used[tuple(coords_mask_position,)]:
                 prev_coords_mask_position = coords_mask_position.copy()
 
                 self.used[tuple(prev_coords_mask_position)] = True
 
-            # Integration
-            _speed = self._speed(coords)
-            if (_speed == 0).all() or \
-                np.isnan(_speed).any() or \
-                np.isinf(_speed).any():
-                    break
+           
 
             # deltat = np.sum(np.square(self.get_delta_coordinates(*coords))) / (4 * _speed)
-            deltat = np.min(self.get_delta_coordinates(*coords)/(10*np.abs(_speed)))
+            deltat = np.min(self.get_delta_coordinates(*coords)/(10*np.max(np.abs(_speed))))
 
             if np.isnan(deltat) or np.isinf(deltat):
-                print(deltat, self.get_delta_coordinates(*coords), _speed)
+                break
 
-            new_coords = self._integration_method(coords, sign, deltat)
-            
-            mean_speed = np.sqrt(np.sum(np.square(new_coords-coords)))/deltat
-            coords = new_coords
+            coords = self._integration_method(coords, sign, deltat)
 
             # Save values
-            for c, coord in enumerate(coords):
-                s[c].append(coord)
-            svelocity.append(mean_speed)
+            s[i] = coords
+            svelocity[i] = np.sqrt(np.sum(np.square(_speed)))
 
 
             # If persistency iterations in a region with previous trajectory break.
             if self.used[tuple(coords_mask_position)] and (prev_coords_mask_position!=coords_mask_position).any():
                 persistency -= 1
                 if persistency <= 0:
                     break
+            
+            i += 1
+            
+             # Integration
+            _speed = self._speed(coords)
+            if (i%8 == 0):
+                if (np.isclose(0, _speed)).all() or \
+                    np.isnan(_speed).any() or \
+                    np.isinf(_speed).any():
+                        break
 
-        return *s, svelocity
+        return s, svelocity, i
 
 
 class Streamlines_base2D(Streamlines_base):
     """
     Streamlines2D
     --------
     Creates trajectories given a `dF` function. Using Euler integrator.
```

### Comparing `phaseportrait-1.2.2/phaseportrait/streamlines/velocity_color_gradient.py` & `phaseportrait-1.3.0/phaseportrait/streamlines/velocity_color_gradient.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,18 @@
 
     def _velocity_normalization(self):
         """ Returns a colour normalization function for colouring the stream lines. """
         vmax = None
         vmin = None
 
         for streamline in self.stream_base.streamlines:
-            *_, v = streamline
-            vmax = max(v + ([vmax] if vmax is not None else []))
-            vmin = min(v + ([vmin] if vmin is not None else []))
+            if streamline is not None:
+                *_, v = streamline
+                vmax = max(np.concatenate((v, ([vmax] if vmax is not None else []))))
+                vmin = min(np.concatenate((v, ([vmin] if vmin is not None else []))))
 
         return Normalize(vmin, vmax)
 
     def plot(self, ax, cmap, cnorm, *, linewidth=None, arrowsize=1, arrowstyle='-|>'):
         # n_segments = 0
         # for streamline in self.stream_base.streamlines:
         #     x, *_ = streamline
@@ -92,16 +93,20 @@
         if linewidth is None:
             linewidth = matplotlib.rcParams['lines.linewidth']
 
         line_kw = {}
         arrow_kw = dict(arrowstyle=arrowstyle, mutation_scale=10 * arrowsize)
 
         for streamline in self.stream_base.streamlines:
-            *coords, v = streamline
-            points = np.array(coords).T.reshape(-1 , 1, 2 if self.proyection=="2d" else 3)
+            if streamline is None:
+                continue
+            coords, v = streamline
+            if len(v) == 1:
+                continue
+            points = np.array(coords).reshape(-1 , 1, 2 if self.proyection=="2d" else 3)
             segments = np.concatenate([points[:-1], points[1:]], axis=1)
 
             s = np.sqrt(np.sum(np.square(points), 2))
             s = np.cumsum(s)
             n = np.searchsorted(s, s[-1] / 2.)
 
             arrows = []
```

### Comparing `phaseportrait-1.2.2/phaseportrait/trajectories/rungekutta.py` & `phaseportrait-1.3.0/phaseportrait/trajectories/rungekutta.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/phaseportrait/trajectories/trajectory.py` & `phaseportrait-1.3.0/phaseportrait/trajectories/trajectory.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,21 +89,21 @@
             self.thermalization = 0
         self.size = kargs.get('size')
         if not self.size:
             self.size = 0.5
         self.color = kargs.get('color')
         if self.color is None:
             self.color =  'viridis'
-        self._mark_start_point = kargs.get('mark_start_point')
+        self._mark_start_position = kargs.get('mark_start_position')
 
     # This functions must be overwriten on child classes:
     def _prepare_plot(self):...
     def _scatter_start_point(self, val_init):...
     def _scatter_trajectory(self, val, color, cmap):...
-    def _plot_lines(self, val, val_init):...
+    def _plot_lines(self, val, val_init, *, color=None):...
 
 
     # General functions
     def _create_sliders_plot(self):
         if not isinstance(self.sliders_fig, plt.Figure):
             self.sliders_fig, self.sliders_ax = plt.subplots() 
             self.sliders_ax.set_visible(False)
@@ -120,21 +120,24 @@
         """
         
         if self.thermalization is None:
             self.thermalization = thermalization_steps
         self.initial_position()
 
 
-    def initial_position(self, *args, **kargs):
+    def initial_position(self, *args, color=None, **kargs):
         """
         Adds a initial position for the computation.
         More than one can be added.
         
         Args:
             args (Union[float, list[2], list[3]], optional) : Initial position for the computation. If None, a random position is chosen.
+           
+        Kargs:
+            color (str|None): If a color is given it is used to plot that trajectory. If None the speed is used to color the line/dots. 
             
         Example:
         -------
         This example generates 2 circles with diferent radius. 
         ```
         def Circle(x,y,*, w=1, z=1):
             return w*y, -z*x
@@ -155,17 +158,22 @@
             for a, b in zip(args, trajectory.initial_value):
                 if a!=b:
                     flag = True
         
         if not flag and len(self.trajectories)>0:
             return
         
+        class coloredRungeKutta(RungeKutta):
+            def __init__(self, portrait, color, dF, dimension, max_values, *, dt=0.1, dF_args=None, initial_values=None, thermalization=0):
+                super().__init__(portrait, dF, dimension, max_values, dt=dt, dF_args=dF_args, initial_values=initial_values, thermalization=thermalization)
+                self.__color__ = color
+        
         self.trajectories.append(
-            RungeKutta(
-                self, self.dF, self._dimension, self.n_points, 
+            coloredRungeKutta(
+                self, color, self.dF, self._dimension, self.n_points, 
                 dt=self.runge_kutta_step,
                 dF_args=self.dF_args, 
                 initial_values=args,
                 thermalization=self.thermalization
                 )
             )
         
@@ -209,30 +217,25 @@
         self._prepare_plot(grid=grid)
         self.dF_args.update({name: slider.value for name, slider in self.sliders.items() if slider.value!= None})
         for trajectory in self.trajectories:
             trajectory.dF_args = self.dF_args
         
         self._calculate_values(all_initial_conditions=True)
 
-
-        # if self.color == 't':
-        #     cmap = color
-        # else:
-        #     cmap = self.color = color
         if color is not None:
             self.color = color
         cmap = self.color
 
         for trajectory in self.trajectories:
             val = trajectory.positions
             vel = trajectory.velocities
             val_init = trajectory.initial_value
             
             if self.lines:
-                self._plot_lines(val, vel, val_init)
+                self._plot_lines(val, vel, val_init, color=trajectory.__color__)
                     
             else:
                 def norma(v):
                     suma = 0
                     for i in range(self._dimension):
                         suma += np.nan_to_num(v[i]**2)
                     return np.sqrt(suma)
@@ -240,15 +243,15 @@
                     color = np.linspace(0,1, vel.shape[1])
                 else:
                     color = norma(vel[:])
                     color /= color.max()
 
                 self._scatter_trajectory(val, color, cmap)
 
-            if self._mark_start_point:
+            if self._mark_start_position:
                 self._scatter_start_point(val_init)
                 
         for fig in self.fig.values():
             if self.lines and labels:
                 fig.legend()
             fig.canvas.draw_idle()
         try:
```

### Comparing `phaseportrait-1.2.2/phaseportrait/utils/manager.py` & `phaseportrait-1.3.0/phaseportrait/utils/manager.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/phaseportrait/utils/utils.py` & `phaseportrait-1.3.0/phaseportrait/utils/utils.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/phaseportrait.egg-info/PKG-INFO` & `phaseportrait-1.3.0/phaseportrait.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phaseportrait
-Version: 1.2.2
+Version: 1.3.0
 Summary: A python package for visualizing non-linear dynamics and chaos. (2D phase portraits, 3D chaotic trajectories, Maps, Cobweb plots...)
 Author-email: Víctor Loras <vhloras@gmail.com>, Unai Lería <unaileria@gmail.com>
 Maintainer-email: Víctor Loras <vhloras@gmail.com>, Unai Lería <unaileria@gmail.com>
 License: MIT license
 Project-URL: Documentation, https://phaseportrait.github.io/
 Project-URL: GitHub, https://github.com/phaseportrait/phaseportrait
 Project-URL: GUI, https://github.com/phaseportrait/phaseportrait-gui
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phaseportrait Version: 1.2.2 Summary: A python
+Metadata-Version: 2.1 Name: phaseportrait Version: 1.3.0 Summary: A python
 package for visualizing non-linear dynamics and chaos. (2D phase portraits, 3D
 chaotic trajectories, Maps, Cobweb plots...) Author-email: VÃ­ctor Loras
 gmail.com>, Unai LerÃ­a
 gmail.com> Maintainer-email: VÃ­ctor Loras
 gmail.com>, Unai LerÃ­a
 gmail.com> License: MIT license Project-URL: Documentation, https://
 phaseportrait.github.io/ Project-URL: GitHub, https://github.com/phaseportrait/
```

### Comparing `phaseportrait-1.2.2/phaseportrait.egg-info/SOURCES.txt` & `phaseportrait-1.3.0/phaseportrait.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.2/pyproject.toml` & `phaseportrait-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 # Minimum requirements for the build system to execute.
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phaseportrait"
-version = "1.2.2"
+version = "1.3.0"
 requires-python = ">=3.8"
 
 description = "A python package for visualizing non-linear dynamics and chaos. (2D phase portraits, 3D chaotic trajectories, Maps, Cobweb plots...)"
 
 authors = [
     {name = "Víctor Loras"  , email = "vhloras@gmail.com"}, 
     {name =  "Unai Lería"   , email =  "unaileria@gmail.com"}]
@@ -37,8 +37,8 @@
     "Topic :: Scientific/Engineering :: Visualization"]
 
 dependencies = ['numpy', 'matplotlib', 'scipy']
 
 [project.urls]
 "Documentation" = "https://phaseportrait.github.io/"
 "GitHub" = "https://github.com/phaseportrait/phaseportrait"
-"GUI" = "https://github.com/phaseportrait/phaseportrait-gui"
+"GUI" = "https://github.com/phaseportrait/phaseportrait-gui"
```

