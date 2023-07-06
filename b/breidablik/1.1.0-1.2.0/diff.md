# Comparing `tmp/breidablik-1.1.0.tar.gz` & `tmp/breidablik-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breidablik-1.1.0.tar", last modified: Wed Jul  5 04:40:35 2023, max compression
+gzip compressed data, was "breidablik-1.2.0.tar", last modified: Thu Jul  6 05:44:09 2023, max compression
```

## Comparing `breidablik-1.1.0.tar` & `breidablik-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 04:40:35.082445 breidablik-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-05 04:40:21.000000 breidablik-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-07-05 04:40:35.082445 breidablik-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-05 04:40:21.000000 breidablik-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 04:40:35.078445 breidablik-1.1.0/breidablik/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 04:40:35.082445 breidablik-1.1.0/breidablik/Balder/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/Balder/wavelengths.dat
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 04:40:35.082445 breidablik-1.1.0/breidablik/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/analysis/format_read.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/analysis/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/analysis/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/analysis/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/analysis/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/grid_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/grid_snapshot.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 04:40:35.082445 breidablik-1.1.0/breidablik/interpolate/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/interpolate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/interpolate/grid_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/interpolate/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/interpolate/nlte.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/interpolate/rew.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/interpolate/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/interpolate/spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/interpolate/test_grid_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/interpolate/test_nlte.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/interpolate/test_rew.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/interpolate/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-05 04:40:21.000000 breidablik-1.1.0/breidablik/interpolate/test_spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 04:40:35.082445 breidablik-1.1.0/breidablik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-07-05 04:40:35.000000 breidablik-1.1.0/breidablik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-05 04:40:35.000000 breidablik-1.1.0/breidablik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 04:40:35.000000 breidablik-1.1.0/breidablik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 04:40:35.000000 breidablik-1.1.0/breidablik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 04:40:35.000000 breidablik-1.1.0/breidablik.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-05 04:40:21.000000 breidablik-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 04:40:35.082445 breidablik-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-07-05 04:40:21.000000 breidablik-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:44:09.161630 breidablik-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-06 05:43:55.000000 breidablik-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-06 05:44:09.161630 breidablik-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-06 05:43:55.000000 breidablik-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:44:09.157629 breidablik-1.2.0/breidablik/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:44:09.157629 breidablik-1.2.0/breidablik/Balder/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/Balder/wavelengths.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:44:09.157629 breidablik-1.2.0/breidablik/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/analysis/format_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/analysis/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/analysis/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/analysis/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/analysis/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/grid_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/grid_snapshot.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:44:09.161630 breidablik-1.2.0/breidablik/interpolate/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/interpolate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/interpolate/grid_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/interpolate/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/interpolate/nlte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/interpolate/rew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/interpolate/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/interpolate/spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/interpolate/test_grid_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/interpolate/test_nlte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/interpolate/test_rew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/interpolate/test_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-06 05:43:55.000000 breidablik-1.2.0/breidablik/interpolate/test_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:44:09.157629 breidablik-1.2.0/breidablik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-06 05:44:09.000000 breidablik-1.2.0/breidablik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-06 05:44:09.000000 breidablik-1.2.0/breidablik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 05:44:09.000000 breidablik-1.2.0/breidablik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 05:44:09.000000 breidablik-1.2.0/breidablik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 05:44:09.000000 breidablik-1.2.0/breidablik.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-06 05:43:55.000000 breidablik-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 05:44:09.161630 breidablik-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-07-06 05:43:55.000000 breidablik-1.2.0/setup.py
```

### Comparing `breidablik-1.1.0/LICENSE` & `breidablik-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `breidablik-1.1.0/PKG-INFO` & `breidablik-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: breidablik
-Version: 1.1.0
-Summary: Interpolate lithium spectra and predict lithium abundance for most main sequence stars
-Home-page: https://github.com/ellawang44/Breidablik
-Author: Ella Xi Wang
-Author-email: Ella Xi Wang <xi.wang3@anu.edu.au>
-Project-URL: Bug Reports, https://github.com/ellawang44/Breidablik/issues
-Project-URL: Source, https://github.com/ellawang44/Breidablik
-Keywords: lithium star spectroscopy
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.4, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Breidablik
 An interpolation routine and abundance predictor wrapper around stellar spectra for lithium generated from Balder (Amarsi et al. 2016) and the Stagger-grid (Magic et al. 2013). The raw synthetic spectra and models can be found on http://www.mso.anu.edu.au/~ellawang/. We use radial basis functions (Bertran de Lis et al. 2022) to interpolate between stellar parameters and lithium abundance inputs to generate interpolated 3D NLTE stellar line profiles; and `pytorch` to interpolate between stellar parameters and stellar line strengths, these interpolation models are provided as part of the package. Using the interpolation routine, we can predict the lithium profile given any stellar parameters and lithium abundance input, we can also predict the lithium abundance given an observed spectrum and stellar parameters.
 
 ## Installation
 ### Install with pip
 #### Automatic
 If you are using linux/macOS, you can install using:
@@ -42,15 +26,15 @@
 ./install
 ```
 
 #### Manual
 If the above automatic installation did not work for you, then to install without using `pip`, there are 5 steps:
 1. Navigate to where you want this repository and clone this git repository.
 2. Navigate into `Breidablik/breidablik`.
