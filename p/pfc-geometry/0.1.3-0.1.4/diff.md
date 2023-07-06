# Comparing `tmp/pfc_geometry-0.1.3.tar.gz` & `tmp/pfc_geometry-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfc_geometry-0.1.3.tar", last modified: Mon Jul  3 07:12:05 2023, max compression
+gzip compressed data, was "pfc_geometry-0.1.4.tar", last modified: Thu Jul  6 10:38:39 2023, max compression
```

## Comparing `pfc_geometry-0.1.3.tar` & `pfc_geometry-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-03 07:12:05.082486 pfc_geometry-0.1.3/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7632 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/LICENSE
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1488 2023-07-03 07:12:05.086485 pfc_geometry-0.1.3/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1191 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/README.md
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-03 07:12:05.082486 pfc_geometry-0.1.3/geometry/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1207 2023-05-29 08:21:19.000000 pfc_geometry-0.1.3/geometry/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     8875 2023-03-30 11:31:01.000000 pfc_geometry-0.1.3/geometry/base.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2956 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/geometry/coordinate_frame.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3573 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/geometry/gps.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1271 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/geometry/mass.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4915 2023-06-30 05:30:43.000000 pfc_geometry-0.1.3/geometry/point.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     8830 2023-06-30 13:19:15.000000 pfc_geometry-0.1.3/geometry/quaternion.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      375 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/geometry/testing.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3870 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/geometry/transformation.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-03 07:12:05.082486 pfc_geometry-0.1.3/pfc_geometry.egg-info/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1488 2023-07-03 07:12:05.000000 pfc_geometry-0.1.3/pfc_geometry.egg-info/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      548 2023-07-03 07:12:05.000000 pfc_geometry-0.1.3/pfc_geometry.egg-info/SOURCES.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-07-03 07:12:05.000000 pfc_geometry-0.1.3/pfc_geometry.egg-info/dependency_links.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       24 2023-07-03 07:12:05.000000 pfc_geometry-0.1.3/pfc_geometry.egg-info/requires.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        9 2023-07-03 07:12:05.000000 pfc_geometry-0.1.3/pfc_geometry.egg-info/top_level.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      404 2023-07-03 07:12:05.086485 pfc_geometry-0.1.3/setup.cfg
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      699 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/setup.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-03 07:12:05.082486 pfc_geometry-0.1.3/tests/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5379 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/tests/test_base.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      875 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/tests/test_coord.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1248 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/tests/test_gps.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1163 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/tests/test_mass.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2639 2023-06-30 05:31:54.000000 pfc_geometry-0.1.3/tests/test_point.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5668 2023-06-30 05:34:46.000000 pfc_geometry-0.1.3/tests/test_quaternion.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1650 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/tests/test_transform.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-06 10:38:39.624537 pfc_geometry-0.1.4/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7632 2023-03-28 15:54:20.000000 pfc_geometry-0.1.4/LICENSE
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1524 2023-07-06 10:38:39.624537 pfc_geometry-0.1.4/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1191 2023-03-28 15:54:20.000000 pfc_geometry-0.1.4/README.md
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-06 10:38:39.620537 pfc_geometry-0.1.4/geometry/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1207 2023-05-29 08:21:19.000000 pfc_geometry-0.1.4/geometry/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     8875 2023-03-30 11:31:01.000000 pfc_geometry-0.1.4/geometry/base.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2956 2023-03-28 15:54:20.000000 pfc_geometry-0.1.4/geometry/coordinate_frame.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3573 2023-03-28 15:54:20.000000 pfc_geometry-0.1.4/geometry/gps.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1271 2023-03-28 15:54:20.000000 pfc_geometry-0.1.4/geometry/mass.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4915 2023-06-30 05:30:43.000000 pfc_geometry-0.1.4/geometry/point.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     9167 2023-07-04 22:38:23.000000 pfc_geometry-0.1.4/geometry/quaternion.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      375 2023-03-28 15:54:20.000000 pfc_geometry-0.1.4/geometry/testing.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3870 2023-03-28 15:54:20.000000 pfc_geometry-0.1.4/geometry/transformation.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-06 10:38:39.624537 pfc_geometry-0.1.4/pfc_geometry.egg-info/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1524 2023-07-06 10:38:39.000000 pfc_geometry-0.1.4/pfc_geometry.egg-info/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      548 2023-07-06 10:38:39.000000 pfc_geometry-0.1.4/pfc_geometry.egg-info/SOURCES.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-07-06 10:38:39.000000 pfc_geometry-0.1.4/pfc_geometry.egg-info/dependency_links.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       24 2023-07-06 10:38:39.000000 pfc_geometry-0.1.4/pfc_geometry.egg-info/requires.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-07-06 10:38:39.000000 pfc_geometry-0.1.4/pfc_geometry.egg-info/top_level.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      404 2023-07-06 10:38:39.624537 pfc_geometry-0.1.4/setup.cfg
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      699 2023-03-28 15:54:20.000000 pfc_geometry-0.1.4/setup.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-06 10:38:39.624537 pfc_geometry-0.1.4/tests/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     5379 2023-03-28 15:54:20.000000 pfc_geometry-0.1.4/tests/test_base.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      875 2023-03-28 15:54:20.000000 pfc_geometry-0.1.4/tests/test_coord.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1248 2023-03-28 15:54:20.000000 pfc_geometry-0.1.4/tests/test_gps.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1163 2023-03-28 15:54:20.000000 pfc_geometry-0.1.4/tests/test_mass.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2639 2023-06-30 05:31:54.000000 pfc_geometry-0.1.4/tests/test_point.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     5668 2023-06-30 05:34:46.000000 pfc_geometry-0.1.4/tests/test_quaternion.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1650 2023-03-28 15:54:20.000000 pfc_geometry-0.1.4/tests/test_transform.py
```

### Comparing `pfc_geometry-0.1.3/LICENSE` & `pfc_geometry-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/PKG-INFO` & `pfc_geometry-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: pfc_geometry
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for handling 3D geometry with a nice interface
 Home-page: https://github.com/PyFlightCoach/geometry
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # geometry #
 
 Tools for handling 3D geometry, mostly just adds a nice interface to various geometric enterties. Each geometric entity can also be a vector of geometric entities. Each entity wraps a numpy array with the relevant number of columns labelled according to the cols class property and rows equal to the number of elements in the vector. Attribute access to each column is available and returns a numpy array. 
 
