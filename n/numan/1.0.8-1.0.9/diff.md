# Comparing `tmp/numan-1.0.8.tar.gz` & `tmp/numan-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numan-1.0.8.tar", last modified: Wed Jul  5 18:39:55 2023, max compression
+gzip compressed data, was "numan-1.0.9.tar", last modified: Thu Jul  6 19:22:24 2023, max compression
```

## Comparing `numan-1.0.8.tar` & `numan-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 18:39:55.596357 numan-1.0.8/
--rw-rw-rw-   0        0        0     1094 2022-05-18 18:25:15.000000 numan-1.0.8/LICENSE.md
--rw-rw-rw-   0        0        0     2181 2023-07-05 18:39:55.594345 numan-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1558 2022-05-18 18:25:15.000000 numan-1.0.8/README.md
--rw-rw-rw-   0        0        0     1314 2023-07-05 18:38:51.000000 numan-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 18:39:55.597357 numan-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0       53 2022-08-16 05:16:10.000000 numan-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 18:39:55.472558 numan-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 18:39:55.557557 numan-1.0.8/src/numan/
--rw-rw-rw-   0        0        0      224 2023-07-05 18:39:03.000000 numan-1.0.8/src/numan/__init__.py
--rw-rw-rw-   0        0        0    45479 2023-07-05 18:23:16.000000 numan-1.0.8/src/numan/analysis.py
--rw-rw-rw-   0        0        0     1382 2022-08-18 08:58:12.000000 numan-1.0.8/src/numan/notifications.py
--rw-rw-rw-   0        0        0    32617 2022-09-25 04:39:18.000000 numan-1.0.8/src/numan/plots.py
--rw-rw-rw-   0        0        0     1097 2022-08-18 04:32:02.000000 numan-1.0.8/src/numan/project.py
--rw-rw-rw-   0        0        0    27184 2023-07-03 21:12:36.000000 numan-1.0.8/src/numan/report.py
--rw-rw-rw-   0        0        0     3396 2022-08-21 22:45:27.000000 numan-1.0.8/src/numan/runner.py
--rw-rw-rw-   0        0        0     6437 2023-07-03 19:08:23.000000 numan-1.0.8/src/numan/utils.py
--rw-rw-rw-   0        0        0    31015 2023-06-06 20:27:40.000000 numan-1.0.8/src/numan/visualization.py
-drwxrwxrwx   0        0        0        0 2023-07-05 18:39:55.581563 numan-1.0.8/src/numan.egg-info/
--rw-rw-rw-   0        0        0     2181 2023-07-05 18:39:55.000000 numan-1.0.8/src/numan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2023-07-05 18:39:55.000000 numan-1.0.8/src/numan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 18:39:55.000000 numan-1.0.8/src/numan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2023-07-05 18:39:55.000000 numan-1.0.8/src/numan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-05 18:39:55.000000 numan-1.0.8/src/numan.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-05 18:39:55.591596 numan-1.0.8/tests/
--rw-rw-rw-   0        0        0    15043 2022-11-29 19:20:20.000000 numan-1.0.8/tests/test_plots.py
--rw-rw-rw-   0        0        0     2153 2023-07-03 19:08:23.000000 numan-1.0.8/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 19:22:24.247105 numan-1.0.9/
+-rw-rw-rw-   0        0        0     1094 2022-05-18 18:25:15.000000 numan-1.0.9/LICENSE.md
+-rw-rw-rw-   0        0        0     2181 2023-07-06 19:22:24.247105 numan-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1558 2022-05-18 18:25:15.000000 numan-1.0.9/README.md
+-rw-rw-rw-   0        0        0     1314 2023-07-06 19:21:25.000000 numan-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 19:22:24.248091 numan-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       53 2022-08-16 05:16:10.000000 numan-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 19:22:24.136089 numan-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 19:22:24.212089 numan-1.0.9/src/numan/
+-rw-rw-rw-   0        0        0      224 2023-07-06 19:21:33.000000 numan-1.0.9/src/numan/__init__.py
+-rw-rw-rw-   0        0        0    45479 2023-07-05 18:23:16.000000 numan-1.0.9/src/numan/analysis.py
+-rw-rw-rw-   0        0        0     1382 2022-08-18 08:58:12.000000 numan-1.0.9/src/numan/notifications.py
+-rw-rw-rw-   0        0        0    32617 2022-09-25 04:39:18.000000 numan-1.0.9/src/numan/plots.py
+-rw-rw-rw-   0        0        0     1097 2022-08-18 04:32:02.000000 numan-1.0.9/src/numan/project.py
+-rw-rw-rw-   0        0        0    27665 2023-07-06 19:14:10.000000 numan-1.0.9/src/numan/report.py
+-rw-rw-rw-   0        0        0     3396 2022-08-21 22:45:27.000000 numan-1.0.9/src/numan/runner.py
+-rw-rw-rw-   0        0        0     6437 2023-07-03 19:08:23.000000 numan-1.0.9/src/numan/utils.py
+-rw-rw-rw-   0        0        0    31015 2023-06-06 20:27:40.000000 numan-1.0.9/src/numan/visualization.py
+drwxrwxrwx   0        0        0        0 2023-07-06 19:22:24.236091 numan-1.0.9/src/numan.egg-info/
+-rw-rw-rw-   0        0        0     2181 2023-07-06 19:22:24.000000 numan-1.0.9/src/numan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-07-06 19:22:24.000000 numan-1.0.9/src/numan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 19:22:24.000000 numan-1.0.9/src/numan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-07-06 19:22:24.000000 numan-1.0.9/src/numan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 19:22:24.000000 numan-1.0.9/src/numan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 19:22:24.245126 numan-1.0.9/tests/
+-rw-rw-rw-   0        0        0    15043 2022-11-29 19:20:20.000000 numan-1.0.9/tests/test_plots.py
+-rw-rw-rw-   0        0        0     2153 2023-07-03 19:08:23.000000 numan-1.0.9/tests/test_utils.py
```

### Comparing `numan-1.0.8/LICENSE.md` & `numan-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `numan-1.0.8/PKG-INFO` & `numan-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numan
-Version: 1.0.8
+Version: 1.0.9
 Summary: numerosity analysis package
 Author-email: Anna Nadtochiy <nadtochi@usc.edu>
 Project-URL: Homepage, https://github.com/LemonJust/numan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `numan-1.0.8/README.md` & `numan-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `numan-1.0.8/pyproject.toml` & `numan-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "numan"
-version = "1.0.8"
+version = "1.0.9"
 description='numerosity analysis package'
 readme = "README.md"
 authors = [{ name = "Anna Nadtochiy", email = "nadtochi@usc.edu" }]
 license = { file = "LICENSE" }
 classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Science/Research',
@@ -34,15 +34,15 @@
 [project.optional-dependencies]
 dev = ["bumpver"]
 
 [project.urls] # Read The Docs will also go in here
 Homepage = "https://github.com/LemonJust/numan"
 
 [tool.bumpver]
-current_version = "1.0.8"
+current_version = "1.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `numan-1.0.8/src/numan/analysis.py` & `numan-1.0.9/src/numan/analysis.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.8/src/numan/notifications.py` & `numan-1.0.9/src/numan/notifications.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.8/src/numan/plots.py` & `numan-1.0.9/src/numan/plots.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.8/src/numan/project.py` & `numan-1.0.9/src/numan/project.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.8/src/numan/report.py` & `numan-1.0.9/src/numan/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,14 +106,15 @@
             signal_idx = np.array([el[3] for el in sorted_zip])
 
         return cells_group, cells_idx, cells_zyx, signal_idx
 
     def make_signal_reports(self,
                             spot_tag, group_tag,
                             annotation_type,
+                            dff_param,
                             labels=None,
                             plot_type="cycle",
                             plot_type_tag='',
                             forward_shift=0,
                             plot_individual=False,
                             groups_to_specify=("sig2v3", "sig2v5", "sig3v5", "sig2vB", "sig3vB", "sig5vB"),
                             tmp_folder=None,
@@ -126,14 +127,17 @@
         :type checkbox:
         :param groups_to_specify:
         :type groups_to_specify:
         :param labels:
         :type labels:
         :param annotation_type:
         :type annotation_type:
+        :param dff_param: parameters for dff calculation (see Signals.as_dff).
+            For example {"method":"sliding", "window":15} or {"method":"step", "step_size":9, "baseline_volumes": [0,1,2]}
+        :type dff_param: dict
         :param spot_tag: what set of spots to use. Chooses the spots*.json based on this.
         :type spot_tag: str
         :param group_tag: what spots group to use.
         :type group_tag: str
         :param plot_type: what plot to output ["cycle","psh_0","psh_b"]
         :type plot_type: str
         :param plot_type_tag: just for the pdf naming : this is to be able to distinguish
@@ -159,14 +163,16 @@
         :param tmp_folder: will store batch images in this folder before merging pdf,
                     will be stored with reports if left None.
         :type tmp_folder: Union(str, Path)
         :param pdf_filename: the name of the pdf file to save, will be generated automatically if left None
         :type pdf_filename: str
 
         """
+        if plot_type == "cycle":
+            assert dff_param["method"] == "sliding", "Cycle plots only work with sliding dff"
         if plot_type == "psh_0" or plot_type == "psh_b":
             assert labels is not None, "Labels must not be None for psh-type plots"
 
         # fill out the defaults
         if tmp_folder is None:
             if checkbox:
                 # where to temporary store images while the code is running
@@ -184,17 +190,16 @@
                 # filename to save pdf with all the significant traces
                 pdf_filename = f"{self.project}/spots/reports/all_significant/signals/" \
                                f"{plot_type}{plot_type_tag}_from_{spot_tag}_group_{group_tag}.pdf"
 
         spots = Spots.from_json(f"{self.project}/spots/signals/spots_{spot_tag}.json")
 
         # initialise the signal plotter with DFF signal
-        SLIDING_WINDOW = 15  # in volumes
-        print(f"Using sliding window {SLIDING_WINDOW} volumes for signal DFF")
-        signals = spots.get_group_signals(spots.groups[group_tag]).as_dff(SLIDING_WINDOW)
+        print(f"Using the following parameters for signal DFF: {dff_param}")
+        signals = spots.get_group_signals(spots.groups[group_tag]).as_dff(**dff_param)
         s_plotter = SignalPlotter(signals, self.experiment, annotation_type)
 
         # prepare title info
         cells_group, cells_idx, cells_zyx, signal_idx = self.prepare_spot_info(spots, group_tag,
                                                                                s_plotter.n_traces,
                                                                                sort_by_sig=True,
                                                                                groups_to_specify=groups_to_specify)
@@ -281,31 +286,31 @@
             create_checkbox_pdf(plot_files, cells_idx_txt, btchs, pdf_filename)
         else:
             merge_pdfs(plot_files, pdf_filename)
 
     def make_avg_intensity_reports(self,
                                    spot_tag, group_tag,
                                    annotation_type,
+                                   dff_param,
                                    labels,
                                    number_cells=False,
                                    plot_type_tag='',
                                    pdf_filename=None):
 
         if pdf_filename is None:
             # filename to save pdf with all the significant traces
             pdf_filename = f"{self.project}/spots/reports/all_significant/signals/" \
                            f"avg_intensity_scatterplot{plot_type_tag}_from_{spot_tag}_group_{group_tag}.pdf"
 
         spots = Spots.from_json(f"{self.project}/spots/signals/spots_{spot_tag}.json")
         cells_idx = spots.get_group_idx(spots.groups[group_tag])
 
         # initialise the signal plotter with DFF signal
-        SLIDING_WINDOW = 15  # in volumes
-        print(f"Using sliding window {SLIDING_WINDOW} volumes for signal DFF")
-        signals = spots.get_group_signals(spots.groups[group_tag]).as_dff(SLIDING_WINDOW)
+        print(f"Using the following parameters for signal DFF: {dff_param}")
+        signals = spots.get_group_signals(spots.groups[group_tag]).as_dff(**dff_param)
         s_plotter = SignalPlotter(signals, self.experiment, annotation_type)
 
         # prepare title info
         main_title = f"Average DFF per stimuli, pairwise comparison."
 
         # figure out figure layout
         if len(labels) == 3:
@@ -328,14 +333,15 @@
 
         plt.savefig(pdf_filename)
         plt.close()
 
     def make_covariate_reports(self,
                                spot_tag, group_tag,
                                annotation_type,
+                               dff_param,
                                conditions=None,
                                plot_type="cycle",
                                plot_type_tag='',
                                forward_shift=0,
                                plot_individual=False,
                                groups_to_specify=("sig2v3", "sig2v5", "sig3v5", "sig2vB", "sig3vB", "sig5vB"),
                                tmp_folder=None,
@@ -380,14 +386,17 @@
         :param tmp_folder: will store batch images in this folder before merging pdf,
                     will be stored with reports if left None.
         :type tmp_folder: Union(str, Path)
         :param pdf_filename: the name of the pdf file to save, will be generated automatically if left None
         :type pdf_filename: str
 
         """
+        if plot_type == "cycle":
+            assert dff_param["method"] == "sliding", "Cycle plots only work with sliding dff"
+
         assert conditions is not None, "Conditions must not be None for psh-type plots"
 
         # fill out the defaults
         if tmp_folder is None:
             # where to temporary store images while the code is running
             tmp_folder = f"{self.project}/spots/reports/covariates/signals/"
 
@@ -395,17 +404,16 @@
             # filename to save pdf with all the significant traces
             pdf_filename = f"{self.project}/spots/reports/covariates/signals/" \
                            f"{plot_type}{plot_type_tag}_from_{spot_tag}_group_{group_tag}.pdf"
 
         spots = Spots.from_json(f"{self.project}/spots/signals/spots_{spot_tag}.json")
 
         # initialise the signal plotter with DFF signal
-        SLIDING_WINDOW = 15  # in volumes
-        print(f"Using sliding window {SLIDING_WINDOW} volumes for signal DFF")
-        signals = spots.get_group_signals(spots.groups[group_tag]).as_dff(SLIDING_WINDOW)
+        print(f"Using the following parameters for signal DFF: {dff_param}")
+        signals = spots.get_group_signals(spots.groups[group_tag]).as_dff(**dff_param)
 
         # choose traces per page
         if plot_type == "psh_0":
             tpp = 10  # traces per page
             s_plotter = SignalPlotter(signals, self.experiment, annotation_type,
                                       c_mean_color='w', c_noise_color='-m', c_edge_color='w')
         else:
```

### Comparing `numan-1.0.8/src/numan/runner.py` & `numan-1.0.9/src/numan/runner.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.8/src/numan/utils.py` & `numan-1.0.9/src/numan/utils.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.8/src/numan/visualization.py` & `numan-1.0.9/src/numan/visualization.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.8/src/numan.egg-info/PKG-INFO` & `numan-1.0.9/src/numan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numan
-Version: 1.0.8
+Version: 1.0.9
 Summary: numerosity analysis package
 Author-email: Anna Nadtochiy <nadtochi@usc.edu>
 Project-URL: Homepage, https://github.com/LemonJust/numan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `numan-1.0.8/tests/test_plots.py` & `numan-1.0.9/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.8/tests/test_utils.py` & `numan-1.0.9/tests/test_utils.py`

 * *Files identical despite different names*

