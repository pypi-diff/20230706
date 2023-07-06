# Comparing `tmp/hdss-1.1.0.tar.gz` & `tmp/hdss-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdss-1.1.0.tar", last modified: Sun Jan 15 11:39:34 2023, max compression
+gzip compressed data, was "hdss-1.1.1.tar", max compression
```

## Comparing `hdss-1.1.0.tar` & `hdss-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,6 @@
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-01-15 11:39:34.067959 hdss-1.1.0/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1258 2023-01-15 11:39:34.067564 hdss-1.1.0/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      718 2022-07-05 12:54:13.000000 hdss-1.1.0/README.md
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-01-15 11:39:34.042806 hdss-1.1.0/hdss/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       48 2022-06-25 08:10:40.000000 hdss-1.1.0/hdss/__init__.py
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     8480 2023-01-15 10:42:27.000000 hdss-1.1.0/hdss/code.py
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-01-15 11:39:34.067088 hdss-1.1.0/hdss.egg-info/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1258 2023-01-15 11:39:34.000000 hdss-1.1.0/hdss.egg-info/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      187 2023-01-15 11:39:34.000000 hdss-1.1.0/hdss.egg-info/SOURCES.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-01-15 11:39:34.000000 hdss-1.1.0/hdss.egg-info/dependency_links.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       29 2023-01-15 11:39:34.000000 hdss-1.1.0/hdss.egg-info/requires.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)        5 2023-01-15 11:39:34.000000 hdss-1.1.0/hdss.egg-info/top_level.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-01-15 11:39:34.068069 hdss-1.1.0/setup.cfg
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1060 2023-01-15 11:34:35.000000 hdss-1.1.0/setup.py
+-rw-r--r--   0        0        0      718 2022-07-05 12:54:13.781427 hdss-1.1.1/README.md
+-rw-r--r--   0        0        0     6148 2023-07-06 10:37:54.977432 hdss-1.1.1/hdss/.DS_Store
+-rw-r--r--   0        0        0       48 2022-06-25 08:10:40.407522 hdss-1.1.1/hdss/__init__.py
+-rw-r--r--   0        0        0     8559 2023-07-06 09:49:51.021515 hdss-1.1.1/hdss/code.py
+-rw-r--r--   0        0        0      363 2023-07-06 10:43:24.726448 hdss-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 hdss-1.1.1/PKG-INFO
```

### Comparing `hdss-1.1.0/PKG-INFO` & `hdss-1.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: hdss
-Version: 1.1.0
+Version: 1.1.1
 Summary: HDSS - Hand-Drawn Shape Simulation
-Home-page: https://boriskravtsov.com/
-Author: Boris Kravtsov
-Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
-Classifier: Intended Audience :: Developers
+Author: Boris Kravtsov
+Author-email: kravtsov.development@gmail.com
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: opencv-python-headless (>=4.8.0.74,<5.0.0.0)
 Description-Content-Type: text/markdown
 
 ## HDSS
 HDSS - Hand-Drawn Shape Simulation
 
 ### Installation
 ```
@@ -29,7 +30,8 @@
 <p>&nbsp;</p>
 <p align="center"><img src="https://boriskravtsov.com/pypi/hdss.png"/>
 <p>&nbsp;</p>
 
 Such distorted forms, "hand-drawn shapes," are handy to test various recognition technologies. 
 [Here](https://kravtsov-development.medium.com/hand-drawn-shape-simulation-a792c9bb2154) 
 we show how to use **hdss package** to generate these objects by using two simple python functions.
+
```

### Comparing `hdss-1.1.0/README.md` & `hdss-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hdss-1.1.0/hdss/code.py` & `hdss-1.1.1/hdss/code.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Jan-15-2023
+# Jul-06-2023
 # code.py
 
 import os
 import cv2 as cv
 import numpy as np
 import random
 
@@ -81,19 +81,19 @@
     channels = 3
     background = 255
     image = np.empty((height, width, channels), dtype=np.uint8)
     image.fill(background)
     # ---------------------------------------------------------
     scale_factor = np.float32(image_size) / np.float32(100)
 
-    M_perspective = (3, 3)
-    M_perspective = np.zeros(M_perspective, dtype=np.float32)
+    matrix_persp = (3, 3)
+    matrix_persp = np.zeros(matrix_persp, dtype=np.float32)
 
     if perspective_flag:
-        M_perspective = set_persp_transform()
+        matrix_persp = set_persp_transform()
     # ---------------------------------------------------------
     for path_curve in curves:
 
         control_points = np.loadtxt(path_curve, delimiter=',')
         n_control_points = control_points.shape[0]
 
         control_points = scale_factor * control_points
@@ -103,15 +103,15 @@
         # -----------------------------------------------------
         if perspective_flag:
 
             for n in range(n_control_points):
                 x_in = control_points[n, 0]
                 y_in = control_points[n, 1]
 
-                x_out, y_out = point_persp_transform(M_perspective, x_in, y_in)
+                x_out, y_out = point_persp_transform(matrix_persp, x_in, y_in)
 
                 control_points[n, 0] = x_out
                 control_points[n, 1] = y_out
         # -----------------------------------------------------
 
         # Random Noise
         # -----------------------------------------------------
@@ -144,35 +144,35 @@
 
         x_bl_in = 0
         y_bl_in = image_size
 
         x_br_in = image_size
         y_br_in = image_size
 
-        M = [[1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]]
+        matrix_persp = [[1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]]
 
-        return M
+        return matrix_persp
 
     # Points order: top-right, top-left, bottom-left, bottom-right
 
     # IN
     # -----------------------------------------------------
     random.seed(None)
 
-    x_tr_in = image_size + random_perspective_shift()
-    y_tr_in = -random_perspective_shift()
+    x_tr_in = image_size + randomatrix_persp_shift()
+    y_tr_in = -randomatrix_persp_shift()
 
-    x_tl_in = -random_perspective_shift()
-    y_tl_in = -random_perspective_shift()
+    x_tl_in = -randomatrix_persp_shift()
+    y_tl_in = -randomatrix_persp_shift()
 
-    x_bl_in = -random_perspective_shift()
-    y_bl_in = image_size + random_perspective_shift()
+    x_bl_in = -randomatrix_persp_shift()
+    y_bl_in = image_size + randomatrix_persp_shift()
 
-    x_br_in = image_size + random_perspective_shift()
-    y_br_in = image_size + random_perspective_shift()
+    x_br_in = image_size + randomatrix_persp_shift()
+    y_br_in = image_size + randomatrix_persp_shift()
     # -----------------------------------------------------
 
     # OUT
     # ---------------------------------------------------------
     x_tr_out = image_size
     y_tr_out = 0
 
@@ -189,31 +189,31 @@
     # ---------------------------------------------------------
     pts1 = np.float32([[x_tr_in, y_tr_in], [x_tl_in, y_tl_in],
                        [x_bl_in, y_bl_in], [x_br_in, y_br_in]])
 
     pts2 = np.float32([[x_tr_out, y_tr_out], [x_tl_out, y_tl_out],
                        [x_bl_out, y_bl_out], [x_br_out, y_br_out]])
 
-    M = cv.getPerspectiveTransform(pts1, pts2)
+    matrix_persp = cv.getPerspectiveTransform(pts1, pts2)
     # ---------------------------------------------------------
 
-    return M
+    return matrix_persp
 
 
-def random_perspective_shift():
+def randomatrix_persp_shift():
 
     global image_size
 
     return random.uniform(0.0, image_size / 2.0)
 
 
-def point_persp_transform(M, x_in, y_in):
-    x_out = M[0, 0] * x_in + M[0, 1] * y_in + M[0, 2]
-    y_out = M[1, 0] * x_in + M[1, 1] * y_in + M[1, 2]
-    z_out = M[2, 0] * x_in + M[2, 1] * y_in + M[2, 2]
+def point_persp_transform(matrix, x_in, y_in):
+    x_out = matrix[0, 0] * x_in + matrix[0, 1] * y_in + matrix[0, 2]
+    y_out = matrix[1, 0] * x_in + matrix[1, 1] * y_in + matrix[1, 2]
+    z_out = matrix[2, 0] * x_in + matrix[2, 1] * y_in + matrix[2, 2]
 
     x_out = x_out / z_out
     y_out = y_out / z_out
 
     return x_out, y_out
 
 
@@ -278,15 +278,14 @@
 """
     Omar Aflak  May 9, 2020.
     https://towardsdatascience.com/bézier-interpolation-8033e9a262c2
     
     Thanks, Omar!!!
 """
 
-
 # find the a & b points
 def get_bezier_coef(points):
     # since the formulas work given that we have n+1 points
     # then n must be this:
     n = len(points) - 1
 
     # build coefficents matrix
```

