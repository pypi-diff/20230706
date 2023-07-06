# Comparing `tmp/RITMO-1.6.0.tar.gz` & `tmp/RITMO-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RITMO-1.6.0.tar", last modified: Thu Jul  6 05:45:45 2023, max compression
+gzip compressed data, was "dist/RITMO-1.6.1.tar", last modified: Thu Jul  6 06:13:35 2023, max compression
```

## Comparing `RITMO-1.6.0.tar` & `RITMO-1.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 rachelstirling   (502) staff       (20)        0 2023-07-06 05:45:45.533535 RITMO-1.6.0/
--rw-r--r--   0 rachelstirling   (502) staff       (20)     1474 2023-01-26 00:45:14.000000 RITMO-1.6.0/LICENSE
--rw-r--r--   0 rachelstirling   (502) staff       (20)       40 2023-01-26 12:47:36.000000 RITMO-1.6.0/MANIFEST.in
--rw-r--r--   0 rachelstirling   (502) staff       (20)     1865 2023-07-06 05:45:45.533048 RITMO-1.6.0/PKG-INFO
--rw-r--r--   0 rachelstirling   (502) staff       (20)     1378 2023-07-06 00:44:12.000000 RITMO-1.6.0/README.md
-drwxr-xr-x   0 rachelstirling   (502) staff       (20)        0 2023-07-06 05:45:45.525859 RITMO-1.6.0/RITMO.egg-info/
--rw-r--r--   0 rachelstirling   (502) staff       (20)     1865 2023-07-06 05:45:44.000000 RITMO-1.6.0/RITMO.egg-info/PKG-INFO
--rw-r--r--   0 rachelstirling   (502) staff       (20)      381 2023-07-06 05:45:45.000000 RITMO-1.6.0/RITMO.egg-info/SOURCES.txt
--rw-r--r--   0 rachelstirling   (502) staff       (20)        1 2023-07-06 05:45:45.000000 RITMO-1.6.0/RITMO.egg-info/dependency_links.txt
--rw-r--r--   0 rachelstirling   (502) staff       (20)      132 2023-07-06 05:45:45.000000 RITMO-1.6.0/RITMO.egg-info/requires.txt
--rw-r--r--   0 rachelstirling   (502) staff       (20)        6 2023-07-06 05:45:45.000000 RITMO-1.6.0/RITMO.egg-info/top_level.txt
-drwxr-xr-x   0 rachelstirling   (502) staff       (20)        0 2023-07-06 05:45:45.530638 RITMO-1.6.0/ritmo/
--rw-r--r--   0 rachelstirling   (502) staff       (20)       49 2023-01-14 06:06:41.000000 RITMO-1.6.0/ritmo/__init__.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)       63 2023-01-13 00:49:08.000000 RITMO-1.6.0/ritmo/__version__.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)      191 2023-03-29 00:00:42.000000 RITMO-1.6.0/ritmo/constants.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)     4542 2023-01-27 05:06:32.000000 RITMO-1.6.0/ritmo/cycles.py
-drwxr-xr-x   0 rachelstirling   (502) staff       (20)        0 2023-07-06 05:45:45.532216 RITMO-1.6.0/ritmo/edm/
--rw-r--r--   0 rachelstirling   (502) staff       (20)     2296 2023-01-26 13:26:42.000000 RITMO-1.6.0/ritmo/edm/edm.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)     2650 2023-07-06 00:42:25.000000 RITMO-1.6.0/ritmo/edm/figure.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)     3837 2023-07-06 01:01:04.000000 RITMO-1.6.0/ritmo/edm/statistics.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)    13997 2023-07-06 05:38:07.000000 RITMO-1.6.0/ritmo/main.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)     8003 2023-07-06 05:40:44.000000 RITMO-1.6.0/ritmo/plots.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)     2483 2023-01-26 02:23:06.000000 RITMO-1.6.0/ritmo/statistics.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)     3730 2023-07-06 00:23:50.000000 RITMO-1.6.0/ritmo/utils.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)       38 2023-07-06 05:45:45.533747 RITMO-1.6.0/setup.cfg
--rw-r--r--   0 rachelstirling   (502) staff       (20)     1302 2023-07-06 05:45:31.000000 RITMO-1.6.0/setup.py
+drwxr-xr-x   0 rachelstirling   (502) staff       (20)        0 2023-07-06 06:13:35.000000 RITMO-1.6.1/
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     1474 2023-01-26 00:45:14.000000 RITMO-1.6.1/LICENSE
+-rw-r--r--   0 rachelstirling   (502) staff       (20)       40 2023-01-26 12:47:36.000000 RITMO-1.6.1/MANIFEST.in
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     1828 2023-07-06 06:13:35.000000 RITMO-1.6.1/PKG-INFO
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     1378 2023-07-06 00:44:12.000000 RITMO-1.6.1/README.md
+drwxr-xr-x   0 rachelstirling   (502) staff       (20)        0 2023-07-06 06:13:35.000000 RITMO-1.6.1/RITMO.egg-info/
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     1828 2023-07-06 06:13:35.000000 RITMO-1.6.1/RITMO.egg-info/PKG-INFO
+-rw-r--r--   0 rachelstirling   (502) staff       (20)      381 2023-07-06 06:13:35.000000 RITMO-1.6.1/RITMO.egg-info/SOURCES.txt
+-rw-r--r--   0 rachelstirling   (502) staff       (20)        1 2023-07-06 06:13:35.000000 RITMO-1.6.1/RITMO.egg-info/dependency_links.txt
+-rw-r--r--   0 rachelstirling   (502) staff       (20)      132 2023-07-06 06:13:35.000000 RITMO-1.6.1/RITMO.egg-info/requires.txt
+-rw-r--r--   0 rachelstirling   (502) staff       (20)        6 2023-07-06 06:13:35.000000 RITMO-1.6.1/RITMO.egg-info/top_level.txt
+drwxr-xr-x   0 rachelstirling   (502) staff       (20)        0 2023-07-06 06:13:35.000000 RITMO-1.6.1/ritmo/
+-rw-r--r--   0 rachelstirling   (502) staff       (20)       49 2023-01-14 06:06:41.000000 RITMO-1.6.1/ritmo/__init__.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)       63 2023-01-13 00:49:08.000000 RITMO-1.6.1/ritmo/__version__.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)      191 2023-03-29 00:00:42.000000 RITMO-1.6.1/ritmo/constants.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     4542 2023-01-27 05:06:32.000000 RITMO-1.6.1/ritmo/cycles.py
+drwxr-xr-x   0 rachelstirling   (502) staff       (20)        0 2023-07-06 06:13:35.000000 RITMO-1.6.1/ritmo/edm/
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     2296 2023-01-26 13:26:42.000000 RITMO-1.6.1/ritmo/edm/edm.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     2670 2023-07-06 06:12:09.000000 RITMO-1.6.1/ritmo/edm/figure.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     3837 2023-07-06 01:01:04.000000 RITMO-1.6.1/ritmo/edm/statistics.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)    13997 2023-07-06 05:38:07.000000 RITMO-1.6.1/ritmo/main.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     8003 2023-07-06 05:40:44.000000 RITMO-1.6.1/ritmo/plots.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     2483 2023-01-26 02:23:06.000000 RITMO-1.6.1/ritmo/statistics.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     3730 2023-07-06 00:23:50.000000 RITMO-1.6.1/ritmo/utils.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)       38 2023-07-06 06:13:35.000000 RITMO-1.6.1/setup.cfg
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     1302 2023-07-06 06:13:27.000000 RITMO-1.6.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `RITMO-1.6.0/LICENSE` & `RITMO-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RITMO-1.6.0/PKG-INFO` & `RITMO-1.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: RITMO
-Version: 1.6.0
+Version: 1.6.1
 Summary: Research Investigation of Timeseries with Multiday Oscillations
 Home-page: https://github.com/rachel-stirling/RITMO
 Author: Rachel E. Stirling
 Author-email: rachelstirling1@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Rhythmic Investigation of Timeseries with Multiday Oscillations (RITMO)
@@ -60,9 +58,7 @@
 
 ```python
 export RELEASE=x.x.x
 git commit --allow-empty -m "Release $RELEASE"
 git tag -a $RELEASE -m "Version $RELEASE"
 git push upstream --tags
 ```
-
-
```

