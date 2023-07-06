# Comparing `tmp/RITMO-1.5.3.tar.gz` & `tmp/RITMO-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/RITMO-1.5.3.tar", last modified: Sat Apr  8 05:19:52 2023, max compression
+gzip compressed data, was "RITMO-1.6.0.tar", last modified: Thu Jul  6 05:45:45 2023, max compression
```

## Comparing `RITMO-1.5.3.tar` & `RITMO-1.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 rachelstirling   (502) staff       (20)        0 2023-04-08 05:19:52.000000 RITMO-1.5.3/
--rw-r--r--   0 rachelstirling   (502) staff       (20)     1474 2023-01-26 00:45:14.000000 RITMO-1.5.3/LICENSE
--rw-r--r--   0 rachelstirling   (502) staff       (20)       40 2023-01-26 12:47:36.000000 RITMO-1.5.3/MANIFEST.in
--rw-r--r--   0 rachelstirling   (502) staff       (20)     1751 2023-04-08 05:19:52.000000 RITMO-1.5.3/PKG-INFO
--rw-r--r--   0 rachelstirling   (502) staff       (20)     1301 2023-01-27 05:02:28.000000 RITMO-1.5.3/README.md
-drwxr-xr-x   0 rachelstirling   (502) staff       (20)        0 2023-04-08 05:19:52.000000 RITMO-1.5.3/RITMO.egg-info/
--rw-r--r--   0 rachelstirling   (502) staff       (20)     1751 2023-04-08 05:19:52.000000 RITMO-1.5.3/RITMO.egg-info/PKG-INFO
--rw-r--r--   0 rachelstirling   (502) staff       (20)      381 2023-04-08 05:19:52.000000 RITMO-1.5.3/RITMO.egg-info/SOURCES.txt
--rw-r--r--   0 rachelstirling   (502) staff       (20)        1 2023-04-08 05:19:52.000000 RITMO-1.5.3/RITMO.egg-info/dependency_links.txt
--rw-r--r--   0 rachelstirling   (502) staff       (20)      132 2023-04-08 05:19:52.000000 RITMO-1.5.3/RITMO.egg-info/requires.txt
--rw-r--r--   0 rachelstirling   (502) staff       (20)        6 2023-04-08 05:19:52.000000 RITMO-1.5.3/RITMO.egg-info/top_level.txt
-drwxr-xr-x   0 rachelstirling   (502) staff       (20)        0 2023-04-08 05:19:52.000000 RITMO-1.5.3/ritmo/
--rw-r--r--   0 rachelstirling   (502) staff       (20)       49 2023-01-14 06:06:41.000000 RITMO-1.5.3/ritmo/__init__.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)       63 2023-01-13 00:49:08.000000 RITMO-1.5.3/ritmo/__version__.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)      191 2023-03-29 00:00:42.000000 RITMO-1.5.3/ritmo/constants.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)     4542 2023-01-27 05:06:32.000000 RITMO-1.5.3/ritmo/cycles.py
-drwxr-xr-x   0 rachelstirling   (502) staff       (20)        0 2023-04-08 05:19:52.000000 RITMO-1.5.3/ritmo/edm/
--rw-r--r--   0 rachelstirling   (502) staff       (20)     2296 2023-01-26 13:26:42.000000 RITMO-1.5.3/ritmo/edm/edm.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)     2390 2023-01-26 02:29:39.000000 RITMO-1.5.3/ritmo/edm/figure.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)     3650 2023-02-02 03:50:40.000000 RITMO-1.5.3/ritmo/edm/statistics.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)    12878 2023-03-29 00:00:42.000000 RITMO-1.5.3/ritmo/main.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)     6141 2023-03-28 23:30:20.000000 RITMO-1.5.3/ritmo/plots.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)     2483 2023-01-26 02:23:06.000000 RITMO-1.5.3/ritmo/statistics.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)     3203 2023-04-08 05:16:19.000000 RITMO-1.5.3/ritmo/utils.py
--rw-r--r--   0 rachelstirling   (502) staff       (20)       38 2023-04-08 05:19:52.000000 RITMO-1.5.3/setup.cfg
--rw-r--r--   0 rachelstirling   (502) staff       (20)     1302 2023-04-08 05:18:59.000000 RITMO-1.5.3/setup.py
+drwxr-xr-x   0 rachelstirling   (502) staff       (20)        0 2023-07-06 05:45:45.533535 RITMO-1.6.0/
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     1474 2023-01-26 00:45:14.000000 RITMO-1.6.0/LICENSE
+-rw-r--r--   0 rachelstirling   (502) staff       (20)       40 2023-01-26 12:47:36.000000 RITMO-1.6.0/MANIFEST.in
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     1865 2023-07-06 05:45:45.533048 RITMO-1.6.0/PKG-INFO
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     1378 2023-07-06 00:44:12.000000 RITMO-1.6.0/README.md
+drwxr-xr-x   0 rachelstirling   (502) staff       (20)        0 2023-07-06 05:45:45.525859 RITMO-1.6.0/RITMO.egg-info/
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     1865 2023-07-06 05:45:44.000000 RITMO-1.6.0/RITMO.egg-info/PKG-INFO
+-rw-r--r--   0 rachelstirling   (502) staff       (20)      381 2023-07-06 05:45:45.000000 RITMO-1.6.0/RITMO.egg-info/SOURCES.txt
+-rw-r--r--   0 rachelstirling   (502) staff       (20)        1 2023-07-06 05:45:45.000000 RITMO-1.6.0/RITMO.egg-info/dependency_links.txt
+-rw-r--r--   0 rachelstirling   (502) staff       (20)      132 2023-07-06 05:45:45.000000 RITMO-1.6.0/RITMO.egg-info/requires.txt
+-rw-r--r--   0 rachelstirling   (502) staff       (20)        6 2023-07-06 05:45:45.000000 RITMO-1.6.0/RITMO.egg-info/top_level.txt
+drwxr-xr-x   0 rachelstirling   (502) staff       (20)        0 2023-07-06 05:45:45.530638 RITMO-1.6.0/ritmo/
+-rw-r--r--   0 rachelstirling   (502) staff       (20)       49 2023-01-14 06:06:41.000000 RITMO-1.6.0/ritmo/__init__.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)       63 2023-01-13 00:49:08.000000 RITMO-1.6.0/ritmo/__version__.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)      191 2023-03-29 00:00:42.000000 RITMO-1.6.0/ritmo/constants.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     4542 2023-01-27 05:06:32.000000 RITMO-1.6.0/ritmo/cycles.py
+drwxr-xr-x   0 rachelstirling   (502) staff       (20)        0 2023-07-06 05:45:45.532216 RITMO-1.6.0/ritmo/edm/
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     2296 2023-01-26 13:26:42.000000 RITMO-1.6.0/ritmo/edm/edm.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     2650 2023-07-06 00:42:25.000000 RITMO-1.6.0/ritmo/edm/figure.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     3837 2023-07-06 01:01:04.000000 RITMO-1.6.0/ritmo/edm/statistics.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)    13997 2023-07-06 05:38:07.000000 RITMO-1.6.0/ritmo/main.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     8003 2023-07-06 05:40:44.000000 RITMO-1.6.0/ritmo/plots.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     2483 2023-01-26 02:23:06.000000 RITMO-1.6.0/ritmo/statistics.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     3730 2023-07-06 00:23:50.000000 RITMO-1.6.0/ritmo/utils.py
+-rw-r--r--   0 rachelstirling   (502) staff       (20)       38 2023-07-06 05:45:45.533747 RITMO-1.6.0/setup.cfg
+-rw-r--r--   0 rachelstirling   (502) staff       (20)     1302 2023-07-06 05:45:31.000000 RITMO-1.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `RITMO-1.5.3/LICENSE` & `RITMO-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RITMO-1.5.3/PKG-INFO` & `RITMO-1.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: RITMO
-Version: 1.5.3
+Version: 1.6.0
 Summary: Research Investigation of Timeseries with Multiday Oscillations
 Home-page: https://github.com/rachel-stirling/RITMO
 Author: Rachel E. Stirling
 Author-email: rachelstirling1@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Rhythmic Investigation of Timeseries with Multiday Oscillations (RITMO)
@@ -34,16 +36,16 @@
 
 ```python
 >>> from ritmo import Ritmo
 >>> import numpy as np
 >>> x = np.arange(0, 100*24*3.6e6, 3.6e6) # UNIX timestamps in milliseconds
 >>> y1 = np.random.random(x.size) # first random timeseries
 >>> y2 = np.random.random(x.size) # second random timeseries
