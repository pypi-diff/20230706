# Comparing `tmp/EzGM-1.6.6.3.tar.gz` & `tmp/EzGM-1.7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EzGM-1.6.6.3.tar", last modified: Thu Jun 15 07:59:34 2023, max compression
+gzip compressed data, was "EzGM-1.7.0.0.tar", last modified: Thu Jul  6 13:04:58 2023, max compression
```

## Comparing `EzGM-1.6.6.3.tar` & `EzGM-1.7.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 07:59:34.541960 EzGM-1.6.6.3/
-drwxrwxrwx   0        0        0        0 2023-06-15 07:59:34.499436 EzGM-1.6.6.3/EzGM/
--rw-rw-rw-   0        0        0      105 2022-10-20 15:03:59.000000 EzGM-1.6.6.3/EzGM/__init__.py
--rw-rw-rw-   0        0        0   180460 2023-06-15 07:17:54.000000 EzGM-1.6.6.3/EzGM/selection.py
--rw-rw-rw-   0        0        0    22786 2023-06-01 17:18:21.000000 EzGM-1.6.6.3/EzGM/signal.py
--rw-rw-rw-   0        0        0    55186 2023-06-15 07:54:21.000000 EzGM-1.6.6.3/EzGM/utility.py
--rw-rw-rw-   0        0        0    26111 2023-06-01 20:23:19.000000 EzGM-1.6.6.3/EzGM/webdriverdownloader.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:59:34.540960 EzGM-1.6.6.3/EzGM.egg-info/
--rw-rw-rw-   0        0        0     6801 2023-06-15 07:59:34.000000 EzGM-1.6.6.3/EzGM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-06-15 07:59:34.000000 EzGM-1.6.6.3/EzGM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 07:59:34.000000 EzGM-1.6.6.3/EzGM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2023-06-15 07:59:34.000000 EzGM-1.6.6.3/EzGM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-15 07:59:34.000000 EzGM-1.6.6.3/EzGM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2022-10-20 15:03:59.000000 EzGM-1.6.6.3/LICENSE
--rw-rw-rw-   0        0        0     6801 2023-06-15 07:59:34.543081 EzGM-1.6.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     6174 2023-03-09 12:54:15.000000 EzGM-1.6.6.3/README.md
--rw-rw-rw-   0        0        0      108 2022-10-20 15:03:59.000000 EzGM-1.6.6.3/pyproject.toml
--rw-rw-rw-   0        0        0      893 2023-06-15 07:59:34.553099 EzGM-1.6.6.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 13:04:58.889093 EzGM-1.7.0.0/
+drwxrwxrwx   0        0        0        0 2023-07-06 13:04:58.871161 EzGM-1.7.0.0/EzGM/
+-rw-rw-rw-   0        0        0      105 2022-10-20 15:03:59.000000 EzGM-1.7.0.0/EzGM/__init__.py
+-rw-rw-rw-   0        0        0   192509 2023-07-06 11:42:36.000000 EzGM-1.7.0.0/EzGM/selection.py
+-rw-rw-rw-   0        0        0    23416 2023-07-06 10:26:36.000000 EzGM-1.7.0.0/EzGM/signal.py
+-rw-rw-rw-   0        0        0    57027 2023-07-06 11:33:37.000000 EzGM-1.7.0.0/EzGM/utility.py
+-rw-rw-rw-   0        0        0    26111 2023-06-01 20:23:19.000000 EzGM-1.7.0.0/EzGM/webdriverdownloader.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:04:58.888126 EzGM-1.7.0.0/EzGM.egg-info/
+-rw-rw-rw-   0        0        0     6964 2023-07-06 13:04:58.000000 EzGM-1.7.0.0/EzGM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-07-06 13:04:58.000000 EzGM-1.7.0.0/EzGM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 13:04:58.000000 EzGM-1.7.0.0/EzGM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2023-07-06 13:04:58.000000 EzGM-1.7.0.0/EzGM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-06 13:04:58.000000 EzGM-1.7.0.0/EzGM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2022-10-20 15:03:59.000000 EzGM-1.7.0.0/LICENSE
+-rw-rw-rw-   0        0        0     6964 2023-07-06 13:04:58.889093 EzGM-1.7.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6337 2023-07-06 12:49:10.000000 EzGM-1.7.0.0/README.md
+-rw-rw-rw-   0        0        0      108 2022-10-20 15:03:59.000000 EzGM-1.7.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      893 2023-07-06 13:04:58.894078 EzGM-1.7.0.0/setup.cfg
```

### Comparing `EzGM-1.6.6.3/EzGM/selection.py` & `EzGM-1.7.0.0/EzGM/selection.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,25 +24,39 @@
 from matplotlib.ticker import ScalarFormatter, NullFormatter
 import matplotlib.pyplot as plt
 import requests
 from selenium import webdriver
 from .webdriverdownloader import ChromeDriverDownloader, GeckoDriverDownloader
 from numba import njit
 from openquake.hazardlib import gsim, imt, const
-from .utility import create_dir, ContentFromZip, ReadNGA, ReadESM
-from .utility import SiteParam_tbec2018, Sae_tbec2018, SiteParam_asce7_16, Sae_asce7_16, Sae_ec8_part1
+from .utility import make_dir, content_from_zip, read_nga, read_esm, get_esm_token
+from .utility import site_parameters_tbec2018, sae_tbec2018, site_parameters_asce7_16, sae_asce7_16, sae_ec8_part1
 from .utility import random_multivariate_normal
 
 
-class _subclass_:
+SMALL_SIZE = 15
+MEDIUM_SIZE = 16
+BIG_SIZE = 18
+BIGGER_SIZE = 20
+
+plt.rc('font', size=SMALL_SIZE)  # controls default text sizes
+plt.rc('axes', titlesize=SMALL_SIZE)  # fontsize of the axes title
+plt.rc('axes', labelsize=BIG_SIZE)  # fontsize of the x and y labels
+plt.rc('xtick', labelsize=SMALL_SIZE)  # fontsize of the tick labels
+plt.rc('ytick', labelsize=SMALL_SIZE)  # fontsize of the tick labels
+plt.rc('legend', fontsize=MEDIUM_SIZE)  # legend fontsize
+plt.rc('figure', titlesize=BIGGER_SIZE)  # fontsize of the figure title
+
+
+class _SubClass_:
     """
     Details
     -------
-    This subclass contains common methods inherited by the two parent classes:
-     conditional_spectrum and code_spectrum.
+    This sub-class contains common methods inherited by the two parent classes:
+    ConditionalSpectrum and CodeSpectrum.
     """
 
     def __init__(self):
         """
         Details
         -------
         Checks if Meta_Data folder exist inside EzGM. If it does not exist it is going to be retrieved
@@ -102,699 +116,743 @@
 
         Parameters
         ----------
         None.
 
         Returns
         -------
-        sampleBig : numpy.array
+        sample_big : numpy.ndarray
             An array which contains the IMLs from filtered database.
-        soil_Vs30 : numpy.array
+        vs30 : numpy.ndarray
             An array which contains the Vs30s from filtered database.
-        Mw : numpy.array
+        magnitude : numpy.ndarray
             An array which contains the magnitudes from filtered database.
-        Rjb : numpy.array
+        rjb : numpy.ndarray
             An array which contains the Rjbs from filtered database.
-        fault : numpy.array
-            An array which contains the fault type info from filtered database.
-        Filename_1 : numpy.array
+        mechanism : numpy.ndarray
+            An array which contains the fault mechanism info from filtered database.
+        filename1 : numpy.ndarray
             An array which contains the filename of 1st gm component from filtered database.
             If selection is set to 1, it will include filenames of both components.
-        Filename_2 : numpy.array
+        filename2 : numpy.ndarray
             An array which contains the filename of 2nd gm component filtered database.
             If selection is set to 1, it will be None value.
-        NGA_num : numpy.array
+        nga_num : numpy.ndarray
             If NGA_W2 is used as record database, record sequence numbers from filtered
             database will be saved, for other databases this variable is None.
-        eq_ID : numpy.array
+        eq_id : numpy.ndarray
             An array which contains event ids from filtered database.
-        station_code : numpy.array
+        station_code : numpy.ndarray
             If ESM_2018 is used as record database, station codes from filtered
             database will be saved, for other databases this variable is None.
         """
 
-        if self.selection == 1:  # SaKnown = Sa_arb
+        if self.num_components == 1:  # sa_known is from arbitrary ground motion component
 
-            SaKnown = np.append(self.database['Sa_1'], self.database['Sa_2'], axis=0)
-            soil_Vs30 = np.append(self.database['soil_Vs30'], self.database['soil_Vs30'], axis=0)
-            Mw = np.append(self.database['magnitude'], self.database['magnitude'], axis=0)
-            Rjb = np.append(self.database['Rjb'], self.database['Rjb'], axis=0)
-            fault = np.append(self.database['mechanism'], self.database['mechanism'], axis=0)
-            Filename_1 = np.append(self.database['Filename_1'], self.database['Filename_2'], axis=0)
-            eq_ID = np.append(self.database['EQID'], self.database['EQID'], axis=0)
+            sa_known = np.append(self.database['Sa_1'], self.database['Sa_2'], axis=0)
+            vs30 = np.append(self.database['soil_Vs30'], self.database['soil_Vs30'], axis=0)
+            magnitude = np.append(self.database['magnitude'], self.database['magnitude'], axis=0)
+            rjb = np.append(self.database['Rjb'], self.database['Rjb'], axis=0)
+            mechanism = np.append(self.database['mechanism'], self.database['mechanism'], axis=0)
+            filename1 = np.append(self.database['Filename_1'], self.database['Filename_2'], axis=0)
+            eq_id = np.append(self.database['EQID'], self.database['EQID'], axis=0)
 
             if self.database['Name'] == "NGA_W2":
-                NGA_num = np.append(self.database['NGA_num'], self.database['NGA_num'], axis=0)
+                nga_num = np.append(self.database['NGA_num'], self.database['NGA_num'], axis=0)
 
             elif self.database['Name'] == "ESM_2018":
                 station_code = np.append(self.database['station_code'], self.database['station_code'], axis=0)
 
-        elif self.selection == 2:
+        elif self.num_components == 2:
 
-            if self.Sa_def == 'GeoMean':
-                SaKnown = np.sqrt(self.database['Sa_1'] * self.database['Sa_2'])
-            elif self.Sa_def == 'SRSS':
-                SaKnown = np.sqrt(self.database['Sa_1'] ** 2 + self.database['Sa_2'] ** 2)
-            elif self.Sa_def == 'ArithmeticMean':
-                SaKnown = (self.database['Sa_1'] + self.database['Sa_2']) / 2
-            elif self.Sa_def == 'RotD50':  # SaKnown = Sa_RotD50.
-                SaKnown = self.database['Sa_RotD50']
-            elif self.Sa_def == 'RotD100':  # SaKnown = Sa_RotD100.
-                SaKnown = self.database['Sa_RotD100']
+            if self.spectrum_definition == 'GeoMean':
+                sa_known = np.sqrt(self.database['Sa_1'] * self.database['Sa_2'])
+            elif self.spectrum_definition == 'SRSS':
+                sa_known = np.sqrt(self.database['Sa_1'] ** 2 + self.database['Sa_2'] ** 2)
+            elif self.spectrum_definition == 'ArithmeticMean':
+                sa_known = (self.database['Sa_1'] + self.database['Sa_2']) / 2
+            elif self.spectrum_definition == 'RotD50':  # sa_known = Sa_RotD50.
+                sa_known = self.database['Sa_RotD50']
+            elif self.spectrum_definition == 'RotD100':  # sa_known = Sa_RotD100.
+                sa_known = self.database['Sa_RotD100']
             else:
                 raise ValueError('Unexpected Sa definition, exiting...')
 
-            soil_Vs30 = self.database['soil_Vs30']
-            Mw = self.database['magnitude']
-            Rjb = self.database['Rjb']
-            fault = self.database['mechanism']
-            Filename_1 = self.database['Filename_1']
-            Filename_2 = self.database['Filename_2']
-            eq_ID = self.database['EQID']
+            vs30 = self.database['soil_Vs30']
+            magnitude = self.database['magnitude']
+            rjb = self.database['Rjb']
+            mechanism = self.database['mechanism']
+            filename1 = self.database['Filename_1']
+            filename2 = self.database['Filename_2']
+            eq_id = self.database['EQID']
 
             if self.database['Name'] == "NGA_W2":
-                NGA_num = self.database['NGA_num']
+                nga_num = self.database['NGA_num']
 
             elif self.database['Name'] == "ESM_2018":
                 station_code = self.database['station_code']
 
         else:
             raise ValueError('Selection can only be performed for one or two components at the moment, exiting...')
 
-        # Limiting the records to be considered using the `notAllowed' variable
+        # Limiting the records to be considered using the `not_allowed' variable
         # Sa cannot be negative or zero, remove these.
-        notAllowed = np.unique(np.where(SaKnown <= 0)[0]).tolist()
+        not_allowed = np.unique(np.where(sa_known <= 0)[0]).tolist()
 
-        if self.Vs30_lim is not None:  # limiting values on soil exist
-            mask = (soil_Vs30 > min(self.Vs30_lim)) * (soil_Vs30 < max(self.Vs30_lim))
+        if self.vs30_limits is not None:  # limiting values on soil exist
+            mask = (vs30 > min(self.vs30_limits)) * (vs30 < max(self.vs30_limits))
             temp = [i for i, x in enumerate(mask) if not x]
-            notAllowed.extend(temp)
+            not_allowed.extend(temp)
 
-        if self.Mw_lim is not None:  # limiting values on magnitude exist
-            mask = (Mw > min(self.Mw_lim)) * (Mw < max(self.Mw_lim))
+        if self.mag_limits is not None:  # limiting values on magnitude exist
+            mask = (magnitude > min(self.mag_limits)) * (magnitude < max(self.mag_limits))
             temp = [i for i, x in enumerate(mask) if not x]
-            notAllowed.extend(temp)
+            not_allowed.extend(temp)
 
-        if self.Rjb_lim is not None:  # limiting values on Rjb exist
-            mask = (Rjb > min(self.Rjb_lim)) * (Rjb < max(self.Rjb_lim))
+        if self.rjb_limits is not None:  # limiting values on Rjb exist
+            mask = (rjb > min(self.rjb_limits)) * (rjb < max(self.rjb_limits))
             temp = [i for i, x in enumerate(mask) if not x]
-            notAllowed.extend(temp)
+            not_allowed.extend(temp)
 
-        if self.fault_lim is not None:  # limiting values on mechanism exist
-            for fault_i in range(len(self.fault_lim)):
-                if fault_i == 0:
-                    mask = fault == self.fault_lim[fault_i]
+        if self.mech_limits is not None:  # limiting values on mechanism exist
+            for mechanism_i in range(len(self.mech_limits)):
+                if mechanism_i == 0:
+                    mask = mechanism == self.mech_limits[mechanism_i]
                 else:
-                    mask = np.logical_or(mask, fault == self.fault_lim[fault_i])
+                    mask = np.logical_or(mask, mechanism == self.mech_limits[mechanism_i])
             temp = [i for i, x in enumerate(mask) if not x]
-            notAllowed.extend(temp)
+            not_allowed.extend(temp)
 
         # get the unique values
-        notAllowed = (list(set(notAllowed)))
-        Allowed = [i for i in range(SaKnown.shape[0])]
-        for i in notAllowed:
-            Allowed.remove(i)
+        not_allowed = (list(set(not_allowed)))
+        allowed = [i for i in range(sa_known.shape[0])]
+        for i in not_allowed:
+            allowed.remove(i)
 
         # Use only allowed records
-        SaKnown = SaKnown[Allowed, :]
-        soil_Vs30 = soil_Vs30[Allowed]
-        Mw = Mw[Allowed]
-        Rjb = Rjb[Allowed]
-        fault = fault[Allowed]
-        eq_ID = eq_ID[Allowed]
-        Filename_1 = Filename_1[Allowed]
+        sa_known = sa_known[allowed, :]
+        vs30 = vs30[allowed]
+        magnitude = magnitude[allowed]
+        rjb = rjb[allowed]
+        mechanism = mechanism[allowed]
+        eq_id = eq_id[allowed]
+        filename1 = filename1[allowed]
 
-        if self.selection == 1:
-            Filename_2 = None
+        if self.num_components == 1:
+            filename2 = None
         else:
-            Filename_2 = Filename_2[Allowed]
+            filename2 = filename2[allowed]
 
         if self.database['Name'] == "NGA_W2":
-            NGA_num = NGA_num[Allowed]
+            nga_num = nga_num[allowed]
             station_code = None
         elif self.database['Name'] == "ESM_2018":
-            NGA_num = None
-            station_code = station_code[Allowed]
+            nga_num = None
+            station_code = station_code[allowed]
 
         # Arrange the available spectra in a usable format and check for invalid input
         # Match periods (known periods and periods for error computations)
-        recPer = []
-        for i in range(len(self.T)):
-            recPer.append(np.where(self.database['Periods'] == self.T[i])[0][0])
+        record_periods = []
+        for i in range(len(self.periods)):
+            record_periods.append(np.where(self.database['Periods'] == self.periods[i])[0][0])
 
         # Check for invalid input
-        sampleBig = SaKnown[:, recPer]
-        if np.any(np.isnan(sampleBig)):
+        sample_big = sa_known[:, record_periods]
+        if np.any(np.isnan(sample_big)):
             raise ValueError('NaNs found in input response spectra')
 
-        if self.nGM > len(eq_ID):
+        if self.num_records > len(eq_id):
             raise ValueError('There are not enough records which satisfy',
                              'the given record selection criteria...',
                              'Please use broaden your selection criteria...')
 
-        return sampleBig, soil_Vs30, Mw, Rjb, fault, Filename_1, Filename_2, NGA_num, eq_ID, station_code
+        return sample_big, vs30, magnitude, rjb, mechanism, filename1, filename2, nga_num, eq_id, station_code
 
-    def write(self, obj=0, recs=1, rtype='acc', recs_f=''):
+    def write(self, object=0, records=1, record_type='acc', zip_parent_path=''):
         """
         Details
         -------
         Writes the object as pickle, selected and scaled records as .txt files.
 
         Parameters
         ----------
-        obj : int, optional
+        object : int, optional
             flag to write the object into the pickle file.
             The default is 0.
-        recs : int, optional
-            flag to write the selected and scaled time histories.
+        records : int, optional
+            flag to write the selected and scaled time histories
+            time-steps, filenames, scaling factors.
             The default is 1.
-        rtype : str, optional
+        record_type : str, optional
             option to choose the type of time history to be written.
             'acc' : for the acceleration series, units: g
             'vel' : for the velocity series, units: g * sec
             'disp': for the displacement series: units: g * sec2
-        recs_f : str, optional
+        zip_parent_path : str, optional
             This is option could be used if the user already has all the
             records in database. This is the folder path which contains
-            "database.zip" file. The records must be placed inside
-            recs_f/database.zip/database/
+            "database.zip" file (e.g., database could be NGA_W2 or ESM_2018). 
+            The records must be placed inside zip_parent_path/database.zip/database/
             The default is ''.
 
         Notes
         -----
         0: no, 1: yes
 
         Returns
         -------
         None.
         """
 
-        def save_signal(path, uns_acc, sf, dt):
+        def save_signal(path, unscaled_acc, sf, dt):
             """
             Details
             -------
             Saves the final signal to the specified path.
 
             Parameters
             ----------
             path : str
                 path of the file to save
-            uns_acc : numpy.ndarray
+            unscaled_acc : numpy.ndarray
                 unscaled acceleration series
             sf : float
                 scaling factor
             dt : float
                 time step 
 
             Returns
             -------
             None.
             """
 
-            if rtype == 'vel':  # integrate once if velocity
-                signal = integrate.cumtrapz(uns_acc * sf, dx=dt, initial=0)
+            if record_type == 'vel':  # integrate once if velocity
+                signal = integrate.cumtrapz(unscaled_acc * sf, dx=dt, initial=0)
 
-            elif rtype == 'disp':  # integrate twice if displacement
-                signal = integrate.cumtrapz(integrate.cumtrapz(uns_acc * sf, dx=dt, initial=0), dx=dt, initial=0)
+            elif record_type == 'disp':  # integrate twice if displacement
+                signal = integrate.cumtrapz(integrate.cumtrapz(unscaled_acc * sf, dx=dt, initial=0), dx=dt, initial=0)
 
             else:
-                signal = uns_acc * sf
+                signal = unscaled_acc * sf
 
             np.savetxt(path, signal, fmt='%1.5e')
 
-        if recs == 1:
+        if records == 1:
             # set the directories and file names
             try:  # this will work if records are downloaded
-                zipName = self.Unscaled_rec_file
+                zip_name = self.unscaled_rec_file
             except AttributeError:
-                zipName = os.path.join(recs_f, self.database['Name'] + '.zip')
-            n = len(self.rec_h1)
-            dts = np.zeros(n)
-            path_H1 = os.path.join(self.outdir, 'GMR_names.txt')
-            if self.selection == 2:
-                path_H1 = os.path.join(self.outdir, 'GMR_H1_names.txt')
-                path_H2 = os.path.join(self.outdir, 'GMR_H2_names.txt')
-                h2s = open(path_H2, 'w')
-            h1s = open(path_H1, 'w')
+                zip_name = os.path.join(zip_parent_path, self.database['Name'] + '.zip')
+            size = len(self.rec_file_h1)
+            dts = np.zeros(size)
+            path_h1 = os.path.join(self.output_directory_path, 'GMR_names.txt')
+            if self.num_components == 2:
+                path_h1 = os.path.join(self.output_directory_path, 'GMR_H1_names.txt')
+                path_h2 = os.path.join(self.output_directory_path, 'GMR_H2_names.txt')
+                h2s = open(path_h2, 'w')
+            h1s = open(path_h1, 'w')
 
             # Get record paths for # NGA_W2 or ESM_2018
-            if zipName != os.path.join(recs_f, self.database['Name'] + '.zip'):
-                rec_paths1 = self.rec_h1
-                if self.selection == 2:
-                    rec_paths2 = self.rec_h2
+            if zip_name != os.path.join(zip_parent_path, self.database['Name'] + '.zip'):
+                rec_paths1 = self.rec_file_h1
+                if self.num_components == 2:
+                    rec_paths2 = self.rec_file_h2
             else:
-                rec_paths1 = [self.database['Name'] + '/' + self.rec_h1[i] for i in range(n)]
-                if self.selection == 2:
-                    rec_paths2 = [self.database['Name'] + '/' + self.rec_h2[i] for i in range(n)]
+                rec_paths1 = [self.database['Name'] + '/' + self.rec_file_h1[i] for i in range(size)]
+                if self.num_components == 2:
+                    rec_paths2 = [self.database['Name'] + '/' + self.rec_file_h2[i] for i in range(size)]
 
             # Read contents from zipfile
-            contents1 = ContentFromZip(rec_paths1, zipName)  # H1 gm components
-            if self.selection == 2:
-                contents2 = ContentFromZip(rec_paths2, zipName)  # H2 gm components
+            contents1 = content_from_zip(rec_paths1, zip_name)  # H1 gm components
+            if self.num_components == 2:
+                contents2 = content_from_zip(rec_paths2, zip_name)  # H2 gm components
 
             # Start saving records
-            for i in range(n):
+            for i in range(size):
 
                 # Read the record files
                 if self.database['Name'].startswith('NGA'):  # NGA
-                    dts[i], npts1, _, _, inp_acc1 = ReadNGA(inFilename=self.rec_h1[i], content=contents1[i])
-                    gmr_file1 = self.rec_h1[i].replace('/', '_')[:-4] + '_' + rtype.upper() + '.txt'
+                    dts[i], npts1, _, _, inp_acc1 = read_nga(in_filename=self.rec_file_h1[i], content=contents1[i])
+                    gmr_file1 = self.rec_file_h1[i].replace('/', '_')[:-4] + '_' + record_type.upper() + '.txt'
 
-                    if self.selection == 2:  # H2 component
-                        _, npts2, _, _, inp_acc2 = ReadNGA(inFilename=self.rec_h2[i], content=contents2[i])
-                        gmr_file2 = self.rec_h2[i].replace('/', '_')[:-4] + '_' + rtype.upper() + '.txt'
+                    if self.num_components == 2:  # H2 component
+                        _, npts2, _, _, inp_acc2 = read_nga(in_filename=self.rec_file_h2[i], content=contents2[i])
+                        gmr_file2 = self.rec_file_h2[i].replace('/', '_')[:-4] + '_' + record_type.upper() + '.txt'
 
                 elif self.database['Name'].startswith('ESM'):  # ESM
-                    dts[i], npts1, _, _, inp_acc1 = ReadESM(inFilename=self.rec_h1[i], content=contents1[i])
-                    gmr_file1 = self.rec_h1[i].replace('/', '_')[:-11] + '_' + rtype.upper() + '.txt'
-                    if self.selection == 2:  # H2 component
-                        _, npts2, _, _, inp_acc2 = ReadESM(inFilename=self.rec_h2[i], content=contents2[i])
-                        gmr_file2 = self.rec_h2[i].replace('/', '_')[:-11] + '_' + rtype.upper() + '.txt'
+                    dts[i], npts1, _, _, inp_acc1 = read_esm(in_filename=self.rec_file_h1[i], content=contents1[i])
+                    gmr_file1 = self.rec_file_h1[i].replace('/', '_')[:-11] + '_' + record_type.upper() + '.txt'
+                    if self.num_components == 2:  # H2 component
+                        _, npts2, _, _, inp_acc2 = read_esm(in_filename=self.rec_file_h2[i], content=contents2[i])
+                        gmr_file2 = self.rec_file_h2[i].replace('/', '_')[:-11] + '_' + record_type.upper() + '.txt'
 
                 # Write the record files
-                if self.selection == 2:
+                if self.num_components == 2:
                     # ensure that two acceleration signals have the same length, if not add zeros.
                     npts = max(npts1, npts2)
                     temp1 = np.zeros(npts)
                     temp1[:npts1] = inp_acc1
                     inp_acc1 = temp1.copy()
                     temp2 = np.zeros(npts)
                     temp2[:npts2] = inp_acc2
                     inp_acc2 = temp2.copy()
 
                     # H2 component
-                    save_signal(os.path.join(self.outdir, gmr_file2), inp_acc2, self.rec_scale[i], dts[i])
+                    save_signal(os.path.join(self.output_directory_path, gmr_file2), inp_acc2, self.rec_scale_factors[i], dts[i])
                     h2s.write(gmr_file2 + '\n')
 
                 # H1 component
-                save_signal(os.path.join(self.outdir, gmr_file1), inp_acc1, self.rec_scale[i], dts[i])
+                save_signal(os.path.join(self.output_directory_path, gmr_file1), inp_acc1, self.rec_scale_factors[i], dts[i])
                 h1s.write(gmr_file1 + '\n')
 
             # Time steps
-            np.savetxt(os.path.join(self.outdir, 'GMR_dts.txt'), dts, fmt='%.5f')
+            np.savetxt(os.path.join(self.output_directory_path, 'GMR_dts.txt'), dts, fmt='%.5f')
             # Scale factors
-            np.savetxt(os.path.join(self.outdir, 'GMR_sf_used.txt'), np.array([self.rec_scale]).T, fmt='%1.5f')
+            np.savetxt(os.path.join(self.output_directory_path, 'GMR_sf_used.txt'), np.array([self.rec_scale_factors]).T, fmt='%1.5f')
             # Close the files
             h1s.close()
-            if self.selection == 2:
+            if self.num_components == 2:
                 h2s.close()
 
-        if obj == 1:
+        if object == 1:
             # save some info as pickle obj
-            obj = vars(copy.deepcopy(self))  # use copy.deepcopy to create independent obj
-            obj['database'] = self.database['Name']
-            del obj['outdir']
+            object = vars(copy.deepcopy(self))  # use copy.deepcopy to create independent obj
+            object['database'] = self.database['Name']
+            del object['output_directory_path']
 
-            if 'bgmpe' in obj:
-                del obj['bgmpe']
+            if 'bgmpe' in object:
+                del object['bgmpe']
 
-            with open(os.path.join(self.outdir, 'obj.pkl'), 'wb') as file:
-                pickle.dump(obj, file)
+            with open(os.path.join(self.output_directory_path, 'obj.pkl'), 'wb') as file:
+                pickle.dump(object, file)
 
-        print(f"Finished writing process, the files are located in\n{self.outdir}")
+        print(f"Finished writing process, the files are located in\n{self.output_directory_path}")
 
-    def plot(self, tgt=0, sim=0, rec=1, save=0, show=1):
+    def plot(self, target=0, simulations=0, records=1, save=0, show=1):
         """
         Details
         -------
         Plots the spectra of selected and simulated records,
         and/or target spectrum.
 
         Parameters
         ----------
-        tgt    : int, optional for conditional_spectrum
+        target : int, optional for ConditionalSpectrum
             Flag to plot target spectrum.
             The default is 1.
-        sim    : int, optional for conditional_spectrum
+        simulations : int, optional for ConditionalSpectrum
             Flag to plot simulated response spectra vs. target spectrum.
             The default is 0.
-        rec    : int, optional for conditional_spectrum
+        records : int, optional for ConditionalSpectrum
             Flag to plot Selected response spectra of selected records
             vs. target spectrum.
             The default is 1.
-        save   : int, optional for all selection options
+        save : int, optional for all selection options
             Flag to save plotted figures in pdf format.
             The default is 0.
-        show  : int, optional for all selection options
+        show : int, optional for all selection options
             Flag to show figures
             The default is 0.
 
         Notes
         -----
         0: no, 1: yes
 
         Returns
         -------
         None.
         """
 
-        SMALL_SIZE = 15
-        MEDIUM_SIZE = 16
-        BIG_SIZE = 18
-        BIGGER_SIZE = 20
-
-        plt.rc('font', size=SMALL_SIZE)  # controls default text sizes
-        plt.rc('axes', titlesize=SMALL_SIZE)  # fontsize of the axes title
-        plt.rc('axes', labelsize=BIG_SIZE)  # fontsize of the x and y labels
-        plt.rc('xtick', labelsize=SMALL_SIZE)  # fontsize of the tick labels
-        plt.rc('ytick', labelsize=SMALL_SIZE)  # fontsize of the tick labels
-        plt.rc('legend', fontsize=MEDIUM_SIZE)  # legend fontsize
-        plt.rc('figure', titlesize=BIGGER_SIZE)  # fontsize of the figure title
         plt.ioff()
 
-        if type(self).__name__ == 'conditional_spectrum':
+        if type(self).__name__ == 'ConditionalSpectrum':
 
             # xticks and yticks to use for plotting
-            xticks = [self.T[0]]
-            for x in [0.01, 0.1, 0.2, 0.5, 1, 2, 4, 7, 10]:
-                if self.T[0] < x < self.T[-1]:
+            xticks = [self.periods[0]]
+            for x in [0.01, 0.1, 0.2, 0.5, 1, 5, 10]:
+                if self.periods[0] < x < self.periods[-1]:
                     xticks.append(x)
-            xticks.append(self.T[-1])
+            xticks.append(self.periods[-1])
             yticks = [0.01, 0.1, 0.2, 0.5, 1, 2, 3, 5]
 
-            if self.cond == 1:
+            if self.is_conditioned == 1:
                 if len(self.Tstar) == 1:
                     hatch = [float(self.Tstar * 0.98), float(self.Tstar * 1.02)]
                 else:
                     hatch = [float(self.Tstar.min()), float(self.Tstar.max())]
 
-            if tgt == 1:
+            if target == 1:
                 # Plot Target spectrum vs. Simulated response spectra
                 fig, ax = plt.subplots(1, 2, figsize=(16, 8))
                 plt.suptitle('Target Spectrum', y=0.95)
