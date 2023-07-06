# Comparing `tmp/pylinalg-0.4.0.tar.gz` & `tmp/pylinalg-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylinalg-0.4.0.tar", max compression
+gzip compressed data, was "pylinalg-0.4.1.tar", max compression
```

## Comparing `pylinalg-0.4.0.tar` & `pylinalg-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-05-08 14:13:36.995311 pylinalg-0.4.0/LICENSE
--rw-r--r--   0        0        0      595 2023-05-08 14:13:36.995311 pylinalg-0.4.0/README.md
--rw-r--r--   0        0        0      390 2023-05-08 14:13:36.995311 pylinalg-0.4.0/pylinalg/__init__.py
--rw-r--r--   0        0        0    19853 2023-05-08 14:13:36.995311 pylinalg-0.4.0/pylinalg/matrix.py
--rw-r--r--   0        0        0     4728 2023-05-08 14:13:36.995311 pylinalg-0.4.0/pylinalg/misc.py
--rw-r--r--   0        0        0     9279 2023-05-08 14:13:36.995311 pylinalg-0.4.0/pylinalg/quaternion.py
--rw-r--r--   0        0        0    16499 2023-05-08 14:13:36.995311 pylinalg-0.4.0/pylinalg/vector.py
--rw-r--r--   0        0        0      900 2023-05-08 14:13:36.995311 pylinalg-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 pylinalg-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-06 09:44:29.916981 pylinalg-0.4.1/LICENSE
+-rw-r--r--   0        0        0      595 2023-07-06 09:44:29.916981 pylinalg-0.4.1/README.md
+-rw-r--r--   0        0        0      390 2023-07-06 09:44:29.920981 pylinalg-0.4.1/pylinalg/__init__.py
+-rw-r--r--   0        0        0    20667 2023-07-06 09:44:29.920981 pylinalg-0.4.1/pylinalg/matrix.py
+-rw-r--r--   0        0        0     4728 2023-07-06 09:44:29.920981 pylinalg-0.4.1/pylinalg/misc.py
+-rw-r--r--   0        0        0     9279 2023-07-06 09:44:29.920981 pylinalg-0.4.1/pylinalg/quaternion.py
+-rw-r--r--   0        0        0    16499 2023-07-06 09:44:29.920981 pylinalg-0.4.1/pylinalg/vector.py
+-rw-r--r--   0        0        0      900 2023-07-06 09:44:29.920981 pylinalg-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 pylinalg-0.4.1/PKG-INFO
```

### Comparing `pylinalg-0.4.0/LICENSE` & `pylinalg-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylinalg-0.4.0/README.md` & `pylinalg-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pylinalg-0.4.0/pylinalg/matrix.py` & `pylinalg-0.4.1/pylinalg/matrix.py`

 * *Files 9% similar despite different names*

```diff
@@ -315,23 +315,28 @@
             mat_from_scale(scaling),
         ],
         out=out,
         dtype=dtype,
     )
 
 
-def mat_decompose(matrix, /, *, dtype=None, out=None):
+def mat_decompose(matrix, /, *, scaling_signs=None, dtype=None, out=None):
     """
     Decompose a transformation matrix into a translation vector, a
     quaternion and a scaling vector.
 
     Parameters
     ----------
     matrix : ndarray, [4, 4]
         transformation matrix
+    scaling_signs : ndarray, [3], optional
+        scaling factor signs. If you wish to preserve the original scaling
+        factors through a compose-decompose roundtrip, you should
+        provide the original scaling factors here, or alternatively just
+        the signs.
     out : ndarray, optional
         A location into which the result is stored. If provided, it
         must have a shape that the inputs broadcast to. If not provided or
         None, a freshly-allocated array is returned. A tuple must have
         length equal to the number of outputs.
     dtype : data-type, optional
         Overrides the data type of the result.
@@ -339,31 +344,43 @@
     Returns
     -------
     translation : ndarray, [3]
         translation vector
     rotation : ndarray, [4]
         quaternion
     scaling : ndarray, [3]
-        scaling factor(s)
+        scaling factors
     """
     matrix = np.asarray(matrix)
 
     if out is not None:
         translation = out[0]
     else:
         translation = np.empty((3,), dtype=dtype)
     translation[:] = matrix[:-1, -1]
 
+    flip = 1 if np.linalg.det(matrix) >= 0 else -1
+    if scaling_signs is not None:
+        # if the user provides the scaling signs, always use them
+        scaling_signs = np.sign(scaling_signs)
+        if np.prod(scaling_signs) != flip:
+            raise ValueError(
+                "Number of negative signs is inconsistent with the determinant"
+            )
+    else:
+        # if not, detect if a flip is needed to reconstruct the transform
+        # and apply it to the first axis arbitrarily
+        scaling_signs = np.array([flip, 1, 1])
+
     if out is not None:
         scaling = out[2]
     else:
         scaling = np.empty((3,), dtype=dtype)
     scaling[:] = np.linalg.norm(matrix[:-1, :-1], axis=0)
-    if np.linalg.det(matrix) < 0:
-        scaling[0] *= -1
+    scaling *= scaling_signs
 
     rotation = out[1] if out is not None else None
     rotation_matrix = matrix[:-1, :-1] * (1 / scaling)[None, :]
     rotation = quat_from_mat(rotation_matrix, out=rotation, dtype=dtype)
 
     return translation, rotation, scaling
```

### Comparing `pylinalg-0.4.0/pylinalg/misc.py` & `pylinalg-0.4.1/pylinalg/misc.py`

 * *Files identical despite different names*

### Comparing `pylinalg-0.4.0/pylinalg/quaternion.py` & `pylinalg-0.4.1/pylinalg/quaternion.py`

 * *Files identical despite different names*

### Comparing `pylinalg-0.4.0/pylinalg/vector.py` & `pylinalg-0.4.1/pylinalg/vector.py`

 * *Files identical despite different names*

### Comparing `pylinalg-0.4.0/pyproject.toml` & `pylinalg-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylinalg"
-version = "0.4.0"
+version = "0.4.1"
 description = "Linear algebra utilities for Python"
 authors = ["Korijn van Golen <korijn@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/pygfx/pylinalg"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `pylinalg-0.4.0/PKG-INFO` & `pylinalg-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylinalg
-Version: 0.4.0
+Version: 0.4.1
 Summary: Linear algebra utilities for Python
 Home-page: https://github.com/pygfx/pylinalg
 License: MIT
 Author: Korijn van Golen
 Author-email: korijn@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylinalg Version: 0.4.0 Summary: Linear algebra
+Metadata-Version: 2.1 Name: pylinalg Version: 0.4.1 Summary: Linear algebra
 utilities for Python Home-page: https://github.com/pygfx/pylinalg License: MIT
 Author: Korijn van Golen Author-email: korijn@gmail.com Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.20.0) Description-Content-Type: text/markdown #
```