->>> ritmo = Ritmo(y1 = y1, y2 = y2, x1 = x)
->>> ritmo.run()
+>>> ritmo = Ritmo(y1 = y1, y2 = y2, x1 = x, y1_name = 'Random_TS_1', y2_name = 'Random_TS_2')
+>>> ritmo.run() # Runs all modules at once
 ```
 
 To run individual modules:
 
 ```python
 >>> ritmo.run_edm() # Empirical dynamical modelling module
 >>> ritmo.run_plv() # Phase locking value module
@@ -58,7 +60,9 @@
 
 ```python
 export RELEASE=x.x.x
 git commit --allow-empty -m "Release $RELEASE"
 git tag -a $RELEASE -m "Version $RELEASE"
 git push upstream --tags
 ```
+
+
```

### Comparing `RITMO-1.5.3/README.md` & `RITMO-1.6.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
 ```python
 >>> from ritmo import Ritmo
 >>> import numpy as np
 >>> x = np.arange(0, 100*24*3.6e6, 3.6e6) # UNIX timestamps in milliseconds
 >>> y1 = np.random.random(x.size) # first random timeseries
 >>> y2 = np.random.random(x.size) # second random timeseries
->>> ritmo = Ritmo(y1 = y1, y2 = y2, x1 = x)
->>> ritmo.run()
+>>> ritmo = Ritmo(y1 = y1, y2 = y2, x1 = x, y1_name = 'Random_TS_1', y2_name = 'Random_TS_2')
+>>> ritmo.run() # Runs all modules at once
 ```
 
 To run individual modules:
 
 ```python
 >>> ritmo.run_edm() # Empirical dynamical modelling module
 >>> ritmo.run_plv() # Phase locking value module
```