-3. Download the models from `models.zip` on http://www.mso.anu.edu.au/~ellawang/ and unzip it.
+3. Download the models from `models_vx.x.x.zip` on http://www.mso.anu.edu.au/~ellawang/ and unzip it. Pick the model based on the version of Breidablik you want to run. The model version number will be just lower than your Breidablik version number. e.g. running Breidablik v1.1.0 will require models v1.0.0. 
 4. Optional, download the raw data from `balder.zip` on http://www.mso.anu.edu.au/~ellawang/ and unzip it.
 5. Optional, add this directory to the python path. This makes the directory findable by python no matter where it is launched.
 
 ### Check that your installation is correct
 Optional, to check that the installation was successful, in the `Breidablik` folder, you can run:
 ```
 python -m pytest
```

### Comparing `breidablik-1.1.0/README.md` & `breidablik-1.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: breidablik
+Version: 1.2.0
+Summary: Interpolate lithium spectra and predict lithium abundance for most main sequence stars
+Home-page: https://github.com/ellawang44/Breidablik
+Author: Ella Xi Wang
+Author-email: Ella Xi Wang <xi.wang3@anu.edu.au>
+Project-URL: Bug Reports, https://github.com/ellawang44/Breidablik/issues
+Project-URL: Source, https://github.com/ellawang44/Breidablik
+Keywords: lithium star spectroscopy
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.4, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Breidablik
 An interpolation routine and abundance predictor wrapper around stellar spectra for lithium generated from Balder (Amarsi et al. 2016) and the Stagger-grid (Magic et al. 2013). The raw synthetic spectra and models can be found on http://www.mso.anu.edu.au/~ellawang/. We use radial basis functions (Bertran de Lis et al. 2022) to interpolate between stellar parameters and lithium abundance inputs to generate interpolated 3D NLTE stellar line profiles; and `pytorch` to interpolate between stellar parameters and stellar line strengths, these interpolation models are provided as part of the package. Using the interpolation routine, we can predict the lithium profile given any stellar parameters and lithium abundance input, we can also predict the lithium abundance given an observed spectrum and stellar parameters.
 
 ## Installation
 ### Install with pip
 #### Automatic
 If you are using linux/macOS, you can install using:
@@ -26,15 +42,15 @@
 ./install
 ```
 
 #### Manual
 If the above automatic installation did not work for you, then to install without using `pip`, there are 5 steps:
 1. Navigate to where you want this repository and clone this git repository.
 2. Navigate into `Breidablik/breidablik`.
-3. Download the models from `models.zip` on http://www.mso.anu.edu.au/~ellawang/ and unzip it.
+3. Download the models from `models_vx.x.x.zip` on http://www.mso.anu.edu.au/~ellawang/ and unzip it. Pick the model based on the version of Breidablik you want to run. The model version number will be just lower than your Breidablik version number. e.g. running Breidablik v1.1.0 will require models v1.0.0. 
 4. Optional, download the raw data from `balder.zip` on http://www.mso.anu.edu.au/~ellawang/ and unzip it.
 5. Optional, add this directory to the python path. This makes the directory findable by python no matter where it is launched.
 
 ### Check that your installation is correct
 Optional, to check that the installation was successful, in the `Breidablik` folder, you can run:
 ```
 python -m pytest
