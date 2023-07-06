# Comparing `tmp/event_vision_library-0.0.1.tar.gz` & `tmp/event_vision_library-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event_vision_library-0.0.1.tar", max compression
+gzip compressed data, was "event_vision_library-0.0.1b0.tar", max compression
```

## Comparing `event_vision_library-0.0.1.tar` & `event_vision_library-0.0.1b0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1070 2023-05-12 10:25:25.998453 event_vision_library-0.0.1/LICENSE
--rw-r--r--   0        0        0     3435 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/README.md
--rw-r--r--   0        0        0     2800 2023-05-12 10:25:42.646519 event_vision_library-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      348 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/__init__.py
--rw-r--r--   0        0        0    23618 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/_version.py
--rw-r--r--   0        0        0       21 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/__init__.py
--rw-r--r--   0        0        0      265 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/block_access.py
--rw-r--r--   0        0        0      552 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/_block_access.py
--rw-r--r--   0        0        0      308 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/_iterator_access.py
--rw-r--r--   0        0        0     2485 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/aedat.py
--rw-r--r--   0        0        0     2712 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/conversion.py
--rw-r--r--   0        0        0      677 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/evk.py
--rw-r--r--   0        0        0     2307 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/hdf5.py
--rw-r--r--   0        0        0        0 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/npy.py
--rw-r--r--   0        0        0     3283 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/text.py
--rw-r--r--   0        0        0      274 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/iterator_access.py
--rw-r--r--   0        0        0      131 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/constant.py
--rw-r--r--   0        0        0       54 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/preproc/__init__.py
--rw-r--r--   0        0        0     1460 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/preproc/hot_pixel.py
--rw-r--r--   0        0        0       25 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/__init__.py
--rw-r--r--   0        0        0       90 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/__init__.py
--rw-r--r--   0        0        0     4673 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid.py
--rw-r--r--   0        0        0        0 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/__init__.py
--rw-r--r--   0        0        0      821 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/base_model.py
--rw-r--r--   0        0        0     3453 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/image_reconstructor.py
--rw-r--r--   0        0        0        0 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/model/__init__.py
--rw-r--r--   0        0        0     2971 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/model/model.py
--rw-r--r--   0        0        0     8677 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/model/submodules.py
--rw-r--r--   0        0        0     7788 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/model/unet.py
--rw-r--r--   0        0        0        0 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/utils/__init__.py
--rw-r--r--   0        0        0     7154 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/utils/inference_utils.py
--rw-r--r--   0        0        0      873 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/utils/loading_utils.py
--rw-r--r--   0        0        0        0 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/py.typed
--rw-r--r--   0        0        0      182 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/representation/__init__.py
--rw-r--r--   0        0        0     1820 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/representation/histogram.py
--rw-r--r--   0        0        0     1462 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/representation/time_map.py
--rw-r--r--   0        0        0     2235 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/representation/voxel_grid.py
--rw-r--r--   0        0        0      246 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/types/__init__.py
--rw-r--r--   0        0        0     1112 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/types/raw_event.py
--rw-r--r--   0        0        0     2159 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/types/raw_events.py
--rw-r--r--   0        0        0       33 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/utils/__init__.py
--rw-r--r--   0        0        0     1918 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/utils/basics.py
--rw-r--r--   0        0        0      638 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/version.py
--rw-r--r--   0        0        0       28 2023-05-12 10:25:26.006453 event_vision_library-0.0.1/src/evlib/vis/__init__.py
--rw-r--r--   0        0        0     3660 2023-05-12 10:25:26.006453 event_vision_library-0.0.1/src/evlib/vis/utils.py
--rw-r--r--   0        0        0     1872 2023-05-12 10:25:26.006453 event_vision_library-0.0.1/src/evlib/vis/view2d.py
--rw-r--r--   0        0        0     4958 1970-01-01 00:00:00.000000 event_vision_library-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/LICENSE
+-rw-r--r--   0        0        0     3595 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/README.md
+-rw-r--r--   0        0        0     2797 2023-07-06 06:51:54.441005 event_vision_library-0.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0      348 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/__init__.py
+-rw-r--r--   0        0        0    23618 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/_version.py
+-rw-r--r--   0        0        0       21 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/codec/__init__.py
+-rw-r--r--   0        0        0      265 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/codec/block_access.py
+-rw-r--r--   0        0        0      552 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/codec/fileformat/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/codec/fileformat/_block_access.py
+-rw-r--r--   0        0        0      308 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/codec/fileformat/_iterator_access.py
+-rw-r--r--   0        0        0     2485 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/codec/fileformat/aedat.py
+-rw-r--r--   0        0        0     2712 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/codec/fileformat/conversion.py
+-rw-r--r--   0        0        0      677 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/codec/fileformat/evk.py
+-rw-r--r--   0        0        0     2307 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/codec/fileformat/hdf5.py
+-rw-r--r--   0        0        0        0 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/codec/fileformat/npy.py
+-rw-r--r--   0        0        0     3283 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/codec/fileformat/text.py
+-rw-r--r--   0        0        0      274 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/codec/iterator_access.py
+-rw-r--r--   0        0        0      131 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/constant.py
+-rw-r--r--   0        0        0       54 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/preproc/__init__.py
+-rw-r--r--   0        0        0     1460 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/preproc/hot_pixel.py
+-rw-r--r--   0        0        0       25 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/processing/__init__.py
+-rw-r--r--   0        0        0       90 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/__init__.py
+-rw-r--r--   0        0        0     4673 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid.py
+-rw-r--r--   0        0        0        0 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/__init__.py
+-rw-r--r--   0        0        0      821 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/base_model.py
+-rw-r--r--   0        0        0     3453 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/image_reconstructor.py
+-rw-r--r--   0        0        0        0 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/model/__init__.py
+-rw-r--r--   0        0        0     2971 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/model/model.py
+-rw-r--r--   0        0        0     8677 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/model/submodules.py
+-rw-r--r--   0        0        0     7788 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/model/unet.py
+-rw-r--r--   0        0        0        0 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/utils/__init__.py
+-rw-r--r--   0        0        0     7154 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/utils/inference_utils.py
+-rw-r--r--   0        0        0      873 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/utils/loading_utils.py
+-rw-r--r--   0        0        0        0 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/py.typed
+-rw-r--r--   0        0        0      182 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/representation/__init__.py
+-rw-r--r--   0        0        0     1820 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/representation/histogram.py
+-rw-r--r--   0        0        0     1462 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/representation/time_map.py
+-rw-r--r--   0        0        0     2235 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/representation/voxel_grid.py
+-rw-r--r--   0        0        0      246 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/types/__init__.py
+-rw-r--r--   0        0        0     1112 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/types/raw_event.py
+-rw-r--r--   0        0        0     2159 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/types/raw_events.py
+-rw-r--r--   0        0        0       33 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/utils/__init__.py
+-rw-r--r--   0        0        0     1918 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/utils/basics.py
+-rw-r--r--   0        0        0      638 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/version.py
+-rw-r--r--   0        0        0       28 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/vis/__init__.py
+-rw-r--r--   0        0        0     3660 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/vis/utils.py
+-rw-r--r--   0        0        0     2643 2023-07-06 06:51:39.696817 event_vision_library-0.0.1b0/src/evlib/vis/view2d.py
+-rw-r--r--   0        0        0     5116 1970-01-01 00:00:00.000000 event_vision_library-0.0.1b0/PKG-INFO
```

### Comparing `event_vision_library-0.0.1/LICENSE` & `event_vision_library-0.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/README.md` & `event_vision_library-0.0.1b0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,33 @@
 [python version]: https://pypi.org/project/event-vision-library
 [read the docs]: https://event-vision-library.readthedocs.io/
 [tests]: https://github.com/shiba24/event-vision-library/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/shiba24/event-vision-library
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
+## Installation
+
+You can install _Event Vision Library_ via [pip] from [PyPI]:
+
+```console
+$ pip install event-vision-library
+
+# you can now `import evlib`
+```
+
+## Usage
+
+Please see our [examples] and [documentation][read the docs].
+
 ## Features
 
 - Python 3.7, 3.8, 3.9, 3.10
 - Pure-python library
