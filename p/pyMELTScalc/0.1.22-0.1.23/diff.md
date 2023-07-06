# Comparing `tmp/pyMELTScalc-0.1.22.tar.gz` & `tmp/pyMELTScalc-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyMELTScalc-0.1.22.tar", last modified: Thu Jun 29 20:48:14 2023, max compression
+gzip compressed data, was "pyMELTScalc-0.1.23.tar", last modified: Wed Jul  5 23:57:41 2023, max compression
```

## Comparing `pyMELTScalc-0.1.22.tar` & `pyMELTScalc-0.1.23.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:48:14.477933 pyMELTScalc-0.1.22/
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-29 20:48:14.477933 pyMELTScalc-0.1.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 20:48:14.477933 pyMELTScalc-0.1.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:48:14.473933 pyMELTScalc-0.1.22/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:48:14.473933 pyMELTScalc-0.1.22/src/pyMELTScalc/
--rw-r--r--   0 runner    (1001) docker     (123)    42082 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/Barom.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/GenFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/Holland.py
--rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/Liq.py
--rw-r--r--   0 runner    (1001) docker     (123)    43028 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/MELTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    24305 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/Path.py
--rw-r--r--   0 runner    (1001) docker     (123)    21663 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/Path_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/PhaseDiagrams.py
--rw-r--r--   0 runner    (1001) docker     (123)    24584 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/Plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/Saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:48:14.477933 pyMELTScalc-0.1.22/src/pyMELTScalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-29 20:48:14.000000 pyMELTScalc-0.1.22/src/pyMELTScalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-29 20:48:14.000000 pyMELTScalc-0.1.22/src/pyMELTScalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:48:14.000000 pyMELTScalc-0.1.22/src/pyMELTScalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 20:48:14.000000 pyMELTScalc-0.1.22/src/pyMELTScalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 20:48:14.000000 pyMELTScalc-0.1.22/src/pyMELTScalc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:57:41.478172 pyMELTScalc-0.1.23/
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-05 23:57:41.478172 pyMELTScalc-0.1.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-05 23:57:26.000000 pyMELTScalc-0.1.23/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 23:57:41.478172 pyMELTScalc-0.1.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-05 23:57:27.000000 pyMELTScalc-0.1.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:57:41.474172 pyMELTScalc-0.1.23/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:57:41.474172 pyMELTScalc-0.1.23/src/pyMELTScalc/
+-rw-r--r--   0 runner    (1001) docker     (123)    43203 2023-07-05 23:57:27.000000 pyMELTScalc-0.1.23/src/pyMELTScalc/Barom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-07-05 23:57:27.000000 pyMELTScalc-0.1.23/src/pyMELTScalc/GenFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-05 23:57:27.000000 pyMELTScalc-0.1.23/src/pyMELTScalc/Holland.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-07-05 23:57:27.000000 pyMELTScalc-0.1.23/src/pyMELTScalc/Liq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43058 2023-07-05 23:57:27.000000 pyMELTScalc-0.1.23/src/pyMELTScalc/MELTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-07-05 23:57:27.000000 pyMELTScalc-0.1.23/src/pyMELTScalc/Path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21698 2023-07-05 23:57:27.000000 pyMELTScalc-0.1.23/src/pyMELTScalc/Path_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-07-05 23:57:27.000000 pyMELTScalc-0.1.23/src/pyMELTScalc/PhaseDiagrams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25070 2023-07-05 23:57:27.000000 pyMELTScalc-0.1.23/src/pyMELTScalc/Plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-07-05 23:57:27.000000 pyMELTScalc-0.1.23/src/pyMELTScalc/Saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-05 23:57:27.000000 pyMELTScalc-0.1.23/src/pyMELTScalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-05 23:57:27.000000 pyMELTScalc-0.1.23/src/pyMELTScalc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:57:41.474172 pyMELTScalc-0.1.23/src/pyMELTScalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-05 23:57:41.000000 pyMELTScalc-0.1.23/src/pyMELTScalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-05 23:57:41.000000 pyMELTScalc-0.1.23/src/pyMELTScalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 23:57:41.000000 pyMELTScalc-0.1.23/src/pyMELTScalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-05 23:57:41.000000 pyMELTScalc-0.1.23/src/pyMELTScalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 23:57:41.000000 pyMELTScalc-0.1.23/src/pyMELTScalc.egg-info/top_level.txt
```

### Comparing `pyMELTScalc-0.1.22/PKG-INFO` & `pyMELTScalc-0.1.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyMELTScalc
-Version: 0.1.22
+Version: 0.1.23
 Summary: pyMELTScalc
 Home-page: https://github.com/gleesonm1/pyMELTScalc
 Author: Matthew Gleeson
 Author-email: gleesonm@berkeley.edu
 License: UNKNOWN
 Description: ## ReadTheDocs