```

### Comparing `breidablik-1.1.0/breidablik/Balder/wavelengths.dat` & `breidablik-1.2.0/breidablik/Balder/wavelengths.dat`

 * *Files identical despite different names*

### Comparing `breidablik-1.1.0/breidablik/analysis/format_read.py` & `breidablik-1.2.0/breidablik/analysis/format_read.py`

 * *Files identical despite different names*

### Comparing `breidablik-1.1.0/breidablik/analysis/read.py` & `breidablik-1.2.0/breidablik/analysis/read.py`

 * *Files 6% similar despite different names*

```diff
@@ -174,18 +174,35 @@
     data : dict
         All the data stored in the specified dimension. The outermost keys are the stellar parameters for the models. The next keys are the lithium abundances. The innermost keys are 'flux' which retreives the NLTE flux or 'fluxl' which retreives the LTE flux. If split is used then the outermost keys are the split sets (either 'train' or 'test').
     """
 
     # set default data_path
     data_path = data_path or _base_path.parent / 'Balder'
     
+    # compact files
     D_path = _get_dimension_path(D = D, a = a, v = v, data_path = data_path)
     if os.path.exists(f'{D_path}.npy'):
-        return np.load(f'{D_path}.npy', allow_pickle=True).item()
+        stored_data = np.load(f'{D_path}.npy')
+        data = {}
+        for eff_t, surf_g, met, abund, ftype, *flux in stored_data:
+            # set ftype
+            if ftype == 0:
+                ftype = 'flux'
+            elif ftype == 1:
+                ftype = 'fluxl'
+            # create sp dict
+            if (eff_t, surf_g, met) not in data.keys():
+                data[eff_t, surf_g, met] = {}
+            # create abund dict
+            if abund not in data[eff_t, surf_g, met].keys():
+                data[eff_t, surf_g, met][abund] = {}
+            data[eff_t, surf_g, met][abund][ftype] = flux
+        return data
 
+    # loose files
     models = os.listdir(D_path)
     data = {}
     for model in models:
         eff_t = float(model[1:8])
         surf_g = float(model[9:13])
         met = float(model[13+1:])
         data[eff_t, surf_g, met] = read_all_abund(eff_t, surf_g, met, D = D, a = a, v = v, data_path = data_path)
```

### Comparing `breidablik-1.1.0/breidablik/analysis/test_read.py` & `breidablik-1.2.0/breidablik/analysis/test_read.py`

 * *Files identical despite different names*

### Comparing `breidablik-1.1.0/breidablik/analysis/test_tools.py` & `breidablik-1.2.0/breidablik/analysis/test_tools.py`

 * *Files identical despite different names*

### Comparing `breidablik-1.1.0/breidablik/analysis/tools.py` & `breidablik-1.2.0/breidablik/analysis/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,45 +24,52 @@
     wavelength = np.array(wavelength)
 
     low = center - lower
     high = center + upper
     wl_cut = wavelength[(low <= wavelength) & (high >= wavelength)]
     return wl_cut
 
-def cut(wavelength, line_profile, center = 670.9659, upper = 10, lower = 10):
+def cut(wavelength, line_profile, errors = None, center = 670.9659, upper = 10, lower = 10):
     """Cuts the wavelength and line profile and returns the values between center - lower and center + upper.
 
     Parameters
     ----------
     wavelength : List[Real] or 1darray
         Input wavelengths. Needs to be monotonically increasing.
     line_profile : List[Real] or 1darray
         Input line profile.
