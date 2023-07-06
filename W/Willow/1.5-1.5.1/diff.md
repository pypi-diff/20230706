# Comparing `tmp/Willow-1.5.tar.gz` & `tmp/Willow-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Willow-1.5.tar", last modified: Wed Mar 29 19:17:07 2023, max compression
+gzip compressed data, was "Willow-1.5.1.tar", last modified: Thu Jul  6 16:05:40 2023, max compression
```

## Comparing `Willow-1.5.tar` & `Willow-1.5.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-03-29 19:17:07.188820 Willow-1.5/
--rw-r--r--   0 matthew    (501) staff       (20)     1545 2018-07-31 10:09:17.000000 Willow-1.5/LICENSE
--rw-r--r--   0 matthew    (501) staff       (20)      101 2022-02-21 11:00:10.000000 Willow-1.5/MANIFEST.in
--rw-r--r--   0 matthew    (501) staff       (20)      973 2023-03-29 19:17:07.189092 Willow-1.5/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)     3679 2022-08-30 14:15:35.000000 Willow-1.5/README.rst
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-03-29 19:17:07.170642 Willow-1.5/Willow.egg-info/
--rw-r--r--   0 matthew    (501) staff       (20)      973 2023-03-29 19:17:07.000000 Willow-1.5/Willow.egg-info/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)      670 2023-03-29 19:17:07.000000 Willow-1.5/Willow.egg-info/SOURCES.txt
--rw-r--r--   0 matthew    (501) staff       (20)        1 2023-03-29 19:17:07.000000 Willow-1.5/Willow.egg-info/dependency_links.txt
--rw-r--r--   0 matthew    (501) staff       (20)        1 2018-07-31 10:19:37.000000 Willow-1.5/Willow.egg-info/not-zip-safe
--rw-r--r--   0 matthew    (501) staff       (20)      135 2023-03-29 19:17:07.000000 Willow-1.5/Willow.egg-info/requires.txt
--rw-r--r--   0 matthew    (501) staff       (20)        7 2023-03-29 19:17:07.000000 Willow-1.5/Willow.egg-info/top_level.txt
--rw-r--r--   0 matthew    (501) staff       (20)       70 2023-03-29 19:17:07.189730 Willow-1.5/setup.cfg
--rw-r--r--   0 matthew    (501) staff       (20)     1748 2023-03-29 19:16:29.000000 Willow-1.5/setup.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-03-29 19:17:07.176376 Willow-1.5/tests/
--rw-r--r--   0 matthew    (501) staff       (20)     6880 2023-03-29 18:10:39.000000 Willow-1.5/tests/test_image.py
--rw-r--r--   0 matthew    (501) staff       (20)     2161 2022-08-30 14:15:35.000000 Willow-1.5/tests/test_opencv.py
--rw-r--r--   0 matthew    (501) staff       (20)    14800 2023-03-29 18:13:32.000000 Willow-1.5/tests/test_pillow.py
--rw-r--r--   0 matthew    (501) staff       (20)    14576 2018-07-31 10:09:17.000000 Willow-1.5/tests/test_registry.py
--rw-r--r--   0 matthew    (501) staff       (20)     9938 2023-03-29 18:10:39.000000 Willow-1.5/tests/test_svg_coordinate_transforms.py
--rw-r--r--   0 matthew    (501) staff       (20)    15110 2023-03-29 18:10:39.000000 Willow-1.5/tests/test_svg_image.py
--rw-r--r--   0 matthew    (501) staff       (20)    13893 2022-08-30 14:15:35.000000 Willow-1.5/tests/test_wand.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-03-29 19:17:07.179163 Willow-1.5/willow/
--rw-r--r--   0 matthew    (501) staff       (20)     1329 2023-03-29 18:10:39.000000 Willow-1.5/willow/__init__.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-03-29 19:17:07.164622 Willow-1.5/willow/data/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-03-29 19:17:07.179841 Willow-1.5/willow/data/cascades/
--rw-r--r--   0 matthew    (501) staff       (20)   837462 2018-07-31 10:09:17.000000 Willow-1.5/willow/data/cascades/haarcascade_frontalface_alt2.xml
--rw-r--r--   0 matthew    (501) staff       (20)     6496 2023-03-29 18:10:39.000000 Willow-1.5/willow/image.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-03-29 19:17:07.186869 Willow-1.5/willow/plugins/
--rw-r--r--   0 matthew    (501) staff       (20)        0 2018-07-31 10:09:17.000000 Willow-1.5/willow/plugins/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)     3867 2022-02-21 11:00:10.000000 Willow-1.5/willow/plugins/opencv.py
--rw-r--r--   0 matthew    (501) staff       (20)     9081 2023-03-29 18:13:32.000000 Willow-1.5/willow/plugins/pillow.py
--rw-r--r--   0 matthew    (501) staff       (20)     6880 2023-03-29 18:10:39.000000 Willow-1.5/willow/plugins/wand.py
--rw-r--r--   0 matthew    (501) staff       (20)    12614 2023-03-29 18:10:39.000000 Willow-1.5/willow/registry.py
--rw-r--r--   0 matthew    (501) staff       (20)    12230 2023-03-29 18:10:39.000000 Willow-1.5/willow/svg.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-03-29 19:17:07.188071 Willow-1.5/willow/utils/
--rw-r--r--   0 matthew    (501) staff       (20)        0 2018-07-31 10:09:17.000000 Willow-1.5/willow/utils/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)       61 2018-07-31 10:09:17.000000 Willow-1.5/willow/utils/deprecation.py
+drwxr-xr-x   0 dan        (503) staff       (20)        0 2023-07-06 16:05:40.298329 Willow-1.5.1/
+-rw-r--r--   0 dan        (503) staff       (20)     1545 2022-07-01 10:58:39.000000 Willow-1.5.1/LICENSE
+-rw-r--r--   0 dan        (503) staff       (20)      101 2022-07-01 10:58:39.000000 Willow-1.5.1/MANIFEST.in
+-rw-r--r--   0 dan        (503) staff       (20)      975 2023-07-06 16:05:40.298450 Willow-1.5.1/PKG-INFO
+-rw-r--r--   0 dan        (503) staff       (20)     3679 2023-07-06 13:57:05.000000 Willow-1.5.1/README.rst
+drwxr-xr-x   0 dan        (503) staff       (20)        0 2023-07-06 16:05:40.285569 Willow-1.5.1/Willow.egg-info/
+-rw-r--r--   0 dan        (503) staff       (20)      975 2023-07-06 16:05:40.000000 Willow-1.5.1/Willow.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (503) staff       (20)      687 2023-07-06 16:05:40.000000 Willow-1.5.1/Willow.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (503) staff       (20)        1 2023-07-06 16:05:40.000000 Willow-1.5.1/Willow.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (503) staff       (20)        1 2023-07-06 16:05:40.000000 Willow-1.5.1/Willow.egg-info/not-zip-safe
+-rw-r--r--   0 dan        (503) staff       (20)      135 2023-07-06 16:05:40.000000 Willow-1.5.1/Willow.egg-info/requires.txt
+-rw-r--r--   0 dan        (503) staff       (20)        7 2023-07-06 16:05:40.000000 Willow-1.5.1/Willow.egg-info/top_level.txt
+-rw-r--r--   0 dan        (503) staff       (20)       70 2023-07-06 16:05:40.298784 Willow-1.5.1/setup.cfg
+-rw-r--r--   0 dan        (503) staff       (20)     1783 2023-07-06 15:55:46.000000 Willow-1.5.1/setup.py
+drwxr-xr-x   0 dan        (503) staff       (20)        0 2023-07-06 16:05:40.293784 Willow-1.5.1/tests/
+-rw-r--r--   0 dan        (503) staff       (20)     6880 2023-07-06 13:57:05.000000 Willow-1.5.1/tests/test_image.py
+-rw-r--r--   0 dan        (503) staff       (20)     2161 2023-07-06 13:57:05.000000 Willow-1.5.1/tests/test_opencv.py
+-rw-r--r--   0 dan        (503) staff       (20)    14800 2023-07-06 13:57:05.000000 Willow-1.5.1/tests/test_pillow.py
+-rw-r--r--   0 dan        (503) staff       (20)    14576 2023-07-06 13:57:05.000000 Willow-1.5.1/tests/test_registry.py
+-rw-r--r--   0 dan        (503) staff       (20)     7326 2023-07-06 14:34:06.000000 Willow-1.5.1/tests/test_svg_coordinate_transforms.py
+-rw-r--r--   0 dan        (503) staff       (20)    16612 2023-07-06 14:34:06.000000 Willow-1.5.1/tests/test_svg_image.py
+-rw-r--r--   0 dan        (503) staff       (20)    13893 2023-07-06 13:57:05.000000 Willow-1.5.1/tests/test_wand.py
+drwxr-xr-x   0 dan        (503) staff       (20)        0 2023-07-06 16:05:40.294914 Willow-1.5.1/willow/
+-rw-r--r--   0 dan        (503) staff       (20)     6148 2023-07-04 23:07:06.000000 Willow-1.5.1/willow/.DS_Store
+-rw-r--r--   0 dan        (503) staff       (20)     1331 2023-07-06 14:49:48.000000 Willow-1.5.1/willow/__init__.py
+drwxr-xr-x   0 dan        (503) staff       (20)        0 2023-07-06 16:05:40.283385 Willow-1.5.1/willow/data/
+drwxr-xr-x   0 dan        (503) staff       (20)        0 2023-07-06 16:05:40.295135 Willow-1.5.1/willow/data/cascades/
+-rw-r--r--   0 dan        (503) staff       (20)   837462 2022-07-01 10:58:40.000000 Willow-1.5.1/willow/data/cascades/haarcascade_frontalface_alt2.xml
+-rw-r--r--   0 dan        (503) staff       (20)     6496 2023-07-06 13:57:05.000000 Willow-1.5.1/willow/image.py
+drwxr-xr-x   0 dan        (503) staff       (20)        0 2023-07-06 16:05:40.297843 Willow-1.5.1/willow/plugins/
+-rw-r--r--   0 dan        (503) staff       (20)        0 2022-07-01 10:58:40.000000 Willow-1.5.1/willow/plugins/__init__.py
+-rw-r--r--   0 dan        (503) staff       (20)     3867 2023-07-06 13:57:05.000000 Willow-1.5.1/willow/plugins/opencv.py
+-rw-r--r--   0 dan        (503) staff       (20)     9081 2023-07-06 13:57:05.000000 Willow-1.5.1/willow/plugins/pillow.py
+-rw-r--r--   0 dan        (503) staff       (20)     6880 2023-07-06 13:57:05.000000 Willow-1.5.1/willow/plugins/wand.py
+-rw-r--r--   0 dan        (503) staff       (20)    12614 2023-07-06 13:57:05.000000 Willow-1.5.1/willow/registry.py
+-rw-r--r--   0 dan        (503) staff       (20)    11803 2023-07-06 14:34:06.000000 Willow-1.5.1/willow/svg.py
+drwxr-xr-x   0 dan        (503) staff       (20)        0 2023-07-06 16:05:40.298069 Willow-1.5.1/willow/utils/
+-rw-r--r--   0 dan        (503) staff       (20)        0 2022-07-01 10:58:40.000000 Willow-1.5.1/willow/utils/__init__.py
+-rw-r--r--   0 dan        (503) staff       (20)       61 2022-07-01 10:58:40.000000 Willow-1.5.1/willow/utils/deprecation.py
```

### Comparing `Willow-1.5/LICENSE` & `Willow-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Willow-1.5/PKG-INFO` & `Willow-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Willow
-Version: 1.5
+Version: 1.5.1
 Summary: A Python image library that sits on top of Pillow, Wand and OpenCV
 Home-page: 
 Author: Karl Hobley
 Author-email: karl@kaed.uk
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Multimedia :: Graphics
```

### Comparing `Willow-1.5/README.rst` & `Willow-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `Willow-1.5/Willow.egg-info/PKG-INFO` & `Willow-1.5.1/Willow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Willow
-Version: 1.5
+Version: 1.5.1
 Summary: A Python image library that sits on top of Pillow, Wand and OpenCV
 Home-page: 
 Author: Karl Hobley
 Author-email: karl@kaed.uk
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Multimedia :: Graphics
```