### Comparing `RITMO-1.5.3/RITMO.egg-info/PKG-INFO` & `RITMO-1.6.0/RITMO.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: RITMO
-Version: 1.5.3
+Version: 1.6.0
 Summary: Research Investigation of Timeseries with Multiday Oscillations
 Home-page: https://github.com/rachel-stirling/RITMO
 Author: Rachel E. Stirling
 Author-email: rachelstirling1@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Rhythmic Investigation of Timeseries with Multiday Oscillations (RITMO)
@@ -34,16 +36,16 @@
 
 ```python
 >>> from ritmo import Ritmo
 >>> import numpy as np
 >>> x = np.arange(0, 100*24*3.6e6, 3.6e6) # UNIX timestamps in milliseconds
 >>> y1 = np.random.random(x.size) # first random timeseries
 >>> y2 = np.random.random(x.size) # second random timeseries
->>> ritmo = Ritmo(y1 = y1, y2 = y2, x1 = x)
->>> ritmo.run()
+>>> ritmo = Ritmo(y1 = y1, y2 = y2, x1 = x, y1_name = 'Random_TS_1', y2_name = 'Random_TS_2')
+>>> ritmo.run() # Runs all modules at once
 ```
 
 To run individual modules:
 
 ```python
 >>> ritmo.run_edm() # Empirical dynamical modelling module
 >>> ritmo.run_plv() # Phase locking value module
@@ -58,7 +60,9 @@
 
 ```python
 export RELEASE=x.x.x
 git commit --allow-empty -m "Release $RELEASE"
 git tag -a $RELEASE -m "Version $RELEASE"
 git push upstream --tags
 ```
+
+
```

### Comparing `RITMO-1.5.3/ritmo/cycles.py` & `RITMO-1.6.0/ritmo/cycles.py`

 * *Files identical despite different names*

### Comparing `RITMO-1.5.3/ritmo/edm/edm.py` & `RITMO-1.6.0/ritmo/edm/edm.py`

 * *Files identical despite different names*

### Comparing `RITMO-1.5.3/ritmo/edm/figure.py` & `RITMO-1.6.0/ritmo/edm/figure.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from matplotlib import pyplot as plt
 import numpy as np
