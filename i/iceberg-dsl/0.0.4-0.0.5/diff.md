# Comparing `tmp/iceberg-dsl-0.0.4.tar.gz` & `tmp/iceberg-dsl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iceberg-dsl-0.0.4.tar", last modified: Tue Jul  4 22:10:47 2023, max compression
+gzip compressed data, was "iceberg-dsl-0.0.5.tar", last modified: Thu Jul  6 01:09:35 2023, max compression
```

## Comparing `iceberg-dsl-0.0.4.tar` & `iceberg-dsl-0.0.5.tar`

### file list

```diff
@@ -1,39 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 22:10:47.773097 iceberg-dsl-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-06-21 20:19:08.000000 iceberg-dsl-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     5814 2023-07-04 22:10:47.773097 iceberg-dsl-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4672 2023-07-04 18:55:35.000000 iceberg-dsl-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 22:10:47.753097 iceberg-dsl-0.0.4/iceberg/
--rw-rw-rw-   0        0        0      202 2023-07-03 23:26:54.000000 iceberg-dsl-0.0.4/iceberg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 22:10:47.754097 iceberg-dsl-0.0.4/iceberg/arrows/
--rw-rw-rw-   0        0        0     7173 2023-06-23 03:25:22.000000 iceberg-dsl-0.0.4/iceberg/arrows/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 22:10:47.757098 iceberg-dsl-0.0.4/iceberg/core/
--rw-rw-rw-   0        0        0      205 2023-06-23 03:35:17.000000 iceberg-dsl-0.0.4/iceberg/core/__init__.py
--rw-rw-rw-   0        0        0     7938 2023-07-04 18:52:13.000000 iceberg-dsl-0.0.4/iceberg/core/drawable.py
--rw-rw-rw-   0        0        0    13769 2023-07-04 07:10:50.000000 iceberg-dsl-0.0.4/iceberg/core/properties.py
--rw-rw-rw-   0        0        0     5090 2023-07-04 21:58:07.000000 iceberg-dsl-0.0.4/iceberg/core/renderer.py
--rw-rw-rw-   0        0        0     2788 2023-03-01 05:13:30.000000 iceberg-dsl-0.0.4/iceberg/geometry.py
-drwxrwxrwx   0        0        0        0 2023-07-04 22:10:47.762098 iceberg-dsl-0.0.4/iceberg/primitives/
--rw-rw-rw-   0        0        0      361 2023-06-28 02:25:22.000000 iceberg-dsl-0.0.4/iceberg/primitives/__init__.py
--rw-rw-rw-   0        0        0     1124 2023-06-21 07:44:59.000000 iceberg-dsl-0.0.4/iceberg/primitives/filters.py
--rw-rw-rw-   0        0        0     1542 2023-07-03 22:55:06.000000 iceberg-dsl-0.0.4/iceberg/primitives/image.py
--rw-rw-rw-   0        0        0     4325 2023-06-23 06:40:33.000000 iceberg-dsl-0.0.4/iceberg/primitives/latex.py
--rw-rw-rw-   0        0        0    12350 2023-07-04 07:10:50.000000 iceberg-dsl-0.0.4/iceberg/primitives/layout.py
--rw-rw-rw-   0        0        0     3935 2023-07-04 07:10:50.000000 iceberg-dsl-0.0.4/iceberg/primitives/shapes.py
--rw-rw-rw-   0        0        0     1612 2023-06-23 04:10:37.000000 iceberg-dsl-0.0.4/iceberg/primitives/svg.py
--rw-rw-rw-   0        0        0     4338 2023-06-23 05:34:56.000000 iceberg-dsl-0.0.4/iceberg/primitives/text.py
--rw-rw-rw-   0        0        0     1281 2023-06-21 18:54:51.000000 iceberg-dsl-0.0.4/iceberg/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-04 22:10:47.767098 iceberg-dsl-0.0.4/iceberg_dsl.egg-info/
--rw-rw-rw-   0        0        0     5814 2023-07-04 22:10:47.000000 iceberg-dsl-0.0.4/iceberg_dsl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      756 2023-07-04 22:10:47.000000 iceberg-dsl-0.0.4/iceberg_dsl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 22:10:47.000000 iceberg-dsl-0.0.4/iceberg_dsl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-07-04 22:10:47.000000 iceberg-dsl-0.0.4/iceberg_dsl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-04 22:10:47.000000 iceberg-dsl-0.0.4/iceberg_dsl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1111 2023-07-04 22:10:47.774096 iceberg-dsl-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      488 2023-06-21 20:31:57.000000 iceberg-dsl-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 22:10:47.772097 iceberg-dsl-0.0.4/tests/
--rw-rw-rw-   0        0        0        0 2023-07-04 19:01:04.000000 iceberg-dsl-0.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0     1115 2023-07-04 21:59:42.000000 iceberg-dsl-0.0.4/tests/scene_tester.py
--rw-rw-rw-   0        0        0      474 2023-07-04 21:58:36.000000 iceberg-dsl-0.0.4/tests/test_blank.py
--rw-rw-rw-   0        0        0     2315 2023-07-04 22:04:53.000000 iceberg-dsl-0.0.4/tests/test_connect.py
--rw-rw-rw-   0        0        0     3380 2023-07-04 22:01:27.000000 iceberg-dsl-0.0.4/tests/test_neural_net.py
--rw-rw-rw-   0        0        0     1137 2023-07-04 22:03:24.000000 iceberg-dsl-0.0.4/tests/test_quickstart.py
+drwxrwxrwx   0        0        0        0 2023-07-06 01:09:35.003729 iceberg-dsl-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-21 20:19:08.000000 iceberg-dsl-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5814 2023-07-06 01:09:35.003729 iceberg-dsl-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4672 2023-07-05 08:33:16.000000 iceberg-dsl-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 01:09:34.821729 iceberg-dsl-0.0.5/iceberg/
+-rw-rw-rw-   0        0        0      202 2023-07-06 01:09:04.000000 iceberg-dsl-0.0.5/iceberg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 01:09:34.846731 iceberg-dsl-0.0.5/iceberg/animation/
+-rw-rw-rw-   0        0        0       81 2023-07-05 08:20:47.000000 iceberg-dsl-0.0.5/iceberg/animation/__init__.py
+-rw-rw-rw-   0        0        0     2994 2023-07-05 08:20:47.000000 iceberg-dsl-0.0.5/iceberg/animation/animatable.py
+-rw-rw-rw-   0        0        0     1988 2023-07-05 08:29:23.000000 iceberg-dsl-0.0.5/iceberg/animation/scene.py
+-rw-rw-rw-   0        0        0     2217 2023-07-05 08:20:47.000000 iceberg-dsl-0.0.5/iceberg/animation/tween.py
+drwxrwxrwx   0        0        0        0 2023-07-06 01:09:34.852731 iceberg-dsl-0.0.5/iceberg/arrows/
+-rw-rw-rw-   0        0        0     7173 2023-06-23 03:25:22.000000 iceberg-dsl-0.0.5/iceberg/arrows/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 01:09:34.880732 iceberg-dsl-0.0.5/iceberg/core/
+-rw-rw-rw-   0        0        0      205 2023-06-23 03:35:17.000000 iceberg-dsl-0.0.5/iceberg/core/__init__.py
+-rw-rw-rw-   0        0        0     7938 2023-07-04 22:12:48.000000 iceberg-dsl-0.0.5/iceberg/core/drawable.py
+-rw-rw-rw-   0        0        0    15185 2023-07-05 08:20:47.000000 iceberg-dsl-0.0.5/iceberg/core/properties.py
+-rw-rw-rw-   0        0        0     5316 2023-07-05 08:03:44.000000 iceberg-dsl-0.0.5/iceberg/core/renderer.py
+-rw-rw-rw-   0        0        0     2788 2023-03-01 05:13:30.000000 iceberg-dsl-0.0.5/iceberg/geometry.py
+drwxrwxrwx   0        0        0        0 2023-07-06 01:09:34.936730 iceberg-dsl-0.0.5/iceberg/primitives/
+-rw-rw-rw-   0        0        0      432 2023-07-05 08:03:44.000000 iceberg-dsl-0.0.5/iceberg/primitives/__init__.py
+-rw-rw-rw-   0        0        0     1124 2023-06-21 07:44:59.000000 iceberg-dsl-0.0.5/iceberg/primitives/filters.py
+-rw-rw-rw-   0        0        0     1542 2023-07-03 22:55:06.000000 iceberg-dsl-0.0.5/iceberg/primitives/image.py
+-rw-rw-rw-   0        0        0     4325 2023-06-23 06:40:33.000000 iceberg-dsl-0.0.5/iceberg/primitives/latex.py
+-rw-rw-rw-   0        0        0    14638 2023-07-05 08:20:47.000000 iceberg-dsl-0.0.5/iceberg/primitives/layout.py
+-rw-rw-rw-   0        0        0     7316 2023-07-05 08:20:47.000000 iceberg-dsl-0.0.5/iceberg/primitives/shapes.py
+-rw-rw-rw-   0        0        0     1612 2023-06-23 04:10:37.000000 iceberg-dsl-0.0.5/iceberg/primitives/svg.py
+-rw-rw-rw-   0        0        0     4338 2023-06-23 05:34:56.000000 iceberg-dsl-0.0.5/iceberg/primitives/text.py
+-rw-rw-rw-   0        0        0     1281 2023-06-21 18:54:51.000000 iceberg-dsl-0.0.5/iceberg/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 01:09:34.959731 iceberg-dsl-0.0.5/iceberg_dsl.egg-info/
+-rw-rw-rw-   0        0        0     5814 2023-07-06 01:09:34.000000 iceberg-dsl-0.0.5/iceberg_dsl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      914 2023-07-06 01:09:34.000000 iceberg-dsl-0.0.5/iceberg_dsl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 01:09:34.000000 iceberg-dsl-0.0.5/iceberg_dsl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-07-06 01:09:34.000000 iceberg-dsl-0.0.5/iceberg_dsl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-06 01:09:34.000000 iceberg-dsl-0.0.5/iceberg_dsl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1111 2023-07-06 01:09:35.005731 iceberg-dsl-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      488 2023-06-21 20:31:57.000000 iceberg-dsl-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 01:09:35.002731 iceberg-dsl-0.0.5/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-04 22:12:48.000000 iceberg-dsl-0.0.5/tests/__init__.py
+-rw-rw-rw-   0        0        0     2692 2023-07-05 08:03:44.000000 iceberg-dsl-0.0.5/tests/scene_tester.py
+-rw-rw-rw-   0        0        0      461 2023-07-05 08:03:44.000000 iceberg-dsl-0.0.5/tests/test_blank.py
+-rw-rw-rw-   0        0        0     2339 2023-07-05 08:03:44.000000 iceberg-dsl-0.0.5/tests/test_connect.py
+-rw-rw-rw-   0        0        0      620 2023-07-05 08:03:44.000000 iceberg-dsl-0.0.5/tests/test_filters.py
+-rw-rw-rw-   0        0        0     3380 2023-07-05 01:21:02.000000 iceberg-dsl-0.0.5/tests/test_neural_net.py
+-rw-rw-rw-   0        0        0     1685 2023-07-05 08:03:44.000000 iceberg-dsl-0.0.5/tests/test_paths.py
+-rw-rw-rw-   0        0        0     1137 2023-07-04 22:12:48.000000 iceberg-dsl-0.0.5/tests/test_quickstart.py
```

### Comparing `iceberg-dsl-0.0.4/LICENSE` & `iceberg-dsl-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.4/PKG-INFO` & `iceberg-dsl-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceberg-dsl
-Version: 0.0.4
+Version: 0.0.5
 Summary: A compositional diagramming tool for Python.
 Home-page: https://github.com/revalo/iceberg
 Author: Shreyas Kapur
 Author-email: srkp@berkeley.edu
 Maintainer: Shreyas Kapur
 Maintainer-email: srkp@berkeley.edu
 License: MIT