### Comparing `Willow-1.5/Willow.egg-info/SOURCES.txt` & `Willow-1.5.1/Willow.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 tests/test_image.py
 tests/test_opencv.py
 tests/test_pillow.py
 tests/test_registry.py
 tests/test_svg_coordinate_transforms.py
 tests/test_svg_image.py
 tests/test_wand.py
+willow/.DS_Store
 willow/__init__.py
 willow/image.py
 willow/registry.py
 willow/svg.py
 willow/data/cascades/haarcascade_frontalface_alt2.xml
 willow/plugins/__init__.py
 willow/plugins/opencv.py
```

### Comparing `Willow-1.5/setup.py` & `Willow-1.5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 # (see http://www.eby-sarna.com/pipermail/peak/2010-May/003357.html)
 try:
     import multiprocessing
 except ImportError:
     pass
 
 
-
 setup(
     name='Willow',
-    version='1.5',
+    version="1.5.1",  # Update willow/__init__.py too!
     description='A Python image library that sits on top of Pillow, Wand and OpenCV',
     author='Karl Hobley',
     author_email='karl@kaed.uk',
     url='',
     packages=find_packages(exclude=['tests']),
     include_package_data=True,
     license='BSD',
```

### Comparing `Willow-1.5/tests/test_image.py` & `Willow-1.5.1/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `Willow-1.5/tests/test_opencv.py` & `Willow-1.5.1/tests/test_opencv.py`

 * *Files identical despite different names*

### Comparing `Willow-1.5/tests/test_pillow.py` & `Willow-1.5.1/tests/test_pillow.py`

 * *Files identical despite different names*

### Comparing `Willow-1.5/tests/test_registry.py` & `Willow-1.5.1/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `Willow-1.5/tests/test_svg_coordinate_transforms.py` & `Willow-1.5.1/tests/test_svg_coordinate_transforms.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from functools import partial
 
 from willow.svg import (
-    get_viewport_to_user_space_transform,
-    transform_rect_to_user_space,
     SvgImage,
     ViewportToUserSpaceTransform,
+    get_viewport_to_user_space_transform,
 )
 
 from .test_svg_image import SvgWrapperTestCase
 
 
 class ViewportToUserSpaceTransformTestCase(SvgWrapperTestCase):
     def test_get_transform_same_ratio(self):
@@ -38,98 +37,33 @@
                 view_box="0 0 50 80",
                 preserve_aspect_ratio="none",
             )
         )
         transform = get_viewport_to_user_space_transform(svg)
         self.assertEqual(transform, ViewportToUserSpaceTransform(2, 1.25, 0, 0))
 
