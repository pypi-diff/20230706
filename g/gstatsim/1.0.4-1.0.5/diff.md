# Comparing `tmp/gstatsim-1.0.4.tar.gz` & `tmp/gstatsim-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gstatsim-1.0.4.tar", last modified: Thu May  4 20:12:07 2023, max compression
+gzip compressed data, was "gstatsim-1.0.5.tar", last modified: Thu Jul  6 19:53:26 2023, max compression
```

## Comparing `gstatsim-1.0.4.tar` & `gstatsim-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 michaelfield   (502) staff       (20)        0 2023-05-04 20:12:07.027526 gstatsim-1.0.4/
--rw-r--r--   0 michaelfield   (502) staff       (20)     1068 2023-05-04 18:46:36.000000 gstatsim-1.0.4/LICENSE
--rw-r--r--   0 michaelfield   (502) staff       (20)     5530 2023-05-04 20:12:07.027387 gstatsim-1.0.4/PKG-INFO
--rw-r--r--   0 michaelfield   (502) staff       (20)     4990 2023-05-04 20:11:32.000000 gstatsim-1.0.4/README.md
-drwxr-xr-x   0 michaelfield   (502) staff       (20)        0 2023-05-04 20:12:07.027192 gstatsim-1.0.4/gstatsim.egg-info/
--rw-r--r--   0 michaelfield   (502) staff       (20)     5530 2023-05-04 20:12:07.000000 gstatsim-1.0.4/gstatsim.egg-info/PKG-INFO
--rw-r--r--   0 michaelfield   (502) staff       (20)      197 2023-05-04 20:12:07.000000 gstatsim-1.0.4/gstatsim.egg-info/SOURCES.txt
--rw-r--r--   0 michaelfield   (502) staff       (20)        1 2023-05-04 20:12:07.000000 gstatsim-1.0.4/gstatsim.egg-info/dependency_links.txt
--rw-r--r--   0 michaelfield   (502) staff       (20)       69 2023-05-04 20:12:07.000000 gstatsim-1.0.4/gstatsim.egg-info/requires.txt
--rw-r--r--   0 michaelfield   (502) staff       (20)        9 2023-05-04 20:12:07.000000 gstatsim-1.0.4/gstatsim.egg-info/top_level.txt
--rw-r--r--   0 michaelfield   (502) staff       (20)    56696 2023-05-04 18:46:36.000000 gstatsim-1.0.4/gstatsim.py
--rw-r--r--   0 michaelfield   (502) staff       (20)       38 2023-05-04 20:12:07.027566 gstatsim-1.0.4/setup.cfg
--rw-r--r--   0 michaelfield   (502) staff       (20)      938 2023-05-04 20:11:51.000000 gstatsim-1.0.4/setup.py
+drwxr-xr-x   0 michaelfield   (502) staff       (20)        0 2023-07-06 19:53:26.477655 gstatsim-1.0.5/
+-rw-r--r--   0 michaelfield   (502) staff       (20)     1068 2023-05-04 18:46:36.000000 gstatsim-1.0.5/LICENSE
+-rw-r--r--   0 michaelfield   (502) staff       (20)     5692 2023-07-06 19:53:26.477516 gstatsim-1.0.5/PKG-INFO
+-rw-r--r--   0 michaelfield   (502) staff       (20)     5152 2023-07-06 19:51:47.000000 gstatsim-1.0.5/README.md
+drwxr-xr-x   0 michaelfield   (502) staff       (20)        0 2023-07-06 19:53:26.477345 gstatsim-1.0.5/gstatsim.egg-info/
+-rw-r--r--   0 michaelfield   (502) staff       (20)     5692 2023-07-06 19:53:26.000000 gstatsim-1.0.5/gstatsim.egg-info/PKG-INFO
+-rw-r--r--   0 michaelfield   (502) staff       (20)      197 2023-07-06 19:53:26.000000 gstatsim-1.0.5/gstatsim.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelfield   (502) staff       (20)        1 2023-07-06 19:53:26.000000 gstatsim-1.0.5/gstatsim.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelfield   (502) staff       (20)       69 2023-07-06 19:53:26.000000 gstatsim-1.0.5/gstatsim.egg-info/requires.txt
+-rw-r--r--   0 michaelfield   (502) staff       (20)        9 2023-07-06 19:53:26.000000 gstatsim-1.0.5/gstatsim.egg-info/top_level.txt
+-rw-r--r--   0 michaelfield   (502) staff       (20)    55709 2023-07-06 16:50:38.000000 gstatsim-1.0.5/gstatsim.py
+-rw-r--r--   0 michaelfield   (502) staff       (20)       38 2023-07-06 19:53:26.477711 gstatsim-1.0.5/setup.cfg
+-rw-r--r--   0 michaelfield   (502) staff       (20)      938 2023-07-06 19:52:10.000000 gstatsim-1.0.5/setup.py
```

### Comparing `gstatsim-1.0.4/LICENSE` & `gstatsim-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gstatsim-1.0.4/PKG-INFO` & `gstatsim-1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: gstatsim
-Version: 1.0.4
+Version: 1.0.5
 Summary: Geostatistics tools for interpolation and simulation.
 Home-page: https://github.com/GatorGlaciology/GStatSim
 Author: (Emma) Mickey MacKie
 Author-email: emackie@ufl.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-[![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](<https://gatorglaciology.github.io/gstatsimbook/intro.html>) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GatorGlaciology/gstatsimbook/HEAD?urlpath=lab)
+
+[![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](<https://gatorglaciology.github.io/gstatsimbook/intro.html>)  [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GatorGlaciology/gstatsimbook/HEAD?urlpath=lab)  ![PyPI](https://img.shields.io/pypi/v/gstatsim?label=pypi%20package) ![PyPI - Downloads](https://img.shields.io/pypi/dm/gstatsim) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/gstatsim.svg?style=social&label=Follow%20%40GatorGlaciology)](https://twitter.com/GatorGlaciology)
+
 
 </p>
 
 # GStatSim
-GStatSim is a Python package specifically designed for geostatistical interpolation and simulation. It is inspired by open source geostatistical resources such as GeostatsPy and SciKit-GStat. The functions are intended to address the challenges of working with datasets with large crossover errors, non-linear trends, variability in measurement density, and non-stationarity. These tools are part of our ongoing effort to develop and adapt open-access geostatistical functions.
+GStatSim is a Python package specifically designed for geostatistical interpolation and simulation. It is inspired by open source geostatistical resources such as GeostatsPy and SciKit-GStat. The functions are intended to address the challenges of working with large data sets, non-linear trends, variability in measurement density, and non-stationarity. These tools are part of our ongoing effort to develop and adapt open-access geostatistical functions.
 
 We have created Jupyter Book tutorials here: https://gatorglaciology.github.io/gstatsimbook/intro.html
 
-In its current state, the demos focus on the geostatistical simulation of subglacial topography. However, these protocols could be applied to a number topics in glaciology, or geoscientific problems in general.
+In its current state, the demos focus on the geostatistical simulation of subglacial topography. However, these protocols could be applied to a number geoscientific topics.
 
 We will continuously develop new tools and tutorials to address specific technical challenges in geostatistics. Do you have feedback or suggestions? Specific things that we should account for? Feel free to contact me at emackie@ufl.edu. Our goal is to create tools that are useful and accessible, so we welcome your thoughts and insight.
 
 
+
 # Features
 
 ## Functions
 Some of the tools in GStatSim:
 
 * **skrige** - Simple kriging
 * **okrige** - Ordinary kriging
@@ -96,32 +99,25 @@
 
 # Educational use
 
 GStatSim is well-suited for educational use. Please contact us if you plan on using GStatSim material in a course so we can track the impact of our work.
 
 # Cite as
 
-MacKie, Emma, Field, Michael, Wang, Lijing, Yin, Zhen, Schoedl, Nathan, & Hibbs, Matthew. (2022). GStatSim (1.0). Zenodo. https://doi.org/10.5281/zenodo.7230276
+MacKie, E. J., Field, M., Wang, L., Yin, Z., Schoedl, N., Hibbs, M., & Zhang, A. (2023). GStatSim V1. 0: a Python package for geostatistical interpolation and conditional simulation. EGUsphere, 1-27.
 
 or
 
-@software{mackie_emma_2022_7274640,
-  author       = {MacKie, Emma and
-                  Field, Michael and
-                  Wang, Lijing and
-                  Yin, Zhen and
-                  Schoedl, Nathan and
-                  Hibbs, Matthew},
-  title        = {GStatSim},
-  month        = oct,
-  year         = 2022,
-  publisher    = {Zenodo},
-  version      = {1.0},
-  doi          = {10.5281/zenodo.7274640},
-  url          = {https://doi.org/10.5281/zenodo.7274640}
+@article{mackie2022gstatsim,
+  title={GStatSim V1. 0: a Python package for geostatistical interpolation and conditional simulation},
+  author={MacKie, Emma Johanne and Field, Michael and Wang, Lijing and Yin, Zhen and Schoedl, Nathan and Hibbs, Matthew and Zhang, Allan},
+  journal={EGUsphere},
+  pages={1--27},
+  year={2023},
+  publisher={Copernicus GmbH}
 }
 
 # Datasets
 
 The demos use radar bed measurements from the Center for the Remote Sensing of Ice Sheets (CReSIS, 2020).
 
 CReSIS. 2020. Radar depth sounder, Lawrence, Kansas, USA. Digital Media. http://data.cresis.ku.edu/.
```

### Comparing `gstatsim-1.0.4/README.md` & `gstatsim-1.0.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 
-[![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](<https://gatorglaciology.github.io/gstatsimbook/intro.html>) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GatorGlaciology/gstatsimbook/HEAD?urlpath=lab)
+
+[![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](<https://gatorglaciology.github.io/gstatsimbook/intro.html>)  [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GatorGlaciology/gstatsimbook/HEAD?urlpath=lab)  ![PyPI](https://img.shields.io/pypi/v/gstatsim?label=pypi%20package) ![PyPI - Downloads](https://img.shields.io/pypi/dm/gstatsim) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/gstatsim.svg?style=social&label=Follow%20%40GatorGlaciology)](https://twitter.com/GatorGlaciology)
+
 
 </p>
 
 # GStatSim
-GStatSim is a Python package specifically designed for geostatistical interpolation and simulation. It is inspired by open source geostatistical resources such as GeostatsPy and SciKit-GStat. The functions are intended to address the challenges of working with datasets with large crossover errors, non-linear trends, variability in measurement density, and non-stationarity. These tools are part of our ongoing effort to develop and adapt open-access geostatistical functions.
+GStatSim is a Python package specifically designed for geostatistical interpolation and simulation. It is inspired by open source geostatistical resources such as GeostatsPy and SciKit-GStat. The functions are intended to address the challenges of working with large data sets, non-linear trends, variability in measurement density, and non-stationarity. These tools are part of our ongoing effort to develop and adapt open-access geostatistical functions.
 
 We have created Jupyter Book tutorials here: https://gatorglaciology.github.io/gstatsimbook/intro.html
 
-In its current state, the demos focus on the geostatistical simulation of subglacial topography. However, these protocols could be applied to a number topics in glaciology, or geoscientific problems in general.
+In its current state, the demos focus on the geostatistical simulation of subglacial topography. However, these protocols could be applied to a number geoscientific topics.
 
 We will continuously develop new tools and tutorials to address specific technical challenges in geostatistics. Do you have feedback or suggestions? Specific things that we should account for? Feel free to contact me at emackie@ufl.edu. Our goal is to create tools that are useful and accessible, so we welcome your thoughts and insight.
 
 
+
 # Features
 
 ## Functions
 Some of the tools in GStatSim:
 
 * **skrige** - Simple kriging
 * **okrige** - Ordinary kriging
@@ -80,32 +83,25 @@
 
 # Educational use
 
 GStatSim is well-suited for educational use. Please contact us if you plan on using GStatSim material in a course so we can track the impact of our work.
 
 # Cite as
 
-MacKie, Emma, Field, Michael, Wang, Lijing, Yin, Zhen, Schoedl, Nathan, & Hibbs, Matthew. (2022). GStatSim (1.0). Zenodo. https://doi.org/10.5281/zenodo.7230276
+MacKie, E. J., Field, M., Wang, L., Yin, Z., Schoedl, N., Hibbs, M., & Zhang, A. (2023). GStatSim V1. 0: a Python package for geostatistical interpolation and conditional simulation. EGUsphere, 1-27.
 
 or
 
-@software{mackie_emma_2022_7274640,
-  author       = {MacKie, Emma and
-                  Field, Michael and
-                  Wang, Lijing and
-                  Yin, Zhen and
-                  Schoedl, Nathan and
-                  Hibbs, Matthew},
-  title        = {GStatSim},
-  month        = oct,
-  year         = 2022,
-  publisher    = {Zenodo},
-  version      = {1.0},
-  doi          = {10.5281/zenodo.7274640},
-  url          = {https://doi.org/10.5281/zenodo.7274640}
+@article{mackie2022gstatsim,
+  title={GStatSim V1. 0: a Python package for geostatistical interpolation and conditional simulation},
+  author={MacKie, Emma Johanne and Field, Michael and Wang, Lijing and Yin, Zhen and Schoedl, Nathan and Hibbs, Matthew and Zhang, Allan},
+  journal={EGUsphere},
+  pages={1--27},
+  year={2023},
+  publisher={Copernicus GmbH}
 }
 
 # Datasets
 
 The demos use radar bed measurements from the Center for the Remote Sensing of Ice Sheets (CReSIS, 2020).
 
 CReSIS. 2020. Radar depth sounder, Lawrence, Kansas, USA. Digital Media. http://data.cresis.ku.edu/.
```

### Comparing `gstatsim-1.0.4/gstatsim.egg-info/PKG-INFO` & `gstatsim-1.0.5/gstatsim.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: gstatsim
-Version: 1.0.4
+Version: 1.0.5
 Summary: Geostatistics tools for interpolation and simulation.
 Home-page: https://github.com/GatorGlaciology/GStatSim
 Author: (Emma) Mickey MacKie
 Author-email: emackie@ufl.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-[![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](<https://gatorglaciology.github.io/gstatsimbook/intro.html>) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GatorGlaciology/gstatsimbook/HEAD?urlpath=lab)
+
+[![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](<https://gatorglaciology.github.io/gstatsimbook/intro.html>)  [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GatorGlaciology/gstatsimbook/HEAD?urlpath=lab)  ![PyPI](https://img.shields.io/pypi/v/gstatsim?label=pypi%20package) ![PyPI - Downloads](https://img.shields.io/pypi/dm/gstatsim) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/gstatsim.svg?style=social&label=Follow%20%40GatorGlaciology)](https://twitter.com/GatorGlaciology)
+
 
 </p>
 
 # GStatSim
-GStatSim is a Python package specifically designed for geostatistical interpolation and simulation. It is inspired by open source geostatistical resources such as GeostatsPy and SciKit-GStat. The functions are intended to address the challenges of working with datasets with large crossover errors, non-linear trends, variability in measurement density, and non-stationarity. These tools are part of our ongoing effort to develop and adapt open-access geostatistical functions.
+GStatSim is a Python package specifically designed for geostatistical interpolation and simulation. It is inspired by open source geostatistical resources such as GeostatsPy and SciKit-GStat. The functions are intended to address the challenges of working with large data sets, non-linear trends, variability in measurement density, and non-stationarity. These tools are part of our ongoing effort to develop and adapt open-access geostatistical functions.
 
 We have created Jupyter Book tutorials here: https://gatorglaciology.github.io/gstatsimbook/intro.html
 
-In its current state, the demos focus on the geostatistical simulation of subglacial topography. However, these protocols could be applied to a number topics in glaciology, or geoscientific problems in general.
+In its current state, the demos focus on the geostatistical simulation of subglacial topography. However, these protocols could be applied to a number geoscientific topics.
 
 We will continuously develop new tools and tutorials to address specific technical challenges in geostatistics. Do you have feedback or suggestions? Specific things that we should account for? Feel free to contact me at emackie@ufl.edu. Our goal is to create tools that are useful and accessible, so we welcome your thoughts and insight.
 
 
+
 # Features
 
 ## Functions
 Some of the tools in GStatSim:
 
 * **skrige** - Simple kriging
 * **okrige** - Ordinary kriging
@@ -96,32 +99,25 @@
 
 # Educational use
 
 GStatSim is well-suited for educational use. Please contact us if you plan on using GStatSim material in a course so we can track the impact of our work.
 
 # Cite as
 
-MacKie, Emma, Field, Michael, Wang, Lijing, Yin, Zhen, Schoedl, Nathan, & Hibbs, Matthew. (2022). GStatSim (1.0). Zenodo. https://doi.org/10.5281/zenodo.7230276
+MacKie, E. J., Field, M., Wang, L., Yin, Z., Schoedl, N., Hibbs, M., & Zhang, A. (2023). GStatSim V1. 0: a Python package for geostatistical interpolation and conditional simulation. EGUsphere, 1-27.
 
 or
 
-@software{mackie_emma_2022_7274640,
-  author       = {MacKie, Emma and
-                  Field, Michael and
-                  Wang, Lijing and
-                  Yin, Zhen and
-                  Schoedl, Nathan and
-                  Hibbs, Matthew},
-  title        = {GStatSim},
-  month        = oct,
-  year         = 2022,
-  publisher    = {Zenodo},
-  version      = {1.0},
-  doi          = {10.5281/zenodo.7274640},
-  url          = {https://doi.org/10.5281/zenodo.7274640}
+@article{mackie2022gstatsim,
+  title={GStatSim V1. 0: a Python package for geostatistical interpolation and conditional simulation},
+  author={MacKie, Emma Johanne and Field, Michael and Wang, Lijing and Yin, Zhen and Schoedl, Nathan and Hibbs, Matthew and Zhang, Allan},
+  journal={EGUsphere},
+  pages={1--27},
+  year={2023},
+  publisher={Copernicus GmbH}
 }
 
 # Datasets
 
 The demos use radar bed measurements from the Center for the Remote Sensing of Ice Sheets (CReSIS, 2020).
 
 CReSIS. 2020. Radar depth sounder, Lawrence, Kansas, USA. Digital Media. http://data.cresis.ku.edu/.
```

### Comparing `gstatsim-1.0.4/gstatsim.py` & `gstatsim-1.0.5/gstatsim.py`

 * *Files 6% similar despite different names*

```diff
@@ -584,28 +584,33 @@
                 lag distance that is normalized to a range of 1
             sill : int, float
                 sill of variogram
             nug : int, float
                 nugget of variogram
             vtype : string
                 type of variogram model (Exponential, Gaussian, or Spherical)
-        
+        Raises
+        ------
+        AtrributeError : if vtype is not 'Exponential', 'Gaussian', or 'Spherical'
+
         Returns
         -------
             c : numpy.ndarray
                 covariance
         """
         
-        if vtype == 'Exponential':
+        if vtype.lower() == 'exponential':
             c = (sill - nug)*np.exp(-3 * effective_lag)
-        elif vtype == 'Gaussian':
+        elif vtype.lower() == 'gaussian':
             c = (sill - nug)*np.exp(-3 * np.square(effective_lag))
-        elif vtype == 'Spherical':
+        elif vtype.lower() == 'spherical':
             c = sill - nug - 1.5 * effective_lag + 0.5 * np.power(effective_lag, 3)
             c[effective_lag > 1] = sill - 1
+        else: 
+            raise AttributeError(f"vtype must be 'Exponential', 'Gaussian', or 'Spherical'")
         return c
 
     def make_covariance_matrix(coord, vario, rotation_matrix):
         """
         Make covariance matrix showing covariances between each pair of input coordinates
         
         Parameters
@@ -626,15 +631,15 @@
         """
         
         nug = vario[1]
         sill = vario[4]  
         vtype = vario[5]
         mat = np.matmul(coord, rotation_matrix)
         effective_lag = pairwise_distances(mat,mat) 
-        covariance_matrix = Covariance.covar(effective_lag, sill, nug, vtype) 
+        covariance_matrix = Covariance.covar(effective_lag, sill, nug, vtype)
 
         return covariance_matrix
 
     def make_covariance_array(coord1, coord2, vario, rotation_matrix):
         """
         Make covariance array showing covariances between each data points and grid cell of interest
         
@@ -723,39 +728,32 @@
         for z, predxy in enumerate(tqdm(prediction_grid, position=0, leave=True)):
             test_idx = np.sum(prediction_grid[z]==df[['X', 'Y']].values,axis = 1)
             if np.sum(test_idx==2)==0:
                 
                 # gather nearest points within radius
                 nearest = NearestNeighbor.nearest_neighbor_search(radius, num_points, 
                                                   prediction_grid[z], df[['X','Y','Z']])
-                norm_data_val = nearest[:,-1] 
-                norm_data_val = norm_data_val.reshape(len(norm_data_val),1)
-                norm_data_val = norm_data_val.T
-                xy_val = nearest[:, :-1]   
-                new_num_pts = len(nearest) 
+                norm_data_val = nearest[:,-1]
+                xy_val = nearest[:, :-1]
+                new_num_pts = len(nearest)
 
-                covariance_matrix = np.zeros(shape=((new_num_pts, new_num_pts)))
+                # covariance between data
                 covariance_matrix = Covariance.make_covariance_matrix(xy_val, 
                                                            vario, rotation_matrix)
 
-                # covariance between data and uknown
-                covariance_array = np.zeros(shape=(new_num_pts))
-                k_weights = np.zeros(shape=(new_num_pts))
+                # covariance between data and unknown
                 covariance_array = Covariance.make_covariance_array(xy_val, 
                                                          np.tile(prediction_grid[z], new_num_pts), 
                                                          vario, rotation_matrix)
                 
-                # covariance between data points
-                covariance_matrix.reshape(((new_num_pts)), ((new_num_pts)))
                 k_weights, res, rank, s = np.linalg.lstsq(covariance_matrix, 
                                                           covariance_array, rcond = None)
 
                 est_sk[z] = mean_1 + (np.sum(k_weights*(norm_data_val[:] - mean_1))) 
                 var_sk[z] = var_1 - np.sum(k_weights*covariance_array)
-                #var_sk[z] = np.absolute(var_sk[z])
                 var_sk[var_sk < 0] = 0
             else:
                 est_sk[z] = df['Z'].values[np.where(test_idx==2)[0][0]]
                 var_sk[z] = 0
         return est_sk, var_sk
 
     def okrige(prediction_grid, df, xx, yy, zz, num_points, vario, radius):
@@ -795,52 +793,49 @@
         azimuth = vario[0]
         major_range = vario[2]
         minor_range = vario[3]
         rotation_matrix = make_rotation_matrix(azimuth, major_range, minor_range) 
 
         df = df.rename(columns = {xx: "X", yy: "Y", zz: "Z"}) 
         var_1 = vario[4]
-        est_ok = np.zeros(shape=len(prediction_grid)) 
+        est_ok = np.zeros(shape=len(prediction_grid))
         var_ok = np.zeros(shape=len(prediction_grid))
 
         for z, predxy in enumerate(tqdm(prediction_grid, position=0, leave=True)):
             test_idx = np.sum(prediction_grid[z]==df[['X', 'Y']].values,axis = 1)
             if np.sum(test_idx==2)==0: 
                 
                 # find nearest data points
                 nearest = NearestNeighbor.nearest_neighbor_search(radius, num_points, 
                                                   prediction_grid[z], df[['X','Y','Z']])    
-                norm_data_val = nearest[:,-1] 
-                local_mean = np.mean(norm_data_val) 
-                norm_data_val = norm_data_val.reshape(len(norm_data_val),1)
-                norm_data_val = norm_data_val.T
+                norm_data_val = nearest[:,-1]
+                local_mean = np.mean(norm_data_val)
                 xy_val = nearest[:,:-1]
-                new_num_pts = len(nearest) 
+                new_num_pts = len(nearest)
 
-                # left hand side (covariance between data)
+                # covariance between data
                 covariance_matrix = np.zeros(shape=((new_num_pts+1, new_num_pts+1))) 
                 covariance_matrix[0:new_num_pts,0:new_num_pts] = Covariance.make_covariance_matrix(xy_val, 
                                                                                         vario, rotation_matrix)
                 covariance_matrix[new_num_pts,0:new_num_pts] = 1
                 covariance_matrix[0:new_num_pts,new_num_pts] = 1
 
-                # Set up Right Hand Side (covariance between data and unknown)
+                # covariance between data and unknown
                 covariance_array = np.zeros(shape=(new_num_pts+1)) 
                 k_weights = np.zeros(shape=(new_num_pts+1))
                 covariance_array[0:new_num_pts] = Covariance.make_covariance_array(xy_val, 
                                                                         np.tile(prediction_grid[z], new_num_pts), 
                                                                         vario, rotation_matrix)
                 covariance_array[new_num_pts] = 1 
                 covariance_matrix.reshape(((new_num_pts+1)), ((new_num_pts+1)))
                 k_weights, res, rank, s = np.linalg.lstsq(covariance_matrix, 
                                                           covariance_array, rcond = None) 
                 
                 est_ok[z] = local_mean + np.sum(k_weights[0:new_num_pts]*(norm_data_val[:] - local_mean)) 
                 var_ok[z] = var_1 - np.sum(k_weights[0:new_num_pts]*covariance_array[0:new_num_pts])
-                #var_ok[z] = np.absolute(var_ok[z])
                 var_ok[var_ok < 0] = 0
             else:
                 est_ok[z] = df['Z'].values[np.where(test_idx==2)[0][0]]
                 var_ok[z] = 0   
         return est_ok, var_ok
   
     def skrige_sgs(prediction_grid, df, xx, yy, zz, num_points, vario, radius):
@@ -895,25 +890,22 @@
                 # get nearest neighbors
                 nearest = NearestNeighbor.nearest_neighbor_search(radius, num_points, 
                                                   prediction_grid[z], df[['X','Y','Z']])  
                 norm_data_val = nearest[:,-1]   
                 xy_val = nearest[:,:-1]   
                 new_num_pts = len(nearest) 
 
-                # left hand side (covariance between data)
-                covariance_matrix = np.zeros(shape=((new_num_pts, new_num_pts))) 
+                # covariance between data
                 covariance_matrix = Covariance.make_covariance_matrix(xy_val, vario, rotation_matrix)
 
-                # Set up Right Hand Side (covariance between data and unknown)
-                covariance_array = np.zeros(shape=(new_num_pts)) 
-                k_weights = np.zeros(shape=(new_num_pts))
+                # covariance between data and unknown
                 covariance_array = Covariance.make_covariance_array(xy_val, 
                                                          np.tile(prediction_grid[z], new_num_pts), 
                                                          vario, rotation_matrix)
-                covariance_matrix.reshape(((new_num_pts)), ((new_num_pts)))
+                
                 k_weights, res, rank, s = np.linalg.lstsq(covariance_matrix, 
                                                           covariance_array, rcond = None) 
                 # get estimates
                 est = mean_1 + np.sum(k_weights*(norm_data_val - mean_1)) 
                 var = var_1 - np.sum(k_weights*covariance_array) 
                 var = np.absolute(var) 
                 sgs[z] = np.random.normal(est,math.sqrt(var),1) 
@@ -985,15 +977,15 @@
                 # covariance between data
                 covariance_matrix = np.zeros(shape=((new_num_pts+1, new_num_pts+1))) 
                 covariance_matrix[0:new_num_pts,0:new_num_pts] = Covariance.make_covariance_matrix(xy_val, 
                                                                                         vario, rotation_matrix)
                 covariance_matrix[new_num_pts,0:new_num_pts] = 1
                 covariance_matrix[0:new_num_pts,new_num_pts] = 1
 
-                # covariance between data and unknown
+                # Set up Right Hand Side (covariance between data and unknown)
                 covariance_array = np.zeros(shape=(new_num_pts+1))
                 k_weights = np.zeros(shape=(new_num_pts+1))
                 covariance_array[0:new_num_pts] = Covariance.make_covariance_array(xy_val, 
                                                                         np.tile(prediction_grid[z], new_num_pts), 
                                                                         vario, rotation_matrix)
                 covariance_array[new_num_pts] = 1 
                 covariance_matrix.reshape(((new_num_pts+1)), ((new_num_pts+1)))
@@ -1171,16 +1163,14 @@
                 # get nearest neighbors
                 nearest = NearestNeighbor.nearest_neighbor_search(radius, num_points, 
                                                                   prediction_grid[z], 
                                                                   df1[['X','Y','Z']])           
                 nearest_second = NearestNeighbor.nearest_neighbor_secondary(prediction_grid[z], 
                                                                             df2[['X','Y','Z']]) 
                 norm_data_val = nearest[:,-1] 
-                norm_data_val = norm_data_val.reshape(len(norm_data_val),1)
-                norm_data_val = norm_data_val.T
                 norm_data_val = np.append(norm_data_val, [nearest_second[-1]]) 
                 xy_val = nearest[:, :-1] 
                 xy_second = nearest_second[:-1] 
                 xy_val = np.append(xy_val, [xy_second], axis = 0) 
                 new_num_pts = len(nearest)
 
                 # covariance between data points
@@ -1283,30 +1273,28 @@
                 
                 # get nearest neighbors
                 nearest = NearestNeighbor.nearest_neighbor_search(radius, num_points, 
                                                                   prediction_grid[z], 
                                                                   df1[['X','Y','Z']]) 
                 nearest_second = NearestNeighbor.nearest_neighbor_secondary(prediction_grid[z], 
                                                                             df2[['X','Y','Z']])
-                norm_data_val = nearest[:,-1] 
-                norm_data_val = norm_data_val.reshape(len(norm_data_val),1)
-                norm_data_val = norm_data_val.T
+                norm_data_val = nearest[:,-1]
                 norm_data_val = np.append(norm_data_val, [nearest_second[-1]]) 
                 xy_val = nearest[:, :-1] 
-                xy_second = nearest_second[:-1] #
+                xy_second = nearest_second[:-1]
                 xy_val = np.append(xy_val, [xy_second], axis = 0) 
                 new_num_pts = len(nearest)
 
                 # covariance between data poitns
                 covariance_matrix = np.zeros(shape=((new_num_pts + 1, new_num_pts + 1))) 
                 covariance_matrix[0:new_num_pts+1, 0:new_num_pts+1] = Covariance.make_covariance_matrix(xy_val, 
                                                                                                         vario, rotation_matrix) 
 
                 # covariance between data and unknown
-                covariance_array = np.zeros(shape=(new_num_pts + 1)) 
+                covariance_array = np.zeros(shape=(new_num_pts + 1))
                 k_weights = np.zeros(shape=(new_num_pts + 1))
                 covariance_array[0:new_num_pts+1] = Covariance.make_covariance_array(xy_val, 
                                                                                      np.tile(prediction_grid[z], 
                                                                                              new_num_pts + 1), 
                                                                                      vario, rotation_matrix)
                 covariance_array[new_num_pts] = covariance_array[new_num_pts] * corrcoef
```

### Comparing `gstatsim-1.0.4/setup.py` & `gstatsim-1.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '1.0.4'
+version = '1.0.5'
 
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Topic :: Scientific/Engineering :: Information Analysis',
 ]
```