-                ax[0].loglog(self.T, np.exp(self.mu_ln), color='red', lw=2, label='Target - $e^{\mu_{ln}}$')
-                if self.useVar == 1:
-                    ax[0].loglog(self.T, np.exp(self.mu_ln + 2 * self.sigma_ln), color='red', linestyle='--', lw=2,
+                ax[0].loglog(self.periods, np.exp(self.mu_ln), color='red', lw=2, label='Target - $e^{\mu_{ln}}$')
+                if self.use_variance == 1:
+                    ax[0].loglog(self.periods, np.exp(self.mu_ln + 2 * self.sigma_ln), color='red', linestyle='--', lw=2,
                                  label='Target - $e^{\mu_{ln}\mp 2\sigma_{ln}}$')
-                    ax[0].loglog(self.T, np.exp(self.mu_ln - 2 * self.sigma_ln), color='red', linestyle='--', lw=2,
+                    ax[0].loglog(self.periods, np.exp(self.mu_ln - 2 * self.sigma_ln), color='red', linestyle='--', lw=2,
                                  label='Target - $e^{\mu_{ln}\mp 2\sigma_{ln}}$')
 
-                ax[0].set_xlim([self.T[0], self.T[-1]])
+                ax[0].set_xlim([self.periods[0], self.periods[-1]])
                 ax[0].set_xticks(xticks)
                 ax[0].get_xaxis().set_major_formatter(ScalarFormatter())
                 ax[0].get_xaxis().set_minor_formatter(NullFormatter())
                 ax[0].set_yticks(yticks)
                 ax[0].get_yaxis().set_major_formatter(ScalarFormatter())
                 ax[0].get_yaxis().set_minor_formatter(NullFormatter())
                 ax[0].set_xlabel('Period [sec]')
                 ax[0].set_ylabel('Spectral Acceleration [g]')
                 ax[0].grid(True)
 
                 handles, labels = ax[0].get_legend_handles_labels()
                 by_label = dict(zip(labels, handles))
                 ax[0].legend(by_label.values(), by_label.keys(), frameon=False)
-                if self.cond == 1:
+                if self.is_conditioned == 1:
                     ax[0].axvspan(hatch[0], hatch[1], facecolor='red', alpha=0.3)
 
                 # Sample and target standard deviations
-                if self.useVar == 1:
-                    ax[1].semilogx(self.T, self.sigma_ln, color='red', linestyle='--', lw=2,
+                if self.use_variance == 1:
+                    ax[1].semilogx(self.periods, self.sigma_ln, color='red', linestyle='--', lw=2,
                                    label='Target - $\sigma_{ln}$')
                     ax[1].set_xlabel('Period [sec]')
                     ax[1].set_ylabel('Dispersion')
                     ax[1].grid(True)
                     ax[1].legend(frameon=False)
-                    ax[1].set_xlim([self.T[0], self.T[-1]])
+                    ax[1].set_xlim([self.periods[0], self.periods[-1]])
                     ax[1].set_xticks(xticks)
                     ax[1].get_xaxis().set_major_formatter(ScalarFormatter())
                     ax[1].get_xaxis().set_minor_formatter(NullFormatter())
                     ax[1].set_ylim(bottom=0)
                     ax[1].get_yaxis().set_major_formatter(ScalarFormatter())
                     ax[1].get_yaxis().set_minor_formatter(NullFormatter())
-                    if self.cond == 1:
+                    if self.is_conditioned == 1:
                         ax[1].axvspan(hatch[0], hatch[1], facecolor='red', alpha=0.3)
 
                 if save == 1:
-                    plt.savefig(os.path.join(self.outdir, 'Targeted.pdf'))
+                    plt.savefig(os.path.join(self.output_directory_path, 'Targeted.pdf'))
 
-            if sim == 1:
+            if simulations == 1:
                 # Plot Target spectrum vs. Simulated response spectra
                 fig, ax = plt.subplots(1, 2, figsize=(16, 8))
                 plt.suptitle('Target Spectrum vs. Simulated Spectra', y=0.95)
 
-                for i in range(self.nGM):
-                    ax[0].loglog(self.T, np.exp(self.sim_spec[i, :]), color='gray', lw=1, label='Selected')
+                for i in range(self.num_records):
+                    ax[0].loglog(self.periods, np.exp(self.sim_spec[i, :]), color='gray', lw=1, label='Selected')
 
-                ax[0].loglog(self.T, np.exp(self.mu_ln), color='red', lw=2, label='Target - $e^{\mu_{ln}}$')
-                if self.useVar == 1:
-                    ax[0].loglog(self.T, np.exp(self.mu_ln + 2 * self.sigma_ln), color='red', linestyle='--', lw=2,
+                ax[0].loglog(self.periods, np.exp(self.mu_ln), color='red', lw=2, label='Target - $e^{\mu_{ln}}$')
+                if self.use_variance == 1:
+                    ax[0].loglog(self.periods, np.exp(self.mu_ln + 2 * self.sigma_ln), color='red', linestyle='--', lw=2,
                                  label='Target - $e^{\mu_{ln}\mp 2\sigma_{ln}}$')
-                    ax[0].loglog(self.T, np.exp(self.mu_ln - 2 * self.sigma_ln), color='red', linestyle='--', lw=2,
+                    ax[0].loglog(self.periods, np.exp(self.mu_ln - 2 * self.sigma_ln), color='red', linestyle='--', lw=2,
                                  label='Target - $e^{\mu_{ln}\mp 2\sigma_{ln}}$')
 
-                ax[0].loglog(self.T, np.exp(np.mean(self.sim_spec, axis=0)), color='blue', lw=2,
+                ax[0].loglog(self.periods, np.exp(np.mean(self.sim_spec, axis=0)), color='blue', lw=2,
                              label='Selected - $e^{\mu_{ln}}$')
-                if self.useVar == 1:
-                    ax[0].loglog(self.T, np.exp(np.mean(self.sim_spec, axis=0) + 2 * np.std(self.sim_spec, axis=0)),
+                if self.use_variance == 1:
+                    ax[0].loglog(self.periods, np.exp(np.mean(self.sim_spec, axis=0) + 2 * np.std(self.sim_spec, axis=0)),
                                  color='blue', linestyle='--', lw=2, label='Selected - $e^{\mu_{ln}\mp 2\sigma_{ln}}$')
-                    ax[0].loglog(self.T, np.exp(np.mean(self.sim_spec, axis=0) - 2 * np.std(self.sim_spec, axis=0)),
+                    ax[0].loglog(self.periods, np.exp(np.mean(self.sim_spec, axis=0) - 2 * np.std(self.sim_spec, axis=0)),
                                  color='blue', linestyle='--', lw=2, label='Selected - $e^{\mu_{ln}\mp 2\sigma_{ln}}$')
 
-                ax[0].set_xlim([self.T[0], self.T[-1]])
+                ax[0].set_xlim([self.periods[0], self.periods[-1]])
                 ax[0].set_xticks(xticks)
                 ax[0].get_xaxis().set_major_formatter(ScalarFormatter())
                 ax[0].get_xaxis().set_minor_formatter(NullFormatter())
                 ax[0].set_yticks(yticks)
                 ax[0].get_yaxis().set_major_formatter(ScalarFormatter())
                 ax[0].get_yaxis().set_minor_formatter(NullFormatter())
                 ax[0].set_xlabel('Period [sec]')
                 ax[0].set_ylabel('Spectral Acceleration [g]')
                 ax[0].grid(True)
                 handles, labels = ax[0].get_legend_handles_labels()
                 by_label = dict(zip(labels, handles))
                 ax[0].legend(by_label.values(), by_label.keys(), frameon=False)
-                if self.cond == 1:
+                if self.is_conditioned == 1:
                     ax[0].axvspan(hatch[0], hatch[1], facecolor='red', alpha=0.3)
 
-                if self.useVar == 1:
+                if self.use_variance == 1:
                     # Sample and target standard deviations
-                    ax[1].semilogx(self.T, self.sigma_ln, color='red', linestyle='--', lw=2,
+                    ax[1].semilogx(self.periods, self.sigma_ln, color='red', linestyle='--', lw=2,
                                    label='Target - $\sigma_{ln}$')
-                    ax[1].semilogx(self.T, np.std(self.sim_spec, axis=0), color='black', linestyle='--', lw=2,
+                    ax[1].semilogx(self.periods, np.std(self.sim_spec, axis=0), color='black', linestyle='--', lw=2,
                                    label='Selected - $\sigma_{ln}$')
                     ax[1].set_xlabel('Period [sec]')
                     ax[1].set_ylabel('Dispersion')
                     ax[1].grid(True)
                     ax[1].legend(frameon=False)
-                    ax[1].set_xlim([self.T[0], self.T[-1]])
+                    ax[1].set_xlim([self.periods[0], self.periods[-1]])
                     ax[1].set_xticks(xticks)
                     ax[1].get_xaxis().set_major_formatter(ScalarFormatter())
                     ax[1].get_xaxis().set_minor_formatter(NullFormatter())
                     ax[1].set_ylim(bottom=0)
                     ax[1].get_yaxis().set_major_formatter(ScalarFormatter())
                     ax[1].get_yaxis().set_minor_formatter(NullFormatter())
-                    if self.cond == 1:
+                    if self.is_conditioned == 1:
                         ax[1].axvspan(hatch[0], hatch[1], facecolor='red', alpha=0.3)
 
                 if save == 1:
-                    plt.savefig(os.path.join(self.outdir, 'Simulated.pdf'))
+                    plt.savefig(os.path.join(self.output_directory_path, 'Simulated.pdf'))
 
-            if rec == 1:
+            if records == 1:
                 # Plot Target spectrum vs. Selected response spectra
                 fig, ax = plt.subplots(1, 2, figsize=(16, 8))
                 plt.suptitle('Target Spectrum vs. Spectra of Selected Records', y=0.95)
 
-                for i in range(self.nGM):
-                    ax[0].loglog(self.T, np.exp(self.rec_spec[i, :]), color='gray', lw=1, label='Selected')
+                for i in range(self.num_records):
+                    ax[0].loglog(self.periods, np.exp(self.rec_sa_ln[i, :]), color='gray', lw=1, label='Selected')
 
-                ax[0].loglog(self.T, np.exp(self.mu_ln), color='red', lw=2, label='Target - $e^{\mu_{ln}}$')
-                if self.useVar == 1:
-                    ax[0].loglog(self.T, np.exp(self.mu_ln + 2 * self.sigma_ln), color='red', linestyle='--', lw=2,
+                ax[0].loglog(self.periods, np.exp(self.mu_ln), color='red', lw=2, label='Target - $e^{\mu_{ln}}$')
+                if self.use_variance == 1:
+                    ax[0].loglog(self.periods, np.exp(self.mu_ln + 2 * self.sigma_ln), color='red', linestyle='--', lw=2,
                                  label='Target - $e^{\mu_{ln}\mp 2\sigma_{ln}}$')
-                    ax[0].loglog(self.T, np.exp(self.mu_ln - 2 * self.sigma_ln), color='red', linestyle='--', lw=2,
+                    ax[0].loglog(self.periods, np.exp(self.mu_ln - 2 * self.sigma_ln), color='red', linestyle='--', lw=2,
                                  label='Target - $e^{\mu_{ln}\mp 2\sigma_{ln}}$')
 
-                ax[0].loglog(self.T, np.exp(np.mean(self.rec_spec, axis=0)), color='blue', lw=2,
+                ax[0].loglog(self.periods, np.exp(np.mean(self.rec_sa_ln, axis=0)), color='blue', lw=2,
                              label='Selected - $e^{\mu_{ln}}$')
-                ax[0].loglog(self.T, np.exp(np.mean(self.rec_spec, axis=0) + 2 * np.std(self.rec_spec, axis=0)),
+                ax[0].loglog(self.periods, np.exp(np.mean(self.rec_sa_ln, axis=0) + 2 * np.std(self.rec_sa_ln, axis=0)),
                              color='blue', linestyle='--', lw=2, label='Selected - $e^{\mu_{ln}\mp 2\sigma_{ln}}$')
-                ax[0].loglog(self.T, np.exp(np.mean(self.rec_spec, axis=0) - 2 * np.std(self.rec_spec, axis=0)),
+                ax[0].loglog(self.periods, np.exp(np.mean(self.rec_sa_ln, axis=0) - 2 * np.std(self.rec_sa_ln, axis=0)),
                              color='blue', linestyle='--', lw=2, label='Selected - $e^{\mu_{ln}\mp 2\sigma_{ln}}$')
 
-                ax[0].set_xlim([self.T[0], self.T[-1]])
+                ax[0].set_xlim([self.periods[0], self.periods[-1]])
                 ax[0].set_xticks(xticks)
                 ax[0].get_xaxis().set_major_formatter(ScalarFormatter())
                 ax[0].get_xaxis().set_minor_formatter(NullFormatter())
                 ax[0].set_yticks(yticks)
                 ax[0].get_yaxis().set_major_formatter(ScalarFormatter())
                 ax[0].get_yaxis().set_minor_formatter(NullFormatter())
                 ax[0].set_xlabel('Period [sec]')
                 ax[0].set_ylabel('Spectral Acceleration [g]')
                 ax[0].grid(True)
                 handles, labels = ax[0].get_legend_handles_labels()
                 by_label = dict(zip(labels, handles))
                 ax[0].legend(by_label.values(), by_label.keys(), frameon=False)
-                if self.cond == 1:
+                if self.is_conditioned == 1:
                     ax[0].axvspan(hatch[0], hatch[1], facecolor='red', alpha=0.3)
 
                 # Sample and target standard deviations
-                ax[1].semilogx(self.T, self.sigma_ln, color='red', linestyle='--', lw=2, label='Target - $\sigma_{ln}$')
-                ax[1].semilogx(self.T, np.std(self.rec_spec, axis=0), color='black', linestyle='--', lw=2,
+                ax[1].semilogx(self.periods, self.sigma_ln, color='red', linestyle='--', lw=2, label='Target - $\sigma_{ln}$')
+                ax[1].semilogx(self.periods, np.std(self.rec_sa_ln, axis=0), color='black', linestyle='--', lw=2,
                                label='Selected - $\sigma_{ln}$')
                 ax[1].set_xlabel('Period [sec]')
                 ax[1].set_ylabel('Dispersion')
                 ax[1].grid(True)
                 ax[1].legend(frameon=False)
-                ax[1].set_xlim([self.T[0], self.T[-1]])
+                ax[1].set_xlim([self.periods[0], self.periods[-1]])
                 ax[1].set_xticks(xticks)
                 ax[1].get_xaxis().set_major_formatter(ScalarFormatter())
                 ax[1].get_xaxis().set_minor_formatter(NullFormatter())
                 ax[1].set_ylim(bottom=0)
                 ax[1].get_yaxis().set_major_formatter(ScalarFormatter())
                 ax[1].get_yaxis().set_minor_formatter(NullFormatter())
-                if self.cond == 1:
+                if self.is_conditioned == 1:
                     ax[1].axvspan(hatch[0], hatch[1], facecolor='red', alpha=0.3)
 
                 if save == 1:
-                    plt.savefig(os.path.join(self.outdir, 'Selected.pdf'))
+                    plt.savefig(os.path.join(self.output_directory_path, 'Selected.pdf'))
 
-        if type(self).__name__ == 'code_spectrum':
+        if type(self).__name__ == 'CodeSpectrum':
 
-            hatch = [self.Tlower, self.Tupper]
+            hatch = [self.lower_bound_period, self.upper_bound_period]
             # Plot Target spectrum vs. Selected response spectra
             fig, ax = plt.subplots(1, 1, figsize=(8, 8))
-            for i in range(self.rec_spec.shape[0]):
-                ax.plot(self.T, self.rec_spec[i, :] * self.rec_scale[i], color='gray', lw=1, label='Selected')
-            ax.plot(self.T, np.mean(self.rec_spec * self.rec_scale.reshape(-1, 1), axis=0), color='black', lw=2,
+            for i in range(self.rec_sa_ln.shape[0]):
+                ax.plot(self.periods, self.rec_sa_ln[i, :] * self.rec_scale_factors[i], color='gray', lw=1, label='Selected')
+            ax.plot(self.periods, np.mean(self.rec_sa_ln * self.rec_scale_factors.reshape(-1, 1), axis=0), color='black', lw=2,
                     label='Selected Mean')
 
             if self.code == 'TBEC 2018':
-                ax.plot(self.T, self.target, color='red', lw=2, label='Design Response Spectrum')
-                if self.selection == 2:
-                    ax.plot(self.T, 1.3 * self.target, color='red', ls='--', lw=2,
+                ax.plot(self.periods, self.target, color='red', lw=2, label='Design Response Spectrum')
+                if self.num_components == 2:
+                    ax.plot(self.periods, 1.3 * self.target, color='red', ls='--', lw=2,
                             label='1.3 x Design Response Spectrum')
 
             if self.code == 'ASCE 7-16':
-                ax.plot(self.T, self.target, color='red', lw=2, label='$MCE_{R}$ Response Spectrum')
-                ax.plot(self.T, 0.9 * self.target, color='red', ls='--', lw=2,
+                ax.plot(self.periods, self.target, color='red', lw=2, label='$MCE_{R}$ Response Spectrum')
+                ax.plot(self.periods, 0.9 * self.target, color='red', ls='--', lw=2,
                         label='0.9 x $MCE_{R}$ Response Spectrum')
 
             if self.code == 'EC8-Part1':
-                ax.plot(self.T, self.target, color='red', lw=2, label='Design Response Spectrum')
-                ax.plot(self.T, 0.9 * self.target, color='red', lw=2, ls='--', label='0.9 x Design Response Spectrum')
+                ax.plot(self.periods, self.target, color='red', lw=2, label='Design Response Spectrum')
+                ax.plot(self.periods, 0.9 * self.target, color='red', lw=2, ls='--', label='0.9 x Design Response Spectrum')
 
             ax.axvspan(hatch[0], hatch[1], facecolor='red', alpha=0.3)
             ax.set_xlabel('Period [sec]')
             ax.set_ylabel('Spectral Acceleration [g]')
             ax.grid(True)
             handles, labels = ax.get_legend_handles_labels()
             by_label = dict(zip(labels, handles))
             ax.legend(by_label.values(), by_label.keys(), frameon=False)
-            ax.set_xlim([self.T[0], self.Tupper * 2])
+            ax.set_xlim([self.periods[0], self.upper_bound_period * 2])
             plt.suptitle(f'Spectra of Selected Records ({self.code})', y=0.95)
 
             if save == 1:
-                plt.savefig(os.path.join(self.outdir, 'Selected.pdf'))
+                plt.savefig(os.path.join(self.output_directory_path, 'Selected.pdf'))
 
         # Show the figure
         if show == 1:
             plt.show()
 
         plt.close('all')
 
-    def esm2018_download(self):
+    def download(self, username=None, password=None, token_path=None, sleeptime=2, browser='chrome'):
+        """
+        Details
+        -------
+        This function has been created as a web automation tool in order to
+        download unscaled record time histories from either
+        NGA-West2 (https://ngawest2.berkeley.edu/) or ESM databases (https://esm-db.eu/).
+
+        Notes
+        -----
+        Either of google-chrome or mozilla-firefox should have been installed priorly to download from NGA-West2.
+
+        Parameters
+        ----------
+        username : str
+            Account username (e-mail),  e.g. 'example_username@email.com'.
+        password : str
+            Account password, e.g. 'example_password123456'.
+        sleeptime : int, optional
+            Time (sec) spent between each browser operation. This can be increased or decreased depending on the internet speed.
+            Used in the case of database='NGA_W2'
+            The default is 2
+        browser : str, optional
+            The browser to use for download purposes. Valid entries are: 'chrome' or 'firefox'. 
+            Used in the case of database='NGA_W2'
+            The default is 'chrome'.
+
+        Returns
+        -------
+        None
+        """
+        
+        if self.database['Name'] == 'ESM_2018':
+
+            if token_path is None:
+                # In order to access token file must be retrieved initially.
+                # copy paste the readily available token.txt into EzGM or generate new one using get_esm_token method.
+                if username is None or password is None:
+                    raise ValueError('You have to enter either credentials or path to the token to download records from ESM database')
+                else:
+                    get_esm_token(username, password)
+                    token_path = 'token.txt'
+
+            self._esm2018_download(token_path)
+
+        elif self.database['Name'] == 'NGA_W2':
+
+            if username is None or password is None:
+                raise ValueError('You have to enter either credentials  to download records from NGA-West2 database')
+
+            self._ngaw2_download(username, password, sleeptime, browser)
+
+        else:
+            raise NotImplementedError('You have to use either of ESM_2018 or NGA_W2 databases to use download method.')
+
+    def _esm2018_download(self, token_path=None):
         """
 
         Details
         -------
         This function has been created as a web automation tool in order to
         download unscaled record time histories from ESM database
         (https://esm-db.eu/) based on their event ID and station_codes.
 
         Parameters
         ----------
-        None.
+        username : str
+            Account username (e-mail),  e.g. 'example_username@email.com'.
+        password : str
+            Account password, e.g. 'example_password123456'.
+        
 
         Returns
         -------
         None.
 
         """
 
-        if self.database['Name'] == 'ESM_2018':
-            print('\nStarted executing esm2018_download method...')
+        print('\nStarted executing download method to retrieve selected records from https://esm-db.eu')
 
-            # temporary zipfile name
-            zip_temp = os.path.join(self.outdir, 'output_temp.zip')
-            # temporary folder to extract files
-            folder_temp = os.path.join(self.outdir, 'output_temp')
-
-            for i in range(self.nGM):
-                print('Downloading %d/%d...' % (i + 1, self.nGM))
-                event = self.rec_eqID[i]
-                station = self.rec_station_code[i]
-                params = (
-                    ('eventid', event),
-                    ('data-type', 'ACC'),
-                    ('station', station),
-                    ('format', 'ascii'),
-                )
-                files = {
-                    'message': ('path/to/token.txt', open('token.txt', 'rb')),
-                }
-
-                url = 'https://esm-db.eu/esmws/eventdata/1/query'
-
-                req = requests.post(url=url, params=params, files=files)
-
-                if req.status_code == 200:
-                    with open(zip_temp, "wb") as zf:
-                        zf.write(req.content)
-
-                    with zipfile.ZipFile(zip_temp, 'r') as zipObj:
-                        zipObj.extractall(folder_temp)
-                    os.remove(zip_temp)
+        # temporary zipfile name
+        zip_temp = os.path.join(self.output_directory_path, 'output_temp.zip')
+        # temporary folder to extract files
+        folder_temp = os.path.join(self.output_directory_path, 'output_temp')
+
+        for i in range(self.num_records):
+            print('Downloading %d/%d...' % (i + 1, self.num_records))
+            event = self.rec_eq_id[i]
+            station = self.rec_station_code[i]
+            params = (
+                ('eventid', event),
+                ('data-type', 'ACC'),
+                ('station', station),
+                ('format', 'ascii'),
+            )
+            files = {
+                'message': ('path/to/token.txt', open(token_path, 'rb')),
+            }
+
+            url = 'https://esm-db.eu/esmws/eventdata/1/query'
+
+            req = requests.post(url=url, params=params, files=files)
+
+            if req.status_code == 200:
+                with open(zip_temp, "wb") as zf:
+                    zf.write(req.content)
+
+                with zipfile.ZipFile(zip_temp, 'r') as zipObj:
+                    zipObj.extractall(folder_temp)
+                os.remove(zip_temp)
 
+            else:
+                if req.status_code == 403:
+                    sys.exit('Problem with ESM download. Maybe the token is no longer valid')
                 else:
-                    if req.status_code == 403:
-                        sys.exit('Problem with ESM download. Maybe the token is no longer valid')
-                    else:
-                        sys.exit('Problem with ESM download. Status code: ' + str(req.status_code))
+                    sys.exit('Problem with ESM download. Status code: ' + str(req.status_code))
 
-            # create the output zipfile for all downloaded records
-            time_tag = gmtime()
-            time_tag_str = f'{time_tag[0]}'
-            for i in range(1, len(time_tag)):
-                time_tag_str += f'_{time_tag[i]}'
-            file_name = os.path.join(self.outdir, f'unscaled_records_{time_tag_str}.zip')
-            with zipfile.ZipFile(file_name, 'w', zipfile.ZIP_DEFLATED) as zipObj:
-                len_dir_path = len(folder_temp)
-                for root, _, files in os.walk(folder_temp):
-                    for file in files:
-                        file_path = os.path.join(root, file)
-                        zipObj.write(file_path, file_path[len_dir_path:])
-
-            shutil.rmtree(folder_temp)
-            self.Unscaled_rec_file = file_name
-            print(f'Downloaded files are located in\n{self.Unscaled_rec_file}')
+        # create the output zipfile for all downloaded records
+        time_tag = gmtime()
+        time_tag_str = f'{time_tag[0]}'
+        for i in range(1, len(time_tag)):
+            time_tag_str += f'_{time_tag[i]}'
+        file_name = os.path.join(self.output_directory_path, f'unscaled_records_{time_tag_str}.zip')
+        with zipfile.ZipFile(file_name, 'w', zipfile.ZIP_DEFLATED) as zipObj:
+            len_dir_path = len(folder_temp)
+            for root, _, files in os.walk(folder_temp):
+                for file in files:
+                    file_path = os.path.join(root, file)
+                    zipObj.write(file_path, file_path[len_dir_path:])
+
+        shutil.rmtree(folder_temp)
+        self.unscaled_rec_file = file_name
+        print(f'Downloaded files are located in\n{self.unscaled_rec_file}')
 
-        else:
-            raise ValueError('You have to use ESM_2018 database to use esm2018_download method.')
-
-    def ngaw2_download(self, username, pwd, sleeptime=2, browser='chrome'):
+    def _ngaw2_download(self, username, password, sleeptime, browser):
         """
         Details
         -------
         This function has been created as a web automation tool in order to
         download unscaled record time histories from NGA-West2 Database
         (https://ngawest2.berkeley.edu/) by Record Sequence Numbers (RSNs).
 
         Notes
         -----
         Either of google-chrome or mozilla-firefox should have been installed priorly.
 
         Parameters
         ----------
-        username     : str
-            Account username (e-mail),  e.g. 'username@mail.com'.
-        pwd          : str
-            Account password, e.g. 'password!12345'.
-        sleeptime    : int, default is 3
+        username : str
+            Account username (e-mail),  e.g. 'example_username@email.com'.
+        password : str
+            Account password, e.g. 'example_password123456'.
+        sleeptime : int, default is 3
             Time (sec) spent between each browser operation. This can be increased or decreased depending on the internet speed.
-        browser       : str, default is 'chrome'
+        browser : str, default is 'chrome'
             The browser to use for download purposes. Valid entries are: 'chrome' or 'firefox'.
 
         Returns
         -------
         None
         """
 
@@ -802,20 +860,20 @@
             """
             Details
             -------
             Measures download directory size
 
             Parameters
             ----------
-            download_dir     : str
+            download_dir : str
                 Directory for the output time histories to be downloaded
 
             Returns
             -------
-            total_size      : float
+            total_size : float
                 Measured size of the download directory
 
             """
 
             total_size = 0
             for path, dirs, files in os.walk(download_dir):
                 for f in files:
@@ -827,15 +885,15 @@
             """
             Details
             -------
             Waits for download to finish, and an additional amount of time based on the predefined sleeptime variable.
 
             Parameters
             ----------
-            download_dir     : str
+            download_dir : str
                 Directory for the output time histories to be downloaded.
 
             Returns
             -------
             None
             """
             delta_size = 100
@@ -855,22 +913,22 @@
             """
             Details
             -------
             This function starts the webdriver in headless mode.
 
             Parameters
             ----------
-            download_dir     : str
+            download_dir : str
                 Directory for the output time histories to be downloaded.
-            browser       : str, default is 'chrome'
+            browser : str, default is 'chrome'
                 The browser to use for download purposes. Valid entries are: 'chrome' or 'firefox'
 
             Returns
             -------
-            driver      : selenium webdriver object
+            driver : selenium webdriver object
                 Driver object used to download NGA_W2 records.
             """
 
             print('Getting the webdriver to use...')
 
             # Check if ipython is installed
             try:
@@ -905,59 +963,59 @@
                     options.set_preference('browser.helperApps.neverAsk.saveToDisk', 'application/zip')
                     driver = webdriver.Firefox(executable_path=driver_path[1], options=options)
 
                 # Running on personal computer (PC) using chrome
                 elif browser == 'chrome':
                     gdd = ChromeDriverDownloader()
                     driver_path = gdd.download_and_install(version = 'compatible')
-                    ChromeOptions = webdriver.ChromeOptions()
+                    options = webdriver.ChromeOptions()
                     prefs = {"download.default_directory": download_dir}
-                    ChromeOptions.add_experimental_option("prefs", prefs)
-                    ChromeOptions.headless = True
-                    driver = webdriver.Chrome(executable_path=driver_path[1], options=ChromeOptions)
+                    options.add_experimental_option("prefs", prefs)
+                    options.headless = True
+                    driver = webdriver.Chrome(executable_path=driver_path[1], options=options)
 
                 print('Webdriver is obtained successfully.')
 
                 return driver
 
             except RuntimeError:
                 print('Failed to get webdriver.')
                 raise
 
-        def sign_in(driver, USERNAME, PASSWORD):
+        def sign_in(driver, username, password):
             """
 
             Details
             -------
             This function signs in to 'https://ngawest2.berkeley.edu/' with
             given account credentials.
 
             Parameters
             ----------
-            driver     : selenium webdriver object
+            driver : selenium webdriver object
                 Driver object used to download NGA_W2 records.
-            USERNAME   : str
+            username : str
                 Account username (e-mail), e.g.: 'username@mail.com'.
-            PASSWORD   : str
+            password : str
                 Account password, e.g.: 'password!12345'.
 
             Returns
             -------
-            driver      : selenium webdriver object
+            driver : selenium webdriver object
                 Driver object used to download NGA_W2 records.
 
             """
             # TODO: For Selenium >= 4.3.0
             #  Deprecated find_element_by_* and find_elements_by_* are now removed (#10712)
             #  https://stackoverflow.com/questions/72773206/selenium-python-attributeerror-webdriver-object-has-no-attribute-find-el
             #  Modify the ngaw2_download method to use greater versions of Selenium than 4.2.0
             print("Signing in with credentials...")
             driver.get('https://ngawest2.berkeley.edu/users/sign_in')
-            driver.find_element_by_id('user_email').send_keys(USERNAME)
-            driver.find_element_by_id('user_password').send_keys(PASSWORD)
+            driver.find_element_by_id('user_email').send_keys(username)
+            driver.find_element_by_id('user_password').send_keys(password)
             driver.find_element_by_id('user_submit').click()
 
             try:
                 alert = driver.find_element_by_css_selector('p.alert')
                 warn = alert.text
             except BaseException as e:
                 warn = None
@@ -967,57 +1025,57 @@
                 driver.quit()
                 raise Warning('Invalid email or password.')
             else:
                 print('Signed in successfully.')
 
             return driver
 
-        def download(RSNs, download_dir, driver):
+        def download(rsn, download_dir, driver):
             """
 
             Details
             -------
-            This function dowloads the timehistories which have been indicated with their RSNs
+            This function dowloads the timehistories which have been indicated with their record sequence numbers (rsn)
             from 'https://ngawest2.berkeley.edu/'.
 
             Parameters
             ----------
-            RSNs     : str
+            rsn : str
                 A string variable contains RSNs to be downloaded which uses ',' as delimiter
                 between RNSs, e.g.: '1,5,91,35,468'.
-            download_dir     : str
+            download_dir : str
                 Directory for the output time histories to be downloaded.
-            driver     : selenium webdriver object
+            driver : class object, (selenium webdriver)
                 Driver object used to download NGA_W2 records.
 
             Returns
             -------
             None
 
             """
             print("Listing the Records...")
             driver.get('https://ngawest2.berkeley.edu/spectras/new?sourceDb_flag=1')
             sleep(sleeptime)
             driver.find_element_by_xpath("//button[@type='button']").submit()
             sleep(sleeptime)
-            driver.find_element_by_id('search_search_nga_number').send_keys(RSNs)
+            driver.find_element_by_id('search_search_nga_number').send_keys(rsn)
             sleep(sleeptime)
             driver.find_element_by_xpath(
                 "//button[@type='button' and @onclick='uncheck_plot_selected();reset_selectedResult();OnSubmit();']").submit()
             sleep(1.5 * sleeptime)
             try:
                 note = driver.find_element_by_id('notice').text
                 print(note)
             except BaseException as e:
                 note = 'NO'
                 error = e
 
             if 'NO' in note:
                 driver.set_window_size(800, 800)
-                driver.save_screenshot(os.path.join(self.outdir, 'download_error.png'))
+                driver.save_screenshot(os.path.join(self.output_directory_path, 'download_error.png'))
                 driver.quit()
                 raise Warning("Could not be able to download records!"
                               "Either they no longer exist in database"
                               "or you have exceeded the download limit")
             else:
                 driver.execute_script("window.scrollTo(0, document.body.scrollHeight)")
                 sleep(sleeptime)
@@ -1033,45 +1091,42 @@
                 print(msg)
                 sleep(sleeptime)
                 obj.accept()
                 sleep(sleeptime)
                 download_wait(download_dir)
                 driver.quit()
 
-        if self.database['Name'] == 'NGA_W2':
-            print('\nStarted executing ngaw2_download method...')
+        print('\nStarted executing download method to retrieve selected records from https://ngawest2.berkeley.edu')
 
-            self.username = username
-            self.pwd = pwd
-            driver = set_driver(self.outdir, browser)
-            driver = sign_in(driver, self.username, self.pwd)
-            RSNs = ''
-            for i in self.rec_rsn:
-                RSNs += str(int(i)) + ','
-            RSNs = RSNs[:-1:]
-            files_before_download = set(os.listdir(self.outdir))
-            download(RSNs, self.outdir, driver)
-            files_after_download = set(os.listdir(self.outdir))
-            Downloaded_File = str(list(files_after_download.difference(files_before_download))[0])
-            file_extension = Downloaded_File[Downloaded_File.find('.')::]
-            time_tag = gmtime()
-            time_tag_str = f'{time_tag[0]}'
-            for i in range(1, len(time_tag)):
-                time_tag_str += f'_{time_tag[i]}'
-            new_file_name = f'unscaled_records_{time_tag_str}{file_extension}'
-            Downloaded_File = os.path.join(self.outdir, Downloaded_File)
-            Downloaded_File_Rename = os.path.join(self.outdir, new_file_name)
-            os.rename(Downloaded_File, Downloaded_File_Rename)
-            self.Unscaled_rec_file = Downloaded_File_Rename
-            print(f'Downloaded files are located in\n{self.Unscaled_rec_file}')
-        else:
-            raise ValueError('You have to use NGA_W2 database to use ngaw2_download method.')
+        self.username = username
+        self.pwd = password
+        driver = set_driver(self.output_directory_path, browser)
+        driver = sign_in(driver, self.username, self.pwd)
+        rsn = ''
+        for i in self.rec_rsn:
+            rsn += str(int(i)) + ','
+        rsn = rsn[:-1:]
+        files_before_download = set(os.listdir(self.output_directory_path))
+        download(rsn, self.output_directory_path, driver)
+        files_after_download = set(os.listdir(self.output_directory_path))
+        downloaded_file = str(list(files_after_download.difference(files_before_download))[0])
+        file_extension = downloaded_file[downloaded_file.find('.')::]
+        time_tag = gmtime()
+        time_tag_str = f'{time_tag[0]}'
+        for i in range(1, len(time_tag)):
+            time_tag_str += f'_{time_tag[i]}'
+        new_file_name = f'unscaled_records_{time_tag_str}{file_extension}'
+        downloaded_file = os.path.join(self.output_directory_path, downloaded_file)
+        downloaded_file_rename = os.path.join(self.output_directory_path, new_file_name)
+        os.rename(downloaded_file, downloaded_file_rename)
+        self.unscaled_rec_file = downloaded_file_rename
+        print(f'Downloaded files are located in\n{self.unscaled_rec_file}')
 
 
-class conditional_spectrum(_subclass_):
+class ConditionalSpectrum(_SubClass_):
     """
     This class is used to
         1) Create target spectrum
             Unconditional spectrum using specified gmpe
             Conditional spectrum using average spectral acceleration
             Conditional spectrum using spectral acceleration
             with and without considering variance
@@ -1094,129 +1149,132 @@
     Reference:
     Baker, J. W., & Bradley, B. A. (2017). Intensity Measure Correlations Observed in the NGA-West2 Database,
     and Dependence of Correlations on Rupture and Site Parameters. In Earthquake Spectra, 33(1): 145–156.
     SAGE Publications. https://doi.org/10.1193/060716eqs095m
 
     """
 
-    def __init__(self, database='NGA_W2', outdir='Outputs', obj_pkl=None):
+    def __init__(self, database='NGA_W2', output_directory='Outputs', obj_path=None):
         # TODO: Combine all metadata into single sql file.
         """
         Details
         -------
         Loads the database and add spectral values for Tstar 
         if they are not present via interpolation.
         
         Parameters
         ----------
         database : str, optional
             Database to use: NGA_W2, ESM_2018
             The default is NGA_W2.
-        outdir     : str, optional, the default is 'Outputs'.
+        output_directory : str, optional.
             output directory to create.
-        obj_pkl    : str, optional, the default is None.
+            The default is 'Outputs'
+        obj_path : str, optional
             This is the path to the previously saved obj.pkl file by EzGM.
             One can use the previously saved instance and use rest of the methods.
+            The default is None.
 
         Returns
         -------
         None.
         """
 
         # Inherit the subclass
         super().__init__()
 
         # Read the old EzGM obj
-        if obj_pkl:
+        if obj_path:
             with open('obj.pkl', 'rb') as file:
                 obj = pickle.load(file)
             self.__dict__.update(obj)
             database = self.database
 
         # Add the input the ground motion database to use
+        # TODO: Combine all metadata into single jason file. Not essential, but makes the code more elegant.
         matfile = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'Meta_Data', database)
         self.database = loadmat(matfile, squeeze_me=True)
         self.database['Name'] = database
 
         # create the output directory and add the path to self
         cwd = os.getcwd()
-        outdir_path = os.path.join(cwd, outdir)
-        self.outdir = outdir_path
-        create_dir(self.outdir)
+        outdir_path = os.path.join(cwd, output_directory)
+        self.output_directory_path = outdir_path
+        make_dir(self.output_directory_path)
 
     @staticmethod
-    def _BakerJayaramCorrelationModel(T1, T2):
+    def _baker_jayaram_correlation_model(period1, period2):
         """
         Details
         -------
         Valid for T = 0.01-10sec
     
         References
         ----------
         Baker JW, Jayaram N. Correlation of Spectral Acceleration Values from NGA Ground Motion Models.
         Earthquake Spectra 2008; 24(1): 299–317. DOI: 10.1193/1.2857544.
     
         Parameters
         ----------
-        T1: float
+        period1 : float
             First period
-        T2: float
+        period2 : float
             Second period
     
         Returns
         -------
         rho: float
              Predicted correlation coefficient
         """
 
-        t_min = min(T1, T2)
-        t_max = max(T1, T2)
+        period_min = min(period1, period2)
+        period_max = max(period1, period2)
 
-        c1 = 1.0 - np.cos(np.pi / 2.0 - np.log(t_max / max(t_min, 0.109)) * 0.366)
+        c1 = 1.0 - np.cos(np.pi / 2.0 - np.log(period_max / max(period_min, 0.109)) * 0.366)
 
-        if t_max < 0.2:
-            c2 = 1.0 - 0.105 * (1.0 - 1.0 / (1.0 + np.exp(100.0 * t_max - 5.0))) * (t_max - t_min) / (t_max - 0.0099)
+        if period_max < 0.2:
+            c2 = 1.0 - 0.105 * (1.0 - 1.0 / (1.0 + np.exp(100.0 * period_max - 5.0))) * (period_max - period_min) / (period_max - 0.0099)
         else:
             c2 = 0
 
-        if t_max < 0.109:
+        if period_max < 0.109:
             c3 = c2
         else:
             c3 = c1
 
-        c4 = c1 + 0.5 * (np.sqrt(c3) - c3) * (1.0 + np.cos(np.pi * t_min / 0.109))
+        c4 = c1 + 0.5 * (np.sqrt(c3) - c3) * (1.0 + np.cos(np.pi * period_min / 0.109))
 
-        if t_max <= 0.109:
+        if period_max <= 0.109:
             rho = c2
-        elif t_min > 0.109:
+        elif period_min > 0.109:
             rho = c1
-        elif t_max < 0.2:
+        elif period_max < 0.2:
             rho = min(c2, c4)
         else:
             rho = c4
 
         return rho
 
     @staticmethod
-    def _AkkarCorrelationModel(T1, T2):
+    def _akkar_correlation_model(period1, period2):
         """
         Details
         -------
         Valid for T = 0.01-4sec
         
         References
         ----------
         Akkar S., Sandikkaya MA., Ay BO., 2014, Compatible ground-motion prediction equations for damping scaling factors and vertical to
         horizontal spectral amplitude ratios for the broader Europe region, Bull Earthquake Eng, 12, pp. 517-547.
     
         Parameters
         ----------
-        T1: float
+        period1 : float
             First period
-        T2: float
+        period2 : float
             Second period
                 
         Returns
         -------
         rho: float
              Predicted correlation coefficient
         """
@@ -1287,107 +1345,106 @@
         0.407614656 0.405891106 0.395959027 0.382643147 0.361144444 0.306970917 0.300263857 0.293617699 0.290206583 0.292110467 0.288451408 0.277634726 0.281420646 0.294133111 0.306425395 0.316085084 0.318255597 0.331189588 0.343741052 0.354811270 0.362685030 0.384069571 0.395008131 0.406239072 0.421772989 0.433855649 0.444875501 0.463713683 0.476248728 0.485714453 0.501197105 0.518704609 0.552881805 0.575140732 0.591795296 0.600662073 0.614480633 0.640059806 0.662520328 0.684390394 0.705186975 0.723105274 0.750903010 0.775111246 0.797159548 0.816003233 0.830185558 0.844973436 0.860372144 0.873284821 0.883214300 0.890966585 0.915648423 0.940025622 0.963690232 0.980406376 0.993026697 1.000000000 0.993978542 0.981867206 0.966916287 0.948046812
         0.396021594 0.394456219 0.384472121 0.371369841 0.347895826 0.299373684 0.293958754 0.287088479 0.285660879 0.289709619 0.286332638 0.274937010 0.279922024 0.292219131 0.305054461 0.313419871 0.315234055 0.327291574 0.337998036 0.349292709 0.355378232 0.376313732 0.385989904 0.396941043 0.412532101 0.423004536 0.430804997 0.446156606 0.456731904 0.465636186 0.482174544 0.499605944 0.533306855 0.557374629 0.573567528 0.579974232 0.592939430 0.619237511 0.640719458 0.661759771 0.683325524 0.701638253 0.730395857 0.752923049 0.776927194 0.794462365 0.809841631 0.825545291 0.840698066 0.853349923 0.862440172 0.870858532 0.898224725 0.923972912 0.948213960 0.965648634 0.981015917 0.993978542 1.000000000 0.994161539 0.982017362 0.965411448
         0.388023676 0.387127235 0.379463066 0.368779338 0.346769536 0.297351745 0.290136746 0.283841030 0.282668509 0.286648955 0.282976017 0.271795167 0.276053857 0.287580691 0.299876324 0.308003502 0.308869052 0.317595706 0.327063915 0.338303391 0.343260457 0.364472634 0.373069949 0.383166929 0.397753600 0.408583246 0.417351819 0.432274411 0.443049297 0.450877709 0.467548386 0.485384263 0.519094244 0.543168691 0.560578412 0.566198740 0.579314389 0.605167550 0.626871803 0.649062742 0.671466883 0.690121946 0.717967558 0.738669004 0.762772025 0.779529183 0.793789262 0.809170358 0.824522815 0.838230714 0.846539221 0.855151540 0.882650968 0.909276123 0.933929338 0.950884209 0.967271742 0.981867206 0.994161539 1.000000000 0.994786494 0.982542990
         0.374414280 0.374517227 0.366941903 0.357389576 0.335928741 0.290186844 0.282338477 0.277461634 0.276289052 0.279832113 0.276909997 0.265717553 0.270090412 0.280332211 0.290794284 0.297064428 0.296407372 0.299746833 0.309826727 0.321379107 0.325705273 0.345928556 0.353855693 0.363913564 0.376298229 0.385674105 0.395571593 0.411058267 0.422456988 0.429516192 0.446761605 0.465544137 0.500329740 0.526976523 0.544366449 0.551510187 0.564841776 0.589955841 0.611834493 0.633832190 0.655909098 0.673817186 0.700891537 0.720369328 0.743974698 0.760413104 0.774388186 0.789750612 0.803606701 0.816197107 0.825195593 0.834216891 0.861796234 0.890558074 0.916174312 0.934166833 0.951464983 0.966916287 0.982017362 0.994786494 1.000000000 0.994598788
         0.327591227 0.327475695 0.319627396 0.309845437 0.287061335 0.244808717 0.246124740 0.243767437 0.246189710 0.251575366 0.249258668 0.239620288 0.245635104 0.255837514 0.264918559 0.271319428 0.267233297 0.264459231 0.276507212 0.286839305 0.290190152 0.306793984 0.313364781 0.322319411 0.334237875 0.343985400 0.354611000 0.368638617 0.380051200 0.387956859 0.405181228 0.425482934 0.465522040 0.492870578 0.510064415 0.517257200 0.530236122 0.553791800 0.575691608 0.595807459 0.616808159 0.635307705 0.664055282 0.684394961 0.706169171 0.721304101 0.734778759 0.750310219 0.763724118 0.777354214 0.788230830 0.798942709 0.830129231 0.863419172 0.891643991 0.911343164 0.931015807 0.948046812 0.965411448 0.982542990 0.994598788 1.000000000
         """, dtype=float, sep=" ").reshape(-1, len(periods))
 
-        if np.any([T1, T2] < periods[0]) or \
-                np.any([T1, T2] > periods[-1]):
+        if np.any([period1, period2] < periods[0]) or \
+                np.any([period1, period2] > periods[-1]):
             raise ValueError("Period array contains values outside of the "
                              "range supported by the Akkar et al. (2014) "
                              "correlation model")
 
-        if T1 == T2:
+        if period1 == period2:
             rho = 1.0
         else:
-            rho = interpolate.interp2d(periods, periods, coeff_table, kind='linear')(T1, T2)[0]
+            rho = interpolate.interp2d(periods, periods, coeff_table, kind='linear')(period1, period2)[0]
 
         return rho
 
-    def _get_correlation(self, T1, T2):
+    def _get_correlation(self, period1, period2):
         """
         Details
         -------
         Compute the inter-period correlation for any two Sa(T) values.
         
         Parameters
         ----------
-        T1: float
+        period1 : float
             First period
-        T2: float
+        period2 : float
             Second period
                 
         Returns
         -------
-        rho: float
+        rho : float
              Predicted correlation coefficient
         """
         # TODO: Add alternative correlation models: https://github.com/bakerjw/NGAW2_correlations
 
         correlation_function_handles = {
-            'baker_jayaram': self._BakerJayaramCorrelationModel,
-            'akkar': self._AkkarCorrelationModel,
+            'baker_jayaram': self._baker_jayaram_correlation_model,
+            'akkar': self._akkar_correlation_model,
         }
 
         # Check for existing correlation function
-        if self.corr_func not in correlation_function_handles:
+        if self.correlation_model not in correlation_function_handles:
             raise ValueError('Not a valid correlation function')
         else:
             rho = \
-                correlation_function_handles[self.corr_func](T1, T2)
+                correlation_function_handles[self.correlation_model](period1, period2)
 
         return rho
 
-    def _gmpe_sb_2014_ratios(self, T):
+    def _gmpe_sb_2014_ratios(self, periods):
         """
         Details
         -------
         Computes Sa_RotD100/Sa_RotD50 ratios.
 
         References
         ----------
         Shahi, S. K., and Baker, J. W. (2014). "NGA-West2 models for ground-
         motion directionality." Earthquake Spectra, 30(3), 1285-1300.
 
         Parameters
         ----------
-        T: numpy.ndarray
+        periods : numpy.ndarray
             Period(s) of interest (sec)
 
         Returns
         -------
-        ratio: float
+        ratio : float
              geometric mean of Sa_RotD100/Sa_RotD50
-        sigma: float
+        sigma : float
             standard deviation of log(Sa_RotD100/Sa_RotD50)
         """
 
         # Model coefficient values from Table 1 of the above-reference paper
         periods_orig = np.array(
             [0.0100000000000000, 0.0200000000000000, 0.0300000000000000, 0.0500000000000000, 0.0750000000000000,
              0.100000000000000, 0.150000000000000, 0.200000000000000, 0.250000000000000, 0.300000000000000,
              0.400000000000000, 0.500000000000000, 0.750000000000000, 1, 1.50000000000000, 2, 3, 4, 5,
              7.50000000000000, 10])
-        ratios_orig = np.array(
+        mu_ratios_orig = np.array(
             [1.19243805900000, 1.19124621700000, 1.18767783300000, 1.18649074900000, 1.18767783300000,
              1.18767783300000, 1.19961419400000, 1.20562728500000, 1.21652690500000, 1.21896239400000,
              1.22875320400000, 1.22875320400000, 1.23738465100000, 1.24110237900000, 1.24234410200000,
              1.24358706800000, 1.24732343100000, 1.25985923900000, 1.264908769000, 1.28531008400000,
              1.29433881900000])
         sigma_orig = np.array(
             [0.08, 0.08, 0.08, 0.08, 0.08, 0.08, 0.08, 0.08, 0.08, 0.08, 0.08, 0.08, 0.08, 0.08, 0.08, 0.08, 0.08,
              0.08, 0.08, 0.08, 0.08])
 
         # Interpolate to compute values for the user-specified periods
-        f = interpolate.interp1d(np.log(periods_orig), ratios_orig)(np.log(T))
-        ratio = interpolate.interp1d(np.log(periods_orig), ratios_orig)(np.log(T))
-        sigma = interpolate.interp1d(np.log(periods_orig), sigma_orig)(np.log(T))
+        mu_ratio = interpolate.interp1d(np.log(periods_orig), mu_ratios_orig)(np.log(periods))
+        sigma = interpolate.interp1d(np.log(periods_orig), sigma_orig)(np.log(periods))
 
-        return ratio, sigma
+        return mu_ratio, sigma
 
     def _get_cond_param(self, sctx, rctx, dctx):
         """
         Details
         -------
         This function calculates the logarithmic mean and standard deviation of intensity measure
         predicted by the selected GMPM at conditioning periods.
@@ -1400,67 +1457,64 @@
         rctx : openquake.hazardlib.gsim object
             An instance of RuptureContext with a single rupture information.
         dctx : openquake.hazardlib.gsim object
             An instance of DistancesContext with information about the distances between sites and a rupture.
     
         Returns
         -------
-        mu_lnSaTstar : float
-            Logarithmic mean of intensity measure according to the selected GMPM.
-        sigma_lnSaTstar : float
-           Logarithmic standard deviation of intensity measure according to the selected GMPM.
-        rho_T_Tstar : numpy.array
+        mu_lnAvgsaTstar : float
+            Logarithmic mean of intensity measure according to the selected GMPE.
+        sigma_lnAvgsaTstar : float
+           Logarithmic standard deviation of intensity measure according to the selected GMPE.
+        rho_lnSaT_lnAvgsaTstar : numpy.ndarray
             Correlation coefficients.
         """
 
-        n = len(self.Tstar)
-        mu_lnSaT = np.zeros(n)
-        sigma_lnSaT = np.zeros(n)
-        MoC = np.zeros((n, n))
-
-        # Get the GMPE output
-        for i in range(n):
-            mu_lnSaT[i], stddvs_lnSa = self.bgmpe.get_mean_and_stddevs(sctx, rctx, dctx, imt.SA(period=self.Tstar[i]),
-                                                                       [const.StdDev.TOTAL])
-            sigma_lnSaT[i] = stddvs_lnSa[0]
-
-            # modify spectral targets if RotD100 values were specified for two-component selection
-            if self.Sa_def == 'RotD100' and not 'RotD100' in self.bgmpe.DEFINED_FOR_INTENSITY_MEASURE_COMPONENT and self.selection == 2:
-                rotD100Ratio, rotD100Sigma = self._gmpe_sb_2014_ratios(self.Tstar[i])
-                mu_lnSaT[i] = mu_lnSaT[i] + np.log(rotD100Ratio)
-                sigma_lnSaT[i] = (sigma_lnSaT[i] ** 2 + rotD100Sigma ** 2) ** 0.5
-
-            for j in range(n):
-                rho = self._get_correlation(self.Tstar[i], self.Tstar[j])
-                MoC[i, j] = rho
-
-        Sa_avg_meanLn = (1 / n) * sum(mu_lnSaT)  # logarithmic mean of AvgSa
-
-        Sa_avg_std = 0
-        for i in range(n):
-            for j in range(n):
-                Sa_avg_std = Sa_avg_std + (MoC[i, j] * sigma_lnSaT[i] * sigma_lnSaT[j])  # logarithmic Var of the AvgSa
-
-        Sa_avg_std = Sa_avg_std * (1 / n) ** 2
-
-        # compute mean of logarithmic average spectral acceleration and logarithmic standard deviation of spectral
-        # acceleration prediction
-        mu_lnSaTstar = Sa_avg_meanLn
-        sigma_lnSaTstar = np.sqrt(Sa_avg_std)
-
-        # compute correlation coefficients
-        rho_T_Tstar = np.zeros(len(self.T))
-        for i in range(len(self.T)):
-            for j in range(len(self.Tstar)):
-                rho_bj = self._get_correlation(self.T[i], self.Tstar[j])
-                rho_T_Tstar[i] = rho_bj * sigma_lnSaT[j] + rho_T_Tstar[i]
+        len_Tstar = len(self.Tstar)
+        mu_lnSaTstar = np.zeros(len_Tstar)
+        sigma_lnSaTstar = np.zeros(len_Tstar)
+        MoC = np.zeros((len_Tstar, len_Tstar))
+
+        # Get the raw GMPE output (SAs only)
+        for i in range(len_Tstar):
+            params = self.bgmpe.get_mean_and_stddevs(sctx, rctx, dctx, imt.SA(period=self.Tstar[i]), [const.StdDev.TOTAL])
+            mu_lnSaTstar[i] = params[0]
+            sigma_lnSaTstar[i] = params[1][0]
+
+            # Modify spectral targets if RotD100 values were specified for two-component selection
+            if self.spectrum_definition == 'RotD100' and not 'RotD100' in self.bgmpe.DEFINED_FOR_INTENSITY_MEASURE_COMPONENT and self.num_components == 2:
+                rotD100_mu_ratio, rotD100_sigma = self._gmpe_sb_2014_ratios(self.Tstar[i])
+                mu_lnSaTstar[i] = mu_lnSaTstar[i] + np.log(rotD100_mu_ratio)
+                sigma_lnSaTstar[i] = (sigma_lnSaTstar[i] ** 2 + rotD100_sigma ** 2) ** 0.5
+
+            # Compute correlations at AvgSA periods
+            for j in range(len_Tstar):
+                rho_lnSaTstar_lnSaTstar = self._get_correlation(self.Tstar[i], self.Tstar[j])
+                MoC[i, j] = rho_lnSaTstar_lnSaTstar
+
+        # Determine logarithmic mean and standard from selected gmpe for IM=AvgSA
+        # In case of IM=SA len_period_star becomes 1, thus, also works in this case
+        mu_lnAvgsaTstar = (1 / len_Tstar) * sum(mu_lnSaTstar)
+        sigma_lnAvgsaTstar = 0
+        for i in range(len_Tstar):
+            for j in range(len_Tstar):
+                sigma_lnAvgsaTstar = sigma_lnAvgsaTstar + (MoC[i, j] * sigma_lnSaTstar[i] * sigma_lnSaTstar[j])
+        sigma_lnAvgsaTstar = np.sqrt(sigma_lnAvgsaTstar * (1 / len_Tstar) ** 2)
+
+        # Compute correlation coefficients for IM=AvgSA
+        # In case of IM=SA len_period_star becomes 1, thus, also works in this case
+        rho_lnSaT_lnAvgsaTstar = np.zeros(len(self.periods))
+        for i in range(len(self.periods)):
+            for j in range(len_Tstar):
+                rho = self._get_correlation(self.periods[i], self.Tstar[j])
+                rho_lnSaT_lnAvgsaTstar[i] = rho_lnSaT_lnAvgsaTstar[i] + rho * sigma_lnSaTstar[j]
 
-            rho_T_Tstar[i] = rho_T_Tstar[i] / (len(self.Tstar) * sigma_lnSaTstar)
+            rho_lnSaT_lnAvgsaTstar[i] = rho_lnSaT_lnAvgsaTstar[i] / (len_Tstar * sigma_lnAvgsaTstar)
 
-        return mu_lnSaTstar, sigma_lnSaTstar, rho_T_Tstar
+        return mu_lnAvgsaTstar, sigma_lnAvgsaTstar, rho_lnSaT_lnAvgsaTstar
 
     def _set_contexts(self, index):
 
         """
         Details
         -------
         Sets the parameters for the computation of a ground motion model. If
@@ -1474,15 +1528,15 @@
         Kaklamanos J, Baise LG, Boore DM. (2011) Estimating unknown input parameters
         when implementing the NGA ground-motion prediction equations in engineering
         practice. Earthquake Spectra 27: 1219-1235.
         https://doi.org/10.1193/1.3650372.
 
         Parameters
         ----------
-        index: int
+        index : int
             The scenario index for which gmm attributes are set
 
         Returns
         -------
         sctx : openquake.hazardlib.contexts.SitesContext
             An instance of SitesContext with sites information to calculate PoEs on.
         rctx : openquake.hazardlib.contexts.RuptureContext
@@ -1598,18 +1652,15 @@
                 if dip == 90:
                     rx = rjb * np.sin(np.radians(azimuth))
                 else:
                     if (0 <= azimuth < 90) or (90 < azimuth <= 180):
                         if rjb * np.abs(np.tan(np.radians(azimuth))) <= width * np.cos(np.radians(dip)):
                             rx = rjb * np.abs(np.tan(np.radians(azimuth)))
                         else:
-                            rx = rjb * np.tan(np.radians(azimuth)) * np.cos(np.radians(azimuth) -
-                                                                            np.arcsin(width * np.cos(
-                                                                                np.radians(dip)) * np.cos(
-                                                                                np.radians(azimuth)) / rjb))
+                            rx = rjb * np.tan(np.radians(azimuth)) * np.cos(np.radians(azimuth) - np.arcsin(width * np.cos(np.radians(dip)) * np.cos(np.radians(azimuth)) / rjb))
                     elif azimuth == 90:  # we assume that Rjb>0
                         rx = rjb + width * np.cos(np.radians(dip))
                     else:
                         rx = rjb * np.sin(np.radians(azimuth))
         elif 'rx' in self.dist_param.keys():
             rx = self.dist_param['rx'][index]
             rjb = None
@@ -1628,20 +1679,18 @@
 
         # rrup
         if rjb and dip == 90:
             rrup = np.sqrt(np.square(rjb) + np.square(ztor))
         elif rx:
             if rx < ztor * np.tan(np.radians(dip)):
                 rrup1 = np.sqrt(np.square(rx) + np.square(ztor))
-            if ztor * np.tan(np.radians(dip)) <= rx <= ztor * np.tan(np.radians(dip)) + width * 1. / np.cos(
-                    np.radians(dip)):
+            if ztor * np.tan(np.radians(dip)) <= rx <= ztor * np.tan(np.radians(dip)) + width * 1. / np.cos(np.radians(dip)):
                 rrup1 = rx * np.sin(np.radians(dip)) + ztor * np.cos(np.radians(dip))
             if rx > ztor * np.tan(np.radians(dip)) + width * 1. / np.cos(np.radians(dip)):
-                rrup1 = np.sqrt(
-                    np.square(rx - width * np.cos(np.radians(dip))) + np.square(ztor + width * np.sin(np.radians(dip))))
+                rrup1 = np.sqrt(np.square(rx - width * np.cos(np.radians(dip))) + np.square(ztor + width * np.sin(np.radians(dip))))
             rrup = np.sqrt(np.square(rrup1) + np.square(ry0))
         elif not 'rrup' in self.dist_param.keys():
             if 'rhypo' in self.dist_param.keys():
                 rrup = self.dist_param['rhypo'][index]
             elif 'repi' in self.dist_param.keys():
                 rrup = self.dist_param['repi'][index]
             else:
@@ -1709,30 +1758,117 @@
                 temp = np.array([self.site_param[key]])
             else:
                 temp = np.array([self.site_param[key]], dtype='float64')
             setattr(sctx, key, temp)
 
         return sctx, rctx, dctx
 
-    def create(self, Tstar=0.5, gmpe='BooreEtAl2014', selection=1, Sa_def='RotD50',
+    @staticmethod
+    @njit
+    def _find_rec_greedy(sample_small, scaling_factors, mu_ln, sigma_ln, rec_id, sample_big, error_weights, max_scale_factor, num_records, penalty):
+        """
+        Details
+        -------
+        Greedy subset modification algorithm
+        The method is defined separately so that njit can be used as wrapper and the routine can be run faster
+
+        Parameters
+        ----------
+        sample_small : numpy.ndarray (2-D)
+            Spectra of the reduced candidate record set (num_records - 1)
+        scaling_factors : numpy.ndarray (1-D)
+            Scaling factors for all records in the filtered database
+        mu_ln : numpy.ndarray (1-D)
+            Logarthmic mean of the target spectrum (conditional or unconditional)
+        sigma_ln : numpy.ndarray (1-D)
+            Logarthmic standard deviation of the target spectrum (conditional or unconditional)
+        rec_id : numpy.ndarray (1-D)
+            Record IDs of the reduced candidate set records in the database (num_records - 1)
+        sample_big : numpy.ndarray (2-D)
+            Spectra of the records in the filtered database
+        error_weights : numpy.ndarray (1-D) or list 
+            Weights for error in mean, standard deviation and skewness
+        max_scale_factor : float
+            The maximum allowable scale factor
+        num_records : int
+            Number of ground motions to be selected.
+        penalty : int
+            > 0 to penalize selected spectra more than 3 sigma from the target at any period, 0 otherwise.
+
+        Returns
+        -------
+        min_id : int
+            ID of the new selected record with the scale factor closest to 1
+        """
+        def mean_numba(arr):
+            """
+            Computes the mean of a 2-D array along axis=0.
+            Required for computations since njit is used as wrapper.
+            """
+
+            res = []
+            for i in range(arr.shape[1]):
+                res.append(arr[:, i].mean())
+
+            return np.array(res)
+
+        def std_numba(arr):
+            """
+            Computes the standard deviation of a 2-D array along axis=0.
+            Required for computations since njit is used as wrapper.
+            """
+
+            res = []
+            for i in range(arr.shape[1]):
+                res.append(arr[:, i].std())
+
+            return np.array(res)
+
+        min_dev = 100000
+        for j in range(sample_big.shape[0]):
+            # Add to the sample the scaled spectrum
+            temp = np.zeros((1, len(sample_big[j, :])))
+            temp[:, :] = sample_big[j, :]
+            sample_small_trial = np.concatenate((sample_small, temp + np.log(scaling_factors[j])), axis=0)
+            dev_mean = mean_numba(sample_small_trial) - mu_ln  # Compute deviations from target
+            dev_sig = std_numba(sample_small_trial) - sigma_ln
+            dev_total = error_weights[0] * np.sum(dev_mean * dev_mean) + error_weights[1] * np.sum(dev_sig * dev_sig)
+
+            # Check if we exceed the scaling limit
+            if scaling_factors[j] > max_scale_factor or scaling_factors[j] < 1 / max_scale_factor or np.any(rec_id == j):
+                dev_total = dev_total + 1000000
+            # Penalize bad spectra
+            elif penalty > 0:
+                for m in range(num_records):
+                    dev_total = dev_total + np.sum(np.abs(np.exp(sample_small_trial[m, :]) > np.exp(mu_ln + 3.0 * sigma_ln))) * penalty
+                    dev_total = dev_total + np.sum(np.abs(np.exp(sample_small_trial[m, :]) < np.exp(mu_ln - 3.0 * sigma_ln))) * penalty
+
+            # Should cause improvement and record should not be repeated
+            if dev_total < min_dev:
+                min_id = j
+                min_dev = dev_total
+
+        return min_id
+
+    def create(self, Tstar=None, gmpe='BooreEtAl2014', num_components=1, spectrum_definition='RotD50',
                site_param={'vs30': 520}, rup_param={'rake': [0.0, 45.0], 'mag': [7.2, 6.5]},
-               dist_param={'rjb': [20, 5]}, Hcont=[0.6, 0.4], T_Tgt_range=[0.01, 4],
-               im_Tstar=1.0, epsilon=None, cond=1, useVar=1, corr_func='baker_jayaram'):
+               dist_param={'rjb': [20, 5]}, hz_cont=[0.6, 0.4], period_range=[0.01, 4],
+               im_Tstar=1.0, epsilon=None, use_variance=1, correlation_model='baker_jayaram'):
         """
         Details
         -------
         Creates the target spectrum (conditional or unconditional).
     
         Notes
         -----
         See https://docs.openquake.org/oq-engine/master/openquake.hazardlib.gsim.html
         in order to check required input parameters for the ground motion models.
         e.g. rupture parameters (rup_param), site parameters (site_param), distance parameters (dist_param).
         Rupture parameters 'fhw', 'azimuth', 'upper_sd' and 'lower_sd' are used to derive some gmm parameters
-        in accordance with Kaklamanos et al. 2011 within conditional_spectrum._set_contexts method. They are not
+        in accordance with Kaklamanos et al. 2011 within ConditionalSpectrum._set_contexts method. They are not
         required by any gmm.
 
         References
         ----------
         Baker JW. Conditional Mean Spectrum: Tool for Ground-Motion Selection.
         Journal of Structural Engineering 2011; 137(3): 322–331.
         DOI: 10.1061/(ASCE)ST.1943-541X.0000215.
@@ -1746,268 +1882,275 @@
         Kohrangi, M., Bazzurro, P., Vamvatsikos, D., and Spillatura, A.
         Conditional spectrum-based ground motion record selection using average 
         spectral acceleration. Earthquake Engineering & Structural Dynamics, 
         2017, 46(10): 1667–1685.
 
         Parameters
         ----------
-        Tstar    : int, float, numpy.array, the default is None.
+        Tstar : int, float, numpy.ndarray
             Conditioning period or periods in case of AvgSa [sec].
-        gmpe     : str, optional
+            If None the target is an unconditional spectrum.
+            The default is None.
+        gmpe : str, optional
             GMPE model (see OpenQuake library).
             The default is 'BooreEtAl2014'.
-        selection : int, optional, The default is 1.
+        num_components : int, optional, the default is 1.
             1 for single-component selection and arbitrary component sigma.
             2 for two-component selection and average component sigma.
-        Sa_def : str, optional, the default is 'RotD50'.
-            The spectra definition. Necessary if selection = 2.
-            'GeoMean', 'RotD50', 'RotD100'.
-        site_param : dictionary, The default is {'vs30': 520}
+        spectrum_definition : str, optional
+            The spectra definition, 'GeoMean', 'RotD50', 'RotD100'. Necessary if num_components = 2.
+            The default is 'RotD50'.
+        site_param : dictionary
             Contains site parameters to define target spectrum.
             Dictionary keys (parameters) are not list type. Same parameters are used for each scenario.
             Some parameters are:
             'vs30': Average shear-wave velocity of the site
             'vs30measured': vs30 type, True (measured) or False (inferred)
             'z1pt0': Depth to Vs=1 km/sec from the site
             'z2pt5': Depth to Vs=2.5 km/sec from the site
-        rup_param  : dictionary, The default is {'rake': [0.0, 45.0], 'mag': [7.2, 6.5]}
+            The default is {'vs30': 520}
+        rup_param : dictionary
             Contains rupture parameters to define target spectrum.
             Dictionary keys (parameters) are list type. Each item in the list corresponds to a scenario.
             Some parameters are:
             'mag': Magnitude of the earthquake (required by all gmm)
             'rake': Fault rake
             'dip': Fault dip
             'width': Fault width
             'hypo_depth': Hypocentral depth of the rupture
             'ztor': Depth to top of coseismic rupture (km)
             'fhw': Hanging-wall factor, 1 for site on down-dip side of top of rupture; 0 otherwise (optional)
             'azimuth': Source-to-site azimuth, alternative of hanging wall factor (optional)
             'upper_sd': Upper seismogenic depth (optional)
             'lower_sd': Lower seismogenic depth (optional)
-        dist_param : dictionary, The default is {'rjb': [20, 5]}
+            The default is {'rake': [0.0, 45.0], 'mag': [7.2, 6.5]}
+        dist_param : dictionary
             Contains distance parameters to define target spectrum.
             Dictionary keys (parameters) are list type. Each item in the list corresponds to a scenario.
             Some parameters are:
             'rjb': Closest distance to surface projection of coseismic rupture (km)
             'rrup': Closest distance to coseismic rupture (km)
             'repi': Epicentral distance (km)
             'rhypo': Hypocentral distance (km)
             'rx': Horizontal distance from top of rupture measured perpendicular to fault strike (km)
             'ry0': The horizontal distance off the end of the rupture measured parallel to strike (km)
-        Hcont      : list, optional, the default is None.
+            The default is {'rjb': [20, 5]}
+        hz_cont : list, optional
             Hazard contribution for considered scenarios. 
             If None hazard contribution is the same for all scenarios.
-        im_Tstar   : int, float, optional, the default is 1.
+            The default is None.
+        im_Tstar : int, float, optional
             Conditioning intensity measure level [g] (conditional selection)
-        epsilon    : list, optional, the default is None.
+            the default is 1.
+        epsilon : list, optional
             Epsilon values for considered scenarios (conditional selection)
-        T_Tgt_range: list, optional, the default is [0.01,4].
+            The default is None.
+        period_range : list, optional
             Lower and upper bound values for the period range of target spectrum.
-        cond       : int, optional
-            0 to run unconditional selection
-            1 to run conditional selection
-        useVar     : int, optional, the default is 1.
+            The default is [0.01,4].
+        use_variance : int, optional
             0 not to use variance in target spectrum
             1 to use variance in target spectrum
-        corr_func: str, optional, the default is baker_jayaram
+            The default is 1.
+        correlation_model : str, optional
             correlation model to use "baker_jayaram","akkar"
+            The default is baker_jayaram
 
         Returns
         -------
         None.                    
         """
         # TODO: gsim.get_mean_and_stddevs is deprecated, use ContextMaker.get_mean_stds in the future.
         # https://docs.openquake.org/oq-engine/advanced/developing.html#working-with-gmpes-directly-the-contextmaker
 
         # TODO:  Make the step size equal in period array. This will result in more realistic matching.
-        #  However, this is not essential. Moreover, this will require generation of new meta_data files
+        # However, this is not essential. Moreover, this will require generation of new meta_data files
+        if Tstar is None:
+            # runing unconditional spectrum based record selection
+            self.is_conditioned = 0
 
-        if cond == 1:
+        else:
+            # runing conditional-spectrum based record selection
+            self.is_conditioned = 1
 
             # add Tstar to self
             if isinstance(Tstar, int) or isinstance(Tstar, float):
                 self.Tstar = np.array([Tstar])
             elif isinstance(Tstar, numpy.ndarray):
                 self.Tstar = Tstar
 
             # check if AvgSa or Sa is used as IM, then in case of Sa(T*) add T* and Sa(T*) if not present
             if not self.Tstar[0] in self.database['Periods'] and len(self.Tstar) == 1:
                 f = interpolate.interp1d(self.database['Periods'], self.database['Sa_1'], axis=1)
-                Sa_int = f(self.Tstar[0])
-                Sa_int.shape = (len(Sa_int), 1)
-                Sa = np.append(self.database['Sa_1'], Sa_int, axis=1)
-                Periods = np.append(self.database['Periods'], self.Tstar[0])
-                self.database['Sa_1'] = Sa[:, np.argsort(Periods)]
+                sa_in = f(self.Tstar[0])
+                sa_in.shape = (len(sa_in), 1)
+                sa = np.append(self.database['Sa_1'], sa_in, axis=1)
+                periods = np.append(self.database['Periods'], self.Tstar[0])
+                self.database['Sa_1'] = sa[:, np.argsort(periods)]
 
                 f = interpolate.interp1d(self.database['Periods'], self.database['Sa_2'], axis=1)
-                Sa_int = f(self.Tstar[0])
-                Sa_int.shape = (len(Sa_int), 1)
-                Sa = np.append(self.database['Sa_2'], Sa_int, axis=1)
-                self.database['Sa_2'] = Sa[:, np.argsort(Periods)]
+                sa_in = f(self.Tstar[0])
+                sa_in.shape = (len(sa_in), 1)
+                sa = np.append(self.database['Sa_2'], sa_in, axis=1)
+                self.database['Sa_2'] = sa[:, np.argsort(periods)]
 
                 f = interpolate.interp1d(self.database['Periods'], self.database['Sa_RotD50'], axis=1)
-                Sa_int = f(self.Tstar[0])
-                Sa_int.shape = (len(Sa_int), 1)
-                Sa = np.append(self.database['Sa_RotD50'], Sa_int, axis=1)
-                self.database['Sa_RotD50'] = Sa[:, np.argsort(Periods)]
+                sa_in = f(self.Tstar[0])
+                sa_in.shape = (len(sa_in), 1)
+                sa = np.append(self.database['Sa_RotD50'], sa_in, axis=1)
+                self.database['Sa_RotD50'] = sa[:, np.argsort(periods)]
 
                 f = interpolate.interp1d(self.database['Periods'], self.database['Sa_RotD100'], axis=1)
-                Sa_int = f(self.Tstar[0])
-                Sa_int.shape = (len(Sa_int), 1)
-                Sa = np.append(self.database['Sa_RotD100'], Sa_int, axis=1)
-                self.database['Sa_RotD100'] = Sa[:, np.argsort(Periods)]
+                sa_in = f(self.Tstar[0])
+                sa_in.shape = (len(sa_in), 1)
+                sa = np.append(self.database['Sa_RotD100'], sa_in, axis=1)
+                self.database['Sa_RotD100'] = sa[:, np.argsort(periods)]
 
-                self.database['Periods'] = Periods[np.argsort(Periods)]
+                self.database['Periods'] = periods[np.argsort(periods)]
 
         try:  # this is smth like self.bgmpe = gsim.boore_2014.BooreEtAl2014()
             self.bgmpe = gsim.get_available_gsims()[gmpe]()
             self.gmpe = gmpe
 
         except KeyError:
             print(f'{gmpe} is not a valid gmpe name')
             raise
 
         # add target spectrum settings to self
-        self.selection = selection
-        self.Sa_def = Sa_def
-        self.cond = cond
-        self.useVar = useVar
-        self.corr_func = corr_func
+        self.num_components = num_components
+        self.spectrum_definition = spectrum_definition
+        self.use_variance = use_variance
+        self.correlation_model = correlation_model
         self.site_param = site_param
         self.rup_param = rup_param
         self.dist_param = dist_param
 
-        nScenarios = len(rup_param['mag'])  # number of scenarios
-        if Hcont is None:  # equal for all
-            self.Hcont = [1 / nScenarios for _ in range(nScenarios)]
+        num_scenarios = len(rup_param['mag'])  # number of scenarios
+        if hz_cont is None:  # equal for all
+            self.hz_cont = [1 / num_scenarios for _ in range(num_scenarios)]
         else:
-            self.Hcont = Hcont
+            self.hz_cont = hz_cont
 
         # Period range of the target spectrum
-        temp = np.abs(self.database['Periods'] - np.min(T_Tgt_range))
+        temp = np.abs(self.database['Periods'] - np.min(period_range))
         idx1 = np.where(temp == np.min(temp))[0][0]
-        temp = np.abs(self.database['Periods'] - np.max(T_Tgt_range))
+        temp = np.abs(self.database['Periods'] - np.max(period_range))
         idx2 = np.where(temp == np.min(temp))[0][0]
-        self.T = self.database['Periods'][idx1:idx2 + 1]
-
-        # Get number of scenarios, and their contribution
-        Hcont_mat = np.matlib.repmat(np.asarray(self.Hcont), len(self.T), 1)
-
-        # Conditional spectrum, log parameters
-        TgtMean = np.zeros((len(self.T), nScenarios))
+        self.periods = self.database['Periods'][idx1:idx2 + 1]
 
-        # Covariance
-        TgtCov = np.zeros((nScenarios, len(self.T), len(self.T)))
+        # Hazard contribution of all rupture scenarios
+        hz_cont_rups = np.matlib.repmat(np.asarray(self.hz_cont), len(self.periods), 1)
+        # Conditional mean spectra (in logartihm) for all rupture scenarios
+        mu_ln_rups = np.zeros((len(self.periods), num_scenarios))
+        # Covariance matrices for all rupture scenarios
+        cov_rups = np.zeros((num_scenarios, len(self.periods), len(self.periods)))
 
-        for n in range(nScenarios):
+        for n in range(num_scenarios):
 
             # gmpe spectral values
-            mu_lnSaT = np.zeros(len(self.T))
-            sigma_lnSaT = np.zeros(len(self.T))
+            mu_lnSaT = np.zeros(len(self.periods))
+            sigma_lnSaT = np.zeros(len(self.periods))
 
             # correlation coefficients
-            rho_T_Tstar = np.zeros(len(self.T))
+            rho_lnSaT_lnAvgsaTstar = np.zeros(len(self.periods))
 
             # Covariance
-            Cov = np.zeros((len(self.T), len(self.T)))
+            cov = np.zeros((len(self.periods), len(self.periods)))
 
             # Set the contexts for the scenario
             sctx, rctx, dctx = self._set_contexts(n)
 
-            # TODO: Combine all metadata into single sql file. Not essential, but makes the code more elegant.
-            for i in range(len(self.T)):
+            for i in range(len(self.periods)):
                 # Get the GMPE output for a rupture scenario
-                mu, sigma = self.bgmpe.get_mean_and_stddevs(sctx, rctx, dctx, imt.SA(period=self.T[i]),
-                                                            [const.StdDev.TOTAL])
-                mu_lnSaT[i] = mu
-                sigma_lnSaT[i] = sigma[0]
+                params = self.bgmpe.get_mean_and_stddevs(sctx, rctx, dctx, imt.SA(period=self.periods[i]), [const.StdDev.TOTAL])
+                mu_lnSaT[i] = params[0]
+                sigma_lnSaT[i] = params[1][0]
                 # modify spectral targets if RotD100 values were specified for two-component selection:
-                if self.Sa_def == 'RotD100' and not 'RotD100' in self.bgmpe.DEFINED_FOR_INTENSITY_MEASURE_COMPONENT and self.selection == 2:
-                    rotD100Ratio, rotD100Sigma = self._gmpe_sb_2014_ratios(self.T[i])
-                    mu_lnSaT[i] = mu_lnSaT[i] + np.log(rotD100Ratio)
-                    sigma_lnSaT[i] = (sigma_lnSaT[i] ** 2 + rotD100Sigma ** 2) ** 0.5
-
-            if self.cond == 1:
-                # Get the GMPE output and calculate AvgSa_Tstar and associated dispersion
-                mu_lnSaTstar, sigma_lnSaTstar, rho_T_Tstar = self._get_cond_param(sctx, rctx, dctx)
+                if self.spectrum_definition == 'RotD100' and not 'RotD100' in self.bgmpe.DEFINED_FOR_INTENSITY_MEASURE_COMPONENT and self.num_components == 2:
+                    rotd100_mu_ratio, rotd100_sigma = self._gmpe_sb_2014_ratios(self.periods[i])
+                    mu_lnSaT[i] = mu_lnSaT[i] + np.log(rotd100_mu_ratio)
+                    sigma_lnSaT[i] = (sigma_lnSaT[i] ** 2 + rotd100_sigma ** 2) ** 0.5
+
+            if self.is_conditioned == 1:
+                # Get the GMPE output and calculate for IM=AvgSA and associated dispersion
+                mu_lnAvgsaTstar, sigma_lnAvgsaTstar, rho_lnSaT_lnAvgsaTstar = self._get_cond_param(sctx, rctx, dctx)
 
                 if epsilon is None:
                     # Back calculate epsilon
-                    rup_eps = (np.log(im_Tstar) - mu_lnSaTstar) / sigma_lnSaTstar
+                    epsilon_rup = (np.log(im_Tstar) - mu_lnAvgsaTstar) / sigma_lnAvgsaTstar
                 else:
-                    rup_eps = epsilon[n]
+                    epsilon_rup = epsilon[n]
 
                 # Get the value of the ln(CMS), conditioned on T_star
-                TgtMean[:, n] = mu_lnSaT + rho_T_Tstar * rup_eps * sigma_lnSaT
+                mu_ln_rups[:, n] = mu_lnSaT + rho_lnSaT_lnAvgsaTstar * epsilon_rup * sigma_lnSaT
 
-            elif self.cond == 0:
-                TgtMean[:, n] = mu_lnSaT
+            elif self.is_conditioned == 0:
+                mu_ln_rups[:, n] = mu_lnSaT
 
-            for i in range(len(self.T)):
-                for j in range(len(self.T)):
+            for i in range(len(self.periods)):
+                for j in range(len(self.periods)):
 
                     var1 = sigma_lnSaT[i] ** 2
                     var2 = sigma_lnSaT[j] ** 2
 
-                    rho = self._get_correlation(self.T[i], self.T[j])
-                    sigma_Corr = rho * np.sqrt(var1 * var2)
+                    rho = self._get_correlation(self.periods[i], self.periods[j])
+                    sigma_corr = rho * np.sqrt(var1 * var2)
 
-                    if self.cond == 1:
-                        varTstar = sigma_lnSaTstar ** 2
-                        sigma11 = np.matrix([[var1, sigma_Corr], [sigma_Corr, var2]])
+                    if self.is_conditioned == 1:
+                        varTstar = sigma_lnAvgsaTstar ** 2
+                        sigma11 = np.matrix([[var1, sigma_corr], [sigma_corr, var2]])
                         sigma22 = np.array([varTstar])
-                        sigma12 = np.array([rho_T_Tstar[i] * np.sqrt(var1 * varTstar),
-                                            rho_T_Tstar[j] * np.sqrt(varTstar * var2)])
+                        sigma12 = np.array([rho_lnSaT_lnAvgsaTstar[i] * np.sqrt(var1 * varTstar), rho_lnSaT_lnAvgsaTstar[j] * np.sqrt(varTstar * var2)])
                         sigma12.shape = (2, 1)
                         sigma22.shape = (1, 1)
                         sigma_cond = sigma11 - sigma12 * 1. / sigma22 * sigma12.T
-                        Cov[i, j] = sigma_cond[0, 1]
+                        cov[i, j] = sigma_cond[0, 1]
 
-                    elif self.cond == 0:
-                        Cov[i, j] = sigma_Corr
+                    elif self.is_conditioned == 0:
+                        cov[i, j] = sigma_corr
 
             # Get the value of standard deviation of target spectrum
-            TgtCov[n, :, :] = Cov
+            cov_rups[n, :, :] = cov
 
         # over-write covariance matrix with zeros if no variance is desired in the ground motion selection
-        if self.useVar == 0:
-            TgtCov = np.zeros(TgtCov.shape)
+        if self.use_variance == 0:
+            cov_rups = np.zeros(cov_rups.shape)
 
-        TgtMean_fin = np.sum(TgtMean * Hcont_mat, 1)
+        mu_ln_target = np.sum(mu_ln_rups * hz_cont_rups, 1)
         # all 2D matrices are the same for each kk scenario, since sigma is only T dependent
-        TgtCov_fin = TgtCov[0, :, :]
-        Cov_elms = np.zeros((len(self.T), nScenarios))
-        for ii in range(len(self.T)):
-            for kk in range(nScenarios):
+        cov_target = cov_rups[0, :, :]
+        cov_elms = np.zeros((len(self.periods), num_scenarios))
+        for ii in range(len(self.periods)):
+            for kk in range(num_scenarios):
                 # Hcont[kk] is hazard contribution of the k-th scenario
-                Cov_elms[ii, kk] = (TgtCov[kk, ii, ii] + (TgtMean[ii, kk] - TgtMean_fin[ii]) ** 2) * self.Hcont[kk]
+                cov_elms[ii, kk] = (cov_rups[kk, ii, ii] + (mu_ln_rups[ii, kk] - mu_ln_target[ii]) ** 2) * self.hz_cont[kk]
 
         # Compute the final covariance matrix
-        cov_diag = np.sum(Cov_elms, 1)
-        TgtCov_fin[np.eye(len(self.T)) == 1] = cov_diag
+        cov_diag = np.sum(cov_elms, 1)
+        cov_target[np.eye(len(self.periods)) == 1] = cov_diag
         # Avoid positive semi-definite covariance matrix with several eigenvalues being exactly zero.
         # See: https://stackoverflow.com/questions/41515522/numpy-positive-semi-definite-warning!
-        min_eig = np.min(np.real(np.linalg.eigvals(TgtCov_fin)))
+        min_eig = np.min(np.real(np.linalg.eigvals(cov_target)))
         if min_eig < 0:
-            TgtCov_fin -= 2 * min_eig * np.eye(*TgtCov_fin.shape)
-        TgtSigma_fin = np.sqrt(np.diagonal(TgtCov_fin))
+            cov_target -= 2 * min_eig * np.eye(*cov_target.shape)
+        sigma_ln_target = np.sqrt(np.diagonal(cov_target))
 
         # Add target spectrum to self
-        self.mu_ln = TgtMean_fin
-        self.sigma_ln = TgtSigma_fin
-        self.cov = TgtCov_fin
+        self.mu_ln = mu_ln_target
+        self.sigma_ln = sigma_ln_target
+        self.cov = cov_target
 
-        if cond == 1:
+        if self.is_conditioned == 1:
             # add intensity measure level to self
             if epsilon is None:
                 self.im_Tstar = im_Tstar
             else:
-                f = interpolate.interp1d(self.T, np.exp(self.mu_ln))
-                Sa_int = f(self.Tstar)
-                self.im_Tstar = np.exp(np.sum(np.log(Sa_int)) / len(self.Tstar))
+                f = interpolate.interp1d(self.periods, np.exp(self.mu_ln))
+                sa_in = f(self.Tstar)
+                self.im_Tstar = np.exp(np.sum(np.log(sa_in)) / len(self.Tstar))
                 self.epsilon = epsilon
 
         print('Target spectrum is created.')
 
     def _simulate_spectra(self):
         """
         Details
@@ -2020,644 +2163,637 @@
         
         Returns
         -------
         None.
         """
 
         # Set initial seed for simulation
-        if self.seedValue:
-            np.random.seed(self.seedValue)
+        if self.seed_value:
+            np.random.seed(self.seed_value)
         else:
             np.random.seed(sum(gmtime()[:6]))
 
-        devTotalSim = np.zeros((self.nTrials, 1))
-        specDict = {}
+        dev_total_sim = np.zeros((self.num_simulations, 1))
+        spectra = {}
         # Generate simulated response spectra with best matches to the target values
-        for j in range(self.nTrials):
+        for j in range(self.num_simulations):
             # It might be better to use the second function if cov_rank = np.linalg.matrix_rank(self.cov) < len(mu_ln)
-            specDict[j] = np.exp(random_multivariate_normal(self.mu_ln, self.cov, self.nGM, 'LHS'))
-            # specDict[j] = np.exp(np.random.multivariate_normal(self.mu_ln, self.cov, size=self.nGM))
+            spectra[j] = np.exp(random_multivariate_normal(self.mu_ln, self.cov, self.num_records, 'LHS'))
+            # specDict[j] = np.exp(np.random.multivariate_normal(self.mu_ln, self.cov, size=self.num_records))
 
             # how close is the mean of the spectra to the target
-            devMeanSim = np.mean(np.log(specDict[j]), axis=0) - self.mu_ln
+            dev_mean_sim = np.mean(np.log(spectra[j]), axis=0) - self.mu_ln
             # how close is the mean of the spectra to the target
-            devSigSim = np.std(np.log(specDict[j]), axis=0) - self.sigma_ln
+            dev_sig_sim = np.std(np.log(spectra[j]), axis=0) - self.sigma_ln
             # how close is the skewness of the spectra to zero (i.e., the target)  
-            devSkewSim = skew(np.log(specDict[j]), axis=0)
+            dev_skew_sim = skew(np.log(spectra[j]), axis=0)
             # combine the three error metrics to compute a total error
-            devTotalSim[j] = self.weights[0] * np.sum(devMeanSim ** 2) + \
-                             self.weights[1] * np.sum(devSigSim ** 2) + \
-                             0.1 * (self.weights[2]) * np.sum(devSkewSim ** 2)
-
-        recUse = np.argmin(np.abs(devTotalSim))  # find the simulated spectra that best match the targets
-        self.sim_spec = np.log(specDict[recUse])  # return the best set of simulations
-
-    def select(self, nGM=30, isScaled=1, maxScale=4,
-               Mw_lim=None, Vs30_lim=None, Rjb_lim=None, fault_lim=None,
-               nTrials=20, seedValue=None, weights=[1, 2, 0.3], nLoop=2, penalty=0, tol=10):
+            dev_total_sim[j] = self.error_weights[0] * np.sum(dev_mean_sim ** 2) + self.error_weights[1] * np.sum(dev_sig_sim ** 2) + 0.1 * (self.error_weights[2]) * np.sum(dev_skew_sim ** 2)
+
+        recUse = np.argmin(np.abs(dev_total_sim))  # find the simulated spectra that best match the targets
+        self.sim_spec = np.log(spectra[recUse])  # return the best set of simulations
+
+    def select(self, num_records=30, is_scaled=1, max_scale_factor=4, mag_limits=None, vs30_limits=None, rjb_limits=None,
+               mech_limits=None, num_simulations=20, seed_value=None, error_weights=[1, 2, 0.3], num_greedy_loops=2, penalty=0, 
+               tolerance=10):
         """
         Details
         -------
         Perform the ground motion selection.
         
         References
         ----------
         Jayaram, N., Lin, T., and Baker, J. W. (2011). 
         A computationally efficient ground-motion selection algorithm for 
         matching a target response spectrum mean and variance.
         Earthquake Spectra, 27(3), 797-815.
         
         Parameters
         ----------
-        nGM : int, optional, the default is 30.
+        num_records : int, optional
             Number of ground motions to be selected.
-        isScaled : int, optional, the default is 1.
-            0 not to allow use of amplitude scaling for spectral matching.
-            1 to allow use of amplitude scaling for spectral matching.
-        maxScale : float, optional, the default is 4.
+            The default is 30.
+        max_scale_factor : float, optional
             The maximum allowable scale factor
-        Mw_lim : list, optional, the default is None.
-            The limiting values on magnitude. 
-        Vs30_lim : list, optional, the default is None.
+            If None use of amplitude scaling for spectral matching is not allowed.
+            If other than None use of amplitude scaling for spectral matching is allowed.
+            The default is 4.
+        is_scaled : int, optional
+            If 1 use of amplitude scaling for spectral matching is not allowed.
+            If 0 None use of amplitude scaling for spectral matching is allowed.
+            The default is 1.        
+        mag_limits : list, optional
+            The limiting values on magnitude.
+            The default is None.
+        vs30_limits : list, optional
             The limiting values on Vs30. 
-        Rjb_lim : list, optional, the default is None.
-            The limiting values on Rjb. 
-        fault_lim : list, optional, the default is None.
+            The default is None.
+        rjb_limits : list, optional
+            The limiting values on Rjb.
+            The default is None.
+        mech_limits : list, optional
             The limiting fault mechanisms.
             For NGA_W2 database:
                 0 for unspecified fault
                 1 for strike-slip fault
                 2 for normal fault
                 3 for reverse fault
             For ESM_2018 database:
                 'NF' for normal faulting
                 'NS' for predominately normal with strike-slip component
                 'O' for oblique
                 'SS' for strike-slip faulting
                 'TF' for thrust faulting
                 'TS' for predominately thrust with strike-slip component
                 'U' for unknown
-        nTrials : int, optional, the default is 20.
-            nTrials sets of response spectra are simulated and the best set (in terms of
+            The default is None.
+        num_simulations : int, optional
+            num_simulations sets of response spectra are simulated and the best set (in terms of
             matching means, variances and skewness is chosen as the seed). The user
             can also optionally rerun this segment multiple times before deciding to
             proceed with the rest of the algorithm. It is to be noted, however, that
             the greedy improvement technique significantly improves the match between
             the means and the variances subsequently.
-        seedValue  : int, optional, the default is None.
-            For repeatability. For a particular seedValue not equal to
+            The default is 20.
+        seed_value : int, optional
+            For repeatability. For a particular seed value not equal to
             zero, the code will output the same set of ground motions.
-            The set will change when the seedValue changes. If set to
+            The set will change when the seed value changes. If set to
             zero, the code randomizes the algorithm and different sets of
             ground motions (satisfying the target mean and variance) are
             generated each time.
-        weights : numpy.array or list, optional, the default is [1,2,0.3].
+            The default is None.
+        error_weights : numpy.ndarray or list, optional
             Weights for error in mean, standard deviation and skewness
-        nLoop   : int, optional, the default is 2.
+            the default is [1, 2, 0.3].
+        num_greedy_loops : int, optional
             Number of loops of optimization to perform.
-        penalty : int, optional, the default is 0.
-            > 0 to penalize selected spectra more than 
-            3 sigma from the target at any period, = 0 otherwise.
-        tol     : int, optional, the default is 10.
-            Tolerable percent error to skip optimization 
+            The default is 2.
+        penalty : int, optional
+            > 0 to penalize selected spectra more than 3 sigma from the target at any period, 
+            0 otherwise.
+            The default is 0.
+        tolerance : int, optional
+            Tolerable percent error to skip optimization
+            The default is 10.
 
         Returns
         -------
         None.
         """
 
         # Add selection settings to self
-        self.nGM = nGM
-        self.isScaled = isScaled
-        self.Mw_lim = Mw_lim
-        self.Vs30_lim = Vs30_lim
-        self.Rjb_lim = Rjb_lim
-        self.fault_lim = fault_lim
-        self.seedValue = seedValue
-        self.weights = weights
-        self.nTrials = nTrials
-        self.maxScale = maxScale
-        self.nLoop = nLoop
-        self.tol = tol
+        self.num_records = num_records
+        self.mag_limits = mag_limits
+        self.vs30_limits = vs30_limits
+        self.rjb_limits = rjb_limits
+        self.mech_limits = mech_limits
+        self.seed_value = seed_value
+        self.error_weights = error_weights
+        self.num_simulations = num_simulations
+        self.max_scale_factor = max_scale_factor
+        self.is_scaled = is_scaled
+        self.num_greedy_loops = num_greedy_loops
+        self.tolerance = tolerance
         self.penalty = penalty
 
         # Simulate response spectra
         self._simulate_spectra()
 
         # Search the database and filter
-        sampleBig, Vs30, Mw, Rjb, fault, Filename_1, Filename_2, NGA_num, eq_ID, station_code = self._search_database()
+        sample_big, vs30, mag, rjb, mechanism, filename1, filename2, rsn, eq_id, station_code = self._search_database()
 
         # Processing available spectra
-        sampleBig = np.log(sampleBig)
-        nBig = sampleBig.shape[0]
+        sample_big = np.log(sample_big)
+        len_big = sample_big.shape[0]
 
         # Find best matches to the simulated spectra from ground-motion database
-        recID = np.ones(self.nGM, dtype=int) * (-1)
-        finalScaleFac = np.ones(self.nGM)
-        sampleSmall = np.ones((self.nGM, sampleBig.shape[1]))
-        weights = np.array(weights)
+        rec_id = np.ones(self.num_records, dtype=int) * (-1)
+        final_scale_factors = np.ones(self.num_records)
+        sample_small = np.ones((self.num_records, sample_big.shape[1]))
+        error_weights = np.array(error_weights)
+
+        # Check if max_scale_factor is None
+        if max_scale_factor is None:
+            max_scale_factor = 10 # use the default value
 
-        if self.cond == 1 and self.isScaled == 1:
+        if self.is_conditioned == 1 and self.is_scaled == 1:
             # Calculate IMLs for the sample
-            f = interpolate.interp1d(self.T, np.exp(sampleBig), axis=1)
-            sampleBig_imls = np.exp(np.sum(np.log(f(self.Tstar)), axis=1) / len(self.Tstar))
+            f = interpolate.interp1d(self.periods, np.exp(sample_big), axis=1)
+            sample_big_imls = np.exp(np.sum(np.log(f(self.Tstar)), axis=1) / len(self.Tstar))
 
-        if self.cond == 1 and len(self.Tstar) == 1:
+        if self.is_conditioned == 1 and len(self.Tstar) == 1:
             # These indices are required in case IM = Sa(T) to break the loop
-            ind2 = (np.where(self.T != self.Tstar[0])[0][0]).tolist()
+            ind2 = (np.where(self.periods != self.Tstar[0])[0][0]).tolist()
 
-        # Find nGM ground motions, initial subset
-        for i in range(self.nGM):
-            err = np.zeros(nBig)
-            scaleFac = np.ones(nBig)
+        # Find num_records ground motions, initial subset
+        for i in range(self.num_records):
+            error = np.zeros(len_big)
+            scaling_factors = np.ones(len_big)
 
             # Calculate the scaling factor
-            if self.isScaled == 1:
+            if self.is_scaled == 1:
                 # using conditioning IML
-                if self.cond == 1:
-                    scaleFac = self.im_Tstar / sampleBig_imls
+                if self.is_conditioned == 1:
+                    scaling_factors = self.im_Tstar / sample_big_imls
                 # using error minimization
-                elif self.cond == 0:
-                    scaleFac = np.sum(np.exp(sampleBig) * np.exp(self.sim_spec[i, :]), axis=1) / np.sum(
-                        np.exp(sampleBig) ** 2, axis=1)
+                elif self.is_conditioned == 0:
+                    scaling_factors = np.sum(np.exp(sample_big) * np.exp(self.sim_spec[i, :]), axis=1) / np.sum(np.exp(sample_big) ** 2, axis=1)
+
             else:
-                scaleFac = np.ones(nBig)
+                scaling_factors = np.ones(len_big)
 
-            mask = (1 / self.maxScale < scaleFac) * (scaleFac < self.maxScale)
+            # check if enough records are found
+            mask = (1 / max_scale_factor < scaling_factors) * (scaling_factors < max_scale_factor)
             idxs = np.where(mask)[0]
-            err[~mask] = 1000000
-            err[mask] = np.sum((np.log(
-                np.exp(sampleBig[idxs, :]) * scaleFac[mask].reshape(len(scaleFac[mask]), 1)) -
-                                self.sim_spec[i, :]) ** 2, axis=1)
-
-            recID[i] = int(np.argsort(err)[0])
-            if err.min() >= 1000000:
+            error[~mask] = 1000000
+            error[mask] = np.sum((np.log(np.exp(sample_big[idxs, :]) * scaling_factors[mask].reshape(len(scaling_factors[mask]), 1)) -self.sim_spec[i, :]) ** 2, axis=1)
+            rec_id[i] = int(np.argsort(error)[0])
+            if error.min() >= 1000000:
                 raise Warning('Possible problem with simulated spectrum. No good matches found')
 
-            if self.isScaled == 1:
-                finalScaleFac[i] = scaleFac[recID[i]]
+            if self.is_scaled == 1:
+                final_scale_factors[i] = scaling_factors[rec_id[i]]
 
             # Save the selected spectra
-            sampleSmall[i, :] = np.log(np.exp(sampleBig[recID[i], :]) * finalScaleFac[i])
-
-        # Apply Greedy subset modification procedure
-        # Use njit to speed up the optimization algorithm
-        @njit
-        def find_rec(sampleSmall, scaleFac, mu_ln, sigma_ln, recIDs):
-
-            def mean_numba(a):
-
-                res = []
-                for i in range(a.shape[1]):
-                    res.append(a[:, i].mean())
+            sample_small[i, :] = np.log(np.exp(sample_big[rec_id[i], :]) * final_scale_factors[i])
 
-                return np.array(res)
+        # Apply greedy subset modification procedure
+        for _ in range(self.num_greedy_loops):  # Number of passes
 
-            def std_numba(a):
-
-                res = []
-                for i in range(a.shape[1]):
-                    res.append(a[:, i].std())
-
-                return np.array(res)
-
-            minDev = 100000
-            for j in range(nBig):
-                # Add to the sample the scaled spectra
-                temp = np.zeros((1, len(sampleBig[j, :])))
-                temp[:, :] = sampleBig[j, :]
-                tempSample = np.concatenate((sampleSmall, temp + np.log(scaleFac[j])), axis=0)
-                devMean = mean_numba(tempSample) - mu_ln  # Compute deviations from target
-                devSig = std_numba(tempSample) - sigma_ln
-                devTotal = weights[0] * np.sum(devMean * devMean) + weights[1] * np.sum(devSig * devSig)
-
-                # Check if we exceed the scaling limit
-                if scaleFac[j] > maxScale or scaleFac[j] < 1 / maxScale or np.any(recIDs == j):
-                    devTotal = devTotal + 1000000
-                # Penalize bad spectra
-                elif penalty > 0:
-                    for m in range(nGM):
-                        devTotal = devTotal + np.sum(
-                            np.abs(np.exp(tempSample[m, :]) > np.exp(mu_ln + 3.0 * sigma_ln))) * penalty
-                        devTotal = devTotal + np.sum(
-                            np.abs(np.exp(tempSample[m, :]) < np.exp(mu_ln - 3.0 * sigma_ln))) * penalty
-
-                # Should cause improvement and record should not be repeated
-                if devTotal < minDev:
-                    minID = j
-                    minDev = devTotal
-
-            return minID
-
-        for k in range(self.nLoop):  # Number of passes
-
-            for i in range(self.nGM):  # Loop for nGM
-                sampleSmall = np.delete(sampleSmall, i, 0)
-                recID = np.delete(recID, i)
+            for i in range(self.num_records):  # Loop for num_records
+                sample_small = np.delete(sample_small, i, 0)
+                rec_id = np.delete(rec_id, i)
 
                 # Calculate the scaling factor
-                if self.isScaled == 1:
+                if self.is_scaled == 1:
                     # using conditioning IML
-                    if self.cond == 1:
-                        scaleFac = self.im_Tstar / sampleBig_imls
+                    if self.is_conditioned == 1:
+                        scaling_factors = self.im_Tstar / sample_big_imls
                     # using error minimization
-                    elif self.cond == 0:
-                        scaleFac = np.sum(np.exp(sampleBig) * np.exp(self.sim_spec[i, :]), axis=1) / np.sum(
-                            np.exp(sampleBig) ** 2, axis=1)
+                    elif self.is_conditioned == 0:
+                        scaling_factors = np.sum(np.exp(sample_big) * np.exp(self.sim_spec[i, :]), axis=1) / np.sum(np.exp(sample_big) ** 2, axis=1)
                 else:
-                    scaleFac = np.ones(nBig)
+                    scaling_factors = np.ones(len_big)
 
-                # Try to add a new spectra to the subset list
-                minID = find_rec(sampleSmall, scaleFac, self.mu_ln, self.sigma_ln, recID)
+                # Try to add a new spectrum to the subset list
+                min_id = self._find_rec_greedy(sample_small, scaling_factors, self.mu_ln, self.sigma_ln, rec_id, sample_big, error_weights, max_scale_factor, num_records, penalty)
 
                 # Add new element in the right slot
-                if self.isScaled == 1:
-                    finalScaleFac[i] = scaleFac[minID]
+                if self.is_scaled == 1:
+                    final_scale_factors[i] = scaling_factors[min_id]
                 else:
-                    finalScaleFac[i] = 1
-                sampleSmall = np.concatenate(
-                    (sampleSmall[:i, :], sampleBig[minID, :].reshape(1, sampleBig.shape[1]) + np.log(scaleFac[minID]),
-                     sampleSmall[i:, :]), axis=0)
-                recID = np.concatenate((recID[:i], np.array([minID]), recID[i:]))
+                    final_scale_factors[i] = 1
+                sample_small = np.concatenate((sample_small[:i, :], sample_big[min_id, :].reshape(1, sample_big.shape[1]) + np.log(scaling_factors[min_id]), sample_small[i:, :]), axis=0)
+                rec_id = np.concatenate((rec_id[:i], np.array([min_id]), rec_id[i:]))
 
             # Lets check if the selected ground motions are good enough, if the errors are sufficiently small stop!
-            if self.cond == 1 and len(self.Tstar) == 1:  # if conditioned on SaT, ignore error at T*
-                medianErr = np.max(
-                    np.abs(np.exp(np.mean(sampleSmall[:, ind2], axis=0)) - np.exp(self.mu_ln[ind2])) / np.exp(
-                        self.mu_ln[ind2])) * 100
-                stdErr = np.max(
-                    np.abs(np.std(sampleSmall[:, ind2], axis=0) - self.sigma_ln[ind2]) / self.sigma_ln[ind2]) * 100
+            if self.is_conditioned == 1 and len(self.Tstar) == 1:  # if conditioned on SaT, ignore error at T*
+                median_error = np.max(np.abs(np.exp(np.mean(sample_small[:, ind2], axis=0)) - np.exp(self.mu_ln[ind2])) / np.exp(self.mu_ln[ind2])) * 100
+                std_error = np.max(np.abs(np.std(sample_small[:, ind2], axis=0) - self.sigma_ln[ind2]) / self.sigma_ln[ind2]) * 100
             else:
-                medianErr = np.max(
-                    np.abs(np.exp(np.mean(sampleSmall, axis=0)) - np.exp(self.mu_ln)) / np.exp(self.mu_ln)) * 100
-                stdErr = np.max(np.abs(np.std(sampleSmall, axis=0) - self.sigma_ln) / self.sigma_ln) * 100
+                median_error = np.max(np.abs(np.exp(np.mean(sample_small, axis=0)) - np.exp(self.mu_ln)) / np.exp(self.mu_ln)) * 100
+                std_error = np.max(np.abs(np.std(sample_small, axis=0) - self.sigma_ln) / self.sigma_ln) * 100
 
-            if medianErr < self.tol and stdErr < self.tol:
+            if median_error < self.tolerance and std_error < self.tolerance:
                 break
+
         print('Ground motion selection is finished.')
-        print(f'For T ∈ [{self.T[0]:.2f} - {self.T[-1]:.2f}]')
-        print(f'Max error in median = {medianErr:.2f} %')
-        print(f'Max error in standard deviation = {stdErr:.2f} %')
-        if medianErr < self.tol and stdErr < self.tol:
-            print(f'The errors are within the target {self.tol:d} percent %')
+        print(f'For T ∈ [{self.periods[0]:.2f} - {self.periods[-1]:.2f}]')
+        print(f'Max error in median = {median_error:.2f} %')
+        print(f'Max error in standard deviation = {std_error:.2f} %')
+        if median_error < self.tolerance and std_error < self.tolerance:
+            print(f'The errors are within the target {self.tolerance:d} percent %')
 
-        recID = recID.tolist()
+        rec_id = rec_id.tolist()
         # Add selected record information to self
-        self.rec_scale = finalScaleFac
-        self.rec_spec = sampleSmall
-        self.rec_Vs30 = Vs30[recID]
-        self.rec_Rjb = Rjb[recID]
-        self.rec_Mw = Mw[recID]
-        self.rec_fault = fault[recID]
-        self.rec_eqID = eq_ID[recID]
-        self.rec_h1 = Filename_1[recID]
+        self.rec_scale_factors = final_scale_factors
+        self.rec_sa_ln = sample_small
+        self.rec_vs30 = vs30[rec_id]
+        self.rec_rjb = rjb[rec_id]
+        self.rec_mag = mag[rec_id]
+        self.rec_mech = mechanism[rec_id]
+        self.rec_eq_id = eq_id[rec_id]
+        self.rec_file_h1 = filename1[rec_id]
 
-        if self.selection == 2:
-            self.rec_h2 = Filename_2[recID]
+        if self.num_components == 2:
+            self.rec_file_h2 = filename2[rec_id]
 
         if self.database['Name'] == 'NGA_W2':
-            self.rec_rsn = NGA_num[recID]
+            self.rec_rsn = rsn[rec_id]
 
         if self.database['Name'] == 'ESM_2018':
-            self.rec_station_code = station_code[recID]
+            self.rec_station_code = station_code[rec_id]
 
 
-class code_spectrum(_subclass_):
+class CodeSpectrum(_SubClass_):
     """
     This class is used for
         1) Creating target spectrum based on various codes (TBEC 2018, ASCE 7-16, EC8-Part1)
         2) Selecting and scaling suitable ground motion sets for target spectrum in accordance with specified code
     """
 
-    def __init__(self, database='NGA_W2', outdir='Outputs', target_path=None, nGM=11, selection=1, opt=1,
-                 Mw_lim=None, Vs30_lim=None, Rjb_lim=None, fault_lim=None, maxScale=2, RecPerEvent=3, obj_pkl=None):
+    def __init__(self, database='NGA_W2', output_directory='Outputs', target_path=None, num_records=11, num_components=1, selection_algorithm=1,
+                 mag_limits=None, vs30_limits=None, rjb_limits=None, mech_limits=None, max_scale_factor=2, max_rec_per_event=3, obj_path=None):
         """
         Details
         -------
         Loads the record database to use, creates output folder, sets selection criteria.
 
         Parameters
         ----------
         database : str, optional
             Database to use: NGA_W2, ESM_2018
             The default is NGA_W2.
-        outdir : str, optional
+        output_directory : str, optional
             Output directory
             The default is 'Outputs'
-        target_path = str, optional, the default is None.
+        target_path : str, optional, the default is None.
             Path for used defined target spectrum.
-        nGM : int, optional, the default is 11.
+        num_records : int, optional, the default is 11.
             Number of records to be selected. 
-        selection : int, optional, the default is 1.
+        num_components : int, optional, the default is 1.
             Number of ground motion components to select.
-        opt : int, optional, the default is 1.
+        selection_algorithm : int, optional, the default is 1.
             If equal to 1, the record set is selected using
             method of “least squares”, each record has individual scaling factor.
             If equal to 2, the record set selected such that each record has
             identical scale factor which is as close as possible to 1.
-        Mw_lim : list, optional, the default is None.
+        mag_limits : list, optional, the default is None.
             The limiting values on magnitude. 
-        Vs30_lim : list, optional, the default is None.
+        vs30_limits : list, optional, the default is None.
             The limiting values on Vs30. 
-        Rjb_lim : list, optional, the default is None.
+        rjb_limits : list, optional, the default is None.
             The limiting values on Rjb. 
-        fault_lim : list, optional, the default is None.
+        mech_limits : list, optional, the default is None.
             The limiting fault mechanisms.
             For NGA_W2 database:
                 0 for unspecified fault
                 1 for strike-slip fault
                 2 for normal fault
                 3 for reverse fault
             For ESM_2018 database:
                 'NF' for normal faulting
                 'NS' for predominately normal with strike-slip component
                 'O' for oblique
                 'SS' for strike-slip faulting
                 'TF' for thrust faulting
                 'TS' for predominately thrust with strike-slip component
                 'U' for unknown
-        maxScale : float, optional, the default is 2.
+        max_scale_factor : float, optional, the default is 2.
             Maximum allowed scaling factor, used with opt=2 case.
-        RecPerEvent: int, the default is 3.
+        max_rec_per_event : int, the default is 3.
             The limit for the maximum number of records belong to the same event
-        obj_pkl    : str, optional, the default is None.
+        obj_path : str, optional, the default is None.
             This is the path to the previously saved obj.pkl file by EzGM.
             One can use the previously saved instance and use rest of the methods.
 
         Returns
         -------
         None.
         """
 
         # Inherit the subclass
         super().__init__()
 
         # Read the old EzGM obj
-        if obj_pkl:
+        if obj_path:
             with open('obj.pkl', 'rb') as file:
                 obj = pickle.load(file)
             self.__dict__.update(obj)
             database = self.database
 
         # Add new selection settings to self
         else:
-            self.nGM = nGM
-            self.selection = selection
-            self.Mw_lim = Mw_lim
-            self.Vs30_lim = Vs30_lim
-            self.Rjb_lim = Rjb_lim
-            self.fault_lim = fault_lim
-            self.opt = opt
-            self.maxScale = maxScale
+            self.num_records = num_records
+            self.num_components = num_components
+            self.mag_limits = mag_limits
+            self.vs30_limits = vs30_limits
+            self.rjb_limits = rjb_limits
+            self.mech_limits = mech_limits
+            self.selection_algorithm = selection_algorithm
+            self.max_scale_factor = max_scale_factor
             self.target_path = target_path
-            self.RecPerEvent = RecPerEvent
+            self.max_rec_per_event = max_rec_per_event
 
         # Add the input the ground motion database to use
         matfile = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'Meta_Data', database)
         self.database = loadmat(matfile, squeeze_me=True)
         if 'Name' in self.database:
             pass
         else:
             self.database['Name'] = database
 
         # create the output directory and add the path to self
         cwd = os.getcwd()
-        outdir_path = os.path.join(cwd, outdir)
-        create_dir(outdir_path)
-        self.outdir = outdir_path
+        outdir_path = os.path.join(cwd, output_directory)
+        make_dir(outdir_path)
+        self.output_directory_path = outdir_path
 
     @staticmethod
     @njit
-    def _opt2(sampleSmall, scaleFac, target_spec, recIDs, eqIDs, minID, nBig, eq_ID, sampleBig, RecPerEvent):
-        # Optimize based on scaling factor
+    def _find_rec_smallest_sf(sample_small, scale_factors_small, target_spectrum, rec_ids_small, eq_ids_small, min_id, eq_ids_big, sample_big, max_rec_per_event):
+        """
+        Details
+        -------
+        Greedy subset modification to obtain set of records the scaling factors closest to 1
+        The method is defined separately so that njit can be used as wrapper and the routine can be run faster
+
+        Parameters
+        ----------
+        sample_small : numpy.ndarray (2-D)
+            Spectra of the reduced candidate record set (num_records - 1)
+        scale_factors_small : numpy.ndarray (2-D)
+            Scale factors for the reduced candidate record set (num_records - 1)
+        target_spectrum : numpy.ndarray (1-D)
+            Target spectrum (elastic spectrum from the code)
+        rec_ids_small : numpy.ndarray (1-D)
+            Record IDs of the reduced candidate set records in the database
+        eq_ids_small : numpy.ndarray (1-D)
+            Event IDs of the reduced candidate set records in the database
+        min_id : int
+            ID of the eliminated record from candidate record set
+        eq_ids_big : numpy.ndarray (2-D)
+            Event IDs of the records in the filtered database
+        sample_big : numpy.ndarray (2-D)
+            Spectra of the records in the filtered database
+        max_rec_per_event : int
+            The limit for the maximum number of records belong to the same event
+
+        Returns
+        -------
+        min_id : int
+            ID of the new selected record with the scale factor closest to 1
+        scale_factors_small : numpy.ndarray (2-D)
+            Scale factors for the candidate record set (num_records) with the addition of new record
+        """
+
         def mean_numba(a):
+            """
+            Computes the mean of a 2-D array along axis=0.
+            Required for computations since njit is used as wrapper.
+            """
 
             res = []
             for i in range(a.shape[1]):
                 res.append(a[:, i].mean())
 
             return np.array(res)
 
-        for j in range(nBig):
-            tmp = eq_ID[j]
+        for j in range(sample_big.shape[0]):
+            tmp = eq_ids_big[j]
             # record should not be repeated and number of eqs from the same event should not exceed 3
-            if not np.any(recIDs == j) and np.sum(eqIDs == tmp) < RecPerEvent:
+            if not np.any(rec_ids_small == j) and np.sum(eq_ids_small == tmp) < max_rec_per_event:
                 # Add to the sample the scaled spectra
-                temp = np.zeros((1, len(sampleBig[j, :])))
-                temp[:, :] = sampleBig[j, :]  # get the trial spectra
-                tempSample = np.concatenate((sampleSmall, temp), axis=0)  # add the trial spectra to subset list
-                tempScale = np.max(target_spec / mean_numba(tempSample))  # compute new scaling factor
+                temp = np.zeros((1, len(sample_big[j, :])))
+                temp[:, :] = sample_big[j, :]  # get the trial spectra
+                sample_small_trial = np.concatenate((sample_small, temp), axis=0)  # add the trial spectra to subset list
+                temp_scale = np.max(target_spectrum / mean_numba(sample_small_trial))  # compute new scaling factor
 
                 # Should cause improvement
-                if abs(tempScale - 1) <= abs(scaleFac - 1):
-                    minID = j
-                    scaleFac = tempScale
+                if abs(temp_scale - 1) <= abs(scale_factors_small - 1):
+                    min_id = j
+                    scale_factors_small = temp_scale
 
-        return minID, scaleFac
+        return min_id, scale_factors_small
 
-    def tbec2018(self, Lat=41.0582, Long=29.00951, DD=2, SiteClass='ZC', Tp=1):
+    def select_tbec2018(self, lat=41.0582, long=29.00951, dd_level=2, site_class='ZC', predominant_period=1):
         """
         Details
         -------
         Selects the suitable ground motion set in accordance with TBEC 2018. 
         If user did not define any target spectrum, the design spectrum defined by the code is going to be used. 
         The latter requires the definition of site parameters
 
-
         References
         ----------
         TBEC. (2018). Turkish building earthquake code.
 
         Notes
         -----
         Rule 1: Mean of selected records should remain above the lower bound target spectra.
-            For selection = 1: Sa_rec = (Sa_1 or Sa_2) - lower bound = 1.0 * SaTarget(0.2Tp-1.5Tp) 
-            For Selection = 2: Sa_rec = (Sa_1**2+Sa_2**2)**0.5 - lower bound = 1.3 * SaTarget(0.2Tp-1.5Tp) 
+            For num_components = 1: Sa_rec = (Sa_1 or Sa_2) - lower bound = 1.0 * SaTarget(0.2Tp-1.5Tp) 
+            For num_components = 2: Sa_rec = (Sa_1**2+Sa_2**2)**0.5 - lower bound = 1.3 * SaTarget(0.2Tp-1.5Tp) 
 
         Rule 2: 
             No more than 3 records can be selected from the same event! In other words,
-            rec_eqID cannot be the same for more than 3 of the selected records.      
+            rec_eq_id cannot be the same for more than 3 of the selected records.      
 
         Rule 3: 
             At least 11 records (or pairs) must be selected.
 
         Parameters
         ----------
-        Lat: float, optional, the default is 41.0582.
+        lat: float, optional, the default is 41.0582.
             Site latitude
-        Long: float, optional, the default is 29.00951.
+        long: float, optional, the default is 29.00951.
             Site longitude
-        DD:  int, optional, the default is 2.
+        dd_level:  int, optional, the default is 2.
             Earthquake ground motion intensity level (1,2,3,4)
-        SiteClass: str, optional, the default is 'ZC'.
+        site_class: str, optional, the default is 'ZC'.
             Site soil class ('ZA','ZB','ZC','ZD','ZE')
-        Tp : float, optional, the default is 1.
+        predominant_period : float, optional, the default is 1.
             Predominant period of the structure. 
         
         Returns
         -------
         None.
         """
 
         # Add selection settings to self
-        self.Lat = Lat
-        self.Long = Long
-        self.DD = DD
-        self.SiteClass = SiteClass
-        self.Tp = Tp
+        self.lat = lat
+        self.long = long
+        self.dd_level = dd_level
+        self.site_class = site_class
+        self.predominant_period = predominant_period
         self.code = 'TBEC 2018'
 
-        if self.nGM < 11:
-            print('Warning! nGM must be at least 11 according to TBEC 2018. Changing...')
-            self.nGM = 11
-
-        if self.RecPerEvent > 3:
-            print('Warning! Limit for Record Per Event must be at most 3 according to TBEC 2018. Changing...')
-            self.RecPerEvent = 3
+        if self.num_records < 11:
+            print('Warning! Number of requested records must be at least 11 according to TBEC 2018. Changing...')
+            self.num_records = 11
+
+        if self.max_rec_per_event > 3:
+            print('Warning! Limit for record per event must be at most 3 according to TBEC 2018. Changing...')
+            self.max_rec_per_event = 3
 
         # Set the period range
-        self.Tlower = 0.2 * Tp
-        self.Tupper = 1.5 * Tp
+        self.lower_bound_period = 0.2 * predominant_period
+        self.upper_bound_period = 1.5 * predominant_period
 
         # Match periods (periods for error computations)
-        self.T = self.database['Periods']
+        self.periods = self.database['Periods']
 
         # Determine the elastic design spectrum from the user-defined spectrum
         if self.target_path:
             data = np.loadtxt(self.target_path)
-            intfunc = interpolate.interp1d(data[:, 0], data[:, 1], kind='linear', fill_value='extrapolate')
-            target_spec = intfunc(self.T)
+            interp_func = interpolate.interp1d(data[:, 0], data[:, 1], kind='linear', fill_value='extrapolate')
+            target_spectrum = interp_func(self.periods)
 
         # Determine the elastic design spectrum from code
         else:
-            PGA, SDS, SD1, TL = SiteParam_tbec2018(Lat, Long, DD, SiteClass)
-            target_spec, _ = Sae_tbec2018(self.T, SDS, SD1, TL)
+            _, sds, sd1, tl = site_parameters_tbec2018(lat, long, dd_level, site_class)
+            target_spectrum, _ = sae_tbec2018(self.periods, sds, sd1, tl)
 
         # Consider the lower bound spectrum specified by the code as target spectrum
-        if self.selection == 1:
-            target_spec = 1.0 * target_spec
-        elif self.selection == 2:
-            target_spec = 1.3 * target_spec
-            self.Sa_def = 'SRSS'
+        if self.num_components == 1:
+            target_spectrum = 1.0 * target_spectrum
+        elif self.num_components == 2:
+            target_spectrum = 1.3 * target_spectrum
+            self.spectrum_definition = 'SRSS'
 
         # Search the database and filter
-        sampleBig, Vs30, Mw, Rjb, fault, Filename_1, Filename_2, NGA_num, eq_ID_, station_code = self._search_database()
+        sample_big, vs30, mag, rjb, mechanism, filename1, filename2, rsn, eq_ids, station_code = self._search_database()
 
         # Sample size of the filtered database
-        nBig = sampleBig.shape[0]
+        len_big = sample_big.shape[0]
 
         # Scale factors based on mse
-        scaleFac = np.array(
-            np.sum(np.matlib.repmat(target_spec, nBig, 1) * sampleBig, axis=1) / np.sum(sampleBig ** 2, axis=1))
+        scale_factors_big = np.array(np.sum(np.matlib.repmat(target_spectrum, len_big, 1) * sample_big, axis=1) / np.sum(sample_big ** 2, axis=1))
 
         # Find best matches to the target spectrum from ground-motion database
-        temp = (np.matlib.repmat(target_spec, nBig, 1) - sampleBig) ** 2
+        temp = (np.matlib.repmat(target_spectrum, len_big, 1) - sample_big) ** 2
         mse = temp.mean(axis=1)
 
         if self.database['Name'].startswith('ESM'):
-            d = {ni: indi for indi, ni in enumerate(set(eq_ID_.tolist()))}
-            eq_ID = np.asarray([d[ni] for ni in eq_ID_.tolist()])
+            d = {ni: indi for indi, ni in enumerate(set(eq_ids.tolist()))}
+            eq_ids_big = np.asarray([d[ni] for ni in eq_ids.tolist()])
         else:
-            eq_ID = eq_ID_.copy()
+            eq_ids_big = eq_ids.copy()
 
-        recID_sorted = np.argsort(mse)
-        recIDs = np.ones(self.nGM, dtype=int) * (-1)
-        eqIDs = np.ones(self.nGM, dtype=int) * (-1)
+        rec_id_sorted = np.argsort(mse)
+        rec_ids_small = np.ones(self.num_records, dtype=int) * (-1)
+        eq_ids_small = np.ones(self.num_records, dtype=int) * (-1)
         idx1 = 0
         idx2 = 0
-        while idx1 < self.nGM:  # not more than 3 of the records should be from the same event
-            tmp1 = recID_sorted[idx2]
+        while idx1 < self.num_records:  # not more than 3 of the records should be from the same event
+            tmp1 = rec_id_sorted[idx2]
             idx2 += 1
-            tmp2 = eq_ID[tmp1]
-            recIDs[idx1] = tmp1
-            eqIDs[idx1] = tmp2
-            if np.sum(eqIDs == tmp2) <= self.RecPerEvent:
+            tmp2 = eq_ids_big[tmp1]
+            rec_ids_small[idx1] = tmp1
+            eq_ids_small[idx1] = tmp2
+            if np.sum(eq_ids_small == tmp2) <= self.max_rec_per_event:
                 idx1 += 1
 
         # Initial selection results - based on MSE
-        finalScaleFac = scaleFac[recIDs]
-        sampleSmall = sampleBig[recIDs, :]
+        scale_factors_small = scale_factors_big[rec_ids_small]
+        sample_small = sample_big[rec_ids_small, :]
 
         # Must not be lower than target within the period range, find the indicies for this period range
-        idxs = np.where((self.database['Periods'] >= self.Tlower) * (self.database['Periods'] <= self.Tupper))[0]
+        idxs = np.where((self.database['Periods'] >= self.lower_bound_period) * (self.database['Periods'] <= self.upper_bound_period))[0]
 
-        if self.opt == 1:
-            self.rec_scale = finalScaleFac * np.max(
-                target_spec[idxs] / (finalScaleFac.reshape(-1, 1) * sampleSmall[:, idxs]).mean(axis=0))
+        if self.selection_algorithm == 1:
+            self.rec_scale_factors = scale_factors_small * np.max(target_spectrum[idxs] / (scale_factors_small.reshape(-1, 1) * sample_small[:, idxs]).mean(axis=0))
 
         # try to optimize scaling factor to make it closest as possible to 1
-        if self.opt == 2:
-            finalScaleFac = np.max(target_spec[idxs] / sampleSmall[:, idxs].mean(axis=0))
-            for i in range(self.nGM):  # Loop for nGM
+        if self.selection_algorithm == 2:
+            scale_factors_small = np.max(target_spectrum[idxs] / sample_small[:, idxs].mean(axis=0))
+            for i in range(self.num_records):  # Loop for num_records
                 # note the ID of the record which is removed
-                minID = recIDs[i]
-                # remove the i'th record search for a candidate, and consider critical periods for error calculations only
-                sampleSmall_reduced = np.delete(sampleSmall[:, idxs], i, 0)
-                recIDs = np.delete(recIDs, i)
-                eqIDs = np.delete(eqIDs, i)
-                # Try to add a new spectra to the subset list
-                minID, finalScaleFac = self._opt2(sampleSmall_reduced, finalScaleFac, target_spec[idxs], recIDs, eqIDs,
-                                                  minID, nBig, eq_ID, sampleBig[:, idxs], self.RecPerEvent)
+                min_id = rec_ids_small[i]
+                # remove the i'th record search for a candidate
+                sample_small = np.delete(sample_small, i, 0)
+                rec_ids_small = np.delete(rec_ids_small, i)
+                eq_ids_small = np.delete(eq_ids_small, i)
+                # Try to add a new spectra to the subset list and consider critical periods for error calculations only (idxs)
+                min_id, scale_factors_small = self._find_rec_smallest_sf(sample_small[:, idxs], scale_factors_small, target_spectrum[idxs], rec_ids_small, eq_ids_small, min_id, eq_ids_big, sample_big[:, idxs], self.max_rec_per_event)
                 # Add new element in the right slot
-                sampleSmall = np.concatenate(
-                    (sampleSmall[:i, :], sampleBig[minID, :].reshape(1, sampleBig.shape[1]), sampleSmall[i:, :]),
-                    axis=0)
-                recIDs = np.concatenate((recIDs[:i], np.array([minID]), recIDs[i:]))
-                eqIDs = np.concatenate((eqIDs[:i], np.array([eq_ID[minID]]), eqIDs[i:]))
-            self.rec_scale = np.ones(self.nGM) * float(finalScaleFac)
+                sample_small = np.concatenate((sample_small[:i, :], sample_big[min_id, :].reshape(1, sample_big.shape[1]), sample_small[i:, :]), axis=0)
+                rec_ids_small = np.concatenate((rec_ids_small[:i], np.array([min_id]), rec_ids_small[i:]))
+                eq_ids_small = np.concatenate((eq_ids_small[:i], np.array([eq_ids_big[min_id]]), eq_ids_small[i:]))
+            self.rec_scale_factors = np.ones(self.num_records) * float(scale_factors_small)
 
         # check the scaling
-        if np.any(self.rec_scale > self.maxScale) or np.any(self.rec_scale < 1 / self.maxScale):
+        if np.any(self.rec_scale_factors > self.max_scale_factor) or np.any(self.rec_scale_factors< 1 / self.max_scale_factor):
             raise ValueError('Scaling factor criteria is not satisfied',
                              'Please broaden your selection and scaling criteria or change the optimization scheme...')
 
-        recIDs = recIDs.tolist()
+        rec_ids_small = rec_ids_small.tolist()
         # Add selected record information to self
-        self.rec_Vs30 = Vs30[recIDs]
-        self.rec_Rjb = Rjb[recIDs]
-        self.rec_Mw = Mw[recIDs]
-        self.rec_fault = fault[recIDs]
-        self.rec_eqID = eq_ID_[recIDs]
-        self.rec_h1 = Filename_1[recIDs]
+        self.rec_vs30 = vs30[rec_ids_small]
+        self.rec_rjb = rjb[rec_ids_small]
+        self.rec_mag = mag[rec_ids_small]
+        self.rec_mech = mechanism[rec_ids_small]
+        self.rec_eq_id = eq_ids[rec_ids_small]
+        self.rec_file_h1 = filename1[rec_ids_small]
 
-        if self.selection == 2:
-            self.rec_h2 = Filename_2[recIDs]
+        if self.num_components == 2:
+            self.rec_file_h2 = filename2[rec_ids_small]
 
         if self.database['Name'] == 'NGA_W2':
-            self.rec_rsn = NGA_num[recIDs]
+            self.rec_rsn = rsn[rec_ids_small]
 
         if self.database['Name'] == 'ESM_2018':
-            self.rec_station_code = station_code[recIDs]
+            self.rec_station_code = station_code[rec_ids_small]
 
         rec_idxs = []
-        if self.selection == 1:
-            SaKnown = np.append(self.database['Sa_1'], self.database['Sa_2'], axis=0)
-            Filename_1 = np.append(self.database['Filename_1'], self.database['Filename_2'], axis=0)
-            for rec in self.rec_h1:
-                rec_idxs.append(np.where(Filename_1 == rec)[0][0])
-            rec_spec = SaKnown[rec_idxs, :]
-        elif self.selection == 2:
-            for rec in self.rec_h1:
+        if self.num_components == 1:
+            sa_known = np.append(self.database['Sa_1'], self.database['Sa_2'], axis=0)
+            filename1 = np.append(self.database['Filename_1'], self.database['Filename_2'], axis=0)
+            for rec in self.rec_file_h1:
+                rec_idxs.append(np.where(filename1 == rec)[0][0])
+            rec_spec = sa_known[rec_idxs, :]
+        elif self.num_components == 2:
+            for rec in self.rec_file_h1:
                 rec_idxs.append(np.where(self.database['Filename_1'] == rec)[0][0])
-            Sa_1 = self.database['Sa_1'][rec_idxs, :]
-            Sa_2 = self.database['Sa_2'][rec_idxs, :]
-            rec_spec = (Sa_1 ** 2 + Sa_2 ** 2) ** 0.5
+            sa1 = self.database['Sa_1'][rec_idxs, :]
+            sa2 = self.database['Sa_2'][rec_idxs, :]
+            rec_spec = (sa1 ** 2 + sa2 ** 2) ** 0.5
 
         # Save the results for whole spectral range
-        self.rec_spec = rec_spec
-        self.T = self.database['Periods']
+        self.rec_sa_ln = rec_spec
+        self.periods = self.database['Periods']
 
         if self.target_path:
-            self.target = intfunc(self.T)
+            self.target = interp_func(self.periods)
         else:
-            self.target, _ = Sae_tbec2018(self.T, SDS, SD1, TL)
+            self.target, _ = sae_tbec2018(self.periods, sds, sd1, tl)
 
         print('TBEC 2018 based ground motion record selection and amplitude scaling are finished...')
 
-    def asce7_16(self, Lat=34, Long=-118, RiskCat='II', SiteClass='C', T1_small=1, T1_big=1, Tlower=None, Tupper=None):
+    def select_asce7_16(self, lat=34, long=-118, risk_cat='II', site_class='C', fundamental_periods = [1, 1], lower_bound_period=None, upper_bound_period=None):
         """
         Details
         -------
         Selects the suitable ground motion set in accordance with ASCE 7-16. 
         If user did not define any target spectrum, the MCE_R response spectrum defined by the code is going to be used. 
         The latter requires the definition of site parameters.
 
@@ -2666,206 +2802,198 @@
         ----------
         American Society of Civil Engineers. (2017, June). Minimum design loads and associated criteria 
         for buildings and other structures. American Society of Civil Engineers.
 
         Notes
         -----
         Rule 1: Mean of selected records should remain above the lower bound target spectra.
-            For selection = 1: Sa_rec = (Sa_1 or Sa_2) - lower bound = 0.9 * Sa_MCEr(Tlower-Tupper) 
-            For Selection = 2: Sa_rec = RotD100 - lower bound = 0.9 * Sa_MCEr(Tlower-Tupper)     
-            Tlower >= 0.2 * T1_small
-            Tupper >= 1.5 * T1_big
+            For num_components = 1: Sa_rec = (Sa1 or Sa2) - lower bound = 0.9 * Sa_MCEr(Tlower-Tupper)
+            For num_components = 2: Sa_rec = RotD100 - lower bound = 0.9 * Sa_MCEr(Tlower-Tupper)
+            lower_bound_period >= 0.2 * min(fundamental_periods)
+            upper_bound_period >= 1.5 * max(fundamental_periods)
             
         Rule 2: 
             At least 11 records (or pairs) must be selected.
 
         Parameters
         ----------
-        Lat: float, optional, the default is 41.0582.
+        lat : float, optional, the default is 41.0582.
             Site latitude
-        Long: float, optional, the default is 29.00951.
+        long : float, optional, the default is 29.00951.
             Site longitude
-        RiskCat:  str, the default is 'III'
+        risk_category :  str, the default is 'III'
             Risk category for structure ('I','II','III','IV')
-        SiteClass: str, optional, the default is 'C'.
+        site_class : str, optional, the default is 'C'.
             Site soil class ('A','B','C','D','E')
-        T1_small: float, the default is 1.
-            The smallest of first-mode periods in principal horizontal directions
-        T1_big: float, the default is 1.
-            The largest of first-mode periods in principal horizontal directions        
-        Tlower: float, the default is None.
-            The lower bound for period range, if None equal to 0.2*T1_small
-        Tupper: float, the default is None.
-            The upper bound for period range, if None equal to 2.0*T1_big
+        fundamental_periods : list, the default is [1, 1].
+            The first-mode periods in principal horizontal directions     
+        lower_bound_period: float, the default is None.
+            The lower bound for matching period range, if None equal to 0.2*min(fundamental_periods)
+        upper_bound_period: float, the default is None.
+            The upper bound for matching period range, if None equal to 2.0*max(fundamental_periods)
         
         Returns
         -------
         None.
         """
 
         # Add selection settings to self
-        self.Lat = Lat
-        self.Long = Long
-        self.RiskCat = RiskCat
-        self.SiteClass = SiteClass
+        self.lat = lat
+        self.long = long
+        self.risk_category = risk_cat
+        self.site_class = site_class
         self.code = 'ASCE 7-16'
 
         # Section 16.2.3.1
-        if not Tlower:
-            Tlower = 0.2 * T1_small
-        elif Tlower < 0.2 * T1_small:
-            Tlower = 0.2 * T1_small
+        if not lower_bound_period:
+            lower_bound_period = 0.2 * min(fundamental_periods)
+        elif lower_bound_period < 0.2 * min(fundamental_periods):
+            lower_bound_period = 0.2 * min(fundamental_periods)
             print('Warning! Lower bound cannot be lower than 0.2 times the largest first-mode period according to '
                   'ASCE 7-16. Changing...')
-        if not Tupper:
-            Tupper = 2.0 * T1_big
-        elif Tupper < 1.5 * T1_big:
-            Tupper = 1.5 * T1_big
+        if not upper_bound_period:
+            upper_bound_period = 2.0 * max(fundamental_periods)
+        elif upper_bound_period < 1.5 * max(fundamental_periods):
+            upper_bound_period = 1.5 * max(fundamental_periods)
             print('Warning! Upper bound cannot be lower than 1.5 times the smallest first-mode period according to '
                   'ASCE 7-16. Changing...')
-        self.Tlower = Tlower
-        self.Tupper = Tupper
+        self.lower_bound_period = lower_bound_period
+        self.upper_bound_period = upper_bound_period
 
         # Section 16.2.2
-        if self.nGM < 11:
-            print('Warning! nGM must be at least 11 according to ASCE 7-16. Changing...')
-            self.nGM = 11
+        if self.num_records < 11:
+            print('Warning! Number of records must be at least 11 according to ASCE 7-16. Changing...')
+            self.num_records = 11
 
         # Match periods (periods for error computations)
-        self.T = self.database['Periods']
+        self.periods = self.database['Periods']
 
         # Determine the elastic design spectrum from the user-defined spectrum
         if self.target_path:
             data = np.loadtxt(self.target_path)
-            intfunc = interpolate.interp1d(data[:, 0], data[:, 1], kind='linear', fill_value='extrapolate')
-            target_spec = intfunc(self.T)
+            interp_func = interpolate.interp1d(data[:, 0], data[:, 1], kind='linear', fill_value='extrapolate')
+            target_spectrum = interp_func(self.periods)
 
         # Determine the elastic design spectrum from code, Section 16.2.1
         else:
-            SDS, SD1, TL = SiteParam_asce7_16(Lat, Long, RiskCat, SiteClass)  # Retrieve site parameters
-            target_spec = 1.5 * Sae_asce7_16(self.T, SDS, SD1,
-                                             TL)  # Retrive the design spectrum and multiply by 1.5 to get MCER
+            sds, sd1, tl = site_parameters_asce7_16(lat, long, risk_cat, site_class)  # Retrieve site parameters
+            target_spectrum = 1.5 * sae_asce7_16(self.periods, sds, sd1, tl)  # Retrive the design spectrum and multiply by 1.5 to get MCER
 
         # Consider the lower bound spectrum specified by the code as target spectrum, Section 16.2.3.2
-        target_spec = 0.9 * target_spec
-        if self.selection == 2:
-            self.Sa_def = 'RotD100'
+        target_spectrum = 0.9 * target_spectrum
+        if self.num_components == 2:
+            self.spectrum_definition = 'RotD100'
 
             # Search the database and filter
-        sampleBig, Vs30, Mw, Rjb, fault, Filename_1, Filename_2, NGA_num, eq_ID_, station_code = self._search_database()
+        sample_big, vs30, mag, rjb, mechanism, filename1, filename2, rsn, eq_ids, station_code = self._search_database()
 
         # Sample size of the filtered database
-        nBig = sampleBig.shape[0]
+        len_big = sample_big.shape[0]
 
         # Scale factors based on mse
-        scaleFac = np.array(
-            np.sum(np.matlib.repmat(target_spec, nBig, 1) * sampleBig, axis=1) / np.sum(sampleBig ** 2, axis=1))
+        scale_factors_big = np.array(np.sum(np.matlib.repmat(target_spectrum, len_big, 1) * sample_big, axis=1) / np.sum(sample_big ** 2, axis=1))
 
         # Find best matches to the target spectrum from ground-motion database
-        temp = (np.matlib.repmat(target_spec, nBig, 1) - sampleBig) ** 2
+        temp = (np.matlib.repmat(target_spectrum, len_big, 1) - sample_big) ** 2
         mse = temp.mean(axis=1)
 
         if self.database['Name'].startswith('ESM'):
-            d = {ni: indi for indi, ni in enumerate(set(eq_ID_.tolist()))}
-            eq_ID = np.asarray([d[ni] for ni in eq_ID_.tolist()])
+            d = {ni: indi for indi, ni in enumerate(set(eq_ids.tolist()))}
+            eq_ids_big = np.asarray([d[ni] for ni in eq_ids.tolist()])
         else:
-            eq_ID = eq_ID_.copy()
+            eq_ids_big = eq_ids.copy()
 
-        recID_sorted = np.argsort(mse)
-        recIDs = np.ones(self.nGM, dtype=int) * (-1)
-        eqIDs = np.ones(self.nGM, dtype=int) * (-1)
+        rec_id_sorted = np.argsort(mse)
+        rec_ids_small = np.ones(self.num_records, dtype=int) * (-1)
+        eq_ids_small = np.ones(self.num_records, dtype=int) * (-1)
         idx1 = 0
         idx2 = 0
-        while idx1 < self.nGM:  # not more than 3 of the records should be from the same event
-            tmp1 = recID_sorted[idx2]
+        while idx1 < self.num_records:  # not more than 3 of the records should be from the same event
+            tmp1 = rec_id_sorted[idx2]
             idx2 += 1
-            tmp2 = eq_ID[tmp1]
-            recIDs[idx1] = tmp1
-            eqIDs[idx1] = tmp2
-            if np.sum(eqIDs == tmp2) <= self.RecPerEvent:
+            tmp2 = eq_ids_big[tmp1]
+            rec_ids_small[idx1] = tmp1
+            eq_ids_small[idx1] = tmp2
+            if np.sum(eq_ids_small == tmp2) <= self.max_rec_per_event:
                 idx1 += 1
 
         # Initial selection results - based on MSE
-        finalScaleFac = scaleFac[recIDs]
-        sampleSmall = sampleBig[recIDs, :]
+        scale_factors_small = scale_factors_big[rec_ids_small]
+        sample_small = sample_big[rec_ids_small, :]
 
         # Must not be lower than target within the period range, find the indicies for this period range
-        idxs = np.where((self.database['Periods'] >= self.Tlower) * (self.database['Periods'] <= self.Tupper))[0]
+        idxs = np.where((self.database['Periods'] >= self.lower_bound_period) * (self.database['Periods'] <= self.upper_bound_period))[0]
 
-        if self.opt == 1:
-            self.rec_scale = finalScaleFac * np.max(
-                target_spec[idxs] / (finalScaleFac.reshape(-1, 1) * sampleSmall[:, idxs]).mean(axis=0))
+        if self.selection_algorithm == 1:
+            self.rec_scale_factors = scale_factors_small * np.max(target_spectrum[idxs] / (scale_factors_small.reshape(-1, 1) * sample_small[:, idxs]).mean(axis=0))
 
         # try to optimize scaling factor to make it closest as possible to 1
-        if self.opt == 2:
-            finalScaleFac = np.max(target_spec[idxs] / sampleSmall[:, idxs].mean(axis=0))
-            for i in range(self.nGM):  # Loop for nGM
+        if self.selection_algorithm == 2:
+            scale_factors_small = np.max(target_spectrum[idxs] / sample_small[:, idxs].mean(axis=0))
+            for i in range(self.num_records):  # Loop for num_records
                 # note the ID of the record which is removed
-                minID = recIDs[i]
-                # remove the i'th record search for a candidate, and consider critical periods for error calculations only
-                sampleSmall_reduced = np.delete(sampleSmall[:, idxs], i, 0)
-                recIDs = np.delete(recIDs, i)
-                eqIDs = np.delete(eqIDs, i)
-                # Try to add a new spectra to the subset list
-                minID, finalScaleFac = self._opt2(sampleSmall_reduced, finalScaleFac, target_spec[idxs], recIDs, eqIDs,
-                                                  minID, nBig, eq_ID, sampleBig[:, idxs], self.RecPerEvent)
+                min_id = rec_ids_small[i]
+                # remove the i'th record search for a candidate 
+                sample_small = np.delete(sample_small, i, 0)
+                rec_ids_small = np.delete(rec_ids_small, i)
+                eq_ids_small = np.delete(eq_ids_small, i)
+                # Try to add a new spectra to the subset list and consider critical periods for error calculations only (idxs)
+                min_id, scale_factors_small = self._find_rec_smallest_sf(sample_small[:, idxs], scale_factors_small, target_spectrum[idxs], rec_ids_small, eq_ids_small, min_id, eq_ids_big, sample_big[:, idxs], self.max_rec_per_event)
                 # Add new element in the right slot
-                sampleSmall = np.concatenate(
-                    (sampleSmall[:i, :], sampleBig[minID, :].reshape(1, sampleBig.shape[1]), sampleSmall[i:, :]),
-                    axis=0)
-                recIDs = np.concatenate((recIDs[:i], np.array([minID]), recIDs[i:]))
-                eqIDs = np.concatenate((eqIDs[:i], np.array([eq_ID[minID]]), eqIDs[i:]))
-            self.rec_scale = np.ones(self.nGM) * float(finalScaleFac)
+                sample_small = np.concatenate((sample_small[:i, :], sample_big[min_id, :].reshape(1, sample_big.shape[1]), sample_small[i:, :]), axis=0)
+                rec_ids_small = np.concatenate((rec_ids_small[:i], np.array([min_id]), rec_ids_small[i:]))
+                eq_ids_small = np.concatenate((eq_ids_small[:i], np.array([eq_ids_big[min_id]]), eq_ids_small[i:]))
+            self.rec_scale_factors = np.ones(self.num_records) * float(scale_factors_small)
 
         # check the scaling
-        if np.any(self.rec_scale > self.maxScale) or np.any(self.rec_scale < 1 / self.maxScale):
+        if np.any(self.rec_scale_factors > self.max_scale_factor) or np.any(self.rec_scale_factors < 1 / self.max_scale_factor):
             raise ValueError('Scaling factor criteria is not satisfied',
                              'Please broaden your selection and scaling criteria or change the optimization scheme...')
-        recIDs = recIDs.tolist()
+        rec_ids_small = rec_ids_small.tolist()
         # Add selected record information to self
-        self.rec_Vs30 = Vs30[recIDs]
-        self.rec_Rjb = Rjb[recIDs]
-        self.rec_Mw = Mw[recIDs]
-        self.rec_fault = fault[recIDs]
-        self.rec_eqID = eq_ID_[recIDs]
-        self.rec_h1 = Filename_1[recIDs]
+        self.rec_vs30 = vs30[rec_ids_small]
+        self.rec_rjb = rjb[rec_ids_small]
+        self.rec_mag = mag[rec_ids_small]
+        self.rec_mech = mechanism[rec_ids_small]
+        self.rec_eq_id = eq_ids[rec_ids_small]
+        self.rec_file_h1 = filename1[rec_ids_small]
 
-        if self.selection == 2:
-            self.rec_h2 = Filename_2[recIDs]
+        if self.num_components == 2:
+            self.rec_file_h2 = filename2[rec_ids_small]
 
         if self.database['Name'] == 'NGA_W2':
-            self.rec_rsn = NGA_num[recIDs]
+            self.rec_rsn = rsn[rec_ids_small]
 
         if self.database['Name'] == 'ESM_2018':
-            self.rec_station_code = station_code[recIDs]
+            self.rec_station_code = station_code[rec_ids_small]
 
         rec_idxs = []
-        if self.selection == 1:
-            SaKnown = np.append(self.database['Sa_1'], self.database['Sa_2'], axis=0)
-            Filename_1 = np.append(self.database['Filename_1'], self.database['Filename_2'], axis=0)
-            for rec in self.rec_h1:
-                rec_idxs.append(np.where(Filename_1 == rec)[0][0])
-            rec_spec = SaKnown[rec_idxs, :]
-        elif self.selection == 2:
-            for rec in self.rec_h1:
+        if self.num_components == 1:
+            sa_known = np.append(self.database['Sa_1'], self.database['Sa_2'], axis=0)
+            filename1 = np.append(self.database['Filename_1'], self.database['Filename_2'], axis=0)
+            for rec in self.rec_file_h1:
+                rec_idxs.append(np.where(filename1 == rec)[0][0])
+            rec_spec = sa_known[rec_idxs, :]
+        elif self.num_components == 2:
+            for rec in self.rec_file_h1:
                 rec_idxs.append(np.where(self.database['Filename_1'] == rec)[0][0])
             rec_spec = self.database['Sa_RotD100'][rec_idxs, :]
 
         # Save the results for whole spectral range
-        self.rec_spec = rec_spec
-        self.T = self.database['Periods']
+        self.rec_sa_ln = rec_spec
+        self.periods = self.database['Periods']
 
         if self.target_path:
-            self.target = intfunc(self.T)
+            self.target = interp_func(self.periods)
         else:
-            self.target = 1.5 * Sae_asce7_16(self.T, SDS, SD1, TL)
+            self.target = 1.5 * sae_asce7_16(self.periods, sds, sd1, tl)
 
         print('ASCE 7-16 based ground motion record selection and amplitude scaling are finished...')
 
-    def ec8_part1(self, ag=0.2, xi=0.05, ImpClass='II', Type='Type1', SiteClass='C', Tp=1):
+    def select_ec8_part1(self, ag=0.2, xi=0.05, importance_class='II', target_type='Type1', site_class='C', predominant_period=1):
         """
         Details
         -------
         Select the suitable ground motion set in accordance with EC8 - PART 1.
         If user did not define any target spectrum, the design spectrum defined by the code is going to be used. 
         The latter requires the definition of site parameters
 
@@ -2883,172 +3011,167 @@
 
         Rule 2 (b): 
             mean(PGA_rec) >= PGA_target
             Here we assume SA(T[0])=PGA, where T[0] is 0.01 for both record databases.
             Not a bad assumption since it is very close to PGA.
 
         Rule 3 (c): Mean of selected records should remain above the lower bound target spectrum.
-            For selection = 1: Sa_rec = (Sa_1 or Sa_2) - lower bound = 0.9 * SaTarget(0.2Tp-2.0Tp)
-            For Selection = 2: Sa_rec = (Sa_1+Sa_2)*0.5 - lower bound = 0.9 * SaTarget(0.2Tp-2.0Tp)
+            For num_components = 1: Sa_rec = (Sa_1 or Sa_2) - lower bound = 0.9 * SaTarget(0.2Tp-2.0Tp)
+            For num_components = 2: Sa_rec = (Sa_1 + Sa_2) * 0.5 - lower bound = 0.9 * SaTarget(0.2Tp-2.0Tp)
 
         Parameters
         ----------
         ag:  float, optional, the default is 0.25.
             Peak ground acceleration [g]
         xi: float, optional, the default is 0.05.
             Damping
-        ImpClass: str, the default is 'II'.
+        importance_class: str, the default is 'II'.
             Importance class ('I','II','III','IV')
-        Type: str, optional, the default is 'Type1'
+        target_type: str, optional, the default is 'Type1'
             Type of spectrum (Option: 'Type1' or 'Type2')
-        SiteClass: str, optional, the default is 'B'
+        site_class: str, optional, the default is 'B'
             Soil Class (Options: 'A', 'B', 'C', 'D' or 'E')
-        Tp : float, optional, the default is 1.
+        predominant_period : float, optional, the default is 1.
             Predominant period of the structure. 
         
         Returns
         -------
         None.
         """
 
         # Add selection settings to self
-        self.Tp = Tp
+        self.predominant_period = predominant_period
         self.ag = ag
-        self.ImpClass = ImpClass
-        self.Type = Type
-        self.SiteClass = SiteClass
+        self.importance_class = importance_class
+        self.target_type = target_type
+        self.site_class = site_class
         self.code = 'EC8-Part1'
 
         # Set the period range
-        self.Tlower = 0.2 * Tp
-        self.Tupper = 2.0 * Tp
+        self.lower_bound_period = 0.2 * predominant_period
+        self.upper_bound_period = 2.0 * predominant_period
 
         # Match periods (periods for error computations)
-        self.T = self.database['Periods']
+        self.periods = self.database['Periods']
 
         # Determine the elastic design spectrum from the user-defined spectrum
         if self.target_path:
             data = np.loadtxt(self.target_path)
-            func = interpolate.interp1d(data[:, 0], data[:, 1], kind='linear', fill_value='extrapolate')
-            target_spec = func(self.T)
+            interp_funct = interpolate.interp1d(data[:, 0], data[:, 1], kind='linear', fill_value='extrapolate')
+            target_spectrum = interp_funct(self.periods)
 
         # Determine the elastic design spectrum from code
         else:
-            target_spec = Sae_ec8_part1(ag, xi, self.T, ImpClass, Type, SiteClass)
+            target_spectrum = sae_ec8_part1(ag, xi, self.periods, importance_class, target_type, site_class)
 
         # Consider the lower bound spectrum specified by the code as target spectrum
-        target_spec = 0.9 * target_spec  # scale down except for Sa(T[0]) or PGA
-        if self.selection == 2:
-            self.Sa_def = 'ArithmeticMean'
+        target_spectrum = 0.9 * target_spectrum  # scale down except for Sa(T[0]) or PGA
+        if self.num_components == 2:
+            self.spectrum_definition = 'ArithmeticMean'
 
         # Search the database and filter
-        sampleBig, Vs30, Mw, Rjb, fault, Filename_1, Filename_2, NGA_num, eq_ID_, station_code = self._search_database()
+        sample_big, vs30, mag, rjb, mechanism, filename1, filename2, rsn, eq_ids, station_code = self._search_database()
 
         # Sample size of the filtered database
-        nBig = sampleBig.shape[0]
+        len_big = sample_big.shape[0]
 
         # Scale factors based on mse
-        scaleFac = np.array(
-            np.sum(np.matlib.repmat(target_spec, nBig, 1) * sampleBig, axis=1) / np.sum(sampleBig ** 2, axis=1))
+        scale_factors_big = np.array(np.sum(np.matlib.repmat(target_spectrum, len_big, 1) * sample_big, axis=1) / np.sum(sample_big ** 2, axis=1))
 
         # Find best matches to the target spectrum from ground-motion database
-        temp = (np.matlib.repmat(target_spec, nBig, 1) - sampleBig) ** 2
+        temp = (np.matlib.repmat(target_spectrum, len_big, 1) - sample_big) ** 2
         mse = temp.mean(axis=1)
 
         if self.database['Name'].startswith('ESM'):
-            d = {ni: indi for indi, ni in enumerate(set(eq_ID_.tolist()))}
-            eq_ID = np.asarray([d[ni] for ni in eq_ID_.tolist()])
+            d = {ni: indi for indi, ni in enumerate(set(eq_ids.tolist()))}
+            eq_ids_big = np.asarray([d[ni] for ni in eq_ids.tolist()])
         else:
-            eq_ID = eq_ID_.copy()
+            eq_ids_big = eq_ids.copy()
 
-        recID_sorted = np.argsort(mse)
-        recIDs = np.ones(self.nGM, dtype=int) * (-1)
-        eqIDs = np.ones(self.nGM, dtype=int) * (-1)
+        rec_id_sorted = np.argsort(mse)
+        rec_ids_small = np.ones(self.num_records, dtype=int) * (-1)
+        eq_ids_small = np.ones(self.num_records, dtype=int) * (-1)
         idx1 = 0
         idx2 = 0
-        while idx1 < self.nGM:  # not more than 3 of the records should be from the same event
-            tmp1 = recID_sorted[idx2]
+        while idx1 < self.num_records:  # not more than 3 of the records should be from the same event
+            tmp1 = rec_id_sorted[idx2]
             idx2 += 1
-            tmp2 = eq_ID[tmp1]
-            recIDs[idx1] = tmp1
-            eqIDs[idx1] = tmp2
-            if np.sum(eqIDs == tmp2) <= self.RecPerEvent:
+            tmp2 = eq_ids_big[tmp1]
+            rec_ids_small[idx1] = tmp1
+            eq_ids_small[idx1] = tmp2
+            if np.sum(eq_ids_small == tmp2) <= self.max_rec_per_event:
                 idx1 += 1
 
         # Initial selection results - based on MSE
-        finalScaleFac = scaleFac[recIDs]
-        sampleSmall = sampleBig[recIDs, :]
-        target_spec[0] = target_spec[0] / 0.9  # scale up for Sa(T[0]) or PGA
+        scale_factors_small = scale_factors_big[rec_ids_small]
+        sample_small = sample_big[rec_ids_small, :]
+        target_spectrum[0] = target_spectrum[0] / 0.9  # scale up for Sa(T[0]) or PGA
 
         # Must not be lower than target within the period range, find the indicies for this period range
-        idxs = np.where((self.database['Periods'] >= self.Tlower) * (self.database['Periods'] <= self.Tupper))[0]
+        idxs = np.where((self.database['Periods'] >= self.lower_bound_period) * (self.database['Periods'] <= self.upper_bound_period))[0]
         idxs = np.append(0, idxs)  # Add Sa(T=0) or PGA, approximated as Sa(T=0.01)
 
-        if self.opt == 1:
-            self.rec_scale = finalScaleFac * np.max(
-                target_spec[idxs] / (finalScaleFac.reshape(-1, 1) * sampleSmall[:, idxs]).mean(axis=0))
+        if self.selection_algorithm == 1:
+            self.rec_scale_factors = scale_factors_small * np.max(target_spectrum[idxs] / (scale_factors_small.reshape(-1, 1) * sample_small[:, idxs]).mean(axis=0))
 
         # try to optimize scaling factor to make it closest as possible to 1
-        if self.opt == 2:
-            finalScaleFac = np.max(target_spec[idxs] / sampleSmall[:, idxs].mean(axis=0))
-            for i in range(self.nGM):  # Loop for nGM
+        if self.selection_algorithm == 2:
+            scale_factors_small = np.max(target_spectrum[idxs] / sample_small[:, idxs].mean(axis=0))
+            for i in range(self.num_records):  # Loop for num_records
                 # note the ID of the record which is removed
-                minID = recIDs[i]
-                # remove the i'th record search for a candidate, and consider critical periods for error calculations only
-                sampleSmall_reduced = np.delete(sampleSmall[:, idxs], i, 0)
-                recIDs = np.delete(recIDs, i)
-                eqIDs = np.delete(eqIDs, i)
-                # Try to add a new spectra to the subset list
-                minID, finalScaleFac = self._opt2(sampleSmall_reduced, finalScaleFac, target_spec[idxs], recIDs, eqIDs,
-                                                  minID, nBig, eq_ID, sampleBig[:, idxs], self.RecPerEvent)
+                min_id = rec_ids_small[i]
+                # remove the i'th record search for a candidate
+                sample_small = np.delete(sample_small, i, 0)
+                rec_ids_small = np.delete(rec_ids_small, i)
+                eq_ids_small = np.delete(eq_ids_small, i)
+                # Try to add a new spectra to the subset list and consider critical periods for error calculations only (idxs)
+                min_id, scale_factors_small = self._find_rec_smallest_sf(sample_small[:, idxs], scale_factors_small, target_spectrum[idxs], rec_ids_small, eq_ids_small, min_id, eq_ids_big, sample_big[:, idxs], self.max_rec_per_event)
                 # Add new element in the right slot
-                sampleSmall = np.concatenate(
-                    (sampleSmall[:i, :], sampleBig[minID, :].reshape(1, sampleBig.shape[1]), sampleSmall[i:, :]),
-                    axis=0)
-                recIDs = np.concatenate((recIDs[:i], np.array([minID]), recIDs[i:]))
-                eqIDs = np.concatenate((eqIDs[:i], np.array([eq_ID[minID]]), eqIDs[i:]))
-            self.rec_scale = np.ones(self.nGM) * float(finalScaleFac)
+                sample_small = np.concatenate((sample_small[:i, :], sample_big[min_id, :].reshape(1, sample_big.shape[1]), sample_small[i:, :]), axis=0)
+                rec_ids_small = np.concatenate((rec_ids_small[:i], np.array([min_id]), rec_ids_small[i:]))
+                eq_ids_small = np.concatenate((eq_ids_small[:i], np.array([eq_ids_big[min_id]]), eq_ids_small[i:]))
+            self.rec_scale_factors = np.ones(self.num_records) * float(scale_factors_small)
 
         # check the scaling
-        if np.any(self.rec_scale > self.maxScale) or np.any(self.rec_scale < 1 / self.maxScale):
+        if np.any(self.rec_scale_factors > self.max_scale_factor) or np.any(self.rec_scale_factors< 1 / self.max_scale_factor):
             raise ValueError('Scaling factor criteria is not satisfied',
                              'Please broaden your selection and scaling criteria or change the optimization scheme...')
 
-        recIDs = recIDs.tolist()
+        rec_ids_small = rec_ids_small.tolist()
         # Add selected record information to self
-        self.rec_Vs30 = Vs30[recIDs]
-        self.rec_Rjb = Rjb[recIDs]
-        self.rec_Mw = Mw[recIDs]
-        self.rec_fault = fault[recIDs]
-        self.rec_eqID = eq_ID[recIDs]
-        self.rec_h1 = Filename_1[recIDs]
+        self.rec_vs30 = vs30[rec_ids_small]
+        self.rec_rjb = rjb[rec_ids_small]
+        self.rec_mag = mag[rec_ids_small]
+        self.rec_mech = mechanism[rec_ids_small]
+        self.rec_eq_id = eq_ids_big[rec_ids_small]
+        self.rec_file_h1 = filename1[rec_ids_small]
 
-        if self.selection == 2:
-            self.rec_h2 = Filename_2[recIDs]
+        if self.num_components == 2:
+            self.rec_file_h2 = filename2[rec_ids_small]
 
         if self.database['Name'] == 'NGA_W2':
-            self.rec_rsn = NGA_num[recIDs]
+            self.rec_rsn = rsn[rec_ids_small]
 
         if self.database['Name'] == 'ESM_2018':
-            self.rec_station_code = station_code[recIDs]
+            self.rec_station_code = station_code[rec_ids_small]
 
         rec_idxs = []
-        if self.selection == 1:
-            SaKnown = np.append(self.database['Sa_1'], self.database['Sa_2'], axis=0)
-            Filename_1 = np.append(self.database['Filename_1'], self.database['Filename_2'], axis=0)
-            for rec in self.rec_h1:
-                rec_idxs.append(np.where(Filename_1 == rec)[0][0])
-            self.rec_spec = SaKnown[rec_idxs, :]
+        if self.num_components == 1:
+            sa_known = np.append(self.database['Sa_1'], self.database['Sa_2'], axis=0)
+            filename1 = np.append(self.database['Filename_1'], self.database['Filename_2'], axis=0)
+            for rec in self.rec_file_h1:
+                rec_idxs.append(np.where(filename1 == rec)[0][0])
+            self.rec_sa_ln = sa_known[rec_idxs, :]
 
-        elif self.selection == 2:
-            for rec in self.rec_h1:
+        elif self.num_components == 2:
+            for rec in self.rec_file_h1:
                 rec_idxs.append(np.where(self.database['Filename_1'] == rec)[0][0])
-            self.rec_spec = 0.5 * (self.database['Sa_1'][rec_idxs, :] + self.database['Sa_2'][rec_idxs, :])
+            self.rec_sa_ln = 0.5 * (self.database['Sa_1'][rec_idxs, :] + self.database['Sa_2'][rec_idxs, :])
 
         # Save the results for whole spectral range
-        self.T = self.database['Periods']
+        self.periods = self.database['Periods']
         if self.target_path:
-            self.target = func(self.T)
+            self.target = interp_funct(self.periods)
         else:
-            self.target = Sae_ec8_part1(ag, xi, self.T, ImpClass, Type, SiteClass)
+            self.target = sae_ec8_part1(ag, xi, self.periods, importance_class, target_type, site_class)
 
         print('EC8 - Part 1 based ground motion record selection and amplitude scaling are finished...')
```

### Comparing `EzGM-1.6.6.3/EzGM/signal.py` & `EzGM-1.7.0.0/EzGM/signal.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,24 +22,24 @@
         
     References
     ----------
     Kramer, Steven L. 1996. Geotechnical Earthquake Engineering. Prentice Hall.
         
     Parameters
     ----------
-    values: numpy.array
+    values : numpy.ndarray
         Input signal values.
-    dt: float          
+    dt : float          
         Sampling interval.
-    polynomial_type: str
+    polynomial_type : str
         Type of baseline correction 'Constant', 'Linear', 'Quadratic', 'Cubic'.
         
     Returns
     -------
-    values_corrected: numpy.array
+    values_corrected : numpy.ndarray
         Corrected signal values
     """
 
     if polynomial_type == 'Constant':
         n = 0
     elif polynomial_type == 'Linear':
         n = 1
@@ -70,54 +70,54 @@
     elastic and inelastic response spectra, Earthquake Eng. Struct. Dyn. 32, 1729–1748.
     Boore, D. M. (2005). On Pads and Filters: Processing Strong-Motion Data. 
     Bulletin of the Seismological Society of America, 95(2), 745–750. 
     doi: 10.1785/0120040160
 
     Parameters
     ----------
-    values: numpy.array
+    values : numpy.ndarray
         Input signal.
-    dt: float
+    dt : float
         Sampling interval.
-    cut_off: float, tuple, list, numpy.array, optional (The default is (0.1, 25)
+    cut_off : float, tuple, list, numpy.ndarray, optional (The default is (0.1, 25)
         Cut off frequencies for the filter (Hz).
         For lowpass and highpass filters this parameters is a float e.g. 25 or 0.1
         For bandpass or bandstop filters this parameter is a tuple or list e.g. (0.1, 25)
-    filter_type: str, optional (The default is 'lowpass')
+    filter_type : str, optional (The default is 'lowpass')
         The type of filter {'lowpass', 'highpass', 'bandpass', 'bandstop'}.
-    filter_order: int, optional (The default is 4)
+    filter_order : int, optional (The default is 4)
         Order of the Butterworth filter.
-    alpha_window: float, optional (The default is 0.0)
+    alpha_window : float, optional (The default is 0.0)
         Shape parameter of the Tukey window
 
     Returns
     -------
-    values_filtered: numpy.array
+    values_filtered : numpy.ndarray
         Filtered signal values.
     """
 
     if isinstance(cut_off, list) or isinstance(cut_off, tuple):
         cut_off = np.array(cut_off)
 
     sampling_rate = 1.0 / dt  # Sampling rate
     nyq_freq = sampling_rate * 0.5  # Nyquist frequency
     wn = cut_off / nyq_freq  # The critical frequency or frequencies. For lowpass and highpass filters,
-    Lpad = round(len(values) /2)  # Half of signal length
+    pad_length = round(len(values) /2)  # Half of signal length
     w = windows.tukey(len(values), alpha_window)  # This is the window
     values = w * values  # Apply the tapered cosine window
-    values = np.append(np.append(np.zeros(Lpad), values), np.zeros(Lpad))  # Add zero pads to start and end
+    values = np.append(np.append(np.zeros(pad_length), values), np.zeros(pad_length))  # Add zero pads to start and end
     # Wn is a scalar; for bandpass and bandstop filters, Wn is a length-2 sequence.
     b, a = butter(filter_order, wn, filter_type)  # Numerator (b) and denominator (a) polynomials of the IIR filter.
     values = filtfilt(b, a, values)  # Filtering data with an IIR or FIR filter.
-    values_filtered = values[Lpad: -Lpad]  # removing extra zeros
+    values_filtered = values[pad_length: -pad_length]  # removing extra zeros
 
     return values_filtered
 
 
-def sdof_ltha(Ag, dt, T, xi, m=1):
+def sdof_ltha(ag, dt, periods, xi, m=1):
     """
     Details
     -------
     This function carries out linear time history analysis for SDOF system
     It currently uses Newmark Beta Method.
     
     References
@@ -133,65 +133,65 @@
     * Average Acceleration Method: Gamma = 1/2, Beta = 1/4
     * Average acceleration method is unconditionally stable,
       whereas linear acceleration method is stable only if dt/Tn <= 0.55
       Linear acceleration method is preferable due to its accuracy.
     
     Parameters
     ----------
-    Ag: numpy.array    
+    ag : numpy.ndarray    
         Acceleration values.
-    dt: float
+    dt : float
         Time step [sec]
-    T:  float, numpy.array.
+    periods :  float, numpy.ndarray.
         Considered period array e.g. 0 sec, 0.1 sec ... 4 sec.
-    xi: float
+    xi : float
         Damping ratio, e.g. 0.05 for 5%.
-    m:  float
+    m :  float
         Mass of SDOF system.
         
     Returns
     -------
-    u: numpy.array       
+    u : numpy.ndarray       
         Relative displacement response history.
-    v: numpy.array   
+    v : numpy.ndarray   
         Relative velocity response history.
-    ac: numpy.array 
+    ac : numpy.ndarray 
         Relative acceleration response history.
-    ac_tot: numpy.array 
+    ac_tot : numpy.ndarray 
         Total acceleration response history.
     """
 
-    if isinstance(T, (int, float)):
-        T = np.array([T])
-    if isinstance(T, list):
-        T = np.array(T)
-    elif isinstance(T, numpy.ndarray):
-        T = T
+    if isinstance(periods, (int, float)):
+        periods = np.array([periods])
+    if isinstance(periods, list):
+        periods = np.array(periods)
+    elif isinstance(periods, numpy.ndarray):
+        periods = periods
 
     # Get the length of acceleration history array
-    n1 = max(Ag.shape)
+    n1 = max(ag.shape)
     # Get the length of period array
-    n2 = max(T.shape)
-    T = T.reshape((1, n2))
+    n2 = max(periods.shape)
+    periods = periods.reshape((1, n2))
 
     # Assign the external force
-    p = -m * Ag
+    p = -m * ag
 
     # Calculate system properties which depend on period
-    fn = 1 / T  # frequency
+    fn = 1 / periods  # frequency
     wn = 2 * np.pi * fn  # circular natural frequency
     k = m * wn ** 2  # actual stiffness
     c = 2 * m * wn * xi  # actual damping coefficient
 
     # Newmark Beta Method coefficients
     Gamma = np.ones((1, n2)) * (1 / 2)
     # Use linear acceleration method for dt/T<=0.55
     Beta = np.ones((1, n2)) * 1 / 6
     # Use average acceleration method for dt/T>0.55
-    Beta[np.where(dt / T > 0.55)] = 1 / 4
+    Beta[np.where(dt / periods > 0.55)] = 1 / 4
 
     # Compute the constants used in Newmark's integration
     a1 = Gamma / (Beta * dt)
     a2 = 1 / (Beta * dt ** 2)
     a3 = 1 / (Beta * dt)
     a4 = Gamma / Beta
     a5 = 1 / (2 * Beta)
@@ -206,198 +206,198 @@
     ac = np.zeros((n1, n2))  # relative acceleration history
     ac_tot = np.zeros((n1, n2))  # total acceleration history
 
     # Set the Initial Conditions
     u[0] = 0
     v[0] = 0
     ac[0] = (p[0] - c * v[0] - k * u[0]) / m
-    ac_tot[0] = ac[0] + Ag[0]
+    ac_tot[0] = ac[0] + ag[0]
 
     for i in range(n1 - 1):
         dpf = (p[i + 1] - p[i]) + a * v[i] + b * ac[i]
         du = dpf / kf
         dv = a1 * du - a4 * v[i] - a6 * ac[i]
         da = a2 * du - a3 * v[i] - a5 * ac[i]
 
         # Update history variables
         u[i + 1] = u[i] + du
         v[i + 1] = v[i] + dv
         ac[i + 1] = ac[i] + da
-        ac_tot[i + 1] = ac[i + 1] + Ag[i + 1]
+        ac_tot[i + 1] = ac[i + 1] + ag[i + 1]
 
     return u, v, ac, ac_tot
 
 
-def get_parameters(Ag, dt, T, xi):
+def get_parameters(ag, dt, periods, xi):
     """
     Details
     -------
     This function computes various ground motion parameters or intensity measures for a given record.
         
     References
     ---------- 
     Kramer, Steven L. 1996. Geotechnical Earthquake Engineering, Prentice Hall
     Chopra, A.K. 2012. Dynamics of Structures: Theory and 
     Applications to Earthquake Engineering, Prentice Hall.
         
     Parameters
     ----------
-    Ag: numpy.array    
+    ag : numpy.ndarray    
         Acceleration values [m/s2].
-    dt: float
+    dt : float
         Time step [sec]
-    T:  float, numpy.array.
+    periods :  float, numpy.ndarray.
         Considered period array e.g. 0 sec, 0.1 sec ... 4 sec.
-    xi: float
+    xi : float
         Damping ratio, e.g. 0.05 for 5%.
         
     Returns
     -------
-    param: dictionary
-        Contains the following intensity measures:
-        PSa: numpy.array
+    param : dictionary
+        Contains the following intensity measures (keys as strings):
+        PSa : numpy.ndarray
             Elastic pseudo-acceleration response spectrum [m/s2].
-        PSv: numpy.array
+        PSv : numpy.ndarray
             Elastic pseudo-velocity response spectrum [m/s].
-        Sd: numpy.array
+        Sd : numpy.ndarray
             Elastic relative displacement response spectrum [m].
-        Sv: numpy.array
+        Sv : numpy.ndarray
             Elastic relative velocity response spectrum [m/s].
-        Sa_r: numpy.array
+        Sa_r : numpy.ndarray
             Elastic relative acceleration response spectrum [m/s2].
-        Sa_a: numpy.array
+        Sa_a : numpy.ndarray
             Elastic absolute acceleration response spectrum [m/s2].
-        Ei_r: numpy.array
+        Ei_r : numpy.ndarray
             Relative input energy spectrum for elastic system [N.m].
-        Ei_a: numpy.array
+        Ei_a : numpy.ndarray
             Absolute input energy spectrum for elastic system [N.m].
-        Periods: numpy.array 
+        Periods : numpy.ndarray 
             Periods where spectral values are calculated [sec].
-        FAS: numpy.array 
+        FAS : numpy.ndarray 
             Fourier amplitude spectra.
-        PAS: numpy.array 
+        PAS : numpy.ndarray 
             Power amplitude spectra.
-        PGA: float
+        PGA : float
             Peak ground acceleration [m/s2].
-        PGV: float
+        PGV : float
             Peak ground velocity [m/s].
-        PGD: float
+        PGD : float
             Peak ground displacement [m].
-        Aint: numpy.array 
+        Aint : numpy.ndarray 
             Arias intensity ratio vector with time [m/s].
-        Arias: float 
+        Arias : float 
             Maximum value of arias intensity ratio [m/s].
-        HI: float
+        HI : float
             Housner intensity ratio [m].
             Requires T to be defined between (0.1-2.5 sec), otherwise not applicable, and equal to -1.
-        CAV: float
+        CAV : float
             Cumulative absolute velocity [m/s]        
-        t_5_75: list
+        t_5_75 : list
             Significant duration time vector between 5% and 75% of energy release (from Aint).
-        D_5_75: float
+        D_5_75 : float
             Significant duration between 5% and 75% of energy release (from Aint).
-        t_5_95: list    
+        t_5_95 : list    
             Significant duration time vector between 5% and 95% of energy release (from Aint).
-        D_5_95: float
+        D_5_95 : float
             Significant duration between 5% and 95% of energy release (from Aint).
-        t_bracketed: list 
+        t_bracketed : list 
             Bracketed duration time vector (acc>0.05g).
             Not applicable, in case of low intensity records, thus, equal to -1.
-        D_bracketed: float
+        D_bracketed : float
             Bracketed duration (acc>0.05g)
         t_uniform: list 
             Uniform duration time vector (acc>0.05g)
             Not applicable, in case of low intensity records, thus, equal to -1.
-        D_uniform: float 
+        D_uniform : float 
             Uniform duration (acc>0.05g)
-        Tm: float
+        Tm : float
             Mean period.
-        Tp: float             
+        Tp : float             
             Predominant Period.
-        aRMS: float 
+        aRMS : float 
             Root mean square root of acceleration [m/s2].
-        vRMS: float
+        vRMS : float
             Root mean square root of velocity [m/s].
-        dRMS: float  
+        dRMS : float  
             Root mean square root of displacement [m].
-        Ic: float
+        Ic : float
             Characteristic intensity.
             End time might which is used herein, is not always a good choice.
-        ASI: float   
+        ASI : float   
             Acceleration spectrum intensity [m/s].
             Requires T to be defined between (0.1-0.5 sec), otherwise not applicable, and equal to -1.
-        MASI: float 
+        MASI : float 
             Modified acceleration spectrum intensity [m].
             Requires T to be defined between (0.1-2.5 sec), otherwise not applicable, and equal to -1.
-        VSI: float
+        VSI : float
             Velocity spectrum intensity [m].
             Requires T to be defined between (0.1-2.5 sec), otherwise not applicable, and equal to -1.
-        VSI: float
+        VSI : float
             Velocity spectrum intensity [m].
             Requires T to be defined between (0.1-2.5 sec), otherwise not applicable, and equal to -1.
     """
     # TODO: there are bunch of other IMs which can be computed. Add them here.
 
     g = 9.81
 
-    if isinstance(T, (int, float)):
-        T = np.array([T])
-    if isinstance(T, list):
-        T = np.array(T)
-    elif isinstance(T, numpy.ndarray):
-        T = T
+    if isinstance(periods, (int, float)):
+        periods = np.array([periods])
+    if isinstance(periods, list):
+        periods = np.array(periods)
+    elif isinstance(periods, numpy.ndarray):
+        periods = periods
 
     # INITIALIZATION
-    T = T[T != 0]  # do not use T = zero for response spectrum calculations
-    param = {'Periods': T}
+    periods = periods[periods != 0]  # do not use T = zero for response spectrum calculations
+    param = {'Periods': periods}
 
     # GET SPECTRAL VALUES
     # Get the length of acceleration history array
-    n1 = max(Ag.shape)
+    n1 = max(ag.shape)
     # Get the length of period array
-    n2 = max(T.shape)
+    n2 = max(periods.shape)
     # Create the time array
     t = dt * np.arange(0, n1, 1)
     # Get ground velocity and displacement through integration
-    Vg = cumtrapz(Ag, t, initial=0)
-    Dg = cumtrapz(Vg, t, initial=0)
+    vg = cumtrapz(ag, t, initial=0)
+    dg = cumtrapz(vg, t, initial=0)
     # Mass (kg)
     m = 1
     # Carry out linear time history analyses for SDOF system
-    u, v, ac, ac_tot = sdof_ltha(Ag, dt, T, xi, m)
+    u, v, ac, ac_tot = sdof_ltha(ag, dt, periods, xi, m)
     # Calculate the spectral values
     param['Sd'] = np.max(np.abs(u), axis=0)
     param['Sv'] = np.max(np.abs(v), axis=0)
     param['Sa_r'] = np.max(np.abs(ac), axis=0)
     param['Sa_a'] = np.max(np.abs(ac_tot), axis=0)
-    param['PSv'] = (2 * np.pi / T) * param['Sd']
-    param['PSa'] = ((2 * np.pi / T) ** 2) * param['Sd']
-    ei_r = cumtrapz(-numpy.matlib.repmat(Ag, n2, 1).T, u, axis=0, initial=0) * m
-    ei_a = cumtrapz(-numpy.matlib.repmat(Dg, n2, 1).T, ac_tot, axis=0, initial=0) * m
+    param['PSv'] = (2 * np.pi / periods) * param['Sd']
+    param['PSa'] = ((2 * np.pi / periods) ** 2) * param['Sd']
+    ei_r = cumtrapz(-numpy.matlib.repmat(ag, n2, 1).T, u, axis=0, initial=0) * m
+    ei_a = cumtrapz(-numpy.matlib.repmat(dg, n2, 1).T, ac_tot, axis=0, initial=0) * m
     param['Ei_r'] = ei_r[-1]
     param['Ei_a'] = ei_a[-1]
 
     # GET PEAK GROUND ACCELERATION, VELOCITY AND DISPLACEMENT
-    param['PGA'] = np.max(np.abs(Ag))
-    param['PGV'] = np.max(np.abs(Vg))
-    param['PGD'] = np.max(np.abs(Dg))
+    param['PGA'] = np.max(np.abs(ag))
+    param['PGV'] = np.max(np.abs(vg))
+    param['PGD'] = np.max(np.abs(dg))
 
     # GET ARIAS INTENSITY
-    Aint = np.cumsum(Ag ** 2) * np.pi * dt / (2 * g)
+    Aint = np.cumsum(ag ** 2) * np.pi * dt / (2 * g)
     param['Arias'] = Aint[-1]
     temp = np.zeros((len(Aint), 2))
     temp[:, 0] = t
     temp[:, 1] = Aint
     param['Aint'] = temp
 
     # GET HOUSNER INTENSITY
     try:
-        index1 = np.where(T == 0.1)[0][0]
-        index2 = np.where(T == 2.5)[0][0]
-        param['HI'] = np.trapz(param['PSv'][index1:index2], T[index1:index2])
+        index1 = np.where(periods == 0.1)[0][0]
+        index2 = np.where(periods == 2.5)[0][0]
+        param['HI'] = np.trapz(param['PSv'][index1:index2], periods[index1:index2])
     except:
         param['HI'] = -1
 
     # SIGNIFICANT DURATION (5%-75% Ia)
     mask = (Aint >= 0.05 * Aint[-1]) * (Aint <= 0.75 * Aint[-1])
     timed = t[mask]
     t1 = round(timed[0], 3)
@@ -411,96 +411,96 @@
     t1 = round(timed[0], 3)
     t2 = round(timed[-1], 3)
     param['t_5_95'] = [t1, t2]
     param['D_5_95'] = round(t2 - t1, 3)
 
     # BRACKETED DURATION (0.05g)
     try:
-        mask = np.abs(Ag) >= 0.05 * g
+        mask = np.abs(ag) >= 0.05 * g
         # mask = np.abs(Ag) >= 0.05 * np.max(np.abs(Ag))
         indices = np.where(mask)[0]
         t1 = round(t[indices[0]], 3)
         t2 = round(t[indices[-1]], 3)
         param['t_bracketed'] = [t1, t2]
         param['D_bracketed'] = round(t2 - t1, 3)
     except:  # in case of ground motions with low intensities
         param['t_bracketed'] = -1
         param['D_bracketed'] = 0
 
     # UNIFORM DURATION (0.05g)
     try:
-        mask = np.abs(Ag) >= 0.05 * g
+        mask = np.abs(ag) >= 0.05 * g
         # mask = np.abs(Ag) >= 0.05 * np.max(np.abs(Ag))
         indices = np.where(mask)[0]
         t_treshold = t[indices]
         param['t_uniform'] = [t_treshold]
         temp = np.round(np.diff(t_treshold), 8)
         param['D_uniform'] = round(np.sum(temp[temp == dt]), 3)
     except:  # in case of ground motions with low intensities
         param['t_uniform'] = -1
         param['D_uniform'] = 0
 
     # CUMULATVE ABSOLUTE VELOCITY
-    param['CAV'] = np.trapz(np.abs(Ag), t)
+    param['CAV'] = np.trapz(np.abs(ag), t)
 
     # CHARACTERISTIC INTENSITY, ROOT MEAN SQUARE OF ACC, VEL, DISP
     Td = t[-1]  # note this might not be the best indicative, different Td might be chosen
-    param['aRMS'] = np.sqrt(np.trapz(Ag ** 2, t) / Td)
-    param['vRMS'] = np.sqrt(np.trapz(Vg ** 2, t) / Td)
-    param['dRMS'] = np.sqrt(np.trapz(Dg ** 2, t) / Td)
+    param['aRMS'] = np.sqrt(np.trapz(ag ** 2, t) / Td)
+    param['vRMS'] = np.sqrt(np.trapz(vg ** 2, t) / Td)
+    param['dRMS'] = np.sqrt(np.trapz(dg ** 2, t) / Td)
     param['Ic'] = param['aRMS'] ** 1.5 * np.sqrt(Td)
 
     # ACCELERATION AND VELOCITY SPECTRUM INTENSITY
     try:
-        index3 = np.where(T == 0.5)[0][0]
-        param['ASI'] = np.trapz(param['PSa'][index1:index3], T[index1:index3])
+        index3 = np.where(periods == 0.5)[0][0]
+        param['ASI'] = np.trapz(param['PSa'][index1:index3], periods[index1:index3])
     except:
         param['ASI'] = -1
     try:
-        param['MASI'] = np.trapz(param['PSa'][index1:index2], T[index1:index2])
-        param['VSI'] = np.trapz(param['PSv'][index1:index2], T[index1:index2])
+        param['MASI'] = np.trapz(param['PSa'][index1:index2], periods[index1:index2])
+        param['VSI'] = np.trapz(param['PSv'][index1:index2], periods[index1:index2])
     except:
         param['MASI'] = -1
         param['VSI'] = -1
 
     # GET FOURIER AMPLITUDE AND POWER AMPLITUDE SPECTRUM
     # Number of sample points, add zeropads
-    N = 2 ** int(np.ceil(np.log2(len(Ag))))
-    Famp = fft(Ag, N)
-    Famp = np.abs(fftshift(Famp)) * dt
-    freq = fftfreq(N, dt)
+    freq_len = 2 ** int(np.ceil(np.log2(len(ag))))
+    famp = fft(ag, freq_len)
+    famp = np.abs(fftshift(famp)) * dt
+    freq = fftfreq(freq_len, dt)
     freq = fftshift(freq)
-    Famp = Famp[freq > 0]
+    famp = famp[freq > 0]
     freq = freq[freq > 0]
-    Pamp = Famp ** 2 / (np.pi * t[-1] * param['aRMS'] ** 2)
-    FAS = np.zeros((len(Famp), 2))
-    FAS[:, 0] = freq
-    FAS[:, 1] = Famp
-    PAS = np.zeros((len(Famp), 2))
-    PAS[:, 0] = freq
-    PAS[:, 1] = Pamp
-    param['FAS'] = FAS
-    param['PAS'] = FAS
+    pamp = famp ** 2 / (np.pi * t[-1] * param['aRMS'] ** 2)
+    fas = np.zeros((len(famp), 2))
+    fas[:, 0] = freq
+    fas[:, 1] = famp
+    pas = np.zeros((len(famp), 2))
+    pas[:, 0] = freq
+    pas[:, 1] = pamp
+    param['FAS'] = fas
+    param['PAS'] = fas
 
     # MEAN PERIOD
     mask = (freq > 0.25) * (freq < 20)
     indices = np.where(mask)[0]
     fi = freq[indices]
-    Ci = Famp[indices]
+    Ci = famp[indices]
     param['Tm'] = np.sum(Ci ** 2 / fi) / np.sum(Ci ** 2)
 
     # PREDOMINANT PERIOD
     mask = param['PSa'] == max(param['PSa'])
     indices = np.where(mask)[0]
-    param['Tp'] = T[indices]
+    param['Tp'] = periods[indices]
 
     return param
 
 
-def RotDxx_spectrum(Ag1, Ag2, dt, T, xi, xx):
+def get_sa_rotdxx(ag1, ag2, dt, periods, xi, xx):
     """
     Details
     -------
     This function computes RotDxx spectrum. It currently uses Newmark Beta Method.
     
     References
     ---------- 
@@ -508,125 +508,124 @@
     Bulletin of the Seismological Society of America, 96(4A), 1502–1511.
     Boore, D. M. (2010). Orientation-Independent, Nongeometric-Mean Measures 
     of Seismic Intensity from Two Horizontal Components of Motion. 
     Bulletin of the Seismological Society of America, 100(4), 1830–1835.
         
     Parameters
     ----------
-    Ag1: numpy.array    
+    ag1: numpy.ndarray    
          Acceleration values of 1st horizontal ground motion component.
-    Ag2: numpy.array    
+    ag2: numpy.ndarray    
          Acceleration values of 2nd horizontal ground motion component.
     dt:  float
          Time step [sec].
-    T:   float, numpy.array
+    periods:   float, numpy.ndarray
          Considered period array e.g. 0 sec, 0.1 sec ... 4 sec.
     xi:  float
          Damping ratio, e.g. 0.05 for 5%.
     xx:  int, list
          Percentile to calculate, e.g. 50 for RotD50.
         
     Returns
     -------
-    Sa_RotDxx: numpy.array 
+    Sa_RotDxx: numpy.ndarray 
         RotDxx Spectra.
     """
 
-    if isinstance(T, (int, float)):
-        T = np.array([T])
-    if isinstance(T, list):
-        T = np.array(T)
-    elif isinstance(T, numpy.ndarray):
-        T = T
+    if isinstance(periods, (int, float)):
+        periods = np.array([periods])
+    if isinstance(periods, list):
+        periods = np.array(periods)
+    elif isinstance(periods, numpy.ndarray):
+        periods = periods
 
-    T = T[T != 0]  # do not use T = zero for response spectrum calculations
+    periods = periods[periods != 0]  # do not use T = zero for response spectrum calculations
 
     # Verify if the length of arrays are the same
-    if len(Ag1) == len(Ag2):
+    if len(ag1) == len(ag2):
         pass
-    elif len(Ag1) > len(Ag2):
-        Ag2 = np.append(Ag2, np.zeros(len(Ag1) - len(Ag2)))
-    elif len(Ag2) > len(Ag1):
-        Ag1 = np.append(Ag1, np.zeros(len(Ag2) - len(Ag1)))
+    elif len(ag1) > len(ag2):
+        ag2 = np.append(ag2, np.zeros(len(ag1) - len(ag2)))
+    elif len(ag2) > len(ag1):
+        ag1 = np.append(ag1, np.zeros(len(ag2) - len(ag1)))
 
     # Get the length of period array 
-    n2 = max(T.shape)
+    n2 = max(periods.shape)
 
     # Mass (kg)
     m = 1
 
     # Carry out linear time history analyses for SDOF system
-    u1, _, _, _ = sdof_ltha(Ag1, dt, T, xi, m)
-    u2, _, _, _ = sdof_ltha(Ag2, dt, T, xi, m)
+    u1, _, _, _ = sdof_ltha(ag1, dt, periods, xi, m)
+    u2, _, _, _ = sdof_ltha(ag2, dt, periods, xi, m)
 
     # RotD definition is taken from Boore 2010.
-    Rot_Disp = np.zeros((180, n2))
+    rot_disp = np.zeros((180, n2))
     for theta in range(0, 180, 1):
-        Rot_Disp[theta] = np.max(np.abs(u1 * np.cos(np.deg2rad(theta)) + u2 * np.sin(np.deg2rad(theta))), axis=0)
+        rot_disp[theta] = np.max(np.abs(u1 * np.cos(np.deg2rad(theta)) + u2 * np.sin(np.deg2rad(theta))), axis=0)
 
     # Pseudo-acceleration
-    Rot_Acc = Rot_Disp * (2 * np.pi / T) ** 2
+    rot_acc = rot_disp * (2 * np.pi / periods) ** 2
     if isinstance(xx, list):
-        Sa_RotDxx = [np.percentile(Rot_Acc, value, axis=0) for value in xx]
+        Sa_RotDxx = [np.percentile(rot_acc, value, axis=0) for value in xx]
     else:
-        Sa_RotDxx = np.percentile(Rot_Acc, xx, axis=0)
-    Periods = T
+        Sa_RotDxx = np.percentile(rot_acc, xx, axis=0)
 
-    return Periods, Sa_RotDxx
+    return periods, Sa_RotDxx
 
-def get_fiv3(Ag, dt, T, alpha = 0.7, beta = 0.85):
+def get_fiv3(ag, dt, periods, alpha = 0.7, beta = 0.85):
     """
     Details
     -------
     This function computes the filtered incremental velocity for a ground motion
 
     References
     ----------
     Dávalos H, Miranda E. Filtered incremental velocity: A novel approach in intensity measures for seismic collapse estimation. 
     Earthquake Engineering & Structural Dynamics 2019; 48(12): 1384-1405. DOI: 10.1002/eqe.3205.
 
     Parameters
     ----------
-    Ag: numpy.array    
+    ag: numpy.ndarray    
         Acceleration values.
     dt: float
         Time step [sec]
-    T:  float, numpy.array.
+    periods:  float, numpy.ndarray.
         Considered period array e.g. 0 sec, 0.1 sec ... 4 sec.
     alpha : float
         Period factor, by default 0.7
     beta : float
         Cut-off frequency factor, by default 0.85
 
     Returns
     ----------
-    fiv3: numpy.array 
+    fiv3: numpy.ndarray 
         filtered incremental velocity, FIV3 as per Eq. (3) of Davalos and Miranda (2019)
     """
     
-    if isinstance(T, (int, float)):
-        T = np.array([T])
-    if isinstance(T, list):
-        T = np.array(T)
-    elif isinstance(T, numpy.ndarray):
-        T = T
+    if isinstance(periods, (int, float)):
+        periods = np.array([periods])
+    if isinstance(periods, list):
+        periods = np.array(periods)
+    elif isinstance(periods, numpy.ndarray):
+        periods = periods
 
-    T = T[T != 0]  # do not use T = zero for response spectrum calculations
+    periods = periods[periods != 0]  # do not use T = zero for response spectrum calculations
 
     # Time series of the signal
-    t = dt * np.arange(0, len(Ag), 1)
+    t = dt * np.arange(0, len(ag), 1)
 
     # FIV3 array
     fiv3 = []
 
     # apply a 2nd order Butterworth low pass filter to the ground motion
-    for tn in T:
+    for tn in periods:
         wn = beta / tn / (0.5 / dt)
         b, a = butter(2, wn, 'lowpass')
-        ugf = filtfilt(b, a, Ag)
+        ugf = filtfilt(b, a, ag)
 
         # filtered incremental velocity (FIV)
         ugf_pc = np.zeros(
             (np.sum(t < t[-1] - alpha * tn), int(np.floor(alpha * tn / dt))))
         for i in range(int(np.floor(alpha * tn / dt))):
             ugf_pc[:, i] = ugf[np.where(t < t[-1] - alpha * tn)[0] + i]
```

### Comparing `EzGM-1.6.6.3/EzGM/utility.py` & `EzGM-1.7.0.0/EzGM/utility.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,26 @@
 from matplotlib import cm
 from matplotlib.patches import Patch
 import requests
 import json
 from openquake.hazardlib import gsim, nrml
 from openquake.baselib.node import Node
 
+SMALL_SIZE = 15
+MEDIUM_SIZE = 16
+BIG_SIZE = 18
+BIGGER_SIZE = 20
+
+plt.rc('font', size=SMALL_SIZE)  # controls default text sizes
+plt.rc('axes', titlesize=SMALL_SIZE)  # fontsize of the axes title
+plt.rc('axes', labelsize=BIG_SIZE)  # fontsize of the x and y labels
+plt.rc('xtick', labelsize=SMALL_SIZE)  # fontsize of the tick labels
+plt.rc('ytick', labelsize=SMALL_SIZE)  # fontsize of the tick labels
+plt.rc('legend', fontsize=MEDIUM_SIZE)  # legend fontsize
+plt.rc('figure', titlesize=BIGGER_SIZE)  # fontsize of the figure title
 
 # FUNCTIONS TO POST-PROCESS OPENQUAKE PSHA RESULTS
 # ---------------------------------------------------------------------
 
 def hazard_curve(poes, path_hazard_results, output_dir='Post_Outputs', filename='hazard_curve-mean', show=1):
     """
     Details
@@ -44,15 +56,15 @@
         Probabilities of exceedance in tw years for which im levels will be obtained.
     path_hazard_results: str
         Path to the hazard results.
     output_dir: str, optional
         Save outputs to a pickle file.
     filename : str, optional
         filename to process.
-    show: int
+    show : int
         flag to show figure (1 or 0)
 
     Returns
     -------
     None.
     """
 
@@ -146,35 +158,35 @@
         imls = np.asarray(iml_data[i])
         imls.shape = (len(imls), 1)
         haz_cur = np.concatenate([imls, poe], axis=1)
         fname = os.path.join(output_dir, 'HazardCurve_' + im[i] + '.out')
         np.savetxt(fname, haz_cur)
 
 
-def disagg_MR(Mbin, dbin, path_disagg_results, output_dir='Post_Outputs', n_rows=1, filename='Mag_Dist', show=1):
+def disaggregation_mag_dist(mag_bin, dist_bin, path_disagg_results, output_dir='Post_Outputs', num_rows=1, filename='Mag_Dist', show=1):
     """
     Details
     -------
     This script will save disaggregation plots including M and R.
 
     Parameters
     ----------
-    Mbin : int, float
+    mag_bin : int, float
         magnitude bin used in disaggregation.
-    dbin : int, float
+    dist_bin : int, float
         distance bin used in disaggregation.
     path_disagg_results: str
         Path to the disaggregation results.
     output_dir: str, optional
         Save outputs to a pickle file.
-    n_rows : int, optional
+    num_rows : int, optional
         total number of rows for subplots.
     filename : str, optional
         filename to process.
-    show: int
+    show : int
         flag to show figure (1 or 0)
 
     Returns
     -------
     None.
     """
 
@@ -194,84 +206,84 @@
             f = open(''.join([path_disagg_results, '/', file]), "r")
             ff = f.readline().split(',')
             lon = float(list(filter(lambda x: 'lon=' in x, ff))[0].replace(" lon=", ""))
             lat = float(list(filter(lambda x: 'lat=' in x, ff))[0].replace(" lat=", "").replace("\"\n", ""))
             inv_t = float(list(filter(lambda x: 'investigation_time=' in x, ff))[0].replace(" investigation_time=", ""))
             ims = np.unique(df['imt'])
             for imt in ims:
-                M, R = [], []
+                mag, dist = [], []
                 hz_cont = []
-                Tr = []
+                return_period = []
                 modeLst, meanLst = [], []
                 for poe in poes:
-                    Tr.append(round(-inv_t / np.log(1 - poe)))
+                    return_period.append(round(-inv_t / np.log(1 - poe)))
                     data = {}
                     data['mag'] = df['mag'][(df['poe'] == poe) & (df['imt'] == imt)]
                     data['dist'] = df['dist'][(df['poe'] == poe) & (df['imt'] == imt)]
                     data['hz_cont'] = df[hz_key][(df['poe'] == poe) & (df['imt'] == imt)]
                     hz_cont.append(data['hz_cont'] / data['hz_cont'].sum())
                     data['hz_cont'] = hz_cont[-1]
                     data = pd.DataFrame(data)
                     # Compute the modal values (highest hazard contribution)
                     mode = data.sort_values(by='hz_cont', ascending=False)[0:1]
                     modeLst.append([mode['mag'].values[0], mode['dist'].values[0]])
                     # Compute the mean value
                     meanLst.append([np.sum(data['mag'] * data['hz_cont']), np.sum(data['dist'] * data['hz_cont'])])
 
                     # Report the individual magnitude and distance bins
-                    M.append(data['mag'])
-                    R.append(data['dist'])
+                    mag.append(data['mag'])
+                    dist.append(data['dist'])
 
-                n_Tr = len(Tr)
+                len_return_period = len(return_period)
                 mean_mags = []
                 mean_dists = []
                 mod_mags = []
                 mod_dists = []
 
-                n_cols = int(np.floor(n_Tr / n_rows))
-                if np.mod(n_Tr, n_rows):
-                    n_cols += 1
+                num_cols = int(np.floor(len_return_period / num_rows))
+                if np.mod(len_return_period, num_rows):
+                    num_cols += 1
 
                 fig = plt.figure(figsize=(19.2, 10.8))
-                for i in range(n_Tr):
+                for i in range(len_return_period):
                     # Save disaggregation results
-                    disagg_results = np.array([M[i], R[i], hz_cont[i]]).T
+                    disagg_results = np.array([mag[i], dist[i], hz_cont[i]]).T
                     disagg_results = disagg_results[disagg_results[:,2] != 0]
                     fname = os.path.join(output_dir, 'MagDist_poe_' + str(poes[i]) + '_' + imt + '.out')
                     np.savetxt(fname, disagg_results)
 
-                    ax1 = fig.add_subplot(n_rows, n_cols, i + 1, projection='3d')
+                    ax1 = fig.add_subplot(num_rows, num_cols, i + 1, projection='3d')
 
-                    X = R[i]
-                    Y = M[i]
-                    Z = np.zeros(len(X))
+                    x = dist[i]
+                    y = mag[i]
+                    z = np.zeros(len(x))
 
-                    dx = np.ones(len(X)) * dbin / 2
-                    dy = np.ones(len(Y)) * Mbin / 2
+                    dx = np.ones(len(x)) * dist_bin / 2
+                    dy = np.ones(len(y)) * mag_bin / 2
                     dz = hz_cont[i] * 100
 
                     # here we may make the colormap based on epsilon instead of hazard contribution
                     max_height = np.max(dz)  # get range of color bars so we can normalize
                     min_height = np.min(dz)
                     # scale each z to [0,1], and get their rgb values
                     rgba = [cmap((k - min_height) / max_height) for k in dz]
-                    ax1.bar3d(X, Y, Z, dx, dy, dz, color=rgba, zsort='average', alpha=0.7, shade=True)
+                    ax1.bar3d(x, y, z, dx, dy, dz, color=rgba, zsort='average', alpha=0.7, shade=True)
 
-                    ax1.set_xlabel('R [km]')
-                    ax1.set_ylabel('$M_{w}$')
-                    if np.mod(i + 1, n_cols) == 1:
+                    ax1.set_xlabel('R [km]', labelpad=10)
+                    ax1.set_ylabel('$M_{w}$', labelpad=10)
+                    if np.mod(i + 1, num_cols) == 1:
                         ax1.set_zlabel('Hazard Contribution [%]')
                         ax1.zaxis.set_rotate_label(False)  # disable automatic rotation
                         ax1.set_zlabel('Hazard Contribution [%]', rotation=90)
                     ax1.zaxis._axinfo['juggled'] = (1, 2, 0)
 
                     plt.title('$T_{R}$=%s years\n$M_{mod}$=%s, $R_{mod}$=%s km\n$M_{mean}$=%s, $R_{mean}$=%s km'
-                              % ("{:.0f}".format(Tr[i]), "{:.2f}".format(modeLst[i][0]), "{:.0f}".format(modeLst[i][1]),
+                              % ("{:.0f}".format(return_period[i]), "{:.2f}".format(modeLst[i][0]), "{:.0f}".format(modeLst[i][1]),
                                  "{:.2f}".format(meanLst[i][0]), "{:.0f}".format(meanLst[i][1])),
-                              fontsize=11, loc='right', verticalalignment='top', y=0.95)
+                              fontsize=16, loc='right', verticalalignment='top', y=0.95)
 
                     mean_mags.append(meanLst[i][0])
                     mean_dists.append(meanLst[i][1])
                     mod_mags.append(modeLst[i][0])
                     mod_dists.append(modeLst[i][1])
 
                 plt.subplots_adjust(hspace=0.05, wspace=0.05)  # adjust the subplot to the right for the legend
@@ -291,35 +303,35 @@
                 fname = os.path.join(output_dir, 'mod_dists_' + imt + '.out')
                 np.savetxt(fname, np.asarray(mod_dists), fmt='%.1f')
                 if show:
                     plt.show()
                 plt.close(fig)
 
 
-def disagg_MReps(Mbin, dbin, path_disagg_results, output_dir='Post_Outputs', n_rows=1, filename='Mag_Dist_Eps', show=1):
+def disaggregation_mag_dist_eps(mag_bin, dist_bind, path_disagg_results, output_dir='Post_Outputs', num_rows=1, filename='Mag_Dist_Eps', show=1):
     """
     Details
     -------
-    This script will save disaggregation plots including M, R and eps.
+    This script will save disaggregation plots including M, R and epsilon.
 
     Parameters
     ----------
-    Mbin : int, float
+    mag_bin : int, float
         magnitude bin used in disaggregation.
-    dbin : int, float
+    dist_bin : int, float
         distance bin used in disaggregation.
     path_disagg_results: str
         Path to the hazard results
     output_dir: str, optional
         Save outputs to a pickle file
-    n_rows : int, optional
+    num_rows : int, optional
         total number of rows for subplots.
     filename : str, optional
         filename to process.
-    show: int
+    show : int
         flag to show figure (1 or 0)
 
     Returns
     -------
     None.
     """
 
@@ -342,104 +354,103 @@
             f = open(''.join([path_disagg_results, '/', file]), "r")
             ff = f.readline().split(',')
             lon = float(list(filter(lambda x: 'lon=' in x, ff))[0].replace(" lon=", ""))
             lat = float(list(filter(lambda x: 'lat=' in x, ff))[0].replace(" lat=", "").replace("\"\n", ""))
             inv_t = float(list(filter(lambda x: 'investigation_time=' in x, ff))[0].replace(" investigation_time=", ""))
             ims = np.unique(df['imt'])
             for imt in ims:
-                modeLst, meanLst = [], []
-                Tr = []
+                mod_list, mean_list = [], []
+                return_period = []
                 hz_cont = []
-                M, R, eps = [], [], []
+                mag, dist, eps = [], [], []
                 for poe in poes:
-                    Tr.append(round(-inv_t / np.log(1 - poe)))
+                    return_period.append(round(-inv_t / np.log(1 - poe)))
                     data = {}
                     data['mag'] = df['mag'][(df['poe'] == poe) & (df['imt'] == imt)]
                     data['dist'] = df['dist'][(df['poe'] == poe) & (df['imt'] == imt)]
                     data['eps'] = df['eps'][(df['poe'] == poe) & (df['imt'] == imt)]
                     data['hz_cont'] = df[hz_key][(df['poe'] == poe) & (df['imt'] == imt)]
                     hz_cont.append(np.array(data['hz_cont'] / data['hz_cont'].sum()))
                     data['hz_cont'] = hz_cont[-1]
                     data = pd.DataFrame(data)
                     data_reduced = data.groupby(['mag', 'dist']).agg(['sum'])[('hz_cont', 'sum')].reset_index().droplevel(1, axis=1)
                     # Compute the modal value (highest poe)
-                    mode = data_reduced.sort_values(by='hz_cont', ascending=False)[0:1]
-                    modeLst.append([mode['mag'].values[0], mode['dist'].values[0]])
+                    mod = data_reduced.sort_values(by='hz_cont', ascending=False)[0:1]
+                    mod_list.append([mod['mag'].values[0], mod['dist'].values[0]])
                     # Compute the mean value
-                    meanLst.append([np.sum(data_reduced['mag'] * data_reduced['hz_cont']), np.sum(data_reduced['dist'] * data_reduced['hz_cont'])])
+                    mean_list.append([np.sum(data_reduced['mag'] * data_reduced['hz_cont']), np.sum(data_reduced['dist'] * data_reduced['hz_cont'])])
 
                     # Report the individual magnitude and distance bins
-                    M.append(np.array(data['mag']))
-                    R.append(np.array(data['dist']))
+                    mag.append(np.array(data['mag']))
+                    dist.append(np.array(data['dist']))
                     eps.append(np.array(data['eps']))
 
-                n_Tr = len(Tr)
+                len_return_period = len(return_period)
                 mean_mags = []
                 mean_dists = []
                 mod_mags = []
                 mod_dists = []
-                n_eps = len(np.unique(np.asarray(eps)))
+                num_eps = len(np.unique(np.asarray(eps)))
                 min_eps = np.min(np.unique(np.asarray(eps)))  # get range of colorbars so we can normalize
                 max_eps = np.max(np.unique(np.asarray(eps)))
 
-                n_cols = int(np.floor(n_Tr / n_rows))
-                if np.mod(n_Tr, n_rows):
-                    n_cols += 1
+                num_cols = int(np.floor(len_return_period / num_rows))
+                if np.mod(len_return_period, num_rows):
+                    num_cols += 1
 
                 fig = plt.figure(figsize=(19.2, 10.8))
-                for i in range(n_Tr):
-                    ax1 = fig.add_subplot(n_rows, n_cols, i + 1, projection='3d')
+                for i in range(len_return_period):
+                    ax1 = fig.add_subplot(num_rows, num_cols, i + 1, projection='3d')
                     # Save disaggregation results
-                    disagg_results = np.array([M[i], R[i], eps[i], hz_cont[i]]).T
+                    disagg_results = np.array([mag[i], dist[i], eps[i], hz_cont[i]]).T
                     disagg_results = disagg_results[disagg_results[:, 3] != 0]
                     fname = os.path.join(output_dir, 'MagDistEps_poe_' + str(poes[i]) + '_' + imt + '.out')
                     np.savetxt(fname, disagg_results)
-                    mean_mags.append(meanLst[i][0])
-                    mean_dists.append(meanLst[i][1])
-                    mod_mags.append(modeLst[i][0])
-                    mod_dists.append(modeLst[i][1])
+                    mean_mags.append(mean_list[i][0])
+                    mean_dists.append(mean_list[i][1])
+                    mod_mags.append(mod_list[i][0])
+                    mod_dists.append(mod_list[i][1])
 
                     # scale each eps to [0,1], and get their rgb values
                     rgba = [cmap((k - min_eps) / max_eps / 2) for k in (np.unique(np.asarray(eps)))]
-                    num_triads_M_R_eps = len(R[i])
-                    Z = np.zeros(int(num_triads_M_R_eps / n_eps))
+                    num_triads_M_R_eps = len(dist[i])
+                    z = np.zeros(int(num_triads_M_R_eps / num_eps))
 
-                    for l in range(n_eps):
-                        X = np.array(R[i][np.arange(l, num_triads_M_R_eps, n_eps)])
-                        Y = np.array(M[i][np.arange(l, num_triads_M_R_eps, n_eps)])
-
-                        dx = np.ones(int(num_triads_M_R_eps / n_eps)) * dbin / 2
-                        dy = np.ones(int(num_triads_M_R_eps / n_eps)) * Mbin / 2
-                        dz = np.array(hz_cont[i][np.arange(l, num_triads_M_R_eps, n_eps)]) * 100
-
-                        ax1.bar3d(X, Y, Z, dx, dy, dz, color=rgba[l], zsort='average', alpha=0.7, shade=True)
-                        Z += dz  # add the height of each bar to know where to start the next
-
-                    ax1.set_xlabel('R [km]')
-                    ax1.set_ylabel('$M_{w}$')
-                    if np.mod(i + 1, n_cols) == 1:
+                    for l in range(num_eps):
+                        x = np.array(dist[i][np.arange(l, num_triads_M_R_eps, num_eps)])
+                        y = np.array(mag[i][np.arange(l, num_triads_M_R_eps, num_eps)])
+
+                        dx = np.ones(int(num_triads_M_R_eps / num_eps)) * dist_bind / 2
+                        dy = np.ones(int(num_triads_M_R_eps / num_eps)) * mag_bin / 2
+                        dz = np.array(hz_cont[i][np.arange(l, num_triads_M_R_eps, num_eps)]) * 100
+
+                        ax1.bar3d(x, y, z, dx, dy, dz, color=rgba[l], zsort='average', alpha=0.7, shade=True)
+                        z += dz  # add the height of each bar to know where to start the next
+
+                    ax1.set_xlabel('R [km]', labelpad=10)
+                    ax1.set_ylabel('$M_{w}$', labelpad=10)
+                    if np.mod(i + 1, num_cols) == 1:
                         ax1.set_zlabel('Hazard Contribution [%]')
                         ax1.zaxis.set_rotate_label(False)  # disable automatic rotation
                         ax1.set_zlabel('Hazard Contribution [%]', rotation=90)
                     ax1.zaxis._axinfo['juggled'] = (1, 2, 0)
 
                     plt.title('$T_{R}$=%s years\n$M_{mod}$=%s, $R_{mod}$=%s km\n$M_{mean}$=%s, $R_{mean}$=%s km'
-                              % ("{:.0f}".format(Tr[i]), "{:.2f}".format(modeLst[i][0]), "{:.0f}".format(modeLst[i][1]),
-                                 "{:.2f}".format(meanLst[i][0]), "{:.0f}".format(meanLst[i][1])),
-                              fontsize=11, loc='right', verticalalignment='top', y=0.95)
+                              % ("{:.0f}".format(return_period[i]), "{:.2f}".format(mod_list[i][0]), "{:.0f}".format(mod_list[i][1]),
+                                 "{:.2f}".format(mean_list[i][0]), "{:.0f}".format(mean_list[i][1])),
+                              fontsize=16, loc='right', verticalalignment='top', y=0.95)
 
-                    mags.append(meanLst[i][0])
-                    dists.append(meanLst[i][1])
+                    mags.append(mean_list[i][0])
+                    dists.append(mean_list[i][1])
 
                 legend_elements = []
-                for j in range(n_eps):
-                    legend_elements.append(Patch(facecolor=rgba[n_eps - j - 1],
-                                                 label=f"\u03B5 = {np.unique(np.asarray(eps))[n_eps - j - 1]:.2f}"))
+                for j in range(num_eps):
+                    legend_elements.append(Patch(facecolor=rgba[num_eps - j - 1], label=f"\u03B5 = {np.unique(np.asarray(eps))[num_eps - j - 1]:.2f}"))
 
-                fig.legend(handles=legend_elements, loc="lower center", borderaxespad=0., ncol=n_eps)
+                fig.legend(handles=legend_elements, loc="lower center", borderaxespad=0., ncol=num_eps)
                 plt.subplots_adjust(hspace=0.05, wspace=0.05)  # adjust the subplot to the right for the legend
                 fig.suptitle(f"Disaggregation of Seismic Hazard\nIntensity Measure: {imt}\nLatitude: "
                              f"{lat:.4f}, Longitude: {lon:.4f}", fontsize=14, weight='bold', ha='left', x=0.0, y=1.0)
                 plt.tight_layout(rect=[0, 0.03, 1, 0.94])
                 fname = os.path.join(output_dir, 'Disaggregation_MReps_' + imt + '.png')
                 plt.savefig(fname, format='png', dpi=300)
 
@@ -454,44 +465,43 @@
                 if show:
                     plt.show()
                 plt.close(fig)
 
 
 # FUNCTIONS TO PARSE A LOGIC TREE FROM SA to AvgSA
 # ---------------------------------------------------------------------
-def parse_sa_lt_to_avgsa(input_lt_file, output_lt_file, periods, correlation):
+def parse_sa_logic_tree_to_avgsa(input_logic_tree_file, output_logic_tree_file, avgsa_periods, correlation_model):
     """
     Details
     -------
     Parses the ordinary SA ground motion logic tree to an AvgSA equivalent
 
     Parameters
     ----------
-    input_lt_file : str
+    input_logic_tree_file : str
         Input GMPE logic tree for SA, e.g. 'gmmLT.xml'
-    output_lt_file : str
+    output_logic_tree_file : str
         The output GMPE LT file, e.g. 'gmmLT_AvgSA.xml'
-    periods : list
-        List of periods for the AvgSA calculation
-        e.g. periods = [[0.4,0.5,0.6,0.7,0.8], [1.1,1.2,1.3,1.4,1.5]]
-    correlation: str
+    avgsa_periods : list
+        Periods used for AvgSA calculation
+        e.g. periods = [0.4,0.5,0.6,0.7,0.8]
+    correlation_model: str
         String for one of the supported correlation models (e.g. 'akkar', 'baker_jayaram')
 
     Returns
     -------
     None.
     """
-    # TODO: modify the method for single AvgSA case, apparently there is no way to run PSHA for multiple AvgSA
 
     def replace_text_str(input_str):
         """
         Details
         -------
         Replaces the text string of an uncertainty model with an alternative
-        formulation in terms of Average Sa
+        formulation in terms of AvgSa
 
         Parameters
         ----------
         input_str : str
             Input string (return carriage delimited) describing entire uncertainty model
 
         Returns
@@ -500,143 +510,135 @@
         """
 
         search_output = re.search(r'\[(.*?)\]', input_str)
         if search_output:
             input_gmpe = search_output.group(1)
         else:
             input_gmpe = input_str.strip()
-        period_str = ",".join(["{:s}".format(str(per)) for per in periods])
+
         # Setup initial arguments for GenericGmpeAvgSa
-        initial_set = ["[GenericGmpeAvgSA]",
-                       "gmpe_name = \"{:s}\"".format(input_gmpe),
-                       "avg_periods = {:s}".format(period_str),
-                       "corr_func = \"{:s}\"".format(correlation)]
+        initial_set = ["[GenericGmpeAvgSA]", 
+                       f"gmpe_name = \"{input_gmpe}\"", 
+                       f"avg_periods = {avgsa_periods}", 
+                       f"corr_func = \"{correlation_model}\""]
         if not search_output:
             # No additional arguments passed to GMPE, just return the string as is
             return "\n".join(initial_set)
 
         for isegment in input_str.split("\n"):
             segment = isegment.strip()
             if not segment:
                 # Empty string
                 continue
             if input_gmpe in segment:
-                new_gmpe = segment.replace(input_gmpe,
-                                           "GenericGmpeAvgSA")
+                new_gmpe = segment.replace(input_gmpe, "GenericGmpeAvgSA")
                 if not new_gmpe in initial_set:
                     initial_set.append(new_gmpe)
             else:
                 initial_set.append(segment)
         return "\n".join(initial_set)
 
-    [input_lt] = nrml.read(input_lt_file)
+    [input_lt] = nrml.read(input_logic_tree_file)
     output_lt = []
     for blev in input_lt:
 
         if blev.tag.endswith("logicTreeBranchingLevel"):
             # Removes the branching level
             bset = blev[0]
         else:
             # Has no branching level, only branch set
             bset = deepcopy(blev)
         bset_branches = []
         for br in bset:
             unc_model_str = br.uncertaintyModel.text
             weight = float(br.uncertaintyWeight.text)
             new_unc_model = replace_text_str(unc_model_str)
-            br_node = Node("logicTreeBranch", br.attrib, nodes=[
-                Node("uncertaintyModel", text=new_unc_model),
-                Node("uncertaintyWeight", text=str(weight))
-            ])
+            br_node = Node("logicTreeBranch", br.attrib, nodes=[Node("uncertaintyModel", text=new_unc_model), Node("uncertaintyWeight", text=str(weight))])
             bset_branches.append(br_node)
-        output_bs = Node("logicTreeBranchSet",
-                         bset.attrib,
-                         nodes=bset_branches)
+        output_bs = Node("logicTreeBranchSet", bset.attrib, nodes=bset_branches)
         output_lt.append(output_bs)
-    output_lt = Node("logicTree",
-                     {"logicTreeID": input_lt["logicTreeID"] + "AvgSA"},
-                     nodes=output_lt)
-    with open(output_lt_file, "wb") as f:
+    output_lt = Node("logicTree", {"logicTreeID": input_lt["logicTreeID"] + "AvgSA"}, nodes=output_lt)
+    with open(output_logic_tree_file, "wb") as f:
         nrml.write([output_lt], f, fmt="%s")
-    print("Written to %s" % output_lt_file)
+    print("Written to %s" % output_logic_tree_file)
 
 
 # FUNCTIONS TO READ GROUND MOTION RECORD FILES
 # ---------------------------------------------------------------------
 
-def ContentFromZip(paths, zipName):
+def content_from_zip(paths, zip_name):
     """
     Details
     -------
     This function reads the contents of all selected records
     from the zipfile in which the records are located
 
     Parameters
     ----------
     paths : list
         Containing file list which are going to be read from the zipfile.
-    zipName    : str
+    zip_name : str
         Path to the zip file where file lists defined in "paths" are located.
 
     Returns
     -------
-    contents   : dictionary
+    contents : dictionary
         Containing raw contents of the files which are read from the zipfile.
     """
 
     contents = {}
-    with zipfile.ZipFile(zipName, 'r') as myzip:
+    with zipfile.ZipFile(zip_name, 'r') as myzip:
         for i in range(len(paths)):
             with myzip.open(paths[i]) as myfile:
                 contents[i] = [x.decode('utf-8') for x in myfile.readlines()]
 
     return contents
 
 
-def ReadNGA(inFilename=None, content=None, outFilename=None):
+def read_nga(in_filename=None, content=None, out_filename=None):
     """
     Details
     -------
     This function process acceleration history for NGA data file (.AT2 format).
 
     Parameters
     ----------
-    inFilename : str, optional
+    in_filename : str, optional
         Location and name of the input file.
         The default is None
-    content    : str, optional
+    content : str, optional
         Raw content of the .AT2 file.
         The default is None
-    outFilename : str, optional
+    out_filename : str, optional
         location and name of the output file.
         The default is None.
 
     Notes
     -----
     At least one of the two variables must be defined: inFilename, content.
 
     Returns
     -------
-    dt   : float
+    dt : float
         time interval of recorded points.
     npts : int
         number of points in ground motion record file.
     desc : str
         Description of the earthquake (e.g., name, year, etc).
-    t    : numpy.array (n x 1)
+    t : numpy.ndarray (n x 1)
         time array, same length with npts.
-    acc  : numpy.array (n x 1)
+    acc : numpy.ndarray (n x 1)
         acceleration array, same length with time unit
         usually in (g) unless stated as other.
     """
 
     try:
         # Read the file content from inFilename
         if content is None:
-            with open(inFilename, 'r') as inFileID:
+            with open(in_filename, 'r') as inFileID:
                 content = inFileID.readlines()
 
         # check the first line
         temp = str(content[0]).split()
         try:  # description is in the end
             float(temp[0])  # do a test with str to float conversion, this will be ok if description is in the end.
             # Description of the record
@@ -684,84 +686,84 @@
         # Acceleration values
         acc = np.array([])
         for line in acc_data:
             acc = np.append(acc, np.array(line.split(), dtype=float))
         dur = len(acc) * dt
         t = np.arange(0, dur, dt)
 
-        if outFilename is not None:
-            np.savetxt(outFilename, acc, fmt='%1.4e')
+        if out_filename is not None:
+            np.savetxt(out_filename, acc, fmt='%1.4e')
 
         return dt, npts, desc, t, acc
 
     except BaseException as error:
-        print(f"Record file reader FAILED for {inFilename}: ", error)
+        print(f"Record file reader FAILED for {in_filename}: ", error)
 
 
-def ReadESM(inFilename=None, content=None, outFilename=None):
+def read_esm(in_filename=None, content=None, out_filename=None):
     """
     Details
     -------
     This function process acceleration history for ESM data file.
 
     Parameters
     ----------
-    inFilename : str, optional
+    in_filename : str, optional
         Location and name of the input file.
         The default is None
-    content    : str, optional
+    content : str, optional
         Raw content of the ESM record file.
         The default is None
-    outFilename : str, optional
+    out_filename : str, optional
         location and name of the output file.
         The default is None.
 
     Returns
     -------
-    dt   : float
+    dt : float
         time interval of recorded points.
     npts : int
         number of points in ground motion record file.
     desc : str
         Description of the earthquake (e.g., name, year, etc).
-    time : numpy.array (n x 1)
+    time : numpy.ndarray (n x 1)
         time array, same length with npts.
-    acc  : numpy.array (n x 1)
+    acc : numpy.ndarray (n x 1)
         acceleration array, same length with time unit
         usually in (g) unless stated as other.
     """
 
     try:
         # Read the file content from inFilename
         if content is None:
-            with open(inFilename, 'r') as inFileID:
+            with open(in_filename, 'r') as inFileID:
                 content = inFileID.readlines()
 
         desc = content[:64]
         dt = float(difflib.get_close_matches('SAMPLING_INTERVAL_S', content)[0].split()[1])
         npts = len(content[64:])
         acc_data = content[64:]
         acc = np.asarray([float(data) for data in acc_data], dtype=float)
         dur = len(acc) * dt
         t = np.arange(0, dur, dt)
         acc = acc / 980.655  # cm/s**2 to g
 
-        if outFilename is not None:
-            np.savetxt(outFilename, acc, fmt='%1.4e')
+        if out_filename is not None:
+            np.savetxt(out_filename, acc, fmt='%1.4e')
 
         return dt, npts, desc, t, acc
 
     except BaseException as error:
-        print(f"Record file reader FAILED for {inFilename}: ", error)
+        print(f"Record file reader FAILED for {in_filename}: ", error)
 
 
 # FUNCTIONS TO CREATE BUILDING CODE DESIGN SPECTRA
 # ---------------------------------------------------------------------
 
-def Sae_ec8_part1(ag, xi, T, ImpClass, Type, SiteClass):
+def sae_ec8_part1(ag, xi, periods, importance_class, spectrum_type, site_class):
     """
     Details
     -------
     Calculates the design response spectrum according to EN 1998-1:2004
 
     References
     ----------
@@ -769,35 +771,35 @@
     Seismic Actions and Rules for Buildings (EN 1998-1:2004). Brussels, Belgium: 2004.
 
     Notes
     -----
 
     Parameters
     ----------
-    ag: float
+    ag : float
         Peak ground acceleration
-    xi: float
+    xi : float
         Damping ratio
-    T: list or numpy.array
+    periods : list or numpy.ndarray
         Period array for which elastic response spectrum is calculated
-    ImpClass: str
+    importance_class : str
         Importance class ('I','II','III','IV')
-    Type: str
+    spectrum_type: str
         Type of spectrum ('Type1','Type2')
-    SiteClass: str
+    site_class : str
         Site Soil Class ('A','B','C','D','E')
 
     Returns
     -------
-    Sae: numpy.array
+    Sae : numpy.ndarray
         Elastic acceleration response spectrum
 
     """
 
-    SpecProp = {
+    spec_props = {
         'Type1': {
             'A': {'S': 1.00, 'Tb': 0.15, 'Tc': 0.4, 'Td': 2.0},
             'B': {'S': 1.20, 'Tb': 0.15, 'Tc': 0.5, 'Td': 2.0},
             'C': {'S': 1.15, 'Tb': 0.20, 'Tc': 0.6, 'Td': 2.0},
             'D': {'S': 1.35, 'Tb': 0.20, 'Tc': 0.8, 'Td': 2.0},
             'E': {'S': 1.40, 'Tb': 0.15, 'Tc': 0.5, 'Td': 2.0},
         },
@@ -807,55 +809,55 @@
             'B': {'S': 1.35, 'Tb': 0.05, 'Tc': 0.25, 'Td': 1.2},
             'C': {'S': 1.50, 'Tb': 0.10, 'Tc': 0.25, 'Td': 1.2},
             'D': {'S': 1.80, 'Tb': 0.10, 'Tc': 0.30, 'Td': 1.2},
             'E': {'S': 1.60, 'Tb': 0.05, 'Tc': 0.25, 'Td': 1.2},
         }
     }
 
-    S = SpecProp[Type][SiteClass]['S']
-    Tb = SpecProp[Type][SiteClass]['Tb']
-    Tc = SpecProp[Type][SiteClass]['Tc']
-    Td = SpecProp[Type][SiteClass]['Td']
+    s = spec_props[spectrum_type][site_class]['S']
+    tb = spec_props[spectrum_type][site_class]['Tb']
+    tc = spec_props[spectrum_type][site_class]['Tc']
+    td = spec_props[spectrum_type][site_class]['Td']
 
     eta = max(np.sqrt(0.10 / (0.05 + xi)), 0.55)
 
-    if ImpClass == 'I':
-        I = 0.8
-    elif ImpClass == 'II':
-        I = 1.0
-    elif ImpClass == 'III':
-        I = 1.2
-    elif ImpClass == 'IV':
-        I = 1.4
+    if importance_class == 'I':
+        imp_factor = 0.8
+    elif importance_class == 'II':
+        imp_factor = 1.0
+    elif importance_class == 'III':
+        imp_factor = 1.2
+    elif importance_class == 'IV':
+        imp_factor = 1.4
     else:
         print('Error! Cannot compute a value of Importance Factor')
 
-    ag = ag * I
+    ag = ag * imp_factor
 
-    Sae = []
-    for i in range(len(T)):
-        if 0 <= T[i] <= Tb:
-            Sa_el = ag * S * (1.0 + T[i] / Tb * (2.5 * eta - 1.0))
-        elif Tb <= T[i] <= Tc:
-            Sa_el = ag * S * 2.5 * eta
-        elif Tc <= T[i] <= Td:
-            Sa_el = ag * S * 2.5 * eta * (Tc / T[i])
-        elif T[i] >= Td:
-            Sa_el = ag * S * 2.5 * eta * (Tc * Td / T[i] / T[i])
+    sae = []
+    for i in range(len(periods)):
+        if 0 <= periods[i] <= tb:
+            sat = ag * s * (1.0 + periods[i] / tb * (2.5 * eta - 1.0))
+        elif tb <= periods[i] <= tc:
+            sat = ag * s * 2.5 * eta
+        elif tc <= periods[i] <= td:
+            sat = ag * s * 2.5 * eta * (tc / periods[i])
+        elif periods[i] >= td:
+            sat = ag * s * 2.5 * eta * (tc * td / periods[i] / periods[i])
         else:
             print('Error! Cannot compute a value of Spectral Acceleration')
 
-        Sae.append(Sa_el)
+        sae.append(sat)
 
-    Sae = np.array(Sae)
+    sae = np.array(sae)
 
-    return Sae
+    return sae
 
 
-def Sae_asce7_16(T, SDS, SD1, TL):
+def sae_asce7_16(periods, sds, sd1, tl):
     """
     Details
     -------
     This method determines the design response spectrum based on ASCE 7-16.
 
     References
     ----------
@@ -863,47 +865,47 @@
     for buildings and other structures. American Society of Civil Engineers.
 
     Notes
     -----
 
     Parameters
     ----------
-    T:  numpy.array
+    periods : numpy.ndarray
         Period array for which elastic response spectrum is calculated
-    SDS: float
+    sds : float
         Numeric seismic design value (0.2 sec)
-    SD1: float
+    sd1 : float
         Numeric seismic design value (1.0 sec)
-    TL: float
+    tl : float
         Long-period transition period
 
 
     Returns
     -------
-    Sae: numpy.array
+    Sae : numpy.ndarray
         Elastic acceleration response spectrum
     """
 
-    T0 = 0.2 * (SD1 / SDS)
-    TS = SD1 / SDS
-    Sae = np.zeros(len(T))
-    for i in range(len(T)):
-        if T[i] < T0:
-            Sae[i] = SDS * (0.4 + 0.6 * T[i] / T0)
-        if T0 <= T[i] <= TS:
-            Sae[i] = SDS
-        if TS <= T[i] <= TL:
-            Sae[i] = SD1 / T[i]
-        if TL < T[i]:
-            Sae[i] = (SD1 * TL) / (T[i] ** 2)
+    t0 = 0.2 * (sd1 / sds)
+    ts = sd1 / sds
+    sae = np.zeros(len(periods))
+    for i in range(len(periods)):
+        if periods[i] < t0:
+            sae[i] = sds * (0.4 + 0.6 * periods[i] / t0)
+        if t0 <= periods[i] <= ts:
+            sae[i] = sds
+        if ts <= periods[i] <= tl:
+            sae[i] = sd1 / periods[i]
+        if tl < periods[i]:
+            sae[i] = (sd1 * tl) / (periods[i] ** 2)
 
-    return Sae
+    return sae
 
 
-def SiteParam_asce7_16(Lat, Long, RiskCat, SiteClass):
+def site_parameters_asce7_16(lat, long, risk_category, site_class):
     """
     Details
     -------
     This method makes use of API developed by USGS to get spectra (ASCE7-16) info in US.
     It retrieves the design response spectrum parameters for the given site.
 
     References
@@ -913,133 +915,132 @@
     for buildings and other structures. American Society of Civil Engineers.
 
     Notes
     -----
 
     Parameters
     ----------
-    Lat: float
+    lat : float
         Site latitude
-    Long: float
+    long : float
         Site longitude
-    RiskCat:  str
+    risk_category :  str
         Risk category for structure ('I','II','III','IV')
-    SiteClass: str
+    site_class : str
         Site soil class ('A','B','C','D','E')
 
     Returns
     -------
-    SDS: float
+    sds : float
         Short period (0.2 sec) spectral acceleration coefficient
-    SD1: float
+    sd1 : float
         Spectral acceleration coefficient at period 1.0
-    TL: float
+    tl : float
         Period value for long-period transition
     """
 
-    thisURL = 'https://earthquake.usgs.gov/ws/designmaps/asce7-16.json?latitude=' + str(Lat) + '&longitude=' + str(
-        Long) + '&riskCategory=' + RiskCat + '&siteClass=' + SiteClass + '&title=Example'
-    web = json.loads(requests.get(thisURL).text)  # get the info from webpage and convert json format to dictionary
-    Ss = web['response']['data']['ss']
-    S1 = web['response']['data']['s1']
-    Fa = web['response']['data']['fa']
-    Fv = web['response']['data']['fv']
-    TL = web['response']['data']['tl']
+    url = 'https://earthquake.usgs.gov/ws/designmaps/asce7-16.json?latitude=' + str(lat) + '&longitude=' + str(long) + '&riskCategory=' + risk_category + '&siteClass=' + site_class + '&title=Example'
+    web = json.loads(requests.get(url).text)  # get the info from webpage and convert json format to dictionary
+    ss = web['response']['data']['ss']
+    s1 = web['response']['data']['s1']
+    fa = web['response']['data']['fa']
+    fv = web['response']['data']['fv']
+    tl = web['response']['data']['tl']
 
-    if Ss is None:
+    if ss is None:
         raise ValueError('Failed to get parameter Ss, define user-defined spectrum instead.')
-    if S1 is None:
+    if s1 is None:
         raise ValueError('Failed to get parameter S1, define user-defined spectrum instead.')
-    if Fa is None:
+    if fa is None:
         raise ValueError('Failed to get parameter Fa, define user-defined spectrum instead.')
-    if Fv is None:
+    if fv is None:
         raise ValueError('Failed to get parameter Fv, define user-defined spectrum instead.')
-    if TL is None:
+    if tl is None:
         raise ValueError('Failed to get parameter TL, define user-defined spectrum instead.')
 
-    Sms = Fa * Ss
-    Sm1 = Fv * S1
-    SDS = (2 / 3) * Sms
-    SD1 = (2 / 3) * Sm1
+    sms = fa * ss
+    sm1 = fv * s1
+    sds = (2 / 3) * sms
+    sd1 = (2 / 3) * sm1
 
-    return SDS, SD1, TL
+    return sds, sd1, tl
 
 
-def SiteParam_tbec2018(Lat, Long, DD, SiteClass):
+def site_parameters_tbec2018(lat, long, dd, site_class):
     """
     Details
     -------
     This method retrieves the elastic design spectrum parameters for the given site according to TBEC2018.
 
     References
     ----------
     TBEC. (2018). Turkish building earthquake code.
 
     Notes
     -----
 
     Parameters
     ----------
-    Lat: float
+    lat : float
         Site latitude
-    Long: float
+    long : float
         Site longitude
-    DD:  int
+    dd_level :  int
         Earthquake ground motion intensity level (1,2,3,4)
-    SiteClass: str
+    site_class : str
         Site soil class ('ZA','ZB','ZC','ZD','ZE')
 
     Returns
     -------
-    PGA: float
+    PGA : float
         Peak ground acceleration
-    SDS: float
+    SDS : float
         Short period (0.2 sec) spectral acceleration coefficient
-    SD1: float
+    SD1 : float
         Spectral acceleration coefficient at period 1.0
-    TL: float
+    TL : float
         Period value for long-period transition
     """
 
     csv_file = 'Parameters_TBEC2018.csv'
     file_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'Meta_Data', csv_file)
     data = pd.read_csv(file_path)
 
     # Check if the coordinates are within the limits
-    if Long > np.max(data['Longitude']) or Long < np.min(data['Longitude']):
+    if long > np.max(data['Longitude']) or long < np.min(data['Longitude']):
         raise ValueError('Longitude value must be within the limits: [24.55,45.95]')
-    if Lat > np.max(data['Latitude']) or Lat < np.min(data['Latitude']):
+    if lat > np.max(data['Latitude']) or lat < np.min(data['Latitude']):
         raise ValueError('Latitude value must be within the limits: [34.25,42.95]')
 
     # Targeted probability of exceedance in 50 years
-    if DD == 1:
-        PoE = '2'
-    elif DD == 2:
-        PoE = '10'
-    elif DD == 3:
-        PoE = '50'
-    elif DD == 4:
-        PoE = '68'
+    if dd == 1:
+        poe = '2'
+    elif dd == 2:
+        poe = '10'
+    elif dd == 3:
+        poe = '50'
+    elif dd == 4:
+        poe = '68'
 
     # Determine Peak Ground Acceleration PGA [g]
-    PGA_col = 'PGA (g) - %' + PoE
-    data_pga = np.array([data['Longitude'], data['Latitude'], data[PGA_col]]).T
-    PGA = interpolate.griddata(data_pga[:, 0:2], data_pga[:, 2], [(Long, Lat)], method='linear')
+    pga_col = 'PGA (g) - %' + poe
+    data_pga = np.array([data['Longitude'], data['Latitude'], data[pga_col]]).T
+    pga = interpolate.griddata(data_pga[:, 0:2], data_pga[:, 2], [(long, lat)], method='linear')
 
     # Short period map spectral acceleration coefficient [dimensionless]
-    SS_col = 'SS (g) - %' + PoE
-    data_ss = np.array([data['Longitude'], data['Latitude'], data[SS_col]]).T
-    SS = interpolate.griddata(data_ss[:, 0:2], data_ss[:, 2], [(Long, Lat)], method='linear')
+    ss_col = 'SS (g) - %' + poe
+    data_ss = np.array([data['Longitude'], data['Latitude'], data[ss_col]]).T
+    ss = interpolate.griddata(data_ss[:, 0:2], data_ss[:, 2], [(long, lat)], method='linear')
 
     # Map spectral acceleration coefficient for a 1.0 second period [dimensionless]
-    S1_col = 'S1 (g) - %' + PoE
-    data_s1 = np.array([data['Longitude'], data['Latitude'], data[S1_col]]).T
-    S1 = interpolate.griddata(data_s1[:, 0:2], data_s1[:, 2], [(Long, Lat)], method='linear')
+    s1_col = 'S1 (g) - %' + poe
+    data_s1 = np.array([data['Longitude'], data['Latitude'], data[s1_col]]).T
+    s1 = interpolate.griddata(data_s1[:, 0:2], data_s1[:, 2], [(long, lat)], method='linear')
 
-    SoilParam = {
+    soil_parameters = {
         'FS': {
             'ZA': [0.8, 0.8, 0.8, 0.8, 0.8, 0.8],
             'ZB': [0.9, 0.9, 0.9, 0.9, 0.9, 0.9],
             'ZC': [1.3, 1.3, 1.2, 1.2, 1.2, 1.2],
             'ZD': [1.6, 1.4, 1.2, 1.1, 1.0, 1.0],
             'ZE': [2.4, 1.7, 1.3, 1.1, 0.9, 0.8]
         },
@@ -1055,133 +1056,133 @@
         },
 
         'S1': [0.1, 0.2, 0.3, 0.4, 0.5, 0.6],
 
     }
 
     # Local soil response coefficient for the short period region
-    if SS <= SoilParam['SS'][0]:
-        FS = SoilParam['FS'][SiteClass][0]
-    elif SoilParam['SS'][0] < SS <= SoilParam['SS'][1]:
-        FS = (SoilParam['FS'][SiteClass][1] - SoilParam['FS'][SiteClass][0]) \
-             * (SS - SoilParam['SS'][0]) / (SoilParam['SS'][1] - SoilParam['SS'][0]) \
-             + SoilParam['FS'][SiteClass][0]
-    elif SoilParam['SS'][1] < SS <= SoilParam['SS'][2]:
-        FS = (SoilParam['FS'][SiteClass][2] - SoilParam['FS'][SiteClass][1]) \
-             * (SS - SoilParam['SS'][1]) / (SoilParam['SS'][2] - SoilParam['SS'][1]) \
-             + SoilParam['FS'][SiteClass][1]
-    elif SoilParam['SS'][2] < SS <= SoilParam['SS'][3]:
-        FS = (SoilParam['FS'][SiteClass][3] - SoilParam['FS'][SiteClass][2]) \
-             * (SS - SoilParam['SS'][2]) / (SoilParam['SS'][3] - SoilParam['SS'][2]) \
-             + SoilParam['FS'][SiteClass][2]
-    elif SoilParam['SS'][3] < SS <= SoilParam['SS'][4]:
-        FS = (SoilParam['FS'][SiteClass][4] - SoilParam['FS'][SiteClass][3]) \
-             * (SS - SoilParam['SS'][3]) / (SoilParam['SS'][4] - SoilParam['SS'][3]) \
-             + SoilParam['FS'][SiteClass][3]
-    elif SoilParam['SS'][4] < SS <= SoilParam['SS'][5]:
-        FS = (SoilParam['FS'][SiteClass][5] - SoilParam['FS'][SiteClass][4]) \
-             * (SS - SoilParam['SS'][4]) / (SoilParam['SS'][5] - SoilParam['SS'][4]) \
-             + SoilParam['FS'][SiteClass][4]
-    elif SS >= SoilParam['SS'][5]:
-        FS = SoilParam['FS'][SiteClass][5]
+    if ss <= soil_parameters['SS'][0]:
+        fs = soil_parameters['FS'][site_class][0]
+    elif soil_parameters['SS'][0] < ss <= soil_parameters['SS'][1]:
+        fs = (soil_parameters['FS'][site_class][1] - soil_parameters['FS'][site_class][0]) \
+             * (ss - soil_parameters['SS'][0]) / (soil_parameters['SS'][1] - soil_parameters['SS'][0]) \
+             + soil_parameters['FS'][site_class][0]
+    elif soil_parameters['SS'][1] < ss <= soil_parameters['SS'][2]:
+        fs = (soil_parameters['FS'][site_class][2] - soil_parameters['FS'][site_class][1]) \
+             * (ss - soil_parameters['SS'][1]) / (soil_parameters['SS'][2] - soil_parameters['SS'][1]) \
+             + soil_parameters['FS'][site_class][1]
+    elif soil_parameters['SS'][2] < ss <= soil_parameters['SS'][3]:
+        fs = (soil_parameters['FS'][site_class][3] - soil_parameters['FS'][site_class][2]) \
+             * (ss - soil_parameters['SS'][2]) / (soil_parameters['SS'][3] - soil_parameters['SS'][2]) \
+             + soil_parameters['FS'][site_class][2]
+    elif soil_parameters['SS'][3] < ss <= soil_parameters['SS'][4]:
+        fs = (soil_parameters['FS'][site_class][4] - soil_parameters['FS'][site_class][3]) \
+             * (ss - soil_parameters['SS'][3]) / (soil_parameters['SS'][4] - soil_parameters['SS'][3]) \
+             + soil_parameters['FS'][site_class][3]
+    elif soil_parameters['SS'][4] < ss <= soil_parameters['SS'][5]:
+        fs = (soil_parameters['FS'][site_class][5] - soil_parameters['FS'][site_class][4]) \
+             * (ss - soil_parameters['SS'][4]) / (soil_parameters['SS'][5] - soil_parameters['SS'][4]) \
+             + soil_parameters['FS'][site_class][4]
+    elif ss >= soil_parameters['SS'][5]:
+        fs = soil_parameters['FS'][site_class][5]
 
     # Local soil response coefficient for 1.0 second period
-    if S1 <= SoilParam['S1'][0]:
-        F1 = SoilParam['F1'][SiteClass][0]
-    elif SoilParam['S1'][0] < S1 <= SoilParam['S1'][1]:
-        F1 = (SoilParam['F1'][SiteClass][1] - SoilParam['F1'][SiteClass][0]) \
-             * (S1 - SoilParam['S1'][0]) / (SoilParam['S1'][1] - SoilParam['S1'][0]) \
-             + SoilParam['F1'][SiteClass][0]
-    elif SoilParam['S1'][1] < S1 <= SoilParam['S1'][2]:
-        F1 = (SoilParam['F1'][SiteClass][2] - SoilParam['F1'][SiteClass][1]) \
-             * (S1 - SoilParam['S1'][1]) / (SoilParam['S1'][2] - SoilParam['S1'][1]) \
-             + SoilParam['F1'][SiteClass][1]
-    elif SoilParam['S1'][2] < S1 <= SoilParam['S1'][3]:
-        F1 = (SoilParam['F1'][SiteClass][3] - SoilParam['F1'][SiteClass][2]) \
-             * (S1 - SoilParam['S1'][2]) / (SoilParam['S1'][3] - SoilParam['S1'][2]) \
-             + SoilParam['F1'][SiteClass][2]
-    elif SoilParam['S1'][3] < S1 <= SoilParam['S1'][4]:
-        F1 = (SoilParam['F1'][SiteClass][4] - SoilParam['F1'][SiteClass][3]) \
-             * (S1 - SoilParam['S1'][3]) / (SoilParam['S1'][4] - SoilParam['S1'][3]) \
-             + SoilParam['F1'][SiteClass][3]
-    elif SoilParam['S1'][4] < S1 <= SoilParam['S1'][5]:
-        F1 = (SoilParam['F1'][SiteClass][5] - SoilParam['F1'][SiteClass][4]) \
-             * (S1 - SoilParam['S1'][4]) / (SoilParam['S1'][5] - SoilParam['S1'][4]) \
-             + SoilParam['F1'][SiteClass][4]
-    elif S1 >= SoilParam['S1'][5]:
-        F1 = SoilParam['F1'][SiteClass][5]
-
-    SDS = SS * FS
-    SD1 = S1 * F1
-    TL = 6
+    if s1 <= soil_parameters['S1'][0]:
+        f1 = soil_parameters['F1'][site_class][0]
+    elif soil_parameters['S1'][0] < s1 <= soil_parameters['S1'][1]:
+        f1 = (soil_parameters['F1'][site_class][1] - soil_parameters['F1'][site_class][0]) \
+             * (s1 - soil_parameters['S1'][0]) / (soil_parameters['S1'][1] - soil_parameters['S1'][0]) \
+             + soil_parameters['F1'][site_class][0]
+    elif soil_parameters['S1'][1] < s1 <= soil_parameters['S1'][2]:
+        f1 = (soil_parameters['F1'][site_class][2] - soil_parameters['F1'][site_class][1]) \
+             * (s1 - soil_parameters['S1'][1]) / (soil_parameters['S1'][2] - soil_parameters['S1'][1]) \
+             + soil_parameters['F1'][site_class][1]
+    elif soil_parameters['S1'][2] < s1 <= soil_parameters['S1'][3]:
+        f1 = (soil_parameters['F1'][site_class][3] - soil_parameters['F1'][site_class][2]) \
+             * (s1 - soil_parameters['S1'][2]) / (soil_parameters['S1'][3] - soil_parameters['S1'][2]) \
+             + soil_parameters['F1'][site_class][2]
+    elif soil_parameters['S1'][3] < s1 <= soil_parameters['S1'][4]:
+        f1 = (soil_parameters['F1'][site_class][4] - soil_parameters['F1'][site_class][3]) \
+             * (s1 - soil_parameters['S1'][3]) / (soil_parameters['S1'][4] - soil_parameters['S1'][3]) \
+             + soil_parameters['F1'][site_class][3]
+    elif soil_parameters['S1'][4] < s1 <= soil_parameters['S1'][5]:
+        f1 = (soil_parameters['F1'][site_class][5] - soil_parameters['F1'][site_class][4]) \
+             * (s1 - soil_parameters['S1'][4]) / (soil_parameters['S1'][5] - soil_parameters['S1'][4]) \
+             + soil_parameters['F1'][site_class][4]
+    elif s1 >= soil_parameters['S1'][5]:
+        f1 = soil_parameters['F1'][site_class][5]
+
+    sds = ss * fs
+    sd1 = s1 * f1
+    tl = 6
 
-    return PGA, SDS, SD1, TL
+    return pga, sds, sd1, tl
 
 
-def Sae_tbec2018(T, SDS, SD1, TL):
+def sae_tbec2018(periods, sds, sd1, tl):
     """
     Details
     -------
     This method calculates the elastic design spectrum according to TBEC2018.
 
     References
     ----------
     TBEC. (2018). Turkish building earthquake code.
 
     Notes
     -----
 
     Parameters
     ----------
-    T:  numpy.array
+    periods :  numpy.ndarray
         Period array for which elastic response spectrum is calculated
-    SDS: float
+    sds : float
         Short period (0.2 sec) spectral acceleration coefficient
-    SD1: float
+    sd1 : float
         Spectral acceleration coefficient at period 1.0
-    TL: float
+    tl : float
         Period value for long-period transition
 
     Returns
     -------
-    Sae: numpy.array
+    sae : numpy.ndarray
         Horizontal elastic acceleration response spectrum
-    SaeD: numpy.array
-        Vertıcal elastic acceleration response spectrum
+    sae_vert : numpy.ndarray
+        Vertical elastic acceleration response spectrum
     """
 
-    TA = 0.2 * SD1 / SDS
-    TB = SD1 / SDS
-    TAD = TA/3
-    TBD = TB/3
-    TLD = TL/2
-    Sae = np.zeros(len(T))
-    SaeD = np.zeros(len(T))
-
-    for i in range(len(T)):
-        if T[i] <= TA:
-            Sae[i] = (0.4 + 0.6 * T[i] / TA) * SDS
-        elif TA < T[i] <= TB:
-            Sae[i] = SDS
-        elif TB < T[i] <= TL:
-            Sae[i] = SD1 / T[i]
-        elif T[i] > TL:
-            Sae[i] = SD1 * TL / T[i] ** 2
-
-        if T[i] <= TAD:
-            SaeD[i] = (0.32 + 0.48 * T[i] / TAD) * SDS
-        elif TAD < T[i] <= TBD:
-            SaeD[i] = 0.8 * SDS
-        elif TBD < T[i] <= TLD:
-            SaeD[i] = 0.8 * SDS * TBD / T[i]
+    ta = 0.2 * sd1 / sds
+    tb = sd1 / sds
+    tad = ta/3
+    tbd = tb/3
+    tld = tl/2
+    sae = np.zeros(len(periods))
+    sae_vert = np.zeros(len(periods))
+
+    for i in range(len(periods)):
+        if periods[i] <= ta:
+            sae[i] = (0.4 + 0.6 * periods[i] / ta) * sds
+        elif ta < periods[i] <= tb:
+            sae[i] = sds
+        elif tb < periods[i] <= tl:
+            sae[i] = sd1 / periods[i]
+        elif periods[i] > tl:
+            sae[i] = sd1 * tl / periods[i] ** 2
+
+        if periods[i] <= tad:
+            sae_vert[i] = (0.32 + 0.48 * periods[i] / tad) * sds
+        elif tad < periods[i] <= tbd:
+            sae_vert[i] = 0.8 * sds
+        elif tbd < periods[i] <= tld:
+            sae_vert[i] = 0.8 * sds * tbd / periods[i]
 
-    return Sae, SaeD
+    return sae, sae_vert
 
 
-def Sae_TBEC2007(T, zone, soil):
+def sae_tbec2007(periods, zone, soil):
 
     """
     Details
     -------
     This method calculates the elastic horizontal design spectrum according to TBEC2007.
 
     References
@@ -1189,66 +1190,64 @@
     TBEC. (2007). Turkish building earthquake code.
 
     Notes
     -----
 
     Parameters
     ----------
-    T:  numpy.array
+    periods :  numpy.ndarray
         Period array for which elastic response spectrum is calculated
-    zone: int
+    zone : int
         Seismic zone (1, 2, 3, 4)
-    soil: str
+    soil : str
         Site class ('Z1', 'Z2', 'Z3', 'Z4')
-    SD1: float
-        Spectral acceleration coefficient at period 1.0
 
     Returns
     -------
-    Sae: numpy.array
+    sae : numpy.ndarray
         Elastic acceleration response spectrum
     """
 
     # Seismic zone
     if zone == 1:
-      A0 = 0.1
+      a0 = 0.1
     elif zone == 2:
-      A0 = 0.2
+      a0 = 0.2
     elif zone == 3:
-      A0 = 0.3
+      a0 = 0.3
     elif zone == 4:
-      A0 = 0.4
+      a0 = 0.4
 
     # site class
     if soil == 'Z1':
-      TA = 0.1
-      TB = 0.30
+      ta = 0.1
+      tb = 0.30
     elif soil == 'Z2':
-       TA = 0.15
-       TB = 0.40     
+       ta = 0.15
+       tb = 0.40     
     elif soil == 'Z3':
-       TA = 0.15
-       TB = 0.60   
+       ta = 0.15
+       tb = 0.60   
     elif soil == 'Z4':
-       TA = 0.2
-       TB = 0.90   
+       ta = 0.2
+       tb = 0.90   
 
     # Response spectrum
-    Sae = np.zeros(len(T))
-    for i in range(len(T)):
-        if T[i] <= TA:
-            Sae[i] = 1+1.5*T[i]/TA
-        elif T[i] > TA and T[i]<=TB:       
-            Sae[i] = 2.5
-        elif T[i] > TB:       
-            Sae[i] = 2.5*(TB/T[i])**0.8  
+    sae = np.zeros(len(periods))
+    for i in range(len(periods)):
+        if periods[i] <= ta:
+            sae[i] = 1+1.5*periods[i]/ta
+        elif periods[i] > ta and periods[i]<=tb:       
+            sae[i] = 2.5
+        elif periods[i] > tb:       
+            sae[i] = 2.5*(tb/periods[i])**0.8  
         
-    Sae = A0*Sae
+    sae = a0*sae
     
-    return Sae
+    return sae
 
 
 # FUNCTIONS TO CHECK GMPES IMPLEMENTED IN OPENQUAKE
 # ---------------------------------------------------------------------
 
 def get_available_gmpes():
     """
@@ -1325,61 +1324,65 @@
     except BaseException as e:
         raise e
 
 
 # MISCELLANEOUS FUNCTIONS
 # ---------------------------------------------------------------------
 
-def get_esm_token(username, pwd):
+def get_esm_token(username, password):
     """
     Details
     -------
     This function retrieves ESM database token.
 
     Notes
     -------
     Data must be obtained using any program supporting the HTTP-POST method, e.g. CURL.
     see: https://esm-db.eu/esmws/generate-signed-message/1/query-options.html
     Credentials must have been retrieved from https://esm-db.eu/#/home.
 
     Parameters
     ----------
-    username     : str
-        Account username (e-mail),  e.g. 'username@mail.com'.
-    pwd          : str
-        Account password, e.g. 'password!12345'.
+    username : str
+        Account username (e-mail),  e.g. 'example_username@email.com'.
+    password : str
+        Account password, e.g. 'example_password123456'.
 
     Returns
     -------
-    None.
+    token_path : str
+        Path to token used to retrieve records from ESM_2018 database
     """
 
     if sys.platform.startswith('win'):
         command = 'curl --ssl-no-revoke -X POST -F ' + '\"' + \
                   'message={' + '\\\"' + 'user_email' + '\\\": ' + '\\\"' + username + '\\\", ' + \
-                  '\\\"' + 'user_password' + '\\\": ' + '\\\"' + pwd + '\\\"}' + \
+                  '\\\"' + 'user_password' + '\\\": ' + '\\\"' + password + '\\\"}' + \
                   '\" ' + '\"https://esm-db.eu/esmws/generate-signed-message/1/query\" > token.txt'
     else:
         command = 'curl -X POST -F \'message={\"user_email\": \"' + \
-                  username + '\",\"user_password\": \"' + pwd + \
+                  username + '\",\"user_password\": \"' + password + \
                   '\"}\' \"https://esm-db.eu/esmws/generate-signed-message/1/query\" > token.txt'
 
     os.system(command)
+    token_path = os.path.join(os.getcwd(), 'token.txt')
+
+    return token_path
 
 
-def create_dir(dir_path):
+def make_dir(dir_path):
     """
     Details
     -------
-    Creates a clean directory by deleting it if it exists.
+    Makes a clean directory by deleting it if it exists.
 
     Parameters
     ----------
     dir_path : str
-        name of directory to create.
+        name of directory to make.
 
     None.
     """
 
     def handle_remove_read_only(func, path, exc):
         excvalue = exc[1]
         if func in (os.rmdir, os.remove) and excvalue.errno == errno.EACCES:
@@ -1394,15 +1397,15 @@
     os.makedirs(dir_path)
 
 
 def run_time(start_time):
     """
     Details
     -------
-    Prints the time passed between startTime and FinishTime (now)
+    Prints the time passed between start_time and finish_time (now)
     in hours, minutes, seconds. startTime is a global variable.
 
     Parameters
     ----------
     start_time : int
         The initial time obtained via time().
 
@@ -1429,26 +1432,26 @@
 
     References
     ----------
     https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.qmc.LatinHypercube.html#scipy.stats.qmc.LatinHypercube
 
     Parameters
     ----------
-    num_dimensions: int
+    num_dimensions : int
         number of dimensions
-    num_samples: int
+    num_samples : int
         number of samples
-    sampling_type: str
+    sampling_type : str
         type of sampling.
         Monte Carlo Sampling: 'MCS'
         Latin Hypercube Sampling: 'LHS'
 
     Returns
     -------
-    sample: numpy.ndarray (num_samples x num_dimensions)
+    sample : numpy.ndarray (num_samples x num_dimensions)
         Array which contains randomly generated numbers between 0 and 1
     """
     # Not really required, but will ensure different realizations each time
     seed = int(datetime.today().strftime("%H%M%S"))
     if sampling_type == 'MCS':
         # Do Monte Carlo Sampling without any grid
         np.random.seed(seed)
@@ -1473,21 +1476,21 @@
     Yang, T. Y., Moehle, J., Stojadinovic, B., & Der Kiureghian, A. (2009).
     Seismic Performance Evaluation of Facilities: Methodology and Implementation.
     In Journal of Structural Engineering (Vol. 135, Issue 10, pp. 1146–1154).
     American Society of Civil Engineers (ASCE). https://doi.org/10.1061/(asce)0733-9445(2009)135:10(1146)
 
     Parameters
     ----------
-    mu: numpy.ndarray (1-D)
+    mu : numpy.ndarray (1-D)
         Mean value vector
-    cov: numpy.ndarray (2-D)
+    cov : numpy.ndarray (2-D)
         Covariance matrix
-    num_samples: int
+    num_samples : int
         number of samples
-    sampling_option: str
+    sampling_option : str
         Monte Carlo Sampling: 'MCS'
         Latin Hypercube Sampling: 'LHS'
 
     Returns
     -------
     z : numpy.ndarray (num_samples x num_dimensions)
         Array which contains randomly generated numbers between 0 and 1
```

### Comparing `EzGM-1.6.6.3/EzGM/webdriverdownloader.py` & `EzGM-1.7.0.0/EzGM/webdriverdownloader.py`

 * *Files identical despite different names*

### Comparing `EzGM-1.6.6.3/EzGM.egg-info/PKG-INFO` & `EzGM-1.7.0.0/EzGM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EzGM
-Version: 1.6.6.3
+Version: 1.7.0.0
 Summary: Toolbox for ground motion record selection and processing
 Home-page: https://github.com/volkanozsarac/EzGM
 Author: Volkan Ozsarac
 Author-email: volkan.ozsarac@iusspavia.it
 Project-URL: Bug Tracker, https://github.com/volkanozsarac/EzGM/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -24,27 +24,27 @@
 ## Getting Started
 
 [![YOUTUBE](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=A2gF4Sc2Sn0)
 
 The package has three different modules: 
 1. **EzGM.selection** deals with the record selection. 
    It can be used to perform unconditional or conditional spectrum based selection in which intensity measure can be chosen as Sa(T*) or AvgSa(T*). The tool makes use of 
-   [OpenQuake hazard library](https://docs.openquake.org/oq-engine/3.14/openquake.hazardlib.gsim.html#ground-shaking-intensity-models) and 
+   [OpenQuake hazard library](https://docs.openquake.org/oq-engine/3.16/reference/openquake.hazardlib.gsim.html#ground-shaking-intensity-models) and 
    thus any available ground motion prediction equation available can directly be used (see Example 1). <br />
    It can also be used to perform the selection based on Turkish Building Earthquake Code (TBEC-2018), ASCE 7-16, and Eurocode 8 Part 1 (see Example 2). <br />
    Currently, the records can be selected from the two publicly available databases: *NGA_W2* and *ESM_2018*. 
    The original flat-files for these databases were modified by discarding the records which are not possible to download. <br />
    The database files which include features to perform record selection are stored as .mat files in path/to/EzGM/Meta_Data.
    Upon installation, during the use of this module for the first time, the default Meta_Data folder will be downloaded from: https://drive.google.com/file/d/15cfA8rVB6uLG7T85HOrar7u0AaCOUdxt/view?usp=sharing.
    If users desire to use/add another database such as ESM_2018.mat, they must stick to the same format in publicly available databases. <br />
    Upon performing ground motion record selection/scaling if users desire to get formatted records, for the given metadata, they should place the available records from metadata file into the Records.zip with the name of database, 
    e.g. *ESM_2018.zip* for database *ESM_2018*. 
    <br /> In case of publicly available databases, users can also download the records directly by using the associated methods since the records are not generally available beforehand.
    To use *ESM_2018* database, users must have access token (path/to/current/directory/token.txt) from https://esm-db.eu. The token
-   can be retrieved using EzGM as well (see Example 1). In order to use *NGA_W2* database, users must have account obtained from https://ngawest2.berkeley.edu.
+   can be retrieved directly using EzGM as well if the user credentials are provided. In order to use *NGA_W2* database, users must have account obtained from https://ngawest2.berkeley.edu.
 2. **EzGM.utility** can be used to post-process results of probabilistic seismic hazard analysis (PSHA) from OpenQuake.Engine. Its methods can be used to read and visualize seismic hazard curves and seismic disaggregation results. The module can be particularly useful
 while performing conditional spectrum (CS) based record selection for multiple-stripe analysis (MSA) (see Example 3).
 3. **EzGM.signal** can be used to process ground motion records. It contains methods for filtering, baseline correction, and intensity measure calculations (see Example 4).
 
 At the moment, no documentation is available for EzGM; hence, users are recommended to see the jupyter notebook examples to get familiar with EzGM.
 These can be accessed and run through *binder* which is an online service to deploy interactive computational environments for online repositories. Likewise, the notebooks which are ready to use through google colaboratory can be accessed.
 For EzGM examples, see:
@@ -61,19 +61,23 @@
    ```
 - Nonetheless, in order to avoid any potential issues, the following is recommended for installation:
    1. First, create a clean python envrionment with python version greater than 3.7. Then, upgrade pip:
    ```
    pip install --upgrade pip
    ```
    2. Clone openquake.engine from https://github.com/gem/oq-engine, and open the terminal inside the clone directory. 
-   Activate the environment you want to install the package. Then, install the package via:
+   Activate the environment you want to install the package. Then, install the package requirements based on your system via:
+   ```
+   pip install -r requirements-py38-win64.txt
+   ```
+   3. Install OpenQuake:
    ```
    pip install -e .
    ```
-   3. Clone EzGM, and open the terminal inside the clone directory. 
+   4. Clone EzGM, and open the terminal inside the clone directory. 
    Activate the environment you want to install the package. Finally, install the package via the same command shown in the previous step.
 - Finally the package can be imported as:
 ```
 import EzGM
 ```
 ***
 ## Acknowledgements
```

### Comparing `EzGM-1.6.6.3/LICENSE` & `EzGM-1.7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EzGM-1.6.6.3/PKG-INFO` & `EzGM-1.7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EzGM
-Version: 1.6.6.3
+Version: 1.7.0.0
 Summary: Toolbox for ground motion record selection and processing
 Home-page: https://github.com/volkanozsarac/EzGM
 Author: Volkan Ozsarac
 Author-email: volkan.ozsarac@iusspavia.it
 Project-URL: Bug Tracker, https://github.com/volkanozsarac/EzGM/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -24,27 +24,27 @@
 ## Getting Started
 
 [![YOUTUBE](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=A2gF4Sc2Sn0)
 
 The package has three different modules: 
 1. **EzGM.selection** deals with the record selection. 
    It can be used to perform unconditional or conditional spectrum based selection in which intensity measure can be chosen as Sa(T*) or AvgSa(T*). The tool makes use of 
-   [OpenQuake hazard library](https://docs.openquake.org/oq-engine/3.14/openquake.hazardlib.gsim.html#ground-shaking-intensity-models) and 
+   [OpenQuake hazard library](https://docs.openquake.org/oq-engine/3.16/reference/openquake.hazardlib.gsim.html#ground-shaking-intensity-models) and 
    thus any available ground motion prediction equation available can directly be used (see Example 1). <br />
    It can also be used to perform the selection based on Turkish Building Earthquake Code (TBEC-2018), ASCE 7-16, and Eurocode 8 Part 1 (see Example 2). <br />
    Currently, the records can be selected from the two publicly available databases: *NGA_W2* and *ESM_2018*. 
    The original flat-files for these databases were modified by discarding the records which are not possible to download. <br />
    The database files which include features to perform record selection are stored as .mat files in path/to/EzGM/Meta_Data.
    Upon installation, during the use of this module for the first time, the default Meta_Data folder will be downloaded from: https://drive.google.com/file/d/15cfA8rVB6uLG7T85HOrar7u0AaCOUdxt/view?usp=sharing.
    If users desire to use/add another database such as ESM_2018.mat, they must stick to the same format in publicly available databases. <br />
    Upon performing ground motion record selection/scaling if users desire to get formatted records, for the given metadata, they should place the available records from metadata file into the Records.zip with the name of database, 
    e.g. *ESM_2018.zip* for database *ESM_2018*. 
    <br /> In case of publicly available databases, users can also download the records directly by using the associated methods since the records are not generally available beforehand.
    To use *ESM_2018* database, users must have access token (path/to/current/directory/token.txt) from https://esm-db.eu. The token
-   can be retrieved using EzGM as well (see Example 1). In order to use *NGA_W2* database, users must have account obtained from https://ngawest2.berkeley.edu.
+   can be retrieved directly using EzGM as well if the user credentials are provided. In order to use *NGA_W2* database, users must have account obtained from https://ngawest2.berkeley.edu.
 2. **EzGM.utility** can be used to post-process results of probabilistic seismic hazard analysis (PSHA) from OpenQuake.Engine. Its methods can be used to read and visualize seismic hazard curves and seismic disaggregation results. The module can be particularly useful
 while performing conditional spectrum (CS) based record selection for multiple-stripe analysis (MSA) (see Example 3).
 3. **EzGM.signal** can be used to process ground motion records. It contains methods for filtering, baseline correction, and intensity measure calculations (see Example 4).
 
 At the moment, no documentation is available for EzGM; hence, users are recommended to see the jupyter notebook examples to get familiar with EzGM.
 These can be accessed and run through *binder* which is an online service to deploy interactive computational environments for online repositories. Likewise, the notebooks which are ready to use through google colaboratory can be accessed.
 For EzGM examples, see:
@@ -61,19 +61,23 @@
    ```
 - Nonetheless, in order to avoid any potential issues, the following is recommended for installation:
    1. First, create a clean python envrionment with python version greater than 3.7. Then, upgrade pip:
    ```
    pip install --upgrade pip
    ```
    2. Clone openquake.engine from https://github.com/gem/oq-engine, and open the terminal inside the clone directory. 
-   Activate the environment you want to install the package. Then, install the package via:
+   Activate the environment you want to install the package. Then, install the package requirements based on your system via:
+   ```
+   pip install -r requirements-py38-win64.txt
+   ```
+   3. Install OpenQuake:
    ```
    pip install -e .
    ```
-   3. Clone EzGM, and open the terminal inside the clone directory. 
+   4. Clone EzGM, and open the terminal inside the clone directory. 
    Activate the environment you want to install the package. Finally, install the package via the same command shown in the previous step.
 - Finally the package can be imported as:
 ```
 import EzGM
 ```
 ***
 ## Acknowledgements
```

### Comparing `EzGM-1.6.6.3/README.md` & `EzGM-1.7.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 ## Getting Started
 
 [![YOUTUBE](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=A2gF4Sc2Sn0)
 
 The package has three different modules: 
 1. **EzGM.selection** deals with the record selection. 
    It can be used to perform unconditional or conditional spectrum based selection in which intensity measure can be chosen as Sa(T*) or AvgSa(T*). The tool makes use of 
-   [OpenQuake hazard library](https://docs.openquake.org/oq-engine/3.14/openquake.hazardlib.gsim.html#ground-shaking-intensity-models) and 
+   [OpenQuake hazard library](https://docs.openquake.org/oq-engine/3.16/reference/openquake.hazardlib.gsim.html#ground-shaking-intensity-models) and 
    thus any available ground motion prediction equation available can directly be used (see Example 1). <br />
    It can also be used to perform the selection based on Turkish Building Earthquake Code (TBEC-2018), ASCE 7-16, and Eurocode 8 Part 1 (see Example 2). <br />
    Currently, the records can be selected from the two publicly available databases: *NGA_W2* and *ESM_2018*. 
    The original flat-files for these databases were modified by discarding the records which are not possible to download. <br />
    The database files which include features to perform record selection are stored as .mat files in path/to/EzGM/Meta_Data.
    Upon installation, during the use of this module for the first time, the default Meta_Data folder will be downloaded from: https://drive.google.com/file/d/15cfA8rVB6uLG7T85HOrar7u0AaCOUdxt/view?usp=sharing.
    If users desire to use/add another database such as ESM_2018.mat, they must stick to the same format in publicly available databases. <br />
    Upon performing ground motion record selection/scaling if users desire to get formatted records, for the given metadata, they should place the available records from metadata file into the Records.zip with the name of database, 
    e.g. *ESM_2018.zip* for database *ESM_2018*. 
    <br /> In case of publicly available databases, users can also download the records directly by using the associated methods since the records are not generally available beforehand.
    To use *ESM_2018* database, users must have access token (path/to/current/directory/token.txt) from https://esm-db.eu. The token
-   can be retrieved using EzGM as well (see Example 1). In order to use *NGA_W2* database, users must have account obtained from https://ngawest2.berkeley.edu.
+   can be retrieved directly using EzGM as well if the user credentials are provided. In order to use *NGA_W2* database, users must have account obtained from https://ngawest2.berkeley.edu.
 2. **EzGM.utility** can be used to post-process results of probabilistic seismic hazard analysis (PSHA) from OpenQuake.Engine. Its methods can be used to read and visualize seismic hazard curves and seismic disaggregation results. The module can be particularly useful
 while performing conditional spectrum (CS) based record selection for multiple-stripe analysis (MSA) (see Example 3).
 3. **EzGM.signal** can be used to process ground motion records. It contains methods for filtering, baseline correction, and intensity measure calculations (see Example 4).
 
 At the moment, no documentation is available for EzGM; hence, users are recommended to see the jupyter notebook examples to get familiar with EzGM.
 These can be accessed and run through *binder* which is an online service to deploy interactive computational environments for online repositories. Likewise, the notebooks which are ready to use through google colaboratory can be accessed.
 For EzGM examples, see:
@@ -45,19 +45,23 @@
    ```
 - Nonetheless, in order to avoid any potential issues, the following is recommended for installation:
    1. First, create a clean python envrionment with python version greater than 3.7. Then, upgrade pip:
    ```
    pip install --upgrade pip
    ```
    2. Clone openquake.engine from https://github.com/gem/oq-engine, and open the terminal inside the clone directory. 
-   Activate the environment you want to install the package. Then, install the package via:
+   Activate the environment you want to install the package. Then, install the package requirements based on your system via:
+   ```
+   pip install -r requirements-py38-win64.txt
+   ```
+   3. Install OpenQuake:
    ```
    pip install -e .
    ```
-   3. Clone EzGM, and open the terminal inside the clone directory. 
+   4. Clone EzGM, and open the terminal inside the clone directory. 
    Activate the environment you want to install the package. Finally, install the package via the same command shown in the previous step.
 - Finally the package can be imported as:
 ```
 import EzGM
 ```
 ***
 ## Acknowledgements
```

### Comparing `EzGM-1.6.6.3/setup.cfg` & `EzGM-1.7.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2045 7a47 4d0d 0a76 6572 7369 6f6e   = EzGM..version
-00000020: 203d 2031 2e36 2e36 2e33 0d0a 6175 7468   = 1.6.6.3..auth
+00000020: 203d 2031 2e37 2e30 2e30 0d0a 6175 7468   = 1.7.0.0..auth
 00000030: 6f72 203d 2056 6f6c 6b61 6e20 4f7a 7361  or = Volkan Ozsa
 00000040: 7261 630d 0a61 7574 686f 725f 656d 6169  rac..author_emai
 00000050: 6c20 3d20 766f 6c6b 616e 2e6f 7a73 6172  l = volkan.ozsar
 00000060: 6163 4069 7573 7370 6176 6961 2e69 740d  ac@iusspavia.it.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2054  .description = T
 00000080: 6f6f 6c62 6f78 2066 6f72 2067 726f 756e  oolbox for groun
 00000090: 6420 6d6f 7469 6f6e 2072 6563 6f72 6420  d motion record
```