+from typing import Tuple
 
 from ritmo.utils import read_pickle
 
 
 def confidence_vals(surr, col, min_lib, max_lib):
     """Find 5th and 95th confidence values using surrogates"""
     x_5 = []
@@ -16,15 +17,16 @@
             for sur in surr
         ]
         x_5.append(np.nanpercentile(all_surr, 5))
         x_95.append(np.nanpercentile(all_surr, 95))
     return x_5, x_95
 
 
-def edm_figure(save_path: str, surrogates: bool):
+def edm_figure(save_path: str, surrogates: bool, variable_names: Tuple[str,
+                                                                       str]):
     """Create EDM CCM figure"""
     results_path = os.path.join(save_path, "results")
     [y1_xmap_y2,
      y2_xmap_y1] = read_pickle(os.path.join(results_path, "edm.pickle"))
 
     x1 = y1_xmap_y2['LibSize']
     y = y1_xmap_y2['y1:y2']
@@ -33,22 +35,29 @@
 
     if surrogates:
         surr = read_pickle(os.path.join(results_path, "surrogates.pickle"))
         y_5, y_95 = confidence_vals(surr[0], 'y1:y2', int(x1.min()),
                                     int(x1.max()))
         z_5, z_95 = confidence_vals(surr[1], 'y2:y1', int(x2.min()),
                                     int(x2.max()))
-        y_min = min(min(y_95), min(y), min(z_95), min(z))
-        y_max = max(max(y_95), max(y), max(z_95), max(z))
+        all_vals = y_95 + y + z_95 + z
+        y_min = min(all_vals)
+        y_max = max(all_vals)
     else:
         y_min, y_max = min(y.min(), z.min()) * 0.9, max(y.max(), z.max()) * 1.1
     x_min, x_max = min(x1.min(), x2.min()), max(x1.max(), x2.max())
 
-    plt.plot(x1, y, c='navy', label='X1 xmap X2')
-    plt.plot(x2, z, c='red', label='X2 xmap X1')
+    plt.plot(x1,
+             y,
+             c='navy',
+             label=f'{variable_names[0]} xmap {variable_names[1]}')
+    plt.plot(x2,
+             z,
+             c='red',
+             label=f'{variable_names[1]} xmap {variable_names[0]}')
     if surrogates:
         plt.fill_between(x1, y_5, y_95, color='navy', alpha=.3)
         plt.fill_between(x2, z_5, z_95, color='red', alpha=.3)
 
     plt.xlim([x_min, x_max])
     plt.ylim([y_min, y_max])
```

### Comparing `RITMO-1.5.3/ritmo/edm/statistics.py` & `RITMO-1.6.0/ritmo/edm/statistics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import pymannkendall as mk
 import numpy as np
 from scipy.stats import norm as nm
 from ritmo.utils import read_pickle
 import pandas as pd
+from typing import Tuple
 
 
 def z_transform(xy, ab, n, n2=None, twotailed=False):
     """Z-transform for Fishers test"""
     xy_z = 0.5 * np.log((1 + xy) / (1 - xy))
     ab_z = 0.5 * np.log((1 + ab) / (1 - ab))
     if n2 is None:
@@ -59,20 +60,23 @@
     y2_skill = z.max() - z.iloc[0]
     skill_above_surr_y1 = y1_skill > y1_95
     skill_above_surr_y2 = y2_skill > y2_95
 
     return skill_above_surr_y1, skill_above_surr_y2
 
 
-def edm_statistics(save_path: str, surrogates: bool):
+def edm_statistics(save_path: str, surrogates: bool,
+                   variable_names: Tuple[str, str]):
     """Runs statistics for EDM model"""
+    y1_y2 = f"{variable_names[0]}-{variable_names[1]}"
+    y2_y1 = f"{variable_names[1]}-{variable_names[0]}"
     df = pd.DataFrame(columns=[
-        'Kendall X1-X2', 'Kendall X2-X1', 'Fisher X1-X2', 'Fisher X2-X1',
-        'Significant surrogate skill X1-X2',
-        'Significant surrogate skill X2-X1'
+        f'Kendall {y1_y2}', f'Kendall {y2_y1}', f'Fisher {y1_y2}',
+        f'Fisher {y2_y1}', f'Significant surrogate skill {y1_y2}',
+        f'Significant surrogate skill {y2_y1}'
     ])
 
     results_path = os.path.join(save_path, "results")
     [y1_xmap_y2,
      y2_xmap_y1] = read_pickle(os.path.join(results_path, "edm.pickle"))
 
     x1 = y1_xmap_y2['LibSize']
