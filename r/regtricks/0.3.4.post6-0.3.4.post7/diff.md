# Comparing `tmp/regtricks-0.3.4.post6.tar.gz` & `tmp/regtricks-0.3.4.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regtricks-0.3.4.post6.tar", last modified: Mon Jun 12 18:59:31 2023, max compression
+gzip compressed data, was "regtricks-0.3.4.post7.tar", last modified: Thu Jul  6 10:08:25 2023, max compression
```

## Comparing `regtricks-0.3.4.post6.tar` & `regtricks-0.3.4.post7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-06-12 18:59:31.916213 regtricks-0.3.4.post6/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1479 2020-10-22 13:00:54.000000 regtricks-0.3.4.post6/LICENSE
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       42 2020-10-22 13:00:54.000000 regtricks-0.3.4.post6/MANIFEST.in
--rw-r--r--   0 thomaskirk   (501) staff       (20)     1102 2023-06-12 18:59:31.915964 regtricks-0.3.4.post6/PKG-INFO
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      790 2020-10-22 13:00:54.000000 regtricks-0.3.4.post6/README.md
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-06-12 18:59:31.913420 regtricks-0.3.4.post6/regtricks/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      425 2020-10-22 13:00:54.000000 regtricks-0.3.4.post6/regtricks/__init__.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       77 2023-06-12 18:59:31.000000 regtricks-0.3.4.post6/regtricks/_version.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     7508 2022-01-05 10:40:43.000000 regtricks-0.3.4.post6/regtricks/application_helpers.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    15290 2022-02-12 22:48:27.000000 regtricks-0.3.4.post6/regtricks/fnirt_coefficients.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11764 2022-10-27 12:09:55.000000 regtricks-0.3.4.post6/regtricks/image_space.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     8120 2020-10-22 13:00:54.000000 regtricks-0.3.4.post6/regtricks/multiplication.py
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-06-12 18:59:31.915620 regtricks-0.3.4.post6/regtricks/transforms/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      215 2020-10-22 13:00:54.000000 regtricks-0.3.4.post6/regtricks/transforms/__init__.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11498 2021-03-17 16:20:16.000000 regtricks-0.3.4.post6/regtricks/transforms/linear.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    14937 2020-11-23 18:51:42.000000 regtricks-0.3.4.post6/regtricks/transforms/nonlinear.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     8452 2022-05-09 11:26:49.000000 regtricks-0.3.4.post6/regtricks/transforms/transform.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     3258 2020-10-30 18:59:14.000000 regtricks-0.3.4.post6/regtricks/wrappers.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     4387 2020-10-22 13:00:54.000000 regtricks-0.3.4.post6/regtricks/x5_interface.py
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-06-12 18:59:31.914602 regtricks-0.3.4.post6/regtricks.egg-info/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1102 2023-06-12 18:59:31.000000 regtricks-0.3.4.post6/regtricks.egg-info/PKG-INFO
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      561 2023-06-12 18:59:31.000000 regtricks-0.3.4.post6/regtricks.egg-info/SOURCES.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)        1 2023-06-12 18:59:31.000000 regtricks-0.3.4.post6/regtricks.egg-info/dependency_links.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       26 2023-06-12 18:59:31.000000 regtricks-0.3.4.post6/regtricks.egg-info/requires.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       10 2023-06-12 18:59:31.000000 regtricks-0.3.4.post6/regtricks.egg-info/top_level.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       25 2020-10-22 13:00:54.000000 regtricks-0.3.4.post6/requirements.txt
--rw-r--r--   0 thomaskirk   (501) staff       (20)       38 2023-06-12 18:59:31.916260 regtricks-0.3.4.post6/setup.cfg
--rwxr-xr-x   0 thomaskirk   (501) staff       (20)     3590 2022-02-12 22:43:08.000000 regtricks-0.3.4.post6/setup.py
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-06 10:08:25.568839 regtricks-0.3.4.post7/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1479 2020-10-22 13:00:54.000000 regtricks-0.3.4.post7/LICENSE
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       42 2020-10-22 13:00:54.000000 regtricks-0.3.4.post7/MANIFEST.in
+-rw-r--r--   0 thomaskirk   (501) staff       (20)     1102 2023-07-06 10:08:25.568677 regtricks-0.3.4.post7/PKG-INFO
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      790 2020-10-22 13:00:54.000000 regtricks-0.3.4.post7/README.md
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-06 10:08:25.566561 regtricks-0.3.4.post7/regtricks/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      425 2020-10-22 13:00:54.000000 regtricks-0.3.4.post7/regtricks/__init__.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       76 2023-07-06 10:08:25.000000 regtricks-0.3.4.post7/regtricks/_version.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     7508 2022-01-05 10:40:43.000000 regtricks-0.3.4.post7/regtricks/application_helpers.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    15290 2022-02-12 22:48:27.000000 regtricks-0.3.4.post7/regtricks/fnirt_coefficients.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11764 2022-10-27 12:09:55.000000 regtricks-0.3.4.post7/regtricks/image_space.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     8120 2020-10-22 13:00:54.000000 regtricks-0.3.4.post7/regtricks/multiplication.py
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-06 10:08:25.568467 regtricks-0.3.4.post7/regtricks/transforms/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      215 2020-10-22 13:00:54.000000 regtricks-0.3.4.post7/regtricks/transforms/__init__.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11571 2023-07-06 10:05:32.000000 regtricks-0.3.4.post7/regtricks/transforms/linear.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    14937 2020-11-23 18:51:42.000000 regtricks-0.3.4.post7/regtricks/transforms/nonlinear.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     8452 2022-05-09 11:26:49.000000 regtricks-0.3.4.post7/regtricks/transforms/transform.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     3258 2020-10-30 18:59:14.000000 regtricks-0.3.4.post7/regtricks/wrappers.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     4387 2020-10-22 13:00:54.000000 regtricks-0.3.4.post7/regtricks/x5_interface.py
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-06 10:08:25.567884 regtricks-0.3.4.post7/regtricks.egg-info/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1102 2023-07-06 10:08:25.000000 regtricks-0.3.4.post7/regtricks.egg-info/PKG-INFO
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      561 2023-07-06 10:08:25.000000 regtricks-0.3.4.post7/regtricks.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)        1 2023-07-06 10:08:25.000000 regtricks-0.3.4.post7/regtricks.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       26 2023-07-06 10:08:25.000000 regtricks-0.3.4.post7/regtricks.egg-info/requires.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       10 2023-07-06 10:08:25.000000 regtricks-0.3.4.post7/regtricks.egg-info/top_level.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       25 2020-10-22 13:00:54.000000 regtricks-0.3.4.post7/requirements.txt
+-rw-r--r--   0 thomaskirk   (501) staff       (20)       38 2023-07-06 10:08:25.568955 regtricks-0.3.4.post7/setup.cfg
+-rwxr-xr-x   0 thomaskirk   (501) staff       (20)     3590 2022-02-12 22:43:08.000000 regtricks-0.3.4.post7/setup.py
```

### Comparing `regtricks-0.3.4.post6/LICENSE` & `regtricks-0.3.4.post7/LICENSE`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4.post6/PKG-INFO` & `regtricks-0.3.4.post7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regtricks
-Version: 0.3.4.post6
+Version: 0.3.4.post7
 Summary: Tools for manipulating and applying registrations
 Home-page: https://github.com/tomfrankkirk/regtricks
 Author: Tom Kirk
 Author-email: thomas.kirk@eng.ox.ac.uk
 License: BSD-3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `regtricks-0.3.4.post6/README.md` & `regtricks-0.3.4.post7/README.md`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4.post6/regtricks/application_helpers.py` & `regtricks-0.3.4.post7/regtricks/application_helpers.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4.post6/regtricks/fnirt_coefficients.py` & `regtricks-0.3.4.post7/regtricks/fnirt_coefficients.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4.post6/regtricks/image_space.py` & `regtricks-0.3.4.post7/regtricks/image_space.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4.post6/regtricks/multiplication.py` & `regtricks-0.3.4.post7/regtricks/multiplication.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4.post6/regtricks/transforms/linear.py` & `regtricks-0.3.4.post7/regtricks/transforms/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,17 @@
             else: 
                 mat = np.loadtxt(mats)
                 if mat.shape[0] % 4: 
                     raise ValueError("Matrix loaded from %s " % mats, 
                                      "should be sized (4xN) x 4.")
                 mats = [ mat[i*4:(i+1)*4,:] for i in range(mat.shape[0] // 4) ]
 
-            
+        if not mats: 
+            raise RuntimeError("No matrices provided")
+        
         self.__transforms = []
         for mat in mats:
             if isinstance(mat, (np.ndarray, str)): 
                 m = Registration(mat)
             else: 
                 m = mat 
             self.__transforms.append(m)
```

### Comparing `regtricks-0.3.4.post6/regtricks/transforms/nonlinear.py` & `regtricks-0.3.4.post7/regtricks/transforms/nonlinear.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4.post6/regtricks/transforms/transform.py` & `regtricks-0.3.4.post7/regtricks/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4.post6/regtricks/wrappers.py` & `regtricks-0.3.4.post7/regtricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4.post6/regtricks/x5_interface.py` & `regtricks-0.3.4.post7/regtricks/x5_interface.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4.post6/regtricks.egg-info/PKG-INFO` & `regtricks-0.3.4.post7/regtricks.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regtricks
-Version: 0.3.4.post6
+Version: 0.3.4.post7
 Summary: Tools for manipulating and applying registrations
 Home-page: https://github.com/tomfrankkirk/regtricks
 Author: Tom Kirk
 Author-email: thomas.kirk@eng.ox.ac.uk
 License: BSD-3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `regtricks-0.3.4.post6/regtricks.egg-info/SOURCES.txt` & `regtricks-0.3.4.post7/regtricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4.post6/setup.py` & `regtricks-0.3.4.post7/setup.py`

 * *Files identical despite different names*