+- Numpy and Torch compatibility.
 - 🚧 This library is under construction and currently alpha version. The APIs may change significantly. Contributions and discussions are welcomed! 🚧
 
 ### Data
 
 - [ ] Support different data types (.text, .raw, .hdf5, .npy, .aedat) for various file encoding of event data
 - [ ] ROS bag files (optional, based on ROS installation)
 - [ ] Support multiple existing dataset (e.g., ECD, MVSEC, DSEC, etc.)
@@ -44,26 +59,14 @@
 - [ ] C++ implementation and extension for faster execution (TODO)
 
 ### Log and Vsualization
 
 - [ ] Various visualization for 2D/3D representation of events
 - [ ] Useful logging
 
-## Installation
-
-You can install _Event Vision Library_ via [pip] from [PyPI]:
-
-```console
-$ pip install event-vision-library
-```
-
-## Usage
-
-Please see our examples and documentations.
-
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
 
@@ -82,10 +85,11 @@
 [pypi]: https://pypi.org/
 [hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
 [file an issue]: https://github.com/shiba24/event-vision-library/issues
 [pip]: https://pip.pypa.io/
 
 <!-- github-only -->
 
+[examples]: https://github.com/shiba24/event-vision-library/blob/main/examples
 [license]: https://github.com/shiba24/event-vision-library/blob/main/LICENSE
 [contributor guide]: https://github.com/shiba24/event-vision-library/blob/main/CONTRIBUTING.md
 [command-line reference]: https://event-vision-library.readthedocs.io/en/latest/usage.html
```

### Comparing `event_vision_library-0.0.1/pyproject.toml` & `event_vision_library-0.0.1b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "event-vision-library"
-version = "0.0.1"
+version = "0.0.1b"
 description = "Event Vision Library"
 authors = ["Shintaro Shiba <shiba.shintaro@gmail.com>", "Friedhelm Hamann <friedhelmha2@gmail.com>"]
 maintainers = [
     "Shintaro Shiba <shiba.shintaro@gmail.com>",
     "Friedhelm Hamann <friedhelmha2@gmail.com>",
 ]
 license = "MIT"
@@ -12,15 +12,15 @@
 homepage = "https://github.com/shiba24/event-vision-library"
 repository = "https://github.com/shiba24/event-vision-library"
 documentation = "https://event-vision-library.readthedocs.io"
 packages = [
     { include = "evlib", from = "src" },
 ]
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/shiba24/event-vision-library/releases"
 
 [tool.poetry.dependencies]
 python = "^3.7,<3.11"
```

### Comparing `event_vision_library-0.0.1/src/evlib/_version.py` & `event_vision_library-0.0.1b0/src/evlib/_version.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/codec/fileformat/__init__.py` & `event_vision_library-0.0.1b0/src/evlib/codec/fileformat/__init__.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/codec/fileformat/aedat.py` & `event_vision_library-0.0.1b0/src/evlib/codec/fileformat/aedat.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/codec/fileformat/conversion.py` & `event_vision_library-0.0.1b0/src/evlib/codec/fileformat/conversion.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/codec/fileformat/evk.py` & `event_vision_library-0.0.1b0/src/evlib/codec/fileformat/evk.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/codec/fileformat/hdf5.py` & `event_vision_library-0.0.1b0/src/evlib/codec/fileformat/hdf5.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/codec/fileformat/text.py` & `event_vision_library-0.0.1b0/src/evlib/codec/fileformat/text.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/preproc/hot_pixel.py` & `event_vision_library-0.0.1b0/src/evlib/preproc/hot_pixel.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid.py` & `event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/base_model.py` & `event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/base_model.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/image_reconstructor.py` & `event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/image_reconstructor.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/model/model.py` & `event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/model/model.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/model/submodules.py` & `event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/model/submodules.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/model/unet.py` & `event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/model/unet.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/utils/inference_utils.py` & `event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/utils/inference_utils.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/utils/loading_utils.py` & `event_vision_library-0.0.1b0/src/evlib/processing/reconstruction/e2vid_module/utils/loading_utils.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/representation/histogram.py` & `event_vision_library-0.0.1b0/src/evlib/representation/histogram.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/representation/time_map.py` & `event_vision_library-0.0.1b0/src/evlib/representation/time_map.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/representation/voxel_grid.py` & `event_vision_library-0.0.1b0/src/evlib/representation/voxel_grid.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/types/raw_event.py` & `event_vision_library-0.0.1b0/src/evlib/types/raw_event.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/types/raw_events.py` & `event_vision_library-0.0.1b0/src/evlib/types/raw_events.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/utils/basics.py` & `event_vision_library-0.0.1b0/src/evlib/utils/basics.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/version.py` & `event_vision_library-0.0.1b0/src/evlib/version.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/src/evlib/vis/utils.py` & `event_vision_library-0.0.1b0/src/evlib/vis/utils.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.1/PKG-INFO` & `event_vision_library-0.0.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: event-vision-library
-Version: 0.0.1
+Version: 0.0.1b0
 Summary: Event Vision Library
 Home-page: https://github.com/shiba24/event-vision-library
 License: MIT
 Author: Shintaro Shiba
 Author-email: shiba.shintaro@gmail.com
 Maintainer: Shintaro Shiba
 Maintainer-email: shiba.shintaro@gmail.com
 Requires-Python: >=3.7,<3.11
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: click (>=8.0.1)
@@ -53,18 +53,33 @@
 [python version]: https://pypi.org/project/event-vision-library
 [read the docs]: https://event-vision-library.readthedocs.io/
 [tests]: https://github.com/shiba24/event-vision-library/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/shiba24/event-vision-library
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
+## Installation
+
+You can install _Event Vision Library_ via [pip] from [PyPI]:
+
+```console
+$ pip install event-vision-library
+
+# you can now `import evlib`
+```
+
+## Usage
+
+Please see our [examples] and [documentation][read the docs].
+
 ## Features
 
 - Python 3.7, 3.8, 3.9, 3.10
 - Pure-python library
+- Numpy and Torch compatibility.
 - 🚧 This library is under construction and currently alpha version. The APIs may change significantly. Contributions and discussions are welcomed! 🚧
 
 ### Data
 
 - [ ] Support different data types (.text, .raw, .hdf5, .npy, .aedat) for various file encoding of event data
 - [ ] ROS bag files (optional, based on ROS installation)
 - [ ] Support multiple existing dataset (e.g., ECD, MVSEC, DSEC, etc.)
@@ -80,26 +95,14 @@
 - [ ] C++ implementation and extension for faster execution (TODO)
 
 ### Log and Vsualization
 
 - [ ] Various visualization for 2D/3D representation of events
 - [ ] Useful logging
 
-## Installation
-
-You can install _Event Vision Library_ via [pip] from [PyPI]:
-
-```console
-$ pip install event-vision-library
-```
-
-## Usage
-
-Please see our examples and documentations.
-
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
 
@@ -118,11 +121,12 @@
 [pypi]: https://pypi.org/
 [hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
 [file an issue]: https://github.com/shiba24/event-vision-library/issues
 [pip]: https://pip.pypa.io/
 
 <!-- github-only -->
 
+[examples]: https://github.com/shiba24/event-vision-library/blob/main/examples
 [license]: https://github.com/shiba24/event-vision-library/blob/main/LICENSE
 [contributor guide]: https://github.com/shiba24/event-vision-library/blob/main/CONTRIBUTING.md
 [command-line reference]: https://event-vision-library.readthedocs.io/en/latest/usage.html
```