```

### Comparing `pyMELTScalc-0.1.22/README.md` & `pyMELTScalc-0.1.23/README.md`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.22/setup.py` & `pyMELTScalc-0.1.23/setup.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.22/src/pyMELTScalc/GenFuncs.py` & `pyMELTScalc-0.1.23/src/pyMELTScalc/GenFuncs.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.22/src/pyMELTScalc/Holland.py` & `pyMELTScalc-0.1.23/src/pyMELTScalc/Holland.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.22/src/pyMELTScalc/Liq.py` & `pyMELTScalc-0.1.23/src/pyMELTScalc/Liq.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.22/src/pyMELTScalc/MELTS.py` & `pyMELTScalc-0.1.23/src/pyMELTScalc/MELTS.py`

 * *Files 1% similar despite different names*

```diff
@@ -506,17 +506,17 @@
 
     Returns:
     ----------
     Results: Dict
         Dict containing a float for each saturation temperature found and the T_Liq and melt H2O values.
 
     '''
-    Results = {'a_sat': np.nan, 'b_sat': np.nan, 'c_sat': np.nan, 'T_Liq': np.nan, 'H2O_melt': np.nan}
+    Results = {phases[0]: np.nan, phases[1]: np.nan, phases[2]: np.nan, 'T_Liq': np.nan, 'H2O_melt': np.nan}
     if len(phases) == 2:
-        del Results['c_sat']
+        del Results[phases[2]]
 
     from meltsdynamic import MELTSdynamic
 
     if Model is None or Model == "MELTSv1.0.2":
         melts = MELTSdynamic(1)
     elif Model == "pMELTS":
         melts = MELTSdynamic(2)
@@ -565,29 +565,29 @@
                 PhaseList = melts.engine.solidNames
                 print(PhaseList)
                 if 'tridymite1' in PhaseList:
                     PhaseList = ['quartz1'] + PhaseList
                 if 'clinopyroxene2' in PhaseList:
                     PhaseList = ['orthopyroxene1'] + PhaseList
 
-                if phases[0] in PhaseList and np.isnan(Results['a_sat']):# == 0:
-                    Results['a_sat'] = melts.engine.temperature
+                if phases[0] in PhaseList and np.isnan(Results[phases[0]]):# == 0:
+                    Results[phases[0]] = melts.engine.temperature
 
-                if phases[1] in PhaseList and np.isnan(Results['b_sat']):# == 0:
-                    Results['b_sat'] = melts.engine.temperature
+                if phases[1] in PhaseList and np.isnan(Results[phases[1]]):# == 0:
+                    Results[phases[1]] = melts.engine.temperature
 
                 if len(phases) == 3:
-                    if phases[2] in PhaseList and np.isnan(Results['c_sat']):# == 0:
-                        Results['c_sat'] = melts.engine.temperature
+                    if phases[2] in PhaseList and np.isnan(Results[phases[2]]):# == 0:
+                        Results[phases[2]] = melts.engine.temperature
 
-                    if ~np.isnan(Results['a_sat']) and ~np.isnan(Results['b_sat']) and ~np.isnan(Results['c_sat']):# > 0:
+                    if ~np.isnan(Results[phases[0]]) and ~np.isnan(Results[phases[1]]) and ~np.isnan(Results[phases[2]]):# > 0:
                         break
 
                 if len(phases) == 2:
-                    if ~np.isnan(Results['a_sat']) and ~np.isnan(Results['b_sat']):# > 0:
+                    if ~np.isnan(Results[phases[0]]) and ~np.isnan(Results[phases[1]]):# > 0:
                         break
 
                 T = T - T_step_C
             except:
                 T = T - T_step_C
```