### Comparing `RITMO-1.6.0/README.md` & `RITMO-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `RITMO-1.6.0/RITMO.egg-info/PKG-INFO` & `RITMO-1.6.1/RITMO.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: RITMO
-Version: 1.6.0
+Version: 1.6.1
 Summary: Research Investigation of Timeseries with Multiday Oscillations
 Home-page: https://github.com/rachel-stirling/RITMO
 Author: Rachel E. Stirling
 Author-email: rachelstirling1@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Rhythmic Investigation of Timeseries with Multiday Oscillations (RITMO)
@@ -60,9 +58,7 @@
 
 ```python
 export RELEASE=x.x.x
 git commit --allow-empty -m "Release $RELEASE"
 git tag -a $RELEASE -m "Version $RELEASE"
 git push upstream --tags
 ```
-
-
```

### Comparing `RITMO-1.6.0/ritmo/cycles.py` & `RITMO-1.6.1/ritmo/cycles.py`

 * *Files identical despite different names*

### Comparing `RITMO-1.6.0/ritmo/edm/edm.py` & `RITMO-1.6.1/ritmo/edm/edm.py`

 * *Files identical despite different names*

### Comparing `RITMO-1.6.0/ritmo/edm/figure.py` & `RITMO-1.6.1/ritmo/edm/figure.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     if surrogates:
         surr = read_pickle(os.path.join(results_path, "surrogates.pickle"))
         y_5, y_95 = confidence_vals(surr[0], 'y1:y2', int(x1.min()),
                                     int(x1.max()))
         z_5, z_95 = confidence_vals(surr[1], 'y2:y1', int(x2.min()),
                                     int(x2.max()))
