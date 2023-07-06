# Comparing `tmp/geotile-0.3.2.tar.gz` & `tmp/geotile-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geotile-0.3.2.tar", last modified: Mon Mar 20 15:43:45 2023, max compression
+gzip compressed data, was "geotile-0.3.3.tar", last modified: Thu Jul  6 00:35:28 2023, max compression
```

## Comparing `geotile-0.3.2.tar` & `geotile-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:43:45.081881 geotile-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-20 15:43:26.000000 geotile-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-03-20 15:43:45.081881 geotile-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-20 15:43:26.000000 geotile-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:43:45.077880 geotile-0.3.2/geotile/
--rw-r--r--   0 runner    (1001) docker     (123)    16491 2023-03-20 15:43:26.000000 geotile-0.3.2/geotile/GeoTile.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-20 15:43:26.000000 geotile-0.3.2/geotile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-20 15:43:26.000000 geotile-0.3.2/geotile/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-03-20 15:43:26.000000 geotile-0.3.2/geotile/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:43:45.077880 geotile-0.3.2/geotile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-03-20 15:43:45.000000 geotile-0.3.2/geotile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-20 15:43:45.000000 geotile-0.3.2/geotile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 15:43:45.000000 geotile-0.3.2/geotile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-20 15:43:45.000000 geotile-0.3.2/geotile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-20 15:43:45.000000 geotile-0.3.2/geotile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 15:43:45.081881 geotile-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-03-20 15:43:26.000000 geotile-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:35:28.978657 geotile-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-06 00:35:09.000000 geotile-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-06 00:35:28.978657 geotile-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-06 00:35:09.000000 geotile-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:35:28.978657 geotile-0.3.3/geotile/
+-rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-07-06 00:35:09.000000 geotile-0.3.3/geotile/GeoTile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 00:35:09.000000 geotile-0.3.3/geotile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-06 00:35:09.000000 geotile-0.3.3/geotile/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-06 00:35:09.000000 geotile-0.3.3/geotile/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:35:28.978657 geotile-0.3.3/geotile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-06 00:35:28.000000 geotile-0.3.3/geotile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-06 00:35:28.000000 geotile-0.3.3/geotile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 00:35:28.000000 geotile-0.3.3/geotile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-06 00:35:28.000000 geotile-0.3.3/geotile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 00:35:28.000000 geotile-0.3.3/geotile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 00:35:28.978657 geotile-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-06 00:35:09.000000 geotile-0.3.3/setup.py
```

### Comparing `geotile-0.3.2/LICENSE` & `geotile-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geotile-0.3.2/PKG-INFO` & `geotile-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geotile
-Version: 0.3.2
+Version: 0.3.3
 Summary: Package for working with geographic raster tiles
 Home-page: https://github.com/iamtekson/geotile
 Author: Tek Kshetri
 Author-email: iamtekson@gmail.com
 License: MIT License
 Keywords: geotile,geotiling,geoTiler,geospatial,geospatial data,geospatial raster tiles,raster tiles,raster,tiles,tile,tiling python,python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `geotile-0.3.2/README.md` & `geotile-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `geotile-0.3.2/geotile/GeoTile.py` & `geotile-0.3.3/geotile/GeoTile.py`

 * *Files 4% similar despite different names*

```diff
@@ -247,18 +247,33 @@
 
         # get the bounds of the vector
         with rio.open(self.path) as src:
             out_image, out_transform = mask(
                 src, df["geometry"], crop=crop, invert=invert, **kwargs)
             out_meta = src.meta.copy()
 
+        # if the raster is 3D, take the first band
+        if out_image.ndim == 3:
+            out_image = out_image[0]
+            
+            # create mask of either 0 or 1
+            out_image = np.where(out_image == 0, 0, 1)
+            
+            # expand the dimension to 3D
+            out_image = np.expand_dims(out_image, axis=0)
+
+        # if the raster is 2D, expand the dimension to 3D
+        elif out_image.ndim == 2:
+            out_image = np.expand_dims(out_image, axis=0)
+
         # update the metadata
         out_meta.update({
             "height": out_image.shape[1],
             "width": out_image.shape[2],
+            'count': 1,
             "transform": out_transform})
 
         # write the output raster
         with rio.open(out_path, 'w', **out_meta) as outds:
             outds.write(out_image)
 
     def rasterization(self, input_vector: str, out_path: str, value_col=None, **kwargs):
```

### Comparing `geotile-0.3.2/geotile/utils.py` & `geotile-0.3.3/geotile/utils.py`

 * *Files identical despite different names*

### Comparing `geotile-0.3.2/geotile.egg-info/PKG-INFO` & `geotile-0.3.3/geotile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geotile
-Version: 0.3.2
+Version: 0.3.3
 Summary: Package for working with geographic raster tiles
 Home-page: https://github.com/iamtekson/geotile
 Author: Tek Kshetri
 Author-email: iamtekson@gmail.com
 License: MIT License
 Keywords: geotile,geotiling,geoTiler,geospatial,geospatial data,geospatial raster tiles,raster tiles,raster,tiles,tile,tiling python,python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `geotile-0.3.2/setup.py` & `geotile-0.3.3/setup.py`

 * *Files identical despite different names*