@@ -30,15 +30,15 @@
 
 ![PyPI](https://img.shields.io/pypi/v/iceberg-dsl)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/iceberg-dsl)
 ![GitHub](https://img.shields.io/github/license/revalo/iceberg)
 
 
 <p align="center">
-<img src="images/logo.png" width="150">
+<img src="images/logo.gif" width="150">
 </p>
 
 Iceberg is a compositional diagramming and graphics library embedding in Python. It is designed to be performant, extensible, and easy to use.
 
 ## Testimonials
 
 <p align="left">
@@ -50,15 +50,15 @@
 
 ## Showcase
 
 ### Neural Network
 
 A composable Neural Network diagramming class written in iceberg. Full example in `examples/neural_network.py`.
 
-<img src="images/nn.png" width="500">
+<img src="images/nn.gif" width="500">
 
 ```python
 network = NeuralNetwork(
     # Number of nodes in each layer!
     [3, 4, 4, 2],
     node_border_color=Colors.BLACK,
     line_path_style=PathStyle(Colors.BLACK, thickness=3),
```

### Comparing `iceberg-dsl-0.0.4/README.md` & `iceberg-dsl-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ![PyPI](https://img.shields.io/pypi/v/iceberg-dsl)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/iceberg-dsl)
 ![GitHub](https://img.shields.io/github/license/revalo/iceberg)
 
 
 <p align="center">
-<img src="images/logo.png" width="150">
+<img src="images/logo.gif" width="150">
 </p>
 
 Iceberg is a compositional diagramming and graphics library embedding in Python. It is designed to be performant, extensible, and easy to use.
 
 ## Testimonials
 
 <p align="left">
@@ -22,15 +22,15 @@
 
 ## Showcase
 
 ### Neural Network
 
 A composable Neural Network diagramming class written in iceberg. Full example in `examples/neural_network.py`.
 
-<img src="images/nn.png" width="500">
+<img src="images/nn.gif" width="500">
 
 ```python
 network = NeuralNetwork(
     # Number of nodes in each layer!
     [3, 4, 4, 2],
     node_border_color=Colors.BLACK,
     line_path_style=PathStyle(Colors.BLACK, thickness=3),
```

### Comparing `iceberg-dsl-0.0.4/iceberg/arrows/__init__.py` & `iceberg-dsl-0.0.5/iceberg/arrows/__init__.py`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.4/iceberg/core/drawable.py` & `iceberg-dsl-0.0.5/iceberg/core/drawable.py`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.4/iceberg/core/properties.py` & `iceberg-dsl-0.0.5/iceberg/core/properties.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import List, Optional, Tuple
 from enum import Enum
 
 import skia
 import numpy as np
 
 from iceberg.geometry import apply_transform
+from iceberg.animation.animatable import Animatable
 
 
 class Corner(object):
     """Specifies the index of the corner in a corners array."""
 
     TOP_LEFT = 0
     TOP_MIDDLE = 1
@@ -19,15 +20,15 @@
     BOTTOM_RIGHT = 4
     BOTTOM_MIDDLE = 5
     BOTTOM_LEFT = 6
     MIDDLE_LEFT = 7
     CENTER = 8
 
 
-class Bounds(object):
+class Bounds(Animatable):
     """Represents a bounding box."""
 
     def __init__(
         self,
         top: float = 0,
         left: float = 0,
         bottom: float = None,
@@ -73,14 +74,22 @@
         self._left = left
         self._right = right
         self._top = top
         self._bottom = bottom
 
         self._compute_corners()
 
+    @property
+    def animatables(self):
+        return [np.array([self.left, self.top, self.right, self.bottom])]
+
+    def copy_with_animatables(self, animatables):
+        scalars = animatables[0]
+        return Bounds(*scalars)
+
     def transform(self, transform: np.ndarray):
         """Transform the bounds by the specified transform matrix.
 
         Args:
             transform: The 3x3 transform matrix to apply.
 
         Returns:
@@ -228,15 +237,15 @@
         Returns:
             The corners of the bounds.
         """
 
         return self._computed_corners
 
 
-class Color(object):
+class Color(Animatable):
     def __init__(self, r: float, g: float, b: float, a: float = 1.0) -> None:
         """Create a color object.
 
         The color components should be in the range [0, 1].
 
         Args:
             r: The red component of the color.
@@ -252,14 +261,22 @@
 
         self._r = r
         self._g = g
         self._b = b
         self._a = a
 
     @property
+    def animatables(self):
+        return [np.array([self.r, self.g, self.b, self.a])]
+
+    def copy_with_animatables(self, animatables):
+        r, g, b, a = animatables[0]
+        return Color(r, g, b, a)
+
+    @property
     def r(self) -> float:
         return self._r
 
     @property
     def g(self) -> float:
         return self._g
 
@@ -393,47 +410,69 @@
     """The cap at the end of a stroke."""
 
     BUTT = skia.Paint.kButt_Cap
     ROUND = skia.Paint.kRound_Cap
     SQUARE = skia.Paint.kSquare_Cap
 
 
-class PathStyle(object):
+class PathStyle(Animatable):
     """A style for drawing paths."""
 
     def __init__(
         self,
         color: Color,
         thickness: float = 1.0,
         anti_alias: bool = True,
         stroke: bool = True,
         stroke_cap: StrokeCap = StrokeCap.BUTT,
+        dashed: bool = False,
+        dash_intervals: List[float] = [20, 10],
+        dash_phase: float = 0,
     ):
         """Create a path style.
 
         Args:
             color: The color of the path.
             thickness: The thickness of the path.
             anti_alias: Whether to use anti-aliasing.
             stroke: Whether to stroke the path or fill it.
             stroke_cap: The cap at the end of a stroke.
+            dashed: Whether to draw the path dashed.
+            dash_intervals: The intervals for the dashed path.
+            dash_phase: The phase of the dashed path.
         """
 
         self._color = color
         self._thickness = thickness
         self._anti_alias = anti_alias
         self._stroke = stroke
         self._stroke_cap = stroke_cap
 
         self._skia_paint = skia.Paint(
             Style=skia.Paint.kStroke_Style if stroke else skia.Paint.kFill_Style,
             AntiAlias=anti_alias,
             StrokeWidth=thickness,
             Color4f=color.to_skia(),
             StrokeCap=stroke_cap.value,
+            PathEffect=skia.DashPathEffect.Make(
+                intervals=dash_intervals, phase=dash_phase
+            )
+            if dashed
+            else None,
+        )
+
+    @property
+    def animatables(self):
+        return [self.color, self.thickness]
+
+    def copy_with_animatables(self, animatables):
+        color, thickness = animatables
+
+        return PathStyle(
+            color, thickness, self._anti_alias, self._stroke, self._stroke_cap
         )
 
     @property
     def color(self) -> Color:
         return self._color
 
     @property
@@ -444,49 +483,52 @@
     def anti_alias(self) -> bool:
         return self._anti_alias
 
     @property
     def skia_paint(self) -> skia.Paint:
         return self._skia_paint
 
+    def __repr__(self) -> str:
+        return f"PathStyle({self.color}, {self.thickness}, {self.anti_alias}, {self._stroke}, {self._stroke_cap})"
+
 
 @dataclass
 class FontStyle(object):
     class Style(Enum):
         NORMAL = skia.FontStyle.Normal()
         ITALIC = skia.FontStyle.Italic()
         BOLD = skia.FontStyle.Bold()
         BOLD_ITALIC = skia.FontStyle.BoldItalic()
 
-    family: str
+    family: str = None
     filename: str = None
     size: float = 16
     font_weight: int = 400
     font_style: Style = Style.NORMAL
     color: Color = Color(0, 0, 0)
     anti_alias: bool = True
 
     def __post_init__(self):
         families = set(FontStyle.available_fonts())
         if self.filename is None and not self.family in families:
             raise ValueError(
-                f"Invalid font family: {self.family}. Please call FontStyle.get_available_fonts_families() to get the list of available fonts."
+                f"Invalid font family: {self.family}. Please call FontStyle.available_fonts() to get the list of available fonts."
             )
 
     def get_skia_paint(self) -> skia.Paint:
         return skia.Paint(
             Style=skia.Paint.kFill_Style,
             AntiAlias=self.anti_alias,
             Color4f=self.color.to_skia(),
         )
 
     def get_skia_font(self) -> skia.Font:
         if self.filename is not None:
             return skia.Font(
-                skia.Typeface.MakeFromFile(self.filename, self.font_style.value),
+                skia.Typeface.MakeFromFile(self.filename),
                 self.size,
             )
 
         return skia.Font(
             skia.Typeface(self.family, self.font_style.value),
             self.size,
         )
```

### Comparing `iceberg-dsl-0.0.4/iceberg/core/renderer.py` & `iceberg-dsl-0.0.5/iceberg/core/renderer.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Union
 from .drawable import Drawable
 from .properties import Color
 
 import skia
 import glfw
 import re
+import os
 
 import numpy as np
 
 
 def get_skia_surface(width, height):
     """Creates a Skia surface for rendering to on the GPU.
 
@@ -104,26 +105,32 @@
 
         Returns:
             The rendered image as a numpy array.
         """
 
         # TODO(revalo): Convert BGR to RGB via Skia.
         image = self._skia_surface.makeImageSnapshot()
-        array = image.toarray()
-        array = array[:, :, [2, 1, 0, 3]]
+        array = image.toarray(colorType=skia.ColorType.kRGBA_8888_ColorType)
 
         return array
 
     def save_rendered_image(self, path: Union[str, Path]):
         """Saves the rendered image to the given path.
 
         Args:
             path: The path to save the image to.
         """
 
+        path = Path(path)
+
+        if not path.parent.exists():
+            raise RuntimeError(
+                f"Destination directory {path.parent} does not exist. Please create it first."
+            )
+
         image = self._skia_surface.makeImageSnapshot()
         image.save(str(path))
 
     def _create_gpu_surface(self):
         return get_skia_surface(self._bounds.width, self._bounds.height)
 
     def _create_cpu_surface(self):
```

### Comparing `iceberg-dsl-0.0.4/iceberg/geometry.py` & `iceberg-dsl-0.0.5/iceberg/geometry.py`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.4/iceberg/primitives/filters.py` & `iceberg-dsl-0.0.5/iceberg/primitives/filters.py`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.4/iceberg/primitives/image.py` & `iceberg-dsl-0.0.5/iceberg/primitives/image.py`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.4/iceberg/primitives/latex.py` & `iceberg-dsl-0.0.5/iceberg/primitives/latex.py`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.4/iceberg/primitives/layout.py` & `iceberg-dsl-0.0.5/iceberg/primitives/layout.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import List, Sequence, Tuple, Union
 import skia
 
 from iceberg import Drawable, Bounds, Color, Colors
+from iceberg.animation import Animatable
+from iceberg.animation.animatable import AnimatableSequence
 from iceberg.core.drawable import Drawable
 from iceberg.geometry import get_transform, apply_transform
 from dataclasses import dataclass
 from abc import ABC, abstractmethod, abstractproperty
 from enum import Enum
 import numpy as np
 
@@ -50,15 +52,15 @@
     def bounds(self) -> Bounds:
         return self._bounds
 
     def draw(self, canvas: skia.Canvas) -> None:
         canvas.drawRect(self._bounds.to_skia(), self._paint)
 
 
-class Transform(Drawable):
+class Transform(Drawable, Animatable):
     """A drawable that transforms its child."""
 
     def __init__(
         self,
         child: Drawable,
         position: Tuple[float, float] = (0, 0),
         scale: Tuple[float, float] = (1, 1),
@@ -79,14 +81,16 @@
 
         super().__init__()
 
         self._child = child
         self._position = position
         self._scale = scale
         self._anchor = anchor
+        self._rotation = rotation
+        self._rotation_in_degrees = rotation_in_degrees
 
         self._child_bounds = self._child.bounds
 
         # Compute the bounds of the transformed child.
         left, top = self._child_bounds.left, self._child_bounds.top
         right, bottom = self._child_bounds.right, self._child_bounds.bottom
 
@@ -145,14 +149,48 @@
 
     def draw(self, canvas: skia.Canvas):
         canvas.save()
         canvas.concat(self._skia_matrix)
         self._child.draw(canvas)
         canvas.restore()
 
+    @property
+    def animatables(self) -> AnimatableSequence:
+        position = np.array(self._position)
+        scale = np.array(self._scale)
+        anchor = np.array(self._anchor)
+
+        rv = [
+            position,
+            scale,
+            anchor,
+            self._rotation,
+        ]
+
+        if isinstance(self._child, Animatable):
+            rv.append(self._child)
+
+        return rv
+
+    def copy_with_animatables(self, animatables: AnimatableSequence):
+        if len(animatables) == 4:
+            position, scale, anchor, rotation = animatables
+            child = self._child
+        else:
+            position, scale, anchor, rotation, child = animatables
+
+        return Transform(
+            child=child,
+            position=tuple(position),
+            scale=tuple(scale),
+            anchor=tuple(anchor),
+            rotation=rotation,
+            rotation_in_degrees=self._rotation_in_degrees,
+        )
+
 
 class Padding(Transform):
     """A drawable that pads its child."""
 
     def __init__(
         self,
         child: Drawable,
@@ -185,14 +223,19 @@
             )
 
         self._padding = padding
         self._child_bounds = self._child.bounds
 
         pl, pt, pr, pb = self._padding
 
+        self._pl = pl
+        self._pt = pt
+        self._pr = pr
+        self._pb = pb
+
         self._padded_bounds = Bounds(
             left=self._child_bounds.left - pl,
             top=self._child_bounds.top - pt,
             right=self._child_bounds.right + pr,
             bottom=self._child_bounds.bottom + pb,
         )
 
@@ -201,16 +244,28 @@
             position=(0, 0),
         )
 
     @property
     def bounds(self) -> Bounds:
         return self._padded_bounds
 
+    @property
+    def animatables(self) -> AnimatableSequence:
+        return [self._pl, self._pt, self._pr, self._pb, self._child]
+
+    def copy_with_animatables(self, animatables: AnimatableSequence):
+        pl, pt, pr, pb, child = animatables
 
-class Compose(Drawable):
+        return Padding(
+            child=child,
+            padding=(pl, pt, pr, pb),
+        )
+
+
+class Compose(Drawable, Animatable):
     """A drawable that composes its children."""
 
     def __init__(self, children: Tuple[Drawable, ...]):
         """Initialize a compose drawable.
 
         Args:
             children: The children to compose.
@@ -229,26 +284,44 @@
             self._composed_bounds = Bounds(
                 left=left,
                 top=top,
                 right=right,
                 bottom=bottom,
             )
 
+        self._animatables = []
+        self._animatables_indices = []
+
+        for i, child in enumerate(self._children):
+            if isinstance(child, Animatable):
+                self._animatables.append(child)
+                self._animatables_indices.append(i)
+
     @property
     def children(self) -> Sequence[Drawable]:
         return self._children
 
     @property
     def bounds(self) -> Bounds:
         return self._composed_bounds
 
     def draw(self, canvas: skia.Canvas):
         for child in self._children:
             child.draw(canvas)
 
+    @property
+    def animatables(self) -> AnimatableSequence:
+        return self._animatables
+
+    def copy_with_animatables(self, animatables: AnimatableSequence):
+        children = list(self.children)
+        for i, animatable in zip(self._animatables_indices, animatables):
+            children[i] = animatable
+        return Compose(tuple(children))
+
 
 class Anchor(Compose):
     """A drawable that composes it's children without expanding the
     borders.
     """
 
     def __init__(self, children: Tuple[Drawable, ...], anchor_index: int = 0):
```

### Comparing `iceberg-dsl-0.0.4/iceberg/primitives/svg.py` & `iceberg-dsl-0.0.5/iceberg/primitives/svg.py`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.4/iceberg/primitives/text.py` & `iceberg-dsl-0.0.5/iceberg/primitives/text.py`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.4/iceberg/utils.py` & `iceberg-dsl-0.0.5/iceberg/utils.py`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.4/iceberg_dsl.egg-info/PKG-INFO` & `iceberg-dsl-0.0.5/iceberg_dsl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceberg-dsl
-Version: 0.0.4
+Version: 0.0.5
 Summary: A compositional diagramming tool for Python.
 Home-page: https://github.com/revalo/iceberg
 Author: Shreyas Kapur
 Author-email: srkp@berkeley.edu
 Maintainer: Shreyas Kapur
 Maintainer-email: srkp@berkeley.edu
 License: MIT
@@ -30,15 +30,15 @@
 
 ![PyPI](https://img.shields.io/pypi/v/iceberg-dsl)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/iceberg-dsl)
 ![GitHub](https://img.shields.io/github/license/revalo/iceberg)
 
 
 <p align="center">
-<img src="images/logo.png" width="150">
+<img src="images/logo.gif" width="150">
 </p>
 
 Iceberg is a compositional diagramming and graphics library embedding in Python. It is designed to be performant, extensible, and easy to use.
 
 ## Testimonials
 
 <p align="left">
@@ -50,15 +50,15 @@
 
 ## Showcase
 
 ### Neural Network
 
 A composable Neural Network diagramming class written in iceberg. Full example in `examples/neural_network.py`.
 
-<img src="images/nn.png" width="500">
+<img src="images/nn.gif" width="500">
 
 ```python
 network = NeuralNetwork(
     # Number of nodes in each layer!
     [3, 4, 4, 2],
     node_border_color=Colors.BLACK,
     line_path_style=PathStyle(Colors.BLACK, thickness=3),
```

### Comparing `iceberg-dsl-0.0.4/iceberg_dsl.egg-info/SOURCES.txt` & `iceberg-dsl-0.0.5/iceberg_dsl.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 iceberg/__init__.py
 iceberg/geometry.py
 iceberg/utils.py
+iceberg/animation/__init__.py
+iceberg/animation/animatable.py
+iceberg/animation/scene.py
+iceberg/animation/tween.py
 iceberg/arrows/__init__.py
 iceberg/core/__init__.py
 iceberg/core/drawable.py
 iceberg/core/properties.py
 iceberg/core/renderer.py
 iceberg/primitives/__init__.py
 iceberg/primitives/filters.py
@@ -23,9 +27,11 @@
 iceberg_dsl.egg-info/dependency_links.txt
 iceberg_dsl.egg-info/requires.txt
 iceberg_dsl.egg-info/top_level.txt
 tests/__init__.py
 tests/scene_tester.py
 tests/test_blank.py
 tests/test_connect.py
+tests/test_filters.py
 tests/test_neural_net.py
+tests/test_paths.py
 tests/test_quickstart.py
```

### Comparing `iceberg-dsl-0.0.4/setup.cfg` & `iceberg-dsl-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.4/tests/test_connect.py` & `iceberg-dsl-0.0.5/tests/test_connect.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,19 +12,19 @@
     Compose,
     Text,
     MathTex,
 )
 from iceberg.arrows import Arrow, LabelArrow
 
 from .scene_tester import check_render
+import os
 
 
 def test_connect():
     # What font?
-    _FONT_FAMILY = "Arial"
     _CIRCLE_WIDTH = 100
     _BORDER_THICKNESS = 8
     _CIRCLE_PAD = 20
 
     left_ellipse = Ellipse(
         Bounds(size=(_CIRCLE_WIDTH, _CIRCLE_WIDTH)),
         border_color=Color.from_hex("#d63031"),
@@ -62,17 +62,17 @@
         arrow_label,
         Corner.BOTTOM_MIDDLE,
         distance=20,
     )
     connection = Compose([ellipses, arrow])
 
     text_block = Text(
-        "This is some really long text, and it's going to wrap around at some point, because it's so long and I spent a lot of time on it.",
+        "This is some really long text, and it's going to wrap around at some point, because it's so long and I spent a lot of time.",
         font_style=FontStyle(
-            family=_FONT_FAMILY,
+            filename=os.path.join("tests", "testdata", "OpenSans-Regular.ttf"),
             size=28,
             color=Colors.BLACK,
         ),
         width=connection.bounds.width,
     )
 
     scene = Arrange(
```

### Comparing `iceberg-dsl-0.0.4/tests/test_neural_net.py` & `iceberg-dsl-0.0.5/tests/test_neural_net.py`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.4/tests/test_quickstart.py` & `iceberg-dsl-0.0.5/tests/test_quickstart.py`

 * *Files identical despite different names*

