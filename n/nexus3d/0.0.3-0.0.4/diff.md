# Comparing `tmp/nexus3d-0.0.3.tar.gz` & `tmp/nexus3d-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus3d-0.0.3.tar", last modified: Fri Jun 30 16:51:21 2023, max compression
+gzip compressed data, was "nexus3d-0.0.4.tar", last modified: Thu Jul  6 11:43:49 2023, max compression
```

## Comparing `nexus3d-0.0.3.tar` & `nexus3d-0.0.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.980065 nexus3d-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.968065 nexus3d-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.972066 nexus3d-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-30 16:51:06.000000 nexus3d-0.0.3/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-30 16:51:06.000000 nexus3d-0.0.3/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-30 16:51:06.000000 nexus3d-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-30 16:51:06.000000 nexus3d-0.0.3/.github/workflows/static.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-30 16:51:06.000000 nexus3d-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-30 16:51:06.000000 nexus3d-0.0.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-06-30 16:51:06.000000 nexus3d-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17997 2023-06-30 16:51:21.980065 nexus3d-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-06-30 16:51:06.000000 nexus3d-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-30 16:51:06.000000 nexus3d-0.0.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.972066 nexus3d-0.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-30 16:51:06.000000 nexus3d-0.0.3/examples/gltf_test_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.972066 nexus3d-0.0.3/examples/threejs/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-30 16:51:06.000000 nexus3d-0.0.3/examples/threejs/experiment.glb
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-30 16:51:06.000000 nexus3d-0.0.3/examples/threejs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-30 16:51:06.000000 nexus3d-0.0.3/examples/threejs/main.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.976065 nexus3d-0.0.3/nexus3d/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/coordinate_systems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.976065 nexus3d-0.0.3/nexus3d/formats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/formats/gltf_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/formats/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/formats/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/formats/stl_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/nexus_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.976065 nexus3d-0.0.3/nexus3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17997 2023-06-30 16:51:21.000000 nexus3d-0.0.3/nexus3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-30 16:51:21.000000 nexus3d-0.0.3/nexus3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:51:21.000000 nexus3d-0.0.3/nexus3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 16:51:21.000000 nexus3d-0.0.3/nexus3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-30 16:51:21.000000 nexus3d-0.0.3/nexus3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 16:51:21.000000 nexus3d-0.0.3/nexus3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-30 16:51:06.000000 nexus3d-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.976065 nexus3d-0.0.3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-06-30 16:51:06.000000 nexus3d-0.0.3/scripts/create_example_glb.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      194 2023-06-30 16:51:06.000000 nexus3d-0.0.3/scripts/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:51:21.980065 nexus3d-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.980065 nexus3d-0.0.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.980065 nexus3d-0.0.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    58888 2023-06-30 16:51:06.000000 nexus3d-0.0.3/tests/data/transformation_example.h5
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-30 16:51:06.000000 nexus3d-0.0.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-30 16:51:06.000000 nexus3d-0.0.3/tests/test_stl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-30 16:51:06.000000 nexus3d-0.0.3/tests/test_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:43:49.686356 nexus3d-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:43:49.678356 nexus3d-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:43:49.682355 nexus3d-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-06 11:43:36.000000 nexus3d-0.0.4/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-06 11:43:36.000000 nexus3d-0.0.4/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-06 11:43:36.000000 nexus3d-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-06 11:43:36.000000 nexus3d-0.0.4/.github/workflows/static.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-06 11:43:36.000000 nexus3d-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-06 11:43:36.000000 nexus3d-0.0.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-06 11:43:36.000000 nexus3d-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17996 2023-07-06 11:43:49.686356 nexus3d-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-06 11:43:36.000000 nexus3d-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-06 11:43:36.000000 nexus3d-0.0.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:43:49.682355 nexus3d-0.0.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-06 11:43:36.000000 nexus3d-0.0.4/examples/gltf_test_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:43:49.682355 nexus3d-0.0.4/examples/threejs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-06 11:43:36.000000 nexus3d-0.0.4/examples/threejs/experiment.glb
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-06 11:43:36.000000 nexus3d-0.0.4/examples/threejs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-06 11:43:36.000000 nexus3d-0.0.4/examples/threejs/main.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:43:49.682355 nexus3d-0.0.4/nexus3d/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:43:36.000000 nexus3d-0.0.4/nexus3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-06 11:43:36.000000 nexus3d-0.0.4/nexus3d/coordinate_systems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:43:49.682355 nexus3d-0.0.4/nexus3d/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:43:36.000000 nexus3d-0.0.4/nexus3d/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-07-06 11:43:36.000000 nexus3d-0.0.4/nexus3d/formats/gltf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-06 11:43:36.000000 nexus3d-0.0.4/nexus3d/formats/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-06 11:43:36.000000 nexus3d-0.0.4/nexus3d/formats/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-06 11:43:36.000000 nexus3d-0.0.4/nexus3d/formats/stl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-06 11:43:36.000000 nexus3d-0.0.4/nexus3d/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-07-06 11:43:36.000000 nexus3d-0.0.4/nexus3d/nexus_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-06 11:43:36.000000 nexus3d-0.0.4/nexus3d/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:43:49.682355 nexus3d-0.0.4/nexus3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17996 2023-07-06 11:43:49.000000 nexus3d-0.0.4/nexus3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-06 11:43:49.000000 nexus3d-0.0.4/nexus3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:43:49.000000 nexus3d-0.0.4/nexus3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-06 11:43:49.000000 nexus3d-0.0.4/nexus3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 11:43:49.000000 nexus3d-0.0.4/nexus3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 11:43:49.000000 nexus3d-0.0.4/nexus3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-06 11:43:36.000000 nexus3d-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:43:49.686356 nexus3d-0.0.4/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      106 2023-07-06 11:43:36.000000 nexus3d-0.0.4/scripts/create_example_glb.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      194 2023-07-06 11:43:36.000000 nexus3d-0.0.4/scripts/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:43:49.686356 nexus3d-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:43:49.686356 nexus3d-0.0.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:43:49.686356 nexus3d-0.0.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    58888 2023-07-06 11:43:36.000000 nexus3d-0.0.4/tests/data/transformation_example.h5
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-06 11:43:36.000000 nexus3d-0.0.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-06 11:43:36.000000 nexus3d-0.0.4/tests/test_stl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-07-06 11:43:36.000000 nexus3d-0.0.4/tests/test_transformations.py
```

### Comparing `nexus3d-0.0.3/.github/workflows/pylint.yml` & `nexus3d-0.0.4/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/.github/workflows/pytest.yml` & `nexus3d-0.0.4/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/.github/workflows/python-publish.yml` & `nexus3d-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/.github/workflows/static.yml` & `nexus3d-0.0.4/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/.gitignore` & `nexus3d-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/LICENSE` & `nexus3d-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/PKG-INFO` & `nexus3d-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus3d
-Version: 0.0.3
+Version: 0.0.4
 Summary: Convert NXtransformation matrices inside a nexus file to 3D file formats
 Author-email: Florian Dobener <florian.dobener@physik.hu-berlin.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -222,16 +222,16 @@
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nexus3d)
 [![PyPI](https://img.shields.io/pypi/v/nexus3d)](https://pypi.org/project/nexus3d/)
 [![Pytest](https://github.com/domna/nexus3d/actions/workflows/pytest.yml/badge.svg)](https://github.com/domna/nexus3d/actions/workflows/pytest.yml)
 
 # Scope
 
-This is a project for reading out NX*TRANSFORMATION matrices from nexus files and
-visualizing them by creating a 3D representation file ([stl](<https://en.wikipedia.org/wiki/STL*(file_format)>) or [gltf/glb](https://en.wikipedia.org/wiki/GlTF) - we recommend using `glb`) which may be imported into 3D visualization software (e.g. blender). It is possible to load CAD drawings from stl files to visualize your experiment with it. For glb files you can easily visualize it in the web with three.js (see the [example](https://github.com/domna/nexus3d/tree/main/examples/threejs))
+This is a project for reading out NXtransformation matrices from nexus files and
+visualizing them by creating a 3D representation file ([stl](<https://en.wikipedia.org/wiki/STL_(file_format)>) or [gltf/glb](https://en.wikipedia.org/wiki/GlTF) - we recommend using `glb`) which may be imported into 3D visualization software (e.g. blender). It is possible to load CAD drawings from stl files to visualize your experiment with it. For glb files you can easily visualize it in the web with three.js (see the [example](https://github.com/domna/nexus3d/tree/main/examples/threejs))
 
 # Install
 
 The easiest way to install is with pip
 
 ```
 pip install nexus3d
```

### Comparing `nexus3d-0.0.3/README.md` & `nexus3d-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nexus3d)
 [![PyPI](https://img.shields.io/pypi/v/nexus3d)](https://pypi.org/project/nexus3d/)
 [![Pytest](https://github.com/domna/nexus3d/actions/workflows/pytest.yml/badge.svg)](https://github.com/domna/nexus3d/actions/workflows/pytest.yml)
 
 # Scope
 
-This is a project for reading out NX*TRANSFORMATION matrices from nexus files and
-visualizing them by creating a 3D representation file ([stl](<https://en.wikipedia.org/wiki/STL*(file_format)>) or [gltf/glb](https://en.wikipedia.org/wiki/GlTF) - we recommend using `glb`) which may be imported into 3D visualization software (e.g. blender). It is possible to load CAD drawings from stl files to visualize your experiment with it. For glb files you can easily visualize it in the web with three.js (see the [example](https://github.com/domna/nexus3d/tree/main/examples/threejs))
+This is a project for reading out NXtransformation matrices from nexus files and
+visualizing them by creating a 3D representation file ([stl](<https://en.wikipedia.org/wiki/STL_(file_format)>) or [gltf/glb](https://en.wikipedia.org/wiki/GlTF) - we recommend using `glb`) which may be imported into 3D visualization software (e.g. blender). It is possible to load CAD drawings from stl files to visualize your experiment with it. For glb files you can easily visualize it in the web with three.js (see the [example](https://github.com/domna/nexus3d/tree/main/examples/threejs))
 
 # Install
 
 The easiest way to install is with pip
 
 ```
 pip install nexus3d
```

### Comparing `nexus3d-0.0.3/dev-requirements.txt` & `nexus3d-0.0.4/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/examples/gltf_test_files.py` & `nexus3d-0.0.4/examples/gltf_test_files.py`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/examples/threejs/experiment.glb` & `nexus3d-0.0.4/examples/threejs/experiment.glb`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/examples/threejs/index.html` & `nexus3d-0.0.4/examples/threejs/index.html`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/examples/threejs/main.css` & `nexus3d-0.0.4/examples/threejs/main.css`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/nexus3d/coordinate_systems.py` & `nexus3d-0.0.4/nexus3d/coordinate_systems.py`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/nexus3d/formats/gltf_writer.py` & `nexus3d-0.0.4/nexus3d/formats/gltf_writer.py`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/nexus3d/formats/interfaces.py` & `nexus3d-0.0.4/nexus3d/formats/interfaces.py`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/nexus3d/formats/mesh.py` & `nexus3d-0.0.4/nexus3d/formats/mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,24 +59,24 @@
         (np.ndarray, np.ndarray): The points and triangles array of the cone.
     """
     aspect_ratio = 2
     vertices = (
         np.array(
             [
                 [0, 0, 0],
-                [-1.3, 0, aspect_ratio],
-                [-0.809017, -0.587785, aspect_ratio],
-                [-0.309017, -0.951057, aspect_ratio],
-                [0.309017, -0.951057, aspect_ratio],
-                [0.809017, -0.587785, aspect_ratio],
-                [1.3, 0, aspect_ratio],
-                [0.809017, 0.587785, aspect_ratio],
-                [0.309017, 0.951057, aspect_ratio],
-                [-0.309017, 0.951057, aspect_ratio],
-                [-0.809017, 0.587785, aspect_ratio],
+                [-1.3, 0, -aspect_ratio],
+                [-0.809017, -0.587785, -aspect_ratio],
+                [-0.309017, -0.951057, -aspect_ratio],
+                [0.309017, -0.951057, -aspect_ratio],
+                [0.809017, -0.587785, -aspect_ratio],
+                [1.3, 0, -aspect_ratio],
+                [0.809017, 0.587785, -aspect_ratio],
+                [0.309017, 0.951057, -aspect_ratio],
+                [-0.309017, 0.951057, -aspect_ratio],
+                [-0.809017, 0.587785, -aspect_ratio],
             ],
             dtype="float32",
         )
         / aspect_ratio
     )
 
     indices = np.array(
```

### Comparing `nexus3d-0.0.3/nexus3d/formats/stl_writer.py` & `nexus3d-0.0.4/nexus3d/formats/stl_writer.py`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/nexus3d/matrix.py` & `nexus3d-0.0.4/nexus3d/matrix.py`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/nexus3d/nexus_transformations.py` & `nexus3d-0.0.4/nexus3d/nexus_transformations.py`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/nexus3d.egg-info/PKG-INFO` & `nexus3d-0.0.4/nexus3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus3d
-Version: 0.0.3
+Version: 0.0.4
 Summary: Convert NXtransformation matrices inside a nexus file to 3D file formats
 Author-email: Florian Dobener <florian.dobener@physik.hu-berlin.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -222,16 +222,16 @@
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nexus3d)
 [![PyPI](https://img.shields.io/pypi/v/nexus3d)](https://pypi.org/project/nexus3d/)
 [![Pytest](https://github.com/domna/nexus3d/actions/workflows/pytest.yml/badge.svg)](https://github.com/domna/nexus3d/actions/workflows/pytest.yml)
 
 # Scope
 
-This is a project for reading out NX*TRANSFORMATION matrices from nexus files and
-visualizing them by creating a 3D representation file ([stl](<https://en.wikipedia.org/wiki/STL*(file_format)>) or [gltf/glb](https://en.wikipedia.org/wiki/GlTF) - we recommend using `glb`) which may be imported into 3D visualization software (e.g. blender). It is possible to load CAD drawings from stl files to visualize your experiment with it. For glb files you can easily visualize it in the web with three.js (see the [example](https://github.com/domna/nexus3d/tree/main/examples/threejs))
+This is a project for reading out NXtransformation matrices from nexus files and
+visualizing them by creating a 3D representation file ([stl](<https://en.wikipedia.org/wiki/STL_(file_format)>) or [gltf/glb](https://en.wikipedia.org/wiki/GlTF) - we recommend using `glb`) which may be imported into 3D visualization software (e.g. blender). It is possible to load CAD drawings from stl files to visualize your experiment with it. For glb files you can easily visualize it in the web with three.js (see the [example](https://github.com/domna/nexus3d/tree/main/examples/threejs))
 
 # Install
 
 The easiest way to install is with pip
 
 ```
 pip install nexus3d
```

### Comparing `nexus3d-0.0.3/nexus3d.egg-info/SOURCES.txt` & `nexus3d-0.0.4/nexus3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/pyproject.toml` & `nexus3d-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/tests/data/transformation_example.h5` & `nexus3d-0.0.4/tests/data/transformation_example.h5`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/tests/test_cli.py` & `nexus3d-0.0.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/tests/test_stl.py` & `nexus3d-0.0.4/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.3/tests/test_transformations.py` & `nexus3d-0.0.4/tests/test_transformations.py`

 * *Files identical despite different names*