### Comparing `pyMELTScalc-0.1.22/src/pyMELTScalc/Path.py` & `pyMELTScalc-0.1.23/src/pyMELTScalc/Path.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,20 @@
     Returns:
     ----------
     Results: Dict
         Dictionary where each entry represents the results of a single calculation. Within the dictionary each single calculation is reported as a series of pandas DataFrames, displaying the composition and thermodynamic properties of each phase.
 
     '''
 
+    if Frac_solid is False:
+        Frac_solid = None
+
+    if Frac_fluid is False:
+        Frac_fluid = None
+
     comp = bulk.copy()
     # set default values if required
     if Model is None:
         Model == "MELTSv1.0.2"
 
     # if comp is entered as a pandas series, it must first be converted to a dict
     if type(comp) == pd.core.series.Series:
```

### Comparing `pyMELTScalc-0.1.22/src/pyMELTScalc/Path_wrappers.py` & `pyMELTScalc-0.1.23/src/pyMELTScalc/Path_wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pandas as pd
 from pyMELTScalc.Path import *
 
-def isobaric_crystallisation(Model = None, bulk = None, Frac_solid = None, Frac_fluid = None, T_path_C = None, T_start_C = None, T_end_C = None, dt_C = None, P_bar = None, Fe3Fet_Liq = None, H2O_Liq = None, find_liquidus = None, fO2_buffer = None, fO2_offset = None, label = None, Crystallinity_limit = None, fluid_sat = None, timeout = None):
+def isobaric_crystallisation(Model = None, bulk = None, Frac_solid = None, Frac_fluid = None, T_path_C = None, T_start_C = None, T_end_C = None, dt_C = None, P_bar = None, Fe3Fet_Liq = None, H2O_Liq = None, CO2_Liq = None, find_liquidus = None, fO2_buffer = None, fO2_offset = None, label = None, Crystallinity_limit = None, fluid_sat = None, timeout = None):
     '''
     Computes isobaric crystallization paths using the multi_path function,which
     computes the phase equilibria between solid, liquid and fluid phases.
 
     Model: string
         "MELTS" or "Holland". Dictates whether MELTS or MAGEMin calculations are performed. Default "MELTS".
         Version of melts can be specified "MELTSv1.0.2", "MELTSv1.1.0", "MELTSv1.2.0", or "pMELTS". Default "v.1.0.2".
@@ -59,15 +59,15 @@
     Returns:
     ----------
     Results: Dict
         Dictionary where each entry represents the results of a single calculation. Within the dictionary each single calculation is reported as a series of pandas DataFrames, displaying the composition and thermodynamic properties of each phase.
     '''
     comp = bulk.copy()
 
-    Results = multi_path(Model = Model, bulk = comp, Frac_solid = Frac_solid, Frac_fluid = Frac_fluid, T_path_C = T_path_C, T_start_C = T_start_C, T_end_C = T_end_C, dt_C = dt_C, P_bar = P_bar, Fe3Fet_Liq = Fe3Fet_Liq, H2O_Liq = H2O_Liq, find_liquidus = find_liquidus, fO2_buffer = fO2_buffer, fO2_offset = fO2_offset, label = label, Crystallinity_limit = Crystallinity_limit, fluid_sat = fluid_sat, timeout = timeout)
+    Results = multi_path(Model = Model, bulk = comp, Frac_solid = Frac_solid, Frac_fluid = Frac_fluid, T_path_C = T_path_C, T_start_C = T_start_C, T_end_C = T_end_C, dt_C = dt_C, P_bar = P_bar, Fe3Fet_Liq = Fe3Fet_Liq, H2O_Liq = H2O_Liq, CO2_Liq = CO2_Liq, find_liquidus = find_liquidus, fO2_buffer = fO2_buffer, fO2_offset = fO2_offset, label = label, Crystallinity_limit = Crystallinity_limit, fluid_sat = fluid_sat, timeout = timeout)
 
     return Results
 
 def isochoric_crystallisation(Model = None, bulk = None, Frac_solid = None, Frac_fluid = None, T_path_C = None, T_start_C = None, T_end_C = None, dt_C = None, P_bar = None, Fe3Fet_Liq = None, H2O_Liq = None, find_liquidus = None, fO2_buffer = None, fO2_offset = None, label = None, Crystallinity_limit = None, fluid_sat = None, timeout = None):
     '''
     Computes isochorics crystallization paths using the multi_path function,which
     computes the phase equilibria between solid, liquid and fluid phases.
```

### Comparing `pyMELTScalc-0.1.22/src/pyMELTScalc/PhaseDiagrams.py` & `pyMELTScalc-0.1.23/src/pyMELTScalc/PhaseDiagrams.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.22/src/pyMELTScalc/Plotting.py` & `pyMELTScalc-0.1.23/src/pyMELTScalc/Plotting.py`

 * *Files 8% similar despite different names*

```diff
@@ -127,35 +127,35 @@
 def plot_surfaces(Results = None, P_bar = None, phases = None, H2O_Liq = None):
     if H2O_Liq is None:
         f, a = plt.subplots(1,1, figsize = (5,4))
         a.set_xlabel('P (bars)')
         a.set_ylabel('T ($\degree$C)')
         for i in range(len(phases)):
             if i == 0:
-                a.plot(P_bar, Results['a_sat'][0,0,:], '-r', linewidth = 2, label = phases[i])
+                a.plot(P_bar, Results[phases[0]][0,0,:], '-r', linewidth = 2, label = phases[i])
             if i == 1:
-                a.plot(P_bar, Results['b_sat'][0,0,:], '-b', linewidth = 2, label = phases[i])
+                a.plot(P_bar, Results[phases[1]][0,0,:], '-b', linewidth = 2, label = phases[i])
             if i == 2:
-                a.plot(P_bar, Results['c_sat'][0,0,:], '-k', linewidth = 2, label = phases[i])
+                a.plot(P_bar, Results[phases[2]][0,0,:], '-k', linewidth = 2, label = phases[i])
 
         a.legend()
 
     if H2O_Liq is not None:
         X, Y = np.meshgrid(P_bar, H2O_Liq)
         Y = Results['H2O_melt'][:,0,:].copy()
 
         f = plt.figure(figsize = (5,4))
         a = f.add_subplot(1,1,1, projection = '3d')
         for i in range(len(phases)):
             if i == 0:
-                a.plot_surface(X, Y, Results['a_sat'][:,0,:], color = 'r', label = phases[i])
+                a.plot_surface(X, Y, Results[phases[0]][:,0,:], color = 'r', label = phases[i])
             if i == 1:
-                a.plot_surface(X, Y, Results['b_sat'][:,0,:], color = 'b', label = phases[i])
+                a.plot_surface(X, Y, Results[phases[1]][:,0,:], color = 'b', label = phases[i])
             if i == 2:
-                a.plot_surface(X, Y, Results['c_sat'][:,0,:], color = 'k', label = phases[i])
+                a.plot_surface(X, Y, Results[phases[2]][:,0,:], color = 'k', label = phases[i])
 
     return f, a
 
 def residualT_plot(Results = None, P_bar = None, phases = None, H2O_Liq = None, Fe3Fet_Liq = None, T_cut_C = None):
 
     if T_cut_C is None:
         T_cut_C = 12
@@ -165,15 +165,15 @@
             f, a = plt.subplots(2,2, figsize = (10,8), sharex = True, sharey = True)
             f.tight_layout()
             a[1][0].set_xlabel('P (bars)')
             a[1][1].set_xlabel('P (bars)')
             a[0][0].set_ylabel('Residual T ($\degree$C)')
             a[1][0].set_ylabel('Residual T ($\degree$C)')
 
-            m = np.array([['Res_abc', 'Res_ab'], ['Res_ac', 'Res_bc']])
+            m = np.array([['3 Phase Saturation', phases[0] + ' - ' + phases[1]], [phases[0] + ' - ' + phases[2], phases[1] + ' - ' + phases[2]]])
             Name = np.array([['Three phase saturation', phases[0] + ' - ' + phases[1]],
                 [phases[0] + ' - ' + phases[2], phases[1] + ' - ' + phases[2]]])
 
             for i in range(2):
                 for j in range(2):
                     a[i][j].set_title(Name[i,j])
                     if ~np.isnan(Results['CurveMin'][m[i,j]]['P_min']):
@@ -186,35 +186,35 @@
                                     [np.nanmin(Results['CurveMin'][m[i,j]]['y_new']) - 5,
                                     np.nanmax(Results['CurveMin'][m[i,j]]['y_new']) + 5], ':k')
         else:
             f, a = plt.subplots(1,1, figsize = (5,4))
             a.set_xlabel('P (bars)')
             a.set_ylabel('Residual T ($\degree$C)')
             a.set_title(phases[0] + ' - ' + phases[1])