+    errors : List[Real] or 1darray, optional
+        Errors associated with input line profile. If using synthetic spectra, then no errors, leave as default value. 
     center : Real, optional
         The center of the wavelengths where the cut should be taken, in the same units as the wavelength. The 3 lithium lines are centered at 610.5298, 670.9659, and 812.8606 nm in the Balder results.
     upper : Positive Real, optional
         The amount to go above the center when taking the cut, in the same units as the wavelength.
     lower : Positive Real, optional
         The amount to go below the center when taking the cut, in the same units as the wavelength.
 
     Returns
     -------
-    cut_data : 2darray
-        Cut wavelengths and line profiles.
+    cut_data : ndarray
+        Cut wavelengths and line profiles, errors if provided.
     """
 
     wavelength = np.array(wavelength)
     line_profile = np.array(line_profile)
+    if errors is not None:
+        errors = np.array(errors)
 
     low = center - lower
     high = center + upper
     mask = (low <= wavelength) & (high >= wavelength)
     wl_cut = wavelength[mask]
     line_cut = line_profile[mask]
-    cut_data = np.array([wl_cut, line_cut])
+    if errors is not None:
+        cut_data = np.array([wl_cut, line_cut, errors[mask]])
+    else:
+        cut_data = np.array([wl_cut, line_cut])
     return cut_data
 
 def rew(wavelength, line_profile, center = 670.9659, upper = 10, lower = 10, num = 10000):
     """Calculates the reduced equivlanet width (REW) of the line profile between center - lower and center + upper.
 
     Parameters
     ----------
```

### Comparing `breidablik-1.1.0/breidablik/grid_snapshot.txt` & `breidablik-1.2.0/breidablik/grid_snapshot.txt`

 * *Files identical despite different names*

### Comparing `breidablik-1.1.0/breidablik/interpolate/grid_check.py` & `breidablik-1.2.0/breidablik/interpolate/grid_check.py`

 * *Files identical despite different names*

### Comparing `breidablik-1.1.0/breidablik/interpolate/nlte.py` & `breidablik-1.2.0/breidablik/interpolate/nlte.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,28 +19,28 @@
         model_path : str, optional
             The path to the rew model to be used to predict the lithium abundance. By default, this path points to ``models/nlte.pkl`` in ``breidablik``.
         scalar_path : str, optional
             The path to the scalar corresponding to the rew model. By default, this path points to ``models/nlte_scalar.pkl`` in ``breidablik``.
         """
 
         # set default paths
-        model_path = model_path or _base_path.parent / 'models1/nlte'
-        scalar_path = scalar_path or _base_path.parent / 'models1/nlte/scalar.npy'
-        model_path_610 = model_path_610 or _base_path.parent / 'models1/nlte_610'
-        scalar_path_610 = scalar_path_610 or _base_path.parent / 'models1/nlte_610/scalar.npy'
-        model_path_810 = model_path_810 or _base_path.parent / 'models1/nlte_810'
-        scalar_path_810 = scalar_path_810 or _base_path.parent / 'models1/nlte_810/scalar.npy'
+        model_path = model_path or _base_path.parent / 'models/nlte'
+        scalar_path = scalar_path or _base_path.parent / 'models/nlte/scalar.npy'
+        model_path_610 = model_path_610 or _base_path.parent / 'models/nlte_610'
+        scalar_path_610 = scalar_path_610 or _base_path.parent / 'models/nlte_610/scalar.npy'
+        model_path_810 = model_path_810 or _base_path.parent / 'models/nlte_810'
+        scalar_path_810 = scalar_path_810 or _base_path.parent / 'models/nlte_810/scalar.npy'
         # load models
         scalar = Scalar()
         scalar.load(scalar_path)
         scalar_610 = Scalar()
         scalar_610.load(scalar_path_610)
         scalar_810 = Scalar()
         scalar_810.load(scalar_path_810)
-        self.models = [FFNN(0, 0, model=str(model_path_610)), FFNN(0, 0, model=str(model_path)), FFNN(0, 0, model=str(model_path_810))]
+        self.models = [FFNN(model=str(model_path_610)), FFNN(model=str(model_path)), FFNN(model=str(model_path_810))]
         self.scalars = [scalar_610, scalar, scalar_810]
 
     def nlte_correction(self, eff_t, surf_g, met, abundance, center = 670.9659):
         """Find the abundance based on the stellar parameters and measured reduced equivalent width.
 
         rew : Real
             The reduced equivalent width for the lithium line at 670.9 nm.