@@ -85,23 +89,24 @@
     if surrogates:
         surr = read_pickle(os.path.join(results_path, "surrogates.pickle"))
         skill_above_surr_y1, skill_above_surr_y2 = surrogates_test(
             surr, y, z, 'y1:y2', 'y2:y1')
     else:
         skill_above_surr_y1, skill_above_surr_y2 = ["N/A"] * 2
 
+    sig_fn = lambda x: '*' if x else ''
     df = df.append(
         {
-            'Kendall X1-X2':
-            f'{round(tau_y1_y2, 4)} ({round(p_y1_y2, 4)}{"*" if p_y1_y2<0.05 and tau_y1_y2 > 0 else ""})',
-            'Kendall X2-X1':
-            f'{round(tau_y2_y1, 4)} ({round(p_y2_y1, 4)}{"*" if p_y2_y1<0.05 and tau_y2_y1 > 0 else ""})',
-            'Fisher X1-X2':
-            f'{round(z_y1_y2, 4)} ({round(zp_y1_y2, 4)}{"*" if zp_y1_y2<0.05 else ""})',
-            'Fisher X2-X1':
-            f'{round(z_y2_y1, 4)} ({round(zp_y2_y1, 4)}{"*" if zp_y2_y1<0.05 else ""})',
-            'Significant surrogate skill X1-X2': str(skill_above_surr_y1),
-            'Significant surrogate skill X2-X1': str(skill_above_surr_y2)
+            f'Kendall {y1_y2}':
+            f'{tau_y1_y2:.4f} ({p_y1_y2:.4f}{sig_fn(p_y1_y2<0.05 and tau_y1_y2 > 0)})',
+            f'Kendall {y2_y1}':
+            f'{tau_y2_y1:.4f} ({p_y2_y1:.4f}{sig_fn(p_y2_y1<0.05 and tau_y2_y1 > 0)})',
+            f'Fisher {y1_y2}':
+            f'{z_y1_y2:.4f} ({zp_y1_y2:.4f}{sig_fn(zp_y1_y2<0.05)})',
+            f'Fisher {y2_y1}':
+            f'{z_y2_y1:.4f} ({zp_y2_y1:.4f}{sig_fn(zp_y2_y1<0.05)})',
+            f'Significant surrogate skill {y1_y2}': str(skill_above_surr_y1),
+            f'Significant surrogate skill {y2_y1}': str(skill_above_surr_y2)
         },
         ignore_index=True)
 
     df.to_csv(os.path.join(results_path, "edm_significance.csv"))
```

### Comparing `RITMO-1.5.3/ritmo/main.py` & `RITMO-1.6.0/ritmo/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,54 +28,61 @@
     Parameters
     ------------
         y1: numpy array of float or int
             Array of values for first timeseries
         y2: numpy array of float or int
             Array of values for second timeseries
         x1: numpy array of float or int
-            Array of UNIX timestamps associated with y1 values
+            Array of UNIX timestamps (in milliseconds) associated with y1 values
         x2: numpy array of float or int (default = None)
-            Array of UNIX timestamps associated with y2 values
+            Array of UNIX timestamps (in milliseconds) associated with y2 values
             If set to None, x2 is set to x1
         resample_method: dictionary (default = None, which uses mean resample method)
             Specified resampling methods for y1 and y2
             e.g. {"y1": "mean", "y2": "sum"}
             Currently only mean and sum methods are set up for resampling
         save_path: str (default = '.')
             Path to save results and plots
             If not set, default stores results and plots in current working directory.
         dataset_name: str (default = None)
             Name of dataset; dictates how files will be stored.
             If set to None, UUID for the dataset will be generated.
         save_plots: bool (default = True)
             Whether to save plots or not