-            if ~np.isnan(Results['CurveMin']['Res_ab']['P_min']):
-                a.plot(P_bar, Results['Res_ab'][0,0,:], 'ok', markerfacecolor="b", label="original", markersize = 8)
-                a.plot(Results['CurveMin']['Res_ab']['P_new'], Results['CurveMin']['Res_ab']['y_new'],
+            if ~np.isnan(Results['CurveMin'][phases[0] + ' - ' + phases[1]]['P_min']):
+                a.plot(P_bar, Results[phases[0] + ' - ' + phases[1]][0,0,:], 'ok', markerfacecolor="b", label="original", markersize = 8)
+                a.plot(Results['CurveMin'][phases[0] + ' - ' + phases[1]]['P_new'], Results['CurveMin'][phases[0] + ' - ' + phases[1]]['y_new'],
                             '-', c="r", label="spline fit")
-                a.plot([np.nanmin(Results['CurveMin']['Res_ab']['P_new']), np.nanmax(Results['CurveMin']['Res_ab']['P_new'])],
-                            [Results['CurveMin']['Res_ab']['Res_min'], Results['CurveMin']['Res_ab']['Res_min']], ':k')
-                a.plot([Results['CurveMin']['Res_ab']['P_min'], Results['CurveMin']['Res_ab']['P_min']],
-                            [np.nanmin(Results['CurveMin']['Res_ab']['y_new']) - 5,
-                            np.nanmax(Results['CurveMin']['Res_ab']['y_new']) + 5], ':k')
+                a.plot([np.nanmin(Results['CurveMin'][phases[0] + ' - ' + phases[1]]['P_new']), np.nanmax(Results['CurveMin'][phases[0] + ' - ' + phases[1]]['P_new'])],
+                            [Results['CurveMin'][phases[0] + ' - ' + phases[1]]['Res_min'], Results['CurveMin'][phases[0] + ' - ' + phases[1]]['Res_min']], ':k')
+                a.plot([Results['CurveMin'][phases[0] + ' - ' + phases[1]]['P_min'], Results['CurveMin'][phases[0] + ' - ' + phases[1]]['P_min']],
+                            [np.nanmin(Results['CurveMin'][phases[0] + ' - ' + phases[1]]['y_new']) - 5,
+                            np.nanmax(Results['CurveMin'][phases[0] + ' - ' + phases[1]]['y_new']) + 5], ':k')
 
     if H2O_Liq is not None and Fe3Fet_Liq is None:
         if len(Results['CurveMin']) == 4:
             f = plt.figure(figsize = (10,8))
             a1 = f.add_subplot(2,2,1, projection = '3d')
             a2 = f.add_subplot(2,2,2, projection = '3d')
             a3 = f.add_subplot(2,2,3, projection = '3d')
             a4 = f.add_subplot(2,2,4, projection = '3d')
 
             a = np.array([[a1,a2], [a3, a4]])
 
-            m = np.array([['Res_abc', 'Res_ab'], ['Res_ac', 'Res_bc']])
+            m = np.array([['3 Phase Saturation', phases[0] + ' - ' + phases[1]], [phases[0] + ' - ' + phases[2], phases[1] + ' - ' + phases[2]]])
             Name = np.array([['Three phase saturation', phases[0] + ' - ' + phases[1]],
                 [phases[0] + ' - ' + phases[2], phases[1] + ' - ' + phases[2]]])
 
             X, Y = np.meshgrid(P_bar, H2O_Liq)
             Y = Results['H2O_melt'][:,0,:].copy()
 
             for i in range(2):
@@ -273,15 +273,15 @@
             a1 = f.add_subplot(2,2,1, projection = '3d')
             a2 = f.add_subplot(2,2,2, projection = '3d')
             a3 = f.add_subplot(2,2,3, projection = '3d')
             a4 = f.add_subplot(2,2,4, projection = '3d')
 
             a = np.array([[a1,a2], [a3, a4]])
 
-            m = np.array([['Res_abc', 'Res_ab'], ['Res_ac', 'Res_bc']])
+            m = np.array([['3 Phase Saturation', phases[0] + ' - ' + phases[1]], [phases[0] + ' - ' + phases[2], phases[1] + ' - ' + phases[2]]])
             Name = np.array([['Three phase saturation', phases[0] + ' - ' + phases[1]],
                 [phases[0] + ' - ' + phases[2], phases[1] + ' - ' + phases[2]]])
 
             X, Y = np.meshgrid(P_bar, H2O_Liq)
             Y = Results['H2O_melt'][:,0,:].copy()
 
             for i in range(2):
```

### Comparing `pyMELTScalc-0.1.22/src/pyMELTScalc/Saturation.py` & `pyMELTScalc-0.1.23/src/pyMELTScalc/Saturation.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.22/src/pyMELTScalc/__init__.py` & `pyMELTScalc-0.1.23/src/pyMELTScalc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.22/src/pyMELTScalc.egg-info/PKG-INFO` & `pyMELTScalc-0.1.23/src/pyMELTScalc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyMELTScalc
-Version: 0.1.22
+Version: 0.1.23
 Summary: pyMELTScalc
 Home-page: https://github.com/gleesonm1/pyMELTScalc
 Author: Matthew Gleeson
 Author-email: gleesonm@berkeley.edu
 License: UNKNOWN
 Description: ## ReadTheDocs
```

### Comparing `pyMELTScalc-0.1.22/src/pyMELTScalc.egg-info/SOURCES.txt` & `pyMELTScalc-0.1.23/src/pyMELTScalc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