-        all_vals = y_95 + y + z_95 + z
+        all_vals = y_95 + y.to_list() + z_95 + z.to_list()
         y_min = min(all_vals)
         y_max = max(all_vals)
     else:
         y_min, y_max = min(y.min(), z.min()) * 0.9, max(y.max(), z.max()) * 1.1
     x_min, x_max = min(x1.min(), x2.min()), max(x1.max(), x2.max())
 
     plt.plot(x1,
```

### Comparing `RITMO-1.6.0/ritmo/edm/statistics.py` & `RITMO-1.6.1/ritmo/edm/statistics.py`

 * *Files identical despite different names*

### Comparing `RITMO-1.6.0/ritmo/main.py` & `RITMO-1.6.1/ritmo/main.py`

 * *Files identical despite different names*

### Comparing `RITMO-1.6.0/ritmo/plots.py` & `RITMO-1.6.1/ritmo/plots.py`

 * *Files identical despite different names*

### Comparing `RITMO-1.6.0/ritmo/statistics.py` & `RITMO-1.6.1/ritmo/statistics.py`

 * *Files identical despite different names*

### Comparing `RITMO-1.6.0/ritmo/utils.py` & `RITMO-1.6.1/ritmo/utils.py`

 * *Files identical despite different names*

### Comparing `RITMO-1.6.0/setup.py` & `RITMO-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Package meta-data.
 NAME = 'RITMO'
 DESCRIPTION = 'Research Investigation of Timeseries with Multiday Oscillations'
 URL = 'https://github.com/rachel-stirling/RITMO'
 EMAIL = 'rachelstirling1@gmail.com'
 AUTHOR = 'Rachel E. Stirling'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '1.6.0'
+VERSION = '1.6.1'
 
 install_requires = [
     'pandas==1.3.5', 'matplotlib==3.5.3', 'numpy==1.21.6', 'pyEDM==1.14.0.0',
     'pymannkendall==1.4.3', 'pycwt==0.3.0a22', 'scikit-learn==1.0.2',
     'scipy==1.7.3'
 ]
```