+        y1_name: str (default 'Y1')
+            Name of the X1 variable / first timeseries signal
+        y2_name: str (default 'Y2')
+            Name of the X2 variable / second timeseries signal
     """
     def __init__(self,
                  y1: tsrs_vtype,
                  y2: tsrs_vtype,
                  x1: tsrs_vtype,
                  x2: Optional[tsrs_vtype] = None,
                  resample_method: Optional[Mapping[str, str]] = None,
                  save_path: str = '.',
                  dataset_name: Optional[str] = None,
-                 save_plots: bool = True) -> None:
+                 save_plots: bool = True,
+                 y1_name: str = 'Y1',
+                 y2_name: str = 'Y2') -> None:
 
         if dataset_name is None:
             dataset_name = str(uuid.uuid4())
             print(f"No dataset name provided. Set to {dataset_name}.")
         self.dataset_name = dataset_name
 
         ## Initiate variables and make paths
         self.save_plots = save_plots
         self.save_path = os.path.join(save_path, "results", self.dataset_name)
         self.cycles = False
         self.tsrs_1_filtered = None
         self.tsrs_2_filtered = None
         self.overlapping_cycles = None
         self.filtered_noise = None
+        self.variable_names = (y1_name, y2_name)
         os.makedirs(os.path.join(self.save_path, "results"), exist_ok=True)
         os.makedirs(os.path.join(self.save_path, "figures"), exist_ok=True)
 
         # check input types
         for var, var_name in zip([y1, y2, x1], ['y1', 'y2', 'x1']):
             error = False
             try:
@@ -95,15 +102,15 @@
         if resample_method is not None:
             if not all(key in resample_method for key in ['y1', 'y2']):
                 raise TypeError(
                     f"resample_method should be dict type with 'y1' and 'y2' as specified keys."
                 )
             y1_rs, y2_rs = resample_method['y1'], resample_method['y2']
         else:
-            y1_rs, y2_rs = ['mean'] * 2 # defaults to mean
+            y1_rs, y2_rs = ['mean'] * 2  # defaults to mean
 
         # check for x2
         if x2 is None:
             if y1.size != y2.size:
                 raise ValueError(
                     "Length of y1 must equal y2 if x2 is not provided.")
             print("x2 was not provided. Assuming timestamps of x2 = x1.")
@@ -120,68 +127,82 @@
                 setattr(self, var_name, var[:, 0])
 
         # interpolation
         self.tsrs_1 = process_data(self.x1, self.y1, freq='1H', method=y1_rs)
         self.tsrs_2 = process_data(self.x2, self.y2, freq='1H', method=y2_rs)
         self._check_start_end_times()
 
-        if len(self.tsrs_1) < MIN_DAYS * 24 or len(self.tsrs_2) < MIN_DAYS * 24:
+        if len(self.tsrs_1) < MIN_DAYS * 24 or len(
+                self.tsrs_2) < MIN_DAYS * 24:
             raise ValueError(
                 f"Timeseries overlap is less than {MIN_DAYS} days.")
 
         # plot moving averages
         if self.save_plots:
-            timeseries_plot(self.tsrs_1, self.tsrs_2, self.save_path)
+            timeseries_plot(self.tsrs_1, self.tsrs_2, self.save_path,
+                            self.variable_names)
 
     def run(self):
         """Runs all RITMO code and produces table"""
 
         # Run all RITMO methods
         plv_all_cycles = self.run_plv()
         mi_all_cycles = self.run_mutual_information()
 
         sig_fn = lambda x: '*' if x else ''
         # Build table
         table = pd.DataFrame(columns=[
-            'X1 period (days)', 'X2 period (days)', 'PLV', 'PLV Noise',
+            f'{self.variable_names[0]} period (days)',
+            f'{self.variable_names[1]} period (days)', 'PLV', 'PLV Noise',
             'MI (lag 0)', 'MI max', 'MI random'
         ])
         for (peak1, peak2), (_, plv, plv_noise) in plv_all_cycles.items():
 
             (mi_vals, lags, mi_random) = mi_all_cycles[(peak1, peak2)]
             max_mi = np.max(mi_vals)
-            max_mi_lag = lags[np.where(mi_vals == max_mi)[0]]
+            max_mi_lag = lags[np.where(mi_vals == max_mi)[0]][0]
 
             # Significance
             mi_0_sig = sig_fn(mi_vals[0] > mi_random)
             mi_max_sig = sig_fn(max_mi > mi_random)
             plv_sig = sig_fn(plv > plv_noise)
 
             table = table.append(
                 {
-                    'X1 period (days)': round(peak1 / 24, 1),
-                    'X2 period (days)': round(peak2 / 24, 1),
-                    'PLV': f'{round(plv, 4)}{plv_sig}',
-                    'PLV Noise': round(plv_noise, 4),
-                    'MI (lag 0)': f'{round(mi_vals[0], 4)}{mi_0_sig}',
+                    f'{self.variable_names[0]} period (days)':
+                    f"{peak1/24:.1f}",
+                    f'{self.variable_names[1]} period (days)':
+                    f"{peak2/24:.1f}",
+                    'PLV': f'{plv:.4f}{plv_sig}',
+                    'PLV Noise': f'{plv_noise:.4f}',
+                    'MI (lag 0)': f'{mi_vals[0]:.4f}{mi_0_sig}',
                     'MI max':
-                    f'{round(max_mi, 4)}{mi_max_sig} (lag {round(max_mi_lag[0])})',
-                    'MI random': round(mi_random, 4),
+                    f'{max_mi:.4f}{mi_max_sig} (lag {max_mi_lag:.0f})',
+                    'MI random': f'{mi_random:.4f}',
                 },
                 ignore_index=True)
         table.to_csv(
             os.path.join(self.save_path, "results", "plv_mi_significance.csv"))
 
         self.run_edm()
 
-    def run_edm(self, surrogates: bool = True):
+    def run_edm(self,
+                surrogates: bool = True,
+                use_existing_surrogates: bool = False):
         """
         Runs pyEDM module on dataset and generates surrogates
         in accordance with input varaibles.
         Default is to generate 100 surrogates.