@@ -76,10 +76,10 @@
         line_centers = np.array([610.5298, 670.9659, 812.8606])
         # get which model is being used
         ind = np.argmin(np.abs(line_centers - center))
         # predict lithium abundance
         scalar = self.scalars[ind]
         model = self.models[ind]
         transformed_input = scalar.transform([[eff_t, surf_g, met, a] for a in abunds])
-        nltec = model.predict(transformed_input)
+        nltec = model(transformed_input)
 
         return nltec
```

### Comparing `breidablik-1.1.0/breidablik/interpolate/rew.py` & `breidablik-1.2.0/breidablik/interpolate/rew.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,28 +19,28 @@
         model_path : str, optional
             The path to the rew model to be used to predict the lithium abundance. By default, this path points to ``models/rew.pkl`` in ``breidablik``.
         scalar_path : str, optional
             The path to the scalar corresponding to the rew model. By default, this path points to ``models/rew_scalar.pkl`` in ``breidablik``.
         """
 
         # set default paths
-        model_path = model_path or _base_path.parent / 'models1/rew'
-        scalar_path = scalar_path or _base_path.parent / 'models1/rew/scalar.npy'
-        model_path_610 = model_path_610 or _base_path.parent / 'models1/rew_610'
-        scalar_path_610 = scalar_path_610 or _base_path.parent / 'models1/rew_610/scalar.npy'
-        model_path_810 = model_path_810 or _base_path.parent / 'models1/rew_810'
-        scalar_path_810 = scalar_path_810 or _base_path.parent / 'models1/rew_810/scalar.npy'
+        model_path = model_path or _base_path.parent / 'models/rew'
+        scalar_path = scalar_path or _base_path.parent / 'models/rew/scalar.npy'
+        model_path_610 = model_path_610 or _base_path.parent / 'models/rew_610'
+        scalar_path_610 = scalar_path_610 or _base_path.parent / 'models/rew_610/scalar.npy'
+        model_path_810 = model_path_810 or _base_path.parent / 'models/rew_810'
+        scalar_path_810 = scalar_path_810 or _base_path.parent / 'models/rew_810/scalar.npy'
         # load models
         scalar = Scalar()
         scalar.load(scalar_path)
         scalar_610 = Scalar()
         scalar_610.load(scalar_path_610)
         scalar_810 = Scalar()
         scalar_810.load(scalar_path_810)
-        self.models = [FFNN(0, 0, model=str(model_path_610)), FFNN(0, 0, model=str(model_path)), FFNN(0, 0, model=str(model_path_810))]
+        self.models = [FFNN(model=str(model_path_610)), FFNN(model=str(model_path)), FFNN(model=str(model_path_810))]
         self.scalars = [scalar_610, scalar, scalar_810]
 
     def find_abund(self, eff_t, surf_g, met, rew, center = 670.9659):
         """Find the abundance based on the stellar parameters and measured reduced equivalent width.
 
         Parameters
         ----------
@@ -83,10 +83,10 @@
         line_centers = np.array([610.5298, 670.9659, 812.8606])
         # get which model is being used
         ind = np.argmin(np.abs(line_centers - center))
         # predict lithium abundance
         scalar = self.scalars[ind]
         model = self.models[ind]
         transformed_input = scalar.transform([[eff_t, surf_g, met, r] for r in rew])
-        predicted_li = model.predict(transformed_input)
+        predicted_li = model(transformed_input)
 
         return predicted_li