@@ -18,7 +20,8 @@
 
 Many convenience methods and constructors are available. Documentation is limited but if you need something it has probably already been written so check the code first. 
 
 
 now available on pypi:
 
 pip install pfc-geometry
+
```

### Comparing `pfc_geometry-0.1.3/README.md` & `pfc_geometry-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/geometry/__init__.py` & `pfc_geometry-0.1.4/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/geometry/base.py` & `pfc_geometry-0.1.4/geometry/base.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/geometry/coordinate_frame.py` & `pfc_geometry-0.1.4/geometry/coordinate_frame.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/geometry/gps.py` & `pfc_geometry-0.1.4/geometry/gps.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/geometry/mass.py` & `pfc_geometry-0.1.4/geometry/mass.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/geometry/point.py` & `pfc_geometry-0.1.4/geometry/point.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/geometry/quaternion.py` & `pfc_geometry-0.1.4/geometry/quaternion.py`

 * *Files 7% similar despite different names*

```diff
@@ -155,41 +155,51 @@
 
     @staticmethod
     def axis_rates(q: Quaternion, qdot: Quaternion) -> Point:
         wdash = qdot * q.conjugate()
         return wdash.norm().to_axis_angle() 
 
     @staticmethod
+    def _axis_rates(q: Quaternion, qdot: Quaternion) -> Point:
+        wdash = qdot * q.conjugate()
+        return wdash.norm()._to_axis_angle() 
+
+    @staticmethod
     def body_axis_rates(q: Quaternion, qdot: Quaternion) -> Point:
         wdash = q.conjugate() * qdot
         return wdash.norm().to_axis_angle() 
 
+    @staticmethod
+    def _body_axis_rates(q: Quaternion, qdot: Quaternion) -> Point:
+        wdash = q.conjugate() * qdot
+        return wdash.norm()._to_axis_angle() 
+
     def rotate(self, rate: Point) -> Quaternion:
         return (Quaternion.from_axis_angle(rate) * self).norm()
 
     def body_rotate(self, rate: Point) -> Quaternion:
         return (self * Quaternion.from_axis_angle(rate)).norm()
 
     def diff(self, dt: np.array) -> Point:
         """differentiate in the world frame"""
         assert len(dt) == len(self)
         dt = dt * len(dt) / (len(dt) - 1)
 
-        ps = Quaternion.axis_rates(
+        ps = Quaternion._axis_rates(
             Quaternion(self.data[:-1, :]),
             Quaternion(self.data[1:, :])
         ) / dt[:-1]
         return Point(np.vstack([ps.data, ps.data[-1,:]]))#.remove_outliers(2)  # Bodge to get rid of phase jump
 
     def body_diff(self, dt: np.array) -> Point:
         """differentiate in the body frame"""
         assert len(dt) == len(self)
         dt = dt * len(dt) / (len(dt) - 1)
 
-        ps = Quaternion.body_axis_rates(
+        ps = Quaternion._body_axis_rates(
             Quaternion(self.data[:-1, :]),
             Quaternion(self.data[1:, :])
         ) / dt[:-1]
         return Point(np.vstack([ps.data, ps.data[-1,:]]))
 
     
     def to_rotation_matrix(self):
```

### Comparing `pfc_geometry-0.1.3/geometry/transformation.py` & `pfc_geometry-0.1.4/geometry/transformation.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/pfc_geometry.egg-info/PKG-INFO` & `pfc_geometry-0.1.4/pfc_geometry.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: pfc-geometry
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for handling 3D geometry with a nice interface
 Home-page: https://github.com/PyFlightCoach/geometry
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # geometry #
 
 Tools for handling 3D geometry, mostly just adds a nice interface to various geometric enterties. Each geometric entity can also be a vector of geometric entities. Each entity wraps a numpy array with the relevant number of columns labelled according to the cols class property and rows equal to the number of elements in the vector. Attribute access to each column is available and returns a numpy array. 
 
@@ -18,7 +20,8 @@
 
 Many convenience methods and constructors are available. Documentation is limited but if you need something it has probably already been written so check the code first. 
 
 
 now available on pypi:
 
 pip install pfc-geometry
+
```

### Comparing `pfc_geometry-0.1.3/pfc_geometry.egg-info/SOURCES.txt` & `pfc_geometry-0.1.4/pfc_geometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/setup.py` & `pfc_geometry-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/tests/test_base.py` & `pfc_geometry-0.1.4/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/tests/test_coord.py` & `pfc_geometry-0.1.4/tests/test_coord.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/tests/test_gps.py` & `pfc_geometry-0.1.4/tests/test_gps.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/tests/test_mass.py` & `pfc_geometry-0.1.4/tests/test_mass.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/tests/test_point.py` & `pfc_geometry-0.1.4/tests/test_point.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/tests/test_quaternion.py` & `pfc_geometry-0.1.4/tests/test_quaternion.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.3/tests/test_transform.py` & `pfc_geometry-0.1.4/tests/test_transform.py`

 * *Files identical despite different names*