-    def test_transform_rect_to_user_space_translate_x(self):
-        svg_wrapper = partial(
-            self.get_svg_wrapper, width=100, height=50, view_box="0 0 25 25"
-        )
-        params = [
-            # transform = (2, 2, 0, 0)
-            ("xMinYMid meet", (10, 10, 20, 20), (5, 5, 10, 10)),
-            # transform = (2, 2, 25, 0)
-            ("xMidYMid meet", (10, 10, 20, 20), (-7.5, 5, -2.5, 10)),
-            # transform = (2, 2, 50, 0)
-            ("xMaxYMid meet", (10, 10, 20, 20), (-20, 5, -15, 10)),
-        ]
-        for preserve_aspect_ratio, rect, expected_result in params:
-            with self.subTest(preserve_aspect_ratio=preserve_aspect_ratio, rect=rect):
-                svg = SvgImage(svg_wrapper(preserve_aspect_ratio=preserve_aspect_ratio))
-                self.assertEqual(
-                    transform_rect_to_user_space(svg, rect), expected_result
-                )
-
-    def test_transform_rect_to_user_space_translate_y(self):
-        svg_wrapper = partial(
-            self.get_svg_wrapper, width=50, height=100, view_box="0 0 25 25"
-        )
-        params = [
-            # transform = (2, 2, 0, 0)
-            ("xMidYMin meet", (10, 10, 20, 20), (5, 5, 10, 10)),
-            # transform = (2, 2, 0, 25)
-            ("xMidYMid meet", (10, 10, 20, 20), (5, -7.5, 10, -2.5)),
-            # transform = (2, 2, 0, 50)
-            ("xMidYMax meet", (10, 10, 20, 20), (5, -20, 10, -15)),
-        ]
-        for preserve_aspect_ratio, rect, expected_result in params:
-            with self.subTest(preserve_aspect_ratio=preserve_aspect_ratio, rect=rect):
-                svg = SvgImage(svg_wrapper(preserve_aspect_ratio=preserve_aspect_ratio))
-                self.assertEqual(
-                    transform_rect_to_user_space(svg, rect), expected_result
-                )
-
-    def test_complex_user_space_origin_transform(self):
-        svg = SvgImage(
-            self.get_svg_wrapper(
-                width=100,
-                height=100,
-                view_box="-50 -50 100 100",
-                preserve_aspect_ratio="none",
-            )
-        )
-        self.assertEqual(
-            transform_rect_to_user_space(svg, (0, 0, 50, 50)),
-            (-50, -50, 0, 0),
-        )
-
-        svg = SvgImage(
-            self.get_svg_wrapper(
-                width=200,
-                height=200,
-                view_box="-50 -50 100 100",
-                preserve_aspect_ratio="none",
-            )
-        )
-        self.assertEqual(
-            transform_rect_to_user_space(svg, (0, 0, 50, 50)),
-            (-25, -25, 0, 0),
-        )
-
 
 class PreserveAspectRatioMeetTestCase(SvgWrapperTestCase):
     def test_portrait_view_box(self):
         # With "meet", the scaling factor will be min(scale_x,
         # scale_y). In the case of a portrait ratio view box in a
         # square viewport, this will be scale_y
         svg_wrapper = partial(
             self.get_svg_wrapper, width=100, height=100, view_box="0 0 50 80"
         )
         params = [
             ("xMinYMin meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, 0)),
             ("xMinYMid meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, 0)),
             ("xMinYMax meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, 0)),
-            ("xMidYMin meet", ViewportToUserSpaceTransform(1.25, 1.25, 18.75, 0)),
-            ("xMidYMid meet", ViewportToUserSpaceTransform(1.25, 1.25, 18.75, 0)),
-            ("xMidYMax meet", ViewportToUserSpaceTransform(1.25, 1.25, 18.75, 0)),
-            ("xMaxYMin meet", ViewportToUserSpaceTransform(1.25, 1.25, 37.5, 0)),
-            ("xMaxYMid meet", ViewportToUserSpaceTransform(1.25, 1.25, 37.5, 0)),
-            ("xMaxYMax meet", ViewportToUserSpaceTransform(1.25, 1.25, 37.5, 0)),
+            ("xMidYMin meet", ViewportToUserSpaceTransform(1.25, 1.25, -18.75, 0)),
+            ("xMidYMid meet", ViewportToUserSpaceTransform(1.25, 1.25, -18.75, 0)),
+            ("xMidYMax meet", ViewportToUserSpaceTransform(1.25, 1.25, -18.75, 0)),
+            ("xMaxYMin meet", ViewportToUserSpaceTransform(1.25, 1.25, -37.5, 0)),
+            ("xMaxYMid meet", ViewportToUserSpaceTransform(1.25, 1.25, -37.5, 0)),
+            ("xMaxYMax meet", ViewportToUserSpaceTransform(1.25, 1.25, -37.5, 0)),
         ]
         for preserve_aspect_ratio, expected_result in params:
             with self.subTest(preserve_aspect_ratio=preserve_aspect_ratio):
                 svg = SvgImage(svg_wrapper(preserve_aspect_ratio=preserve_aspect_ratio))
                 self.assertEqual(
                     get_viewport_to_user_space_transform(svg), expected_result
                 )
@@ -140,20 +74,20 @@
         svg_wrapper = partial(
             self.get_svg_wrapper, width=100, height=100, view_box="0 0 80 50"
         )
         params = [
             ("xMinYMin meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, 0)),
             ("xMidYMin meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, 0)),
             ("xMaxYMin meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, 0)),
-            ("xMinYMid meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, 18.75)),
-            ("xMidYMid meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, 18.75)),
-            ("xMaxYMid meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, 18.75)),
-            ("xMinYMax meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, 37.5)),
-            ("xMidYMax meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, 37.5)),
-            ("xMaxYMax meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, 37.5)),
+            ("xMinYMid meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, -18.75)),
+            ("xMidYMid meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, -18.75)),
+            ("xMaxYMid meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, -18.75)),
+            ("xMinYMax meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, -37.5)),
+            ("xMidYMax meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, -37.5)),
+            ("xMaxYMax meet", ViewportToUserSpaceTransform(1.25, 1.25, 0, -37.5)),
         ]
         for preserve_aspect_ratio, expected_result in params:
             with self.subTest(preserve_aspect_ratio=preserve_aspect_ratio):
                 svg = SvgImage(svg_wrapper(preserve_aspect_ratio=preserve_aspect_ratio))
                 self.assertEqual(
                     get_viewport_to_user_space_transform(svg), expected_result
                 )
@@ -167,20 +101,20 @@
         svg_wrapper = partial(
             self.get_svg_wrapper, width=100, height=100, view_box="0 0 40 80"
         )
         params = [
             ("xMinYMin slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, 0)),
             ("xMidYMin slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, 0)),
             ("xMaxYMin slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, 0)),
-            ("xMinYMid slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, -50)),
-            ("xMidYMid slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, -50)),
-            ("xMaxYMid slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, -50)),
-            ("xMinYMax slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, -100)),
-            ("xMidYMax slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, -100)),
-            ("xMaxYMax slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, -100)),
+            ("xMinYMid slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, 50)),
+            ("xMidYMid slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, 50)),
+            ("xMaxYMid slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, 50)),
+            ("xMinYMax slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, 100)),
+            ("xMidYMax slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, 100)),
+            ("xMaxYMax slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, 100)),
         ]
         for preserve_aspect_ratio, expected_result in params:
             with self.subTest(preserve_aspect_ratio=preserve_aspect_ratio):
                 svg = SvgImage(svg_wrapper(preserve_aspect_ratio=preserve_aspect_ratio))
                 self.assertEqual(
                     get_viewport_to_user_space_transform(svg), expected_result
                 )
@@ -191,20 +125,20 @@
         svg_wrapper = partial(
             self.get_svg_wrapper, width=100, height=100, view_box="0 0 80 40"
         )
         params = [
             ("xMinYMin slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, 0)),
             ("xMinYMid slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, 0)),
             ("xMinYMax slice", ViewportToUserSpaceTransform(2.5, 2.5, 0, 0)),
-            ("xMidYMin slice", ViewportToUserSpaceTransform(2.5, 2.5, -50, 0)),
-            ("xMidYMid slice", ViewportToUserSpaceTransform(2.5, 2.5, -50, 0)),
-            ("xMidYMax slice", ViewportToUserSpaceTransform(2.5, 2.5, -50, 0)),
-            ("xMaxYMin slice", ViewportToUserSpaceTransform(2.5, 2.5, -100, 0)),
-            ("xMaxYMid slice", ViewportToUserSpaceTransform(2.5, 2.5, -100, 0)),
-            ("xMaxYMax slice", ViewportToUserSpaceTransform(2.5, 2.5, -100, 0)),
+            ("xMidYMin slice", ViewportToUserSpaceTransform(2.5, 2.5, 50, 0)),
+            ("xMidYMid slice", ViewportToUserSpaceTransform(2.5, 2.5, 50, 0)),
+            ("xMidYMax slice", ViewportToUserSpaceTransform(2.5, 2.5, 50, 0)),
+            ("xMaxYMin slice", ViewportToUserSpaceTransform(2.5, 2.5, 100, 0)),
+            ("xMaxYMid slice", ViewportToUserSpaceTransform(2.5, 2.5, 100, 0)),
+            ("xMaxYMax slice", ViewportToUserSpaceTransform(2.5, 2.5, 100, 0)),
         ]
         for preserve_aspect_ratio, expected_result in params:
             with self.subTest(preserve_aspect_ratio=preserve_aspect_ratio):
                 svg = SvgImage(svg_wrapper(preserve_aspect_ratio=preserve_aspect_ratio))
                 self.assertEqual(
                     get_viewport_to_user_space_transform(svg), expected_result
                 )
```

### Comparing `Willow-1.5/tests/test_svg_image.py` & `Willow-1.5.1/tests/test_svg_image.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+import glob
 import unittest
 from io import BytesIO
 from itertools import product
+from pathlib import Path
 from string import Template
 
 from defusedxml import ElementTree
 
-from willow.image import Image, SvgImageFile, BadImageOperationError
+from willow.image import BadImageOperationError, Image, SvgImageFile
 from willow.svg import (
-    SvgWrapper,
     InvalidSvgAttribute,
     InvalidSvgSizeAttribute,
     SvgImage,
+    SvgWrapper,
     ViewBox,
 )
 
 
 class SvgWrapperTestCase(unittest.TestCase):
     svg_template = Template(
         '<svg width="$width" height="$height" viewBox="$view_box" '
@@ -262,45 +264,110 @@
 
         with self.assertRaises(BadImageOperationError):
             svg_image_file.resize((0, 10))
 
         with self.assertRaises(BadImageOperationError):
             svg_image_file.resize((10, 0))
 
-    def test_crop(self):
+    def test_save_as_svg(self):
+        f = BytesIO(b'<svg width="13" height="13" viewBox="0 0 13 13"></svg>')
+        svg_image_file = Image.open(f)
+        svg = SvgImage(image=SvgWrapper(svg_image_file.dom))
+        written = svg.save_as_svg(BytesIO())
+        self.assertIsInstance(written, SvgImageFile)
+        self.assertEqual(written.dom.getroot().get("width"), "13")
+        self.assertEqual(written.dom.getroot().get("height"), "13")
+
+    def test_get_frame_count(self):
+        svg = SvgImage(self.get_svg_wrapper())
+        self.assertEqual(svg.get_frame_count(), 1)
+
+    def test_resize_preserves_original_image(self):
         f = BytesIO(b'<svg width="42" height="42" viewBox="0 0 42 42"></svg>')
         svg_image_file = Image.open(f)
-        cropped = svg_image_file.crop((5, 5, 15, 15))
-        self.assertEqual(cropped.get_size(), (10, 10))
-        self.assertEqual(cropped.image.view_box, ViewBox(5, 5, 10, 10))
+        svg = SvgImage.open(svg_image_file)
+        svg.resize((21, 21))
+        self.assertEqual(svg.get_size(), (42, 42))
 
-        # Check the underlying etree has been updated
-        self.assertEqual(float(cropped.image.root.get("width")), 10)
-        self.assertEqual(float(cropped.image.root.get("height")), 10)
-        self.assertEqual(
-            [float(x) for x in cropped.image.root.get("viewBox").split()],
-            [5, 5, 10, 10],
-        )
 
-    def test_crop_with_transform(self):
-        # user coordinates scaled by 2 and translated 50 units south
-        svg = SvgImage(
-            self.get_svg_wrapper(
-                width=50,
-                height=100,
-                view_box="0 0 25 25",
-                preserve_aspect_ratio="xMidYMax meet",
+class SvgCropTestCase(SvgWrapperTestCase):
+    def test_crop(self):
+        """
+        Test cropping SVGs.
+
+        This finds, recursively, all of the relevant SVG files in the
+        tests/images/svg/originals directory. For each file it finds, it:
+        - opens the file;
+        - performs a crop based on the filename; and
+        - compares the attributes on the cropped SVG in memory to the expected
+          cropped version stored in the corresponding tests/images/svg/results
+          subdirectory.
+
+        An SVG named `some-name-crop-original.svg' will be cropped to the
+        dimensions of its original viewport.
+
+        A specific bounding rect for a crop can be specified in the file name
+        like this:
+
+            <some descriptive prefix>-crop-<left>_<top>_<right>_<bottom>.svg
+
+        For example, the file `my-svg-crop-0_10_20_30.svg' will be cropped to
+        the rect (left=0, top=10, right=20, bottom=30).
+
+        The cropping test files are organised into subdirectories by their
+        `preserveAspectRatio' value. To save duplication, files with specific
+        crop directives are symlinks to their corresponding 'original' crop
+        file.
+        """
+
+        def get_original_crop_rect(svg_image):
+            # left, top, right, bottom (not left, top, width, height,
+            # like viewBox but the same in this case)
+            return (0, 0, svg_image.image.width, svg_image.image.height)
+
+        base_dir = Path("tests/images/svg")
+        original_file_paths = (
+            Path(x)
+            for x in glob.iglob(
+                str(base_dir / "originals/**/*-crop-*.svg"), recursive=True
             )
         )
 
-        cropped = svg.crop((10, 10, 20, 20))
-        self.assertEqual(cropped.get_size(), (10, 10))
-        self.assertEqual(cropped.image.view_box, ViewBox(5, -20, 5, 5))
-        self.assertEqual(float(cropped.image.root.get("width")), 10)
-        self.assertEqual(float(cropped.image.root.get("height")), 10)
+        for original_file_path in original_file_paths:
+            with open(original_file_path, "rb") as f:
+                original_file = Image.open(f)
+            original = SvgImage.open(original_file)
+            directive = original_file_path.stem.split("-")[-1]
+            if directive == "original":
+                rect = get_original_crop_rect(original)
+            else:
+                rect = tuple(int(x) for x in directive.split("_"))
+            cropped = original.crop(rect)
+
+            result_file_path = str(original_file_path).replace("originals", "results")
+            with open(result_file_path, "rb") as f:
+                expected_file = Image.open(f)
+            expected = SvgImage.open(expected_file)
+
+            with self.subTest(
+                original=str(original_file_path), expected=str(result_file_path)
+            ):
+                self.assertEqual(expected.image.view_box, cropped.image.view_box)
+                self.assertEqual(expected.image.width, cropped.image.width)
+                self.assertEqual(expected.image.height, cropped.image.height)
+
+    def test_crop_preserves_original_image(self):
+        """
+        Cropping should create a new image, leaving the original untouched.
+        """
+        f = BytesIO(b'<svg width="42" height="42" viewBox="0 0 42 42"></svg>')
+        svg_image_file = Image.open(f)
+        svg = SvgImage.open(svg_image_file)
+        svg.crop((0, 0, 10, 10))
+        self.assertEqual(svg.image.view_box, ViewBox(0, 0, 42, 42))
 
     def test_crop_throws(self):
         f = BytesIO(b'<svg width="42" height="42" viewBox="0 0 42 42"></svg>')
         svg_image_file = Image.open(f)
 
         with self.assertRaises(BadImageOperationError):
             # left > right
@@ -314,44 +381,14 @@
             # top > bottom
             svg_image_file.crop((0, 10, 10, 0))
 
         with self.assertRaises(BadImageOperationError):
             # top == bottom
             svg_image_file.crop((0, 10, 10, 10))
 
-    def test_save_as_svg(self):
-        f = BytesIO(b'<svg width="13" height="13" viewBox="0 0 13 13"></svg>')
-        svg_image_file = Image.open(f)
-        svg = SvgImage(image=SvgWrapper(svg_image_file.dom))
-        written = svg.save_as_svg(BytesIO())
-        self.assertIsInstance(written, SvgImageFile)
-        self.assertEqual(written.dom.getroot().get("width"), "13")
-        self.assertEqual(written.dom.getroot().get("height"), "13")
-
-    def test_get_frame_count(self):
-        svg = SvgImage(self.get_svg_wrapper())
-        self.assertEqual(svg.get_frame_count(), 1)
-
-    def test_crop_preserves_original_image(self):
-        """
-        Cropping should create a new image, leaving the original untouched.
-        """
-        f = BytesIO(b'<svg width="42" height="42" viewBox="0 0 42 42"></svg>')
-        svg_image_file = Image.open(f)
-        svg = SvgImage.open(svg_image_file)
-        svg.crop((0, 0, 10, 10))
-        self.assertEqual(svg.image.view_box, ViewBox(0, 0, 42, 42))
-
-    def test_resize_preserves_original_image(self):
-        f = BytesIO(b'<svg width="42" height="42" viewBox="0 0 42 42"></svg>')
-        svg_image_file = Image.open(f)
-        svg = SvgImage.open(svg_image_file)
-        svg.resize((21, 21))
-        self.assertEqual(svg.get_size(), (42, 42))
-
 
 class SvgViewBoxTestCase(unittest.TestCase):
     def test_view_box_re(self):
         params = [
             ("0 0 1 1", ViewBox(0, 0, 1, 1)),
             (" 0 0 1 1 ", ViewBox(0, 0, 1, 1)),
             ("-0 +0 -1 +1", ViewBox(0, 0, -1, 1)),
```

### Comparing `Willow-1.5/tests/test_wand.py` & `Willow-1.5.1/tests/test_wand.py`

 * *Files identical despite different names*

### Comparing `Willow-1.5/willow/__init__.py` & `Willow-1.5.1/willow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,8 +40,8 @@
     # namespaces, e.g. "<ns0:svg ..."
     ElementTree.register_namespace("", "http://www.w3.org/2000/svg")
 
 
 setup()
 
 
-__version__ = "1.4"
+__version__ = "1.5.1"
```

### Comparing `Willow-1.5/willow/data/cascades/haarcascade_frontalface_alt2.xml` & `Willow-1.5.1/willow/data/cascades/haarcascade_frontalface_alt2.xml`

 * *Files identical despite different names*

### Comparing `Willow-1.5/willow/image.py` & `Willow-1.5.1/willow/image.py`

 * *Files identical despite different names*

### Comparing `Willow-1.5/willow/plugins/opencv.py` & `Willow-1.5.1/willow/plugins/opencv.py`

 * *Files identical despite different names*

### Comparing `Willow-1.5/willow/plugins/pillow.py` & `Willow-1.5.1/willow/plugins/pillow.py`

 * *Files identical despite different names*

### Comparing `Willow-1.5/willow/plugins/wand.py` & `Willow-1.5.1/willow/plugins/wand.py`

 * *Files identical despite different names*

### Comparing `Willow-1.5/willow/registry.py` & `Willow-1.5.1/willow/registry.py`

 * *Files identical despite different names*

### Comparing `Willow-1.5/willow/svg.py` & `Willow-1.5.1/willow/svg.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,78 +32,86 @@
 class ViewportToUserSpaceTransform:
     def __init__(self, scale_x, scale_y, translate_x, translate_y):
         self.scale_x = scale_x
         self.scale_y = scale_y
         self.translate_x = translate_x
         self.translate_y = translate_y
 
+    def __repr__(self):
+        return (
+            f"{self.__class__.__name__}(scale_x={self.scale_x}, scale_y="
+            f"{self.scale_y}, translate_x={self.translate_x}, "
+            f"translate_y={self.translate_y})"
+        )
+
     def __eq__(self, other):
         if not isinstance(other, self.__class__):
             return False
         return (
             self.scale_x == other.scale_x
             and self.scale_y == other.scale_y
             and self.translate_x == other.translate_x
             and self.translate_y == other.translate_y
         )
 
     def __call__(self, rect):
         left, top, right, bottom = rect
         return (
-            (left - self.translate_x) / self.scale_x,
-            (top - self.translate_y) / self.scale_y,
-            (right - self.translate_x) / self.scale_x,
-            (bottom - self.translate_y) / self.scale_y,
+            (left + self.translate_x) / self.scale_x,
+            (top + self.translate_y) / self.scale_y,
+            (right + self.translate_x) / self.scale_x,
+            (bottom + self.translate_y) / self.scale_y,
         )
 
 
 def get_viewport_to_user_space_transform(
     svg: "SvgImage",
 ) -> ViewportToUserSpaceTransform:
     # cairosvg used as a reference
     view_box = svg.image.view_box
 
-    viewport_aspect_ratio = svg.image.width / svg.image.height
-    user_aspect_ratio = view_box.width / view_box.height
-    if viewport_aspect_ratio == user_aspect_ratio:
-        scale = svg.image.width / view_box.width
-        translate = 0
-        return ViewportToUserSpaceTransform(scale, scale, translate, translate)
-
-    aspect_ratio = svg.image.preserve_aspect_ratio.split()
+    preserve_aspect_ratio = svg.image.preserve_aspect_ratio.split()
     try:
-        align, meet_or_slice = aspect_ratio
+        align, meet_or_slice = preserve_aspect_ratio
     except ValueError:
-        align = aspect_ratio[0]
+        align = preserve_aspect_ratio[0]
         meet_or_slice = None
 
     scale_x = svg.image.width / view_box.width
     scale_y = svg.image.height / view_box.height
 
     if align == "none":
+        # if align is "none", the viewBox will be scaled non-uniformly,
+        # so we keep and use both scale_x and scale_y
         x_position = "min"
         y_position = "min"
     else:
         x_position = align[1:4].lower()
         y_position = align[5:].lower()
         choose_coefficient = max if meet_or_slice == "slice" else min
+        # all values of preserveAspectRatio's `align', other than
+        # "none", force uniform scaling, so choose the appropriate
+        # coefficient and use it for scaling both axes
         scale_x = scale_y = choose_coefficient(scale_x, scale_y)
 
-    # Translations to be applied after scaling
-    translate_x = 0
+    # initial offsets to account for non-zero viewBox min-x and min-y
+    translate_x = view_box.min_x * scale_x
+    translate_y = view_box.min_y * scale_y
+
+    # adjust the offsets by the amount the viewBox has been translated
+    # to fit into the viewport (if any)
     if x_position == "mid":
-        translate_x = (svg.image.width - view_box.width * scale_x) / 2
+        translate_x -= (svg.image.width - view_box.width * scale_x) / 2
     elif x_position == "max":
-        translate_x = svg.image.width - view_box.width * scale_x
+        translate_x -= svg.image.width - view_box.width * scale_x
 
-    translate_y = 0
     if y_position == "mid":
-        translate_y += (svg.image.height - view_box.height * scale_y) / 2
+        translate_y -= (svg.image.height - view_box.height * scale_y) / 2
     elif y_position == "max":
-        translate_y += svg.image.height - view_box.height * scale_y
+        translate_y -= svg.image.height - view_box.height * scale_y
 
     return ViewportToUserSpaceTransform(scale_x, scale_y, translate_x, translate_y)
 
 
 class SvgWrapper:
     # https://developer.mozilla.org/en-US/docs/Web/SVG/Content_type#length
     UNIT_RE = re.compile(r"(?:em|ex|px|in|cm|mm|pt|pc|%)$")
@@ -269,48 +277,28 @@
         self.set_root_attr("viewBox", view_box_to_attr_str(view_box))
         self.view_box = view_box
 
     def write(self, f):
         self.dom.write(f, encoding="utf-8")
 
 
-def transform_rect_to_user_space(svg: "SvgImage", rect):
-    # As well as scaling and translating the input rect to handle the
-    # preserveAspectRatio attribute, we need to account for the fact
-    # that the origin in the viewport coordinate space (i.e. as a
-    # viewer perceives the image) is not necessarily the same as
-    # the origin in the user coordinate space. For example, if we
-    # may have an SVG with a viewBox of (-8, -8, 10, 10), what the
-    # viewer perceives as (0, 0), is (-8, -8) in the user space.
-    left, top, right, bottom = rect
-    width = right - left
-    height = bottom - top
-    left += svg.image.view_box.min_x
-    top += svg.image.view_box.min_y
-    right = left + width
-    bottom = top + height
-
-    transform = get_viewport_to_user_space_transform(svg)
-    return transform((left, top, right, bottom))
-
-
 class SvgImage(Image):
     def __init__(self, image):
         self.image: SvgWrapper = image
 
     @Image.operation
-    def crop(self, rect, transformer=transform_rect_to_user_space):
+    def crop(self, rect, get_transformer=get_viewport_to_user_space_transform):
         left, top, right, bottom = rect
         if left >= right or top >= bottom:
             raise BadImageOperationError(f"Invalid crop dimensions: {rect}")
 
         viewport_width = right - left
         viewport_height = bottom - top
 
-        transformed_rect = transformer(self, rect) if callable(transformer) else rect
+        transformed_rect = get_transformer(self)(rect)
         left, top, right, bottom = transformed_rect
 
         svg_wrapper = copy(self.image)
         view_box_width = right - left
         view_box_height = bottom - top
         svg_wrapper.set_view_box(ViewBox(left, top, view_box_width, view_box_height))
         svg_wrapper.set_width(viewport_width)
```