```

### Comparing `breidablik-1.1.0/breidablik/interpolate/scalar.py` & `breidablik-1.2.0/breidablik/interpolate/scalar.py`

 * *Files identical despite different names*

### Comparing `breidablik-1.1.0/breidablik/interpolate/spectra.py` & `breidablik-1.2.0/breidablik/interpolate/spectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         scalar_path : str, optional
             The path to the scalar corresponding to the model. By default, this path points to ``models/kri/scalar.npy`` in ``breidablik``.
         save_num : int
             The number of cubic spline models to save. This makes the code run faster, but takes memory. Only worth increasing if you are repeatedly analysing different observations of multiple stars.
         """
 
         # set default paths
-        model_path = model_path or _base_path.parent / 'models1/rbf'
-        scalar_path = scalar_path or _base_path.parent / 'models1/rbf/scalar.npy'
+        model_path = model_path or _base_path.parent / 'models/rbf'
+        scalar_path = scalar_path or _base_path.parent / 'models/rbf/scalar.npy'
         # load models
         self.scalar = Scalar()
         self.scalar.load(scalar_path)
         self.models = np.load(os.path.join(model_path, 'rbf.npy'))
         self.X = np.load(os.path.join(model_path, 'X.npy'))
         self.relative_error = np.load(os.path.join(model_path, 'relative_err.npy'), allow_pickle = False)
         self.save_num = save_num
```

### Comparing `breidablik-1.1.0/breidablik/interpolate/test_nlte.py` & `breidablik-1.2.0/breidablik/interpolate/test_nlte.py`

 * *Files identical despite different names*

### Comparing `breidablik-1.1.0/breidablik/interpolate/test_rew.py` & `breidablik-1.2.0/breidablik/interpolate/test_rew.py`

 * *Files identical despite different names*

### Comparing `breidablik-1.1.0/breidablik/interpolate/test_scalar.py` & `breidablik-1.2.0/breidablik/interpolate/test_scalar.py`

 * *Files identical despite different names*

### Comparing `breidablik-1.1.0/breidablik/interpolate/test_spectra.py` & `breidablik-1.2.0/breidablik/interpolate/test_spectra.py`

 * *Files identical despite different names*

### Comparing `breidablik-1.1.0/breidablik.egg-info/PKG-INFO` & `breidablik-1.2.0/breidablik.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breidablik
-Version: 1.1.0
+Version: 1.2.0
 Summary: Interpolate lithium spectra and predict lithium abundance for most main sequence stars
 Home-page: https://github.com/ellawang44/Breidablik
 Author: Ella Xi Wang
 Author-email: Ella Xi Wang <xi.wang3@anu.edu.au>
 Project-URL: Bug Reports, https://github.com/ellawang44/Breidablik/issues
 Project-URL: Source, https://github.com/ellawang44/Breidablik
 Keywords: lithium star spectroscopy
@@ -42,15 +42,15 @@
 ./install
 ```
 
 #### Manual
 If the above automatic installation did not work for you, then to install without using `pip`, there are 5 steps:
 1. Navigate to where you want this repository and clone this git repository.
 2. Navigate into `Breidablik/breidablik`.
-3. Download the models from `models.zip` on http://www.mso.anu.edu.au/~ellawang/ and unzip it.
+3. Download the models from `models_vx.x.x.zip` on http://www.mso.anu.edu.au/~ellawang/ and unzip it. Pick the model based on the version of Breidablik you want to run. The model version number will be just lower than your Breidablik version number. e.g. running Breidablik v1.1.0 will require models v1.0.0. 
 4. Optional, download the raw data from `balder.zip` on http://www.mso.anu.edu.au/~ellawang/ and unzip it.
 5. Optional, add this directory to the python path. This makes the directory findable by python no matter where it is launched.
 
 ### Check that your installation is correct
 Optional, to check that the installation was successful, in the `Breidablik` folder, you can run:
 ```
 python -m pytest
```

### Comparing `breidablik-1.1.0/breidablik.egg-info/SOURCES.txt` & `breidablik-1.2.0/breidablik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `breidablik-1.1.0/setup.py` & `breidablik-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.1.0',  # Required
+    version='1.2.0',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Interpolate lithium spectra and predict lithium abundance for most main sequence stars',  # Optional
 
     # This is an optional longer description of your project that represents
@@ -132,15 +132,14 @@
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     install_requires=['hypothesis>=4.17',
                       'numpy>=1.15',
-                      'torch>=1.12',
                       'scipy>=1.3',
                       'pytest>=3.5'],  # Optional
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
```