+        Parameters
+        ------------
+            surrogates: bool (default True)
+                Toggle to generate surrogates
+            use_existing_surrogates: bool (default False)
+                Toggle to look for existing surrogates in results folder
+                Useful variable in cases where script termiates early
         """
 
         # run EDM on timeseries
         df1 = self.tsrs_1.resample('1D', on='timestamp',
                                    label='right').mean().reset_index()
         df2 = self.tsrs_2.resample('1D', on='timestamp',
                                    label='right').mean().reset_index()
@@ -190,15 +211,15 @@
         write_pickle([y1_xmap_y2, y2_xmap_y1],
                      os.path.join(self.save_path, "results", "edm.pickle"))
 
         # run EDM on surrogates
         if surrogates:
             surr_path = os.path.join(self.save_path, "results",
                                      "surrogates.pickle")
-            if os.path.exists(surr_path):
+            if use_existing_surrogates and os.path.exists(surr_path):
                 [y1_xmap_y2_surr, y2_xmap_y1_surr] = read_pickle(surr_path)
                 start_from = len(y1_xmap_y2_surr)
             else:
                 start_from = 0
                 y1_xmap_y2_surr = []
                 y2_xmap_y1_surr = []
 
@@ -209,18 +230,18 @@
                 y1_xmap_y2_surr.append(y1_y2_surr)
                 y2_xmap_y1_surr.append(y2_y1_surr)
                 print(f'Surrogate {k + 1}/{N_SURROGATES}')
                 write_pickle([y1_xmap_y2_surr, y2_xmap_y1_surr], surr_path)
 
         # Figure
         if self.save_plots:
-            edm_figure(self.save_path, surrogates)
+            edm_figure(self.save_path, surrogates, self.variable_names)
 
         # EDM statistics
-        edm_statistics(self.save_path, surrogates)
+        edm_statistics(self.save_path, surrogates, self.variable_names)
 
     def run_plv(self):
         """
         Runs phase locking value method on cycle pairs of the two timeseries.
         """
         if not self.cycles:
             self._detect_cycles()
@@ -247,15 +268,15 @@
                 plv_sig = sig_fn(plv > plv_noise)
                 plv_all_cycles[(peak1, i)] = (phase_synchrony, plv, plv_noise)
 
                 if self.save_plots:
                     plot_phase_synchony(self.tsrs_1_filtered,
                                         self.tsrs_2_filtered, peak1, i,
                                         phase_synchrony, plv, plv_sig,
-                                        self.save_path)
+                                        self.save_path, self.variable_names)
 
         return plv_all_cycles
 
     def run_mutual_information(self):
         """
         Runs mutual information method on cycle pairs of the two timeseries.
         """
@@ -270,15 +291,16 @@
             for i in peak2:
 
                 value2 = self.tsrs_2_filtered[f'{i}_value'].to_numpy()
                 mi_vals = stats_shifted(value1, value2, lags=lags)
                 mi_random = stats_random(self.filtered_noise, peak1, i)
                 if self.save_plots:
                     plot_mutual_information(peak1, i, mi_vals, lags, mi_random,
-                                            self.save_path)
+                                            self.save_path,
+                                            self.variable_names)
                 mi_all_cycles[(peak1, i)] = (mi_vals, lags, mi_random)
 
         return mi_all_cycles
 
     def _detect_cycles(self):
         """Detects and filters cycles in timeseries (and noise) using Morlet wavelet"""
 
@@ -299,15 +321,15 @@
 
         ## Create surrogates
         self.filtered_noise = get_noise_dists(self.tsrs_1, self.tsrs_2, peaks1,
                                               peaks2, cutoffs1, cutoffs2)
 
         if self.save_plots:
             wavelet_plot(wavelet_df1, wavelet_df2, self.overlapping_cycles,
-                         self.save_path)
+                         self.save_path, self.variable_names)
 
     def _check_start_end_times(self):
         """
         Ensures both timeseries start and end
         at the same time. i.e. checks for overlap.
         """
         args = (self.tsrs_1, self.tsrs_2)
```

### Comparing `RITMO-1.5.3/ritmo/statistics.py` & `RITMO-1.6.0/ritmo/statistics.py`

 * *Files identical despite different names*

### Comparing `RITMO-1.5.3/ritmo/utils.py` & `RITMO-1.6.0/ritmo/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from multiprocessing.pool import Pool
 import os
 import pickle
 import numpy as np
 import pandas as pd
+import warnings
 
 from ritmo.constants import MULTIPROCESSING
 
 
 def read_pickle(file_path):
     """Reads pickle file to Python object."""
     try:
@@ -52,15 +53,28 @@
 
 def resample_df(args):
     """
     Resamples df at freq using specified method
     Currently only set up for mean and sum methods
     """
     df, freq, method = args
-    df.loc[:, 'timestamp'] = df['timestamp'].astype('datetime64[ms]')
+    try:
+        df.loc[:, 'timestamp'] = df['timestamp'].astype('datetime64[ms]')
+    except pd.errors.OutOfBoundsDatetime as error:
+        print(
+            f"Timestamps given {df['timestamp'].iloc[0]}...{df['timestamp'].iloc[-1]}"
+            + " are not in milliseconds")
+        raise pd.errors.OutOfBoundsDatetime(error)
+
+    if df['timestamp'].iloc[0].year == 1970:
+        warnings.warn(
+            f"Timestamps convereted to {df['timestamp'].iloc[0]}..." +
+            f"{df['timestamp'].iloc[-1]}. Double check" +
+            " that timestamps are in milliseconds.")
+
     if method == 'mean':
         return df.resample(freq, on='timestamp',
                            label='right').mean().reset_index()
     elif method == 'sum':
         return df.resample(freq, on='timestamp',
                            label='right').sum().reset_index()
     else:
```

### Comparing `RITMO-1.5.3/setup.py` & `RITMO-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Package meta-data.
 NAME = 'RITMO'
 DESCRIPTION = 'Research Investigation of Timeseries with Multiday Oscillations'
 URL = 'https://github.com/rachel-stirling/RITMO'
 EMAIL = 'rachelstirling1@gmail.com'
 AUTHOR = 'Rachel E. Stirling'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '1.5.3'
+VERSION = '1.6.0'
 
 install_requires = [
     'pandas==1.3.5', 'matplotlib==3.5.3', 'numpy==1.21.6', 'pyEDM==1.14.0.0',
     'pymannkendall==1.4.3', 'pycwt==0.3.0a22', 'scikit-learn==1.0.2',
     'scipy==1.7.3'
 ]
```

