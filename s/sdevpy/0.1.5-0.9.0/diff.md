# Comparing `tmp/sdevpy-0.1.5.tar.gz` & `tmp/sdevpy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdevpy-0.1.5.tar", last modified: Tue Jun 27 07:38:13 2023, max compression
+gzip compressed data, was "sdevpy-0.9.0.tar", last modified: Thu Jul  6 06:56:09 2023, max compression
```

## Comparing `sdevpy-0.1.5.tar` & `sdevpy-0.9.0.tar`

### file list

```diff
@@ -1,63 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 07:38:13.651656 sdevpy-0.1.5/
--rw-rw-rw-   0        0        0     1098 2023-06-17 02:41:33.000000 sdevpy-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1725 2023-06-27 07:38:13.649656 sdevpy-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1206 2023-06-18 08:19:59.000000 sdevpy-0.1.5/README.md
--rw-rw-rw-   0        0        0      695 2023-06-27 07:34:23.000000 sdevpy-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-27 07:38:13.651656 sdevpy-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-27 07:38:13.251786 sdevpy-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-27 07:38:13.290773 sdevpy-0.1.5/src/sdevpy/
--rw-rw-rw-   0        0        0       23 2023-06-27 07:34:31.000000 sdevpy-0.1.5/src/sdevpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:38:13.379745 sdevpy-0.1.5/src/sdevpy/analytics/
--rw-rw-rw-   0        0        0     2415 2023-04-15 10:09:55.000000 sdevpy-0.1.5/src/sdevpy/analytics/bachelier.py
--rw-rw-rw-   0        0        0     2810 2023-06-20 03:38:43.000000 sdevpy-0.1.5/src/sdevpy/analytics/black.py
--rw-rw-rw-   0        0        0     6316 2023-06-22 09:20:26.000000 sdevpy-0.1.5/src/sdevpy/analytics/fbsabr.py
--rw-rw-rw-   0        0        0     6913 2023-06-24 04:26:35.000000 sdevpy-0.1.5/src/sdevpy/analytics/mcheston.py
--rw-rw-rw-   0        0        0     7657 2023-06-20 03:43:39.000000 sdevpy-0.1.5/src/sdevpy/analytics/mcsabr.py
--rw-rw-rw-   0        0        0     8747 2023-06-27 03:03:31.000000 sdevpy-0.1.5/src/sdevpy/analytics/mczabr.py
--rw-rw-rw-   0        0        0     2790 2023-05-07 07:20:24.000000 sdevpy-0.1.5/src/sdevpy/analytics/sabr.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:38:13.431728 sdevpy-0.1.5/src/sdevpy/machinelearning/
--rw-rw-rw-   0        0        0     4350 2023-06-19 11:59:56.000000 sdevpy-0.1.5/src/sdevpy/machinelearning/callbacks.py
--rw-rw-rw-   0        0        0     2510 2023-06-26 08:54:39.000000 sdevpy-0.1.5/src/sdevpy/machinelearning/datasets.py
--rw-rw-rw-   0        0        0     6101 2023-06-20 09:15:35.000000 sdevpy-0.1.5/src/sdevpy/machinelearning/learningmodel.py
--rw-rw-rw-   0        0        0      997 2023-05-01 01:07:36.000000 sdevpy-0.1.5/src/sdevpy/machinelearning/learningschedules.py
--rw-rw-rw-   0        0        0     2390 2023-04-08 04:29:36.000000 sdevpy-0.1.5/src/sdevpy/machinelearning/topology.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:38:13.454721 sdevpy-0.1.5/src/sdevpy/maths/
--rw-rw-rw-   0        0        0      840 2023-06-20 06:44:09.000000 sdevpy-0.1.5/src/sdevpy/maths/interpolations.py
--rw-rw-rw-   0        0        0      654 2023-06-24 09:12:10.000000 sdevpy-0.1.5/src/sdevpy/maths/metrics.py
--rw-rw-rw-   0        0        0       85 2022-11-12 05:23:02.000000 sdevpy-0.1.5/src/sdevpy/maths/optimization.py
--rw-rw-rw-   0        0        0     3773 2023-05-20 06:07:54.000000 sdevpy-0.1.5/src/sdevpy/maths/rand.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:38:13.457719 sdevpy-0.1.5/src/sdevpy/projects/
--rw-rw-rw-   0        0        0      893 2023-06-25 05:21:23.000000 sdevpy-0.1.5/src/sdevpy/projects/datafiles.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:38:13.494708 sdevpy-0.1.5/src/sdevpy/projects/pinns/
--rw-rw-rw-   0        0        0    10211 2022-11-29 00:51:51.000000 sdevpy-0.1.5/src/sdevpy/projects/pinns/ernst_pinns.py
--rw-rw-rw-   0        0        0    11863 2022-12-19 07:49:15.000000 sdevpy-0.1.5/src/sdevpy/projects/pinns/pinns.py
--rw-rw-rw-   0        0        0    23680 2023-02-26 08:44:57.000000 sdevpy-0.1.5/src/sdevpy/projects/pinns/pinns_worst_of.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:38:13.528696 sdevpy-0.1.5/src/sdevpy/projects/stovol/
--rw-rw-rw-   0        0        0     3361 2023-06-27 02:50:04.000000 sdevpy-0.1.5/src/sdevpy/projects/stovol/stovolgen.py
--rw-rw-rw-   0        0        0     5033 2023-06-21 13:31:09.000000 sdevpy-0.1.5/src/sdevpy/projects/stovol/stovolplot.py
--rw-rw-rw-   0        0        0    11084 2023-06-27 02:46:03.000000 sdevpy-0.1.5/src/sdevpy/projects/stovol/stovoltrain.py
--rw-rw-rw-   0        0        0      400 2023-06-19 11:47:07.000000 sdevpy-0.1.5/src/sdevpy/settings.py
--rw-rw-rw-   0        0        0     7644 2023-06-26 06:59:16.000000 sdevpy-0.1.5/src/sdevpy/test.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:38:13.575681 sdevpy-0.1.5/src/sdevpy/tools/
--rw-rw-rw-   0        0        0     1048 2023-06-20 09:17:04.000000 sdevpy-0.1.5/src/sdevpy/tools/clipboard.py
--rw-rw-rw-   0        0        0       48 2023-04-16 03:13:45.000000 sdevpy-0.1.5/src/sdevpy/tools/constants.py
--rw-rw-rw-   0        0        0     1759 2023-06-25 09:09:17.000000 sdevpy-0.1.5/src/sdevpy/tools/filemanager.py
--rw-rw-rw-   0        0        0     1190 2023-06-10 07:03:10.000000 sdevpy-0.1.5/src/sdevpy/tools/jsonmanager.py
--rw-rw-rw-   0        0        0     3426 2023-06-24 04:23:59.000000 sdevpy-0.1.5/src/sdevpy/tools/timegrids.py
--rw-rw-rw-   0        0        0      867 2023-04-09 05:08:45.000000 sdevpy-0.1.5/src/sdevpy/tools/timer.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:38:13.638660 sdevpy-0.1.5/src/sdevpy/volsurfacegen/
--rw-rw-rw-   0        0        0     2377 2023-06-24 06:47:56.000000 sdevpy-0.1.5/src/sdevpy/volsurfacegen/fbsabrgenerator.py
--rw-rw-rw-   0        0        0     9160 2023-06-24 06:47:14.000000 sdevpy-0.1.5/src/sdevpy/volsurfacegen/mchestongenerator.py
--rw-rw-rw-   0        0        0     2534 2023-06-24 06:42:09.000000 sdevpy-0.1.5/src/sdevpy/volsurfacegen/mcsabrgenerator.py
--rw-rw-rw-   0        0        0     8564 2023-06-24 06:46:09.000000 sdevpy-0.1.5/src/sdevpy/volsurfacegen/mczabrgenerator.py
--rw-rw-rw-   0        0        0     9278 2023-06-24 06:37:02.000000 sdevpy-0.1.5/src/sdevpy/volsurfacegen/sabrgenerator.py
--rw-rw-rw-   0        0        0     5807 2023-06-24 05:59:47.000000 sdevpy-0.1.5/src/sdevpy/volsurfacegen/smilegenerator.py
--rw-rw-rw-   0        0        0     1705 2023-06-24 06:53:18.000000 sdevpy-0.1.5/src/sdevpy/volsurfacegen/stovolfactory.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:38:13.320763 sdevpy-0.1.5/src/sdevpy.egg-info/
--rw-rw-rw-   0        0        0     1725 2023-06-27 07:38:13.000000 sdevpy-0.1.5/src/sdevpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1591 2023-06-27 07:38:13.000000 sdevpy-0.1.5/src/sdevpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 07:38:13.000000 sdevpy-0.1.5/src/sdevpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-27 07:38:13.000000 sdevpy-0.1.5/src/sdevpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-27 07:38:13.000000 sdevpy-0.1.5/src/sdevpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-27 07:38:13.648657 sdevpy-0.1.5/tests/
--rw-rw-rw-   0        0        0      212 2023-06-18 06:08:53.000000 sdevpy-0.1.5/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:56:09.795324 sdevpy-0.9.0/
+-rw-rw-rw-   0        0        0     1098 2023-06-17 02:41:33.000000 sdevpy-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0     2349 2023-07-06 06:56:09.794324 sdevpy-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-07-04 08:24:33.000000 sdevpy-0.9.0/README.md
+-rw-rw-rw-   0        0        0      695 2023-07-04 08:14:00.000000 sdevpy-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 06:56:09.795324 sdevpy-0.9.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 06:56:09.446437 sdevpy-0.9.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 06:56:09.472428 sdevpy-0.9.0/src/sdevpy/
+-rw-rw-rw-   0        0        0       23 2023-07-06 06:52:31.000000 sdevpy-0.9.0/src/sdevpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:56:09.560400 sdevpy-0.9.0/src/sdevpy/analytics/
+-rw-rw-rw-   0        0        0     2415 2023-04-15 10:09:55.000000 sdevpy-0.9.0/src/sdevpy/analytics/bachelier.py
+-rw-rw-rw-   0        0        0     2810 2023-06-20 03:38:43.000000 sdevpy-0.9.0/src/sdevpy/analytics/black.py
+-rw-rw-rw-   0        0        0     6316 2023-06-22 09:20:26.000000 sdevpy-0.9.0/src/sdevpy/analytics/fbsabr.py
+-rw-rw-rw-   0        0        0     6911 2023-07-04 04:34:26.000000 sdevpy-0.9.0/src/sdevpy/analytics/mcheston.py
+-rw-rw-rw-   0        0        0     7657 2023-06-20 03:43:39.000000 sdevpy-0.9.0/src/sdevpy/analytics/mcsabr.py
+-rw-rw-rw-   0        0        0     8747 2023-06-27 03:03:31.000000 sdevpy-0.9.0/src/sdevpy/analytics/mczabr.py
+-rw-rw-rw-   0        0        0     2790 2023-05-07 07:20:24.000000 sdevpy-0.9.0/src/sdevpy/analytics/sabr.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:56:09.593390 sdevpy-0.9.0/src/sdevpy/machinelearning/
+-rw-rw-rw-   0        0        0     4350 2023-06-19 11:59:56.000000 sdevpy-0.9.0/src/sdevpy/machinelearning/callbacks.py
+-rw-rw-rw-   0        0        0     2510 2023-06-26 08:54:39.000000 sdevpy-0.9.0/src/sdevpy/machinelearning/datasets.py
+-rw-rw-rw-   0        0        0     6101 2023-06-20 09:15:35.000000 sdevpy-0.9.0/src/sdevpy/machinelearning/learningmodel.py
+-rw-rw-rw-   0        0        0      997 2023-05-01 01:07:36.000000 sdevpy-0.9.0/src/sdevpy/machinelearning/learningschedules.py
+-rw-rw-rw-   0        0        0     2390 2023-04-08 04:29:36.000000 sdevpy-0.9.0/src/sdevpy/machinelearning/topology.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:56:09.622380 sdevpy-0.9.0/src/sdevpy/maths/
+-rw-rw-rw-   0        0        0      840 2023-06-20 06:44:09.000000 sdevpy-0.9.0/src/sdevpy/maths/interpolations.py
+-rw-rw-rw-   0        0        0      654 2023-06-24 09:12:10.000000 sdevpy-0.9.0/src/sdevpy/maths/metrics.py
+-rw-rw-rw-   0        0        0       85 2022-11-12 05:23:02.000000 sdevpy-0.9.0/src/sdevpy/maths/optimization.py
+-rw-rw-rw-   0        0        0     3773 2023-05-20 06:07:54.000000 sdevpy-0.9.0/src/sdevpy/maths/rand.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:56:09.632377 sdevpy-0.9.0/src/sdevpy/projects/
+-rw-rw-rw-   0        0        0      893 2023-06-25 05:21:23.000000 sdevpy-0.9.0/src/sdevpy/projects/datafiles.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:56:09.664368 sdevpy-0.9.0/src/sdevpy/projects/stovol/
+-rw-rw-rw-   0        0        0     3732 2023-07-05 19:36:23.000000 sdevpy-0.9.0/src/sdevpy/projects/stovol/stovolgen.py
+-rw-rw-rw-   0        0        0     3851 2023-07-04 06:40:20.000000 sdevpy-0.9.0/src/sdevpy/projects/stovol/stovolplot.py
+-rw-rw-rw-   0        0        0    11225 2023-07-06 06:42:17.000000 sdevpy-0.9.0/src/sdevpy/projects/stovol/stovoltrain.py
+-rw-rw-rw-   0        0        0      400 2023-06-19 11:47:07.000000 sdevpy-0.9.0/src/sdevpy/settings.py
+-rw-rw-rw-   0        0        0     7644 2023-06-26 06:59:16.000000 sdevpy-0.9.0/src/sdevpy/test.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:56:09.722347 sdevpy-0.9.0/src/sdevpy/tools/
+-rw-rw-rw-   0        0        0     1048 2023-06-20 09:17:04.000000 sdevpy-0.9.0/src/sdevpy/tools/clipboard.py
+-rw-rw-rw-   0        0        0       48 2023-04-16 03:13:45.000000 sdevpy-0.9.0/src/sdevpy/tools/constants.py
+-rw-rw-rw-   0        0        0     1759 2023-06-25 09:09:17.000000 sdevpy-0.9.0/src/sdevpy/tools/filemanager.py
+-rw-rw-rw-   0        0        0     1190 2023-06-10 07:03:10.000000 sdevpy-0.9.0/src/sdevpy/tools/jsonmanager.py
+-rw-rw-rw-   0        0        0     3426 2023-06-24 04:23:59.000000 sdevpy-0.9.0/src/sdevpy/tools/timegrids.py
+-rw-rw-rw-   0        0        0      867 2023-04-09 05:08:45.000000 sdevpy-0.9.0/src/sdevpy/tools/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:56:09.784328 sdevpy-0.9.0/src/sdevpy/volsurfacegen/
+-rw-rw-rw-   0        0        0     2377 2023-06-24 06:47:56.000000 sdevpy-0.9.0/src/sdevpy/volsurfacegen/fbsabrgenerator.py
+-rw-rw-rw-   0        0        0     9160 2023-06-24 06:47:14.000000 sdevpy-0.9.0/src/sdevpy/volsurfacegen/mchestongenerator.py
+-rw-rw-rw-   0        0        0     2534 2023-06-24 06:42:09.000000 sdevpy-0.9.0/src/sdevpy/volsurfacegen/mcsabrgenerator.py
+-rw-rw-rw-   0        0        0     8564 2023-06-24 06:46:09.000000 sdevpy-0.9.0/src/sdevpy/volsurfacegen/mczabrgenerator.py
+-rw-rw-rw-   0        0        0     9278 2023-06-24 06:37:02.000000 sdevpy-0.9.0/src/sdevpy/volsurfacegen/sabrgenerator.py
+-rw-rw-rw-   0        0        0     5807 2023-06-24 05:59:47.000000 sdevpy-0.9.0/src/sdevpy/volsurfacegen/smilegenerator.py
+-rw-rw-rw-   0        0        0     1729 2023-07-02 10:32:58.000000 sdevpy-0.9.0/src/sdevpy/volsurfacegen/stovolfactory.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:56:09.501419 sdevpy-0.9.0/src/sdevpy.egg-info/
+-rw-rw-rw-   0        0        0     2349 2023-07-06 06:56:09.000000 sdevpy-0.9.0/src/sdevpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1471 2023-07-06 06:56:09.000000 sdevpy-0.9.0/src/sdevpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 06:56:09.000000 sdevpy-0.9.0/src/sdevpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-06 06:56:09.000000 sdevpy-0.9.0/src/sdevpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 06:56:09.000000 sdevpy-0.9.0/src/sdevpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 06:56:09.793326 sdevpy-0.9.0/tests/
+-rw-rw-rw-   0        0        0      212 2023-06-18 06:08:53.000000 sdevpy-0.9.0/tests/test.py
```

### Comparing `sdevpy-0.1.5/LICENSE` & `sdevpy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/PKG-INFO` & `sdevpy-0.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 Metadata-Version: 2.1
 Name: sdevpy
-Version: 0.1.5
+Version: 0.9.0
 Summary: Python package for Machine Learning in Finance
 Author-email: Sebastien Gurrieri <sebgur@gmail.com>
 Project-URL: Git page, https://github.com/sebgur/SDev.Python
 Project-URL: SDev Finance, http://sdev-finance.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SDev.Python
 
 Python repository for various tools and projects in Machine Learning for Quantitative Finance. In the current release,
-we mostly work on stochastic volatility surfaces and their calibration through Machine Learning methods.
-
-See other work on our main website [SDev-Finance](http://sdev-finance.com/).
+we focus on stochastic volatility surfaces and their calibration through Machine Learning methods. See other work on our main 
+website [SDev-Finance](http://sdev-finance.com/) and [github](https://github.com/sebgur/SDev.Python).
 
 ## Stochastic volatility calibration
 
-In this project we intend to use Neural Networks to improve the calibration speed for stochastic volatility models. For now
+In this project we use Neural Networks to improve the calibration speed for stochastic volatility models. For now
 we consider only the direct map, i.e. the calculation from model parameters to implied volatilities.
 
 We first generate datasets of parameters (inputs) and vanilla option prices (outputs) and then train the network to replicate the prices.
-In this manner, the machine learning model is used as a pricing function to replace costly closed-forms or PDE/MC price calculations.
+In this manner, the learning model is used as a pricing function to replace costly closed-forms or PDE/MC price calculations.
 
-Our models can be saved to files for later usage, and can also be re-trained from a saved state. We cover (Hagan) SABR, Free-Boundary
-SABR, ZABR and Heston models.
+Our models can be saved to files for later usage, and can be re-trained from a saved state. We cover (Hagan) SABR, No-Arbitrage SABR
+(i.e. the actual SABR dynamic), Free-Boundary SABR, ZABR and Heston models.
 
+Jupyter notebooks are available, trained models and datasets are available in our [github](https://github.com/sebgur/SDev.Python) and
+[Kaggle account](https://www.kaggle.com/sebastiengurrieri/datasets).
 
 ## Other Tools
 
 The package contains various other tools including Black-Scholes/Bachelier formulas, Monte-Carlo simulation of vanilla prices and 
-other utilities.
+other utilities. It also features a wrapper class above Keras for easier management of trained models with their scalers,
+as well as custom callbacks and learning schedules.
+
+Jupyter notebooks of previous work are also available [github](https://github.com/sebgur/SDev.Python) (PINNs, AAD Monte-Carlo),
+waiting to be fully integrated here in a next iteration.
```

### Comparing `sdevpy-0.1.5/pyproject.toml` & `sdevpy-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sdevpy"
-version = "0.1.5"
+version = "0.9.0"
 authors = [
   { name="Sebastien Gurrieri", email="sebgur@gmail.com" },
 ]
 description = "Python package for Machine Learning in Finance"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `sdevpy-0.1.5/src/sdevpy/analytics/bachelier.py` & `sdevpy-0.9.0/src/sdevpy/analytics/bachelier.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/analytics/black.py` & `sdevpy-0.9.0/src/sdevpy/analytics/black.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/analytics/fbsabr.py` & `sdevpy-0.9.0/src/sdevpy/analytics/fbsabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/analytics/mcheston.py` & `sdevpy-0.9.0/src/sdevpy/analytics/mcheston.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
     # Build time grid
     time_grid_builder = SimpleTimeGridBuilder(points_per_year=points_per_year)
     time_grid_builder.add_grid(expiries)
     time_grid = time_grid_builder.complete_grid()
     num_factors = 2
 
-
     # Find payoff times
     is_payoff = np.in1d(time_grid, expiries)
 
     # Retrieve parameters
     lnvol = parameters['LnVol']
     kappa = parameters['Kappa']
     theta = parameters['Theta']
```

### Comparing `sdevpy-0.1.5/src/sdevpy/analytics/mcsabr.py` & `sdevpy-0.9.0/src/sdevpy/analytics/mcsabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/analytics/mczabr.py` & `sdevpy-0.9.0/src/sdevpy/analytics/mczabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/analytics/sabr.py` & `sdevpy-0.9.0/src/sdevpy/analytics/sabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/machinelearning/callbacks.py` & `sdevpy-0.9.0/src/sdevpy/machinelearning/callbacks.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/machinelearning/datasets.py` & `sdevpy-0.9.0/src/sdevpy/machinelearning/datasets.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/machinelearning/learningmodel.py` & `sdevpy-0.9.0/src/sdevpy/machinelearning/learningmodel.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/machinelearning/learningschedules.py` & `sdevpy-0.9.0/src/sdevpy/machinelearning/learningschedules.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/machinelearning/topology.py` & `sdevpy-0.9.0/src/sdevpy/machinelearning/topology.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/maths/interpolations.py` & `sdevpy-0.9.0/src/sdevpy/maths/interpolations.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/maths/metrics.py` & `sdevpy-0.9.0/src/sdevpy/maths/metrics.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/maths/rand.py` & `sdevpy-0.9.0/src/sdevpy/maths/rand.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/projects/datafiles.py` & `sdevpy-0.9.0/src/sdevpy/projects/datafiles.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/projects/stovol/stovolgen.py` & `sdevpy-0.9.0/src/sdevpy/projects/stovol/stovolgen.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 """ Generate training data for Stochastic Local Vol models. We implement the direct map here.
     Datasets of parameters (inputs) vs prices/implied vols (outputs) are generated to later train
     a network that learns the so-called 'direct' calculation, i.e. prices from parameter. """
 import os
+from datetime import datetime
 from sdevpy.volsurfacegen import stovolfactory
 from sdevpy import settings
 from sdevpy.tools import filemanager
 from sdevpy.tools.timer import Stopwatch
 
 
 # ################ Runtime configuration ##########################################################
 # MODEL_TYPE = "SABR"
-# MODEL_TYPE = "McSABR"
+MODEL_TYPE = "McSABR"
 # MODEL_TYPE = "FbSABR"
 # MODEL_TYPE = "McZABR"
-MODEL_TYPE = "McHeston"
+# MODEL_TYPE = "McHeston"
 SHIFT = 0.03
-NUM_SAMPLES = 1 * 1000
+NUM_SAMPLES = 35 * 1000
 # The 4 parameters below are only relevant for models whose reference is calculated by MC
 NUM_EXPIRIES = 10
 NUM_STRIKES = 5
 NUM_MC = 100 * 1000 # 100 * 1000
 POINTS_PER_YEAR = 25 # 25
-SEED = 42# [123456789, 6789, 9191, 888, 4321, 100, 4444, 72, 1234, 42]
+SEED = 4549# [123456789, 6789, 9191, 888, 4321, 100, 4444, 72, 1234, 42]
 
 print(">> Set up runtime configuration")
 project_folder = os.path.join(settings.WORKFOLDER, "stovol")
 print("> Project folder: " + project_folder)
 dataset_folder = os.path.join(project_folder, "datasets")
 print("> Data folder: " + dataset_folder)
 filemanager.check_directory(dataset_folder)
 print("> Chosen model: " + MODEL_TYPE)
-data_file = os.path.join(dataset_folder, MODEL_TYPE + "_data.tsv")
+# data_file = os.path.join(dataset_folder, MODEL_TYPE + "_data.tsv")
 
 # ################ Select model ###################################################################
 generator = stovolfactory.set_generator(MODEL_TYPE, SHIFT, NUM_EXPIRIES, NUM_STRIKES, NUM_MC,
                                         POINTS_PER_YEAR, SEED)
 
 # ################ Select training ranges #########################################################
-# # SABR
-# RANGES = {'Ttm': [1.0 / 12.0, 35.0], 'K': [0.01, 0.99], 'F': [-0.009, 0.041], 'LnVol': [0.05, 0.5],
-#           'Beta': [0.1, 0.9], 'Nu': [0.1, 1.0], 'Rho': [-0.6, 0.6]}
+# SABR
+RANGES = {'Ttm': [1.0 / 12.0, 35.0], 'K': [0.01, 0.99], 'F': [-0.009, 0.041], 'LnVol': [0.05, 0.5],
+          'Beta': [0.1, 0.9], 'Nu': [0.1, 1.0], 'Rho': [-0.6, 0.6]}
+# # FBSABR
+# RANGES = {'Ttm': [1.0 / 12.0, 5.0], 'K': [0.01, 0.99], 'F': [-0.009, 0.041], 'LnVol': [0.05, 0.5],
+#           'Beta': [0.25, 0.75], 'Nu': [0.1, 1.0], 'Rho': [-0.6, 0.6]}
 # # ZABR
-# RANGES = {'Ttm': [1.0 / 12.0, 35.0], 'K': [0.01, 0.99], 'F': [-0.009, 0.041], 'LnVol': [0.05, 0.25],
-#           'Beta': [0.49, 0.51], 'Nu': [0.20, 0.80], 'Rho': [-0.4, 0.4],
-#           'Gamma': [0.10, 0.9]}
+# RANGES = {'Ttm': [1.0 / 12.0, 35.0], 'K': [0.01, 0.99], 'F': [-0.009, 0.041], 'LnVol': [0.05, 0.5],
+#           'Beta': [0.1, 0.9], 'Nu': [0.10, 1.0], 'Rho': [-0.6, 0.6],
+#           'Gamma': [0.1, 0.9]}
 # Heston
-RANGES = {'Ttm': [1.0 / 12.0, 35.0], 'K': [0.01, 0.99], 'F': [-0.009, 0.041], 'LnVol': [0.05, 0.25],
-          'Kappa': [0.25, 4.00], 'Theta': [0.05**2, 0.25**2], 'Xi': [0.10, 0.50],
-          'Rho': [-0.40, 0.40]}
+# RANGES = {'Ttm': [1.0 / 12.0, 35.0], 'K': [0.01, 0.99], 'F': [-0.009, 0.041], 'LnVol': [0.05, 0.25],
+#           'Kappa': [0.25, 4.00], 'Theta': [0.05**2, 0.25**2], 'Xi': [0.10, 0.50],
+#           'Rho': [-0.40, 0.40]}
 
 # ################ Generate dataset ###############################################################
 print(">> Generate dataset")
 
 print(f"> Generate {NUM_SAMPLES:,} price samples")
 timer_gen = Stopwatch("Generating Samples")
 timer_gen.trigger()
@@ -64,17 +68,20 @@
 timer_conv = Stopwatch("Converting Prices")
 timer_conv.trigger()
 data_df = generator.to_nvol(data_df, cleanse=True)
 num_clean = len(data_df.index)
 print(f"> Dataset size after cleansing: {num_clean:,}")
 timer_conv.stop()
 
-print("> Output to file: " + data_file)
 timer_out = Stopwatch("File Output")
 timer_out.trigger()
+now = datetime.now()
+dt_string = now.strftime("%Y%m%d-%H_%M_%S")
+data_file = os.path.join(dataset_folder, MODEL_TYPE + "_data_" + dt_string + ".tsv")
+print("> Output to file: " + data_file)
 generator.to_file(data_df, data_file)
 timer_out.stop()
 
 # Show timers
 timer_gen.print()
 timer_conv.print()
 timer_out.print()
```

### Comparing `sdevpy-0.1.5/src/sdevpy/projects/stovol/stovoltrain.py` & `sdevpy-0.9.0/src/sdevpy/projects/stovol/stovoltrain.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,61 +12,63 @@
 from sdevpy.machinelearning.topology import compose_model
 from sdevpy.machinelearning.learningmodel import LearningModel, load_learning_model
 from sdevpy.machinelearning.learningschedules import FlooredExponentialDecay
 from sdevpy.machinelearning.callbacks import RefCallback
 from sdevpy.machinelearning import datasets
 from sdevpy.tools import filemanager
 from sdevpy.tools.timer import Stopwatch
-from sdevpy.tools import clipboard
+# from sdevpy.tools import clipboard
 from sdevpy.maths.metrics import bps_rmse, tf_bps_rmse
 from sdevpy.volsurfacegen.stovolfactory import set_generator
 from sdevpy.projects.stovol import stovolplot as xplt
 
 
-# Get back to Colab to test generate from downloaded models (which works locally), Colab to train
-# Fine-train models
-# Store data in Kaggle
-
 # ################ Runtime configuration ##########################################################
 # MODEL_TYPE = "SABR"
-# MODEL_TYPE = "McSABR"
+MODEL_TYPE = "McSABR"
 # MODEL_TYPE = "FbSABR"
 # MODEL_TYPE = "McZABR"
-MODEL_TYPE = "McHeston"
-MODEL_ID = "McHeston" # Pre-trained model ID (we can pre-train several versions)
+# MODEL_TYPE = "McHeston"
+# MODEL_ID = "SABR_3L_64n" # For pre-trained model ID (we can pre-train several versions)
+MODEL_ID = MODEL_TYPE # For pre-trained model ID (we can pre-train several versions)
 SHIFT = 0.03
 USE_TRAINED = True
 DOWNLOAD_MODELS = False # Only used when USE_TRAINED is True
 DOWNLOAD_DATASETS = False # Use when already created/downloaded
-TRAIN = False
+TRAIN = True
 if USE_TRAINED is False and TRAIN is False:
     raise RuntimeError("When not using pre-trained models, a new model must be trained")
 
 NUM_SAMPLES = 500 * 1000 # Number of samples to read from sample files
 TRAIN_PERCENT = 0.90 # Proportion of dataset used for training (rest used for test)
 EPOCHS = 200
 BATCH_SIZE = 1000
 SHOW_VOL_CHARTS = True # Show smile section charts
 # For comparison to reference values (accuracy of reference)
-NUM_MC = 250000 #100 * 1000 # 100 * 1000
-POINTS_PER_YEAR = 50# 25 # 25
+NUM_MC = 100 * 1000 # 100 * 1000
+POINTS_PER_YEAR = 25# 25
+project_folder = os.path.join(settings.WORKFOLDER, "stovol")
 
 print(">> Set up runtime configuration")
 print("> Chosen model type: " + MODEL_TYPE)
 if USE_TRAINED:
     print("> Pre-trained model ID: " + MODEL_ID)
 
-project_folder = os.path.join(settings.WORKFOLDER, "stovol")
+filemanager.check_directory(project_folder)
 print("> Project folder: " + project_folder)
+
 dataset_folder = os.path.join(project_folder, "datasets")
 data_folder = os.path.join(dataset_folder, MODEL_TYPE)
+filemanager.check_directory(data_folder)
 print("> Data folder: " + data_folder)
 data_file = os.path.join(dataset_folder, MODEL_TYPE + "_data.tsv")
 print("> Data file: " + data_file)
+
 model_folder = os.path.join(project_folder, "models")
+filemanager.check_directory(model_folder)
 print("> Model folder: " + model_folder)
 
 if USE_TRAINED and DOWNLOAD_MODELS:
     url = 'https://github.com/sebgur/SDev.Python/raw/main/models/stovol/models.zip'
     print("> Downloading and unzipping models from: " + url)
     filemanager.download_unzip(url, model_folder)
 
@@ -135,16 +137,16 @@
 print(f"> Hidden layer structure: {HIDDEN_LAYERS}")
 print(f"> Number of neurons per layer: {NUM_NEURONS}")
 print(f"> Drop-out rate: {DROP_OUT:.2f}")
 
 # ################ Train the model ################################################################
 if TRAIN:
     # Learning rate scheduler
-    INIT_LR = 1.5e-3
-    FINAL_LR = 5.0e-4
+    INIT_LR = 1.0e-2
+    FINAL_LR = 1.0e-4
     DECAY = 0.97
     STEPS = 250
     lr_schedule = FlooredExponentialDecay(INIT_LR, FINAL_LR, DECAY, STEPS)
 
     # Optimizer
     optimizer = tf.keras.optimizers.Adam(learning_rate=lr_schedule)
     model.optimizer_ = optimizer.get_config()
@@ -196,23 +198,25 @@
     print("> Choosing a sample parameter set to display chart")
     NUM_STRIKES = 100
     PARAMS = { 'LnVol': 0.20, 'Beta': 0.5, 'Nu': 0.55, 'Rho': -0.25, 'Gamma': 0.7, 'Kappa': 1.0,
                 'Theta': 0.03, 'Xi': 0.35 }
     FWD = 0.028
 
     # Any number of expiries can be calculated, but for optimum display choose no more than 6
-    # EXPIRIES = np.asarray([0.125, 0.250, 0.5, 1.00, 2.0, 5.0]).reshape(-1, 1)
-    EXPIRIES = np.asarray([0.25, 0.50, 1.0, 5.00, 10.0, 30.0]).reshape(-1, 1)
+    if MODEL_TYPE == "FbSABR":
+        EXPIRIES = np.asarray([0.25, 0.50, 1.0, 2.0, 5.0, 10.0]).reshape(-1, 1) # Only trained up to 5y
+    else:
+        EXPIRIES = np.asarray([0.25, 0.50, 1.0, 5.0, 10.0, 30.0]).reshape(-1, 1)
     NUM_EXPIRIES = EXPIRIES.shape[0]
     METHOD = 'Percentiles'
     PERCENTS = np.linspace(0.01, 0.99, num=NUM_STRIKES)
     PERCENTS = np.asarray([PERCENTS] * NUM_EXPIRIES)
 
     strikes = generator.convert_strikes(EXPIRIES, PERCENTS, FWD, PARAMS, METHOD)
-    clipboard.export2d(strikes)
+    # clipboard.export2d(strikes)
     ARE_CALLS = [[False] * NUM_STRIKES] * NUM_EXPIRIES # All puts
     # ARE_CALLS = [[False if s < FWD else True for s in expks] for expks in strikes] # Puts/calls
     # print(ARE_CALLS)
 
     print("> Calculating chart surface with reference model")
     timer_ref = Stopwatch("Reference surface calculation")
     timer_ref.trigger()
@@ -235,15 +239,14 @@
     TITLE = f"{MODEL_TYPE} smile sections, forward={FWD*100:.2f}"#,%\n parameters={PARAMS}"
     # TRANSFORM = "Bachelier"
     # TRANSFORM = "Price"
     TRANSFORM = "ShiftedBlackScholes"
     xplt.plot_transform_surface(EXPIRIES, strikes, ARE_CALLS, FWD, ref_prices, mod_prices,
                                 TITLE, transform=TRANSFORM)
 
-
 # Show training history
 if TRAIN:
     hist_epochs = callback.epochs
     hist_losses = callback.losses
     hist_lr = callback.learning_rates
     sampled_epochs = callback.sampled_epochs
     test_losses = callback.test_losses
```

### Comparing `sdevpy-0.1.5/src/sdevpy/test.py` & `sdevpy-0.9.0/src/sdevpy/test.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/tools/clipboard.py` & `sdevpy-0.9.0/src/sdevpy/tools/clipboard.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/tools/filemanager.py` & `sdevpy-0.9.0/src/sdevpy/tools/filemanager.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/tools/jsonmanager.py` & `sdevpy-0.9.0/src/sdevpy/tools/jsonmanager.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/tools/timegrids.py` & `sdevpy-0.9.0/src/sdevpy/tools/timegrids.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/tools/timer.py` & `sdevpy-0.9.0/src/sdevpy/tools/timer.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/volsurfacegen/fbsabrgenerator.py` & `sdevpy-0.9.0/src/sdevpy/volsurfacegen/fbsabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/volsurfacegen/mchestongenerator.py` & `sdevpy-0.9.0/src/sdevpy/volsurfacegen/mchestongenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/volsurfacegen/mcsabrgenerator.py` & `sdevpy-0.9.0/src/sdevpy/volsurfacegen/mcsabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/volsurfacegen/mczabrgenerator.py` & `sdevpy-0.9.0/src/sdevpy/volsurfacegen/mczabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/volsurfacegen/sabrgenerator.py` & `sdevpy-0.9.0/src/sdevpy/volsurfacegen/sabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/volsurfacegen/smilegenerator.py` & `sdevpy-0.9.0/src/sdevpy/volsurfacegen/smilegenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.5/src/sdevpy/volsurfacegen/stovolfactory.py` & `sdevpy-0.9.0/src/sdevpy/volsurfacegen/stovolfactory.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 def set_generator(type_, shift=0.03, num_expiries=10, num_strikes=5, num_mc=100000,
                   points_per_year=25, seed=42):
     """ Select generator based on type and other information. Currently available are: SABR,
         McSABR, FbSABR, McZABR and McHeston. """
     if type_ == "SABR":
         generator = SabrGenerator(shift, num_expiries, num_strikes, seed)
     elif type_ == "McSABR":
-        generator = McSabrGenerator(shift, num_expiries, num_strikes, num_mc, points_per_year)
+        generator = McSabrGenerator(shift, num_expiries, num_strikes, num_mc, points_per_year, seed)
     elif type_ == "FbSABR":
-        generator = FbSabrGenerator(num_expiries, num_strikes, num_mc, points_per_year)
+        generator = FbSabrGenerator(num_expiries, num_strikes, num_mc, points_per_year, seed)
     elif type_ == "McZABR":
-        generator = McZabrGenerator(shift, num_expiries, num_strikes, num_mc, points_per_year)
+        generator = McZabrGenerator(shift, num_expiries, num_strikes, num_mc, points_per_year, seed)
     elif type_ == "McHeston":
-        generator = McHestonGenerator(shift, num_expiries, num_strikes, num_mc, points_per_year)
+        generator = McHestonGenerator(shift, num_expiries, num_strikes, num_mc, points_per_year, seed)
     else:
         raise ValueError("Unknown model: " + type_)
 
     return generator
 
 if __name__ == "__main__":
     NUM_MC = 1 * 1000
```

### Comparing `sdevpy-0.1.5/src/sdevpy.egg-info/PKG-INFO` & `sdevpy-0.9.0/src/sdevpy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 Metadata-Version: 2.1
 Name: sdevpy
-Version: 0.1.5
+Version: 0.9.0
 Summary: Python package for Machine Learning in Finance
 Author-email: Sebastien Gurrieri <sebgur@gmail.com>
 Project-URL: Git page, https://github.com/sebgur/SDev.Python
 Project-URL: SDev Finance, http://sdev-finance.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SDev.Python
 
 Python repository for various tools and projects in Machine Learning for Quantitative Finance. In the current release,
-we mostly work on stochastic volatility surfaces and their calibration through Machine Learning methods.
-
-See other work on our main website [SDev-Finance](http://sdev-finance.com/).
+we focus on stochastic volatility surfaces and their calibration through Machine Learning methods. See other work on our main 
+website [SDev-Finance](http://sdev-finance.com/) and [github](https://github.com/sebgur/SDev.Python).
 
 ## Stochastic volatility calibration
 
-In this project we intend to use Neural Networks to improve the calibration speed for stochastic volatility models. For now
+In this project we use Neural Networks to improve the calibration speed for stochastic volatility models. For now
 we consider only the direct map, i.e. the calculation from model parameters to implied volatilities.
 
 We first generate datasets of parameters (inputs) and vanilla option prices (outputs) and then train the network to replicate the prices.
-In this manner, the machine learning model is used as a pricing function to replace costly closed-forms or PDE/MC price calculations.
+In this manner, the learning model is used as a pricing function to replace costly closed-forms or PDE/MC price calculations.
 
-Our models can be saved to files for later usage, and can also be re-trained from a saved state. We cover (Hagan) SABR, Free-Boundary
-SABR, ZABR and Heston models.
+Our models can be saved to files for later usage, and can be re-trained from a saved state. We cover (Hagan) SABR, No-Arbitrage SABR
+(i.e. the actual SABR dynamic), Free-Boundary SABR, ZABR and Heston models.
 
+Jupyter notebooks are available, trained models and datasets are available in our [github](https://github.com/sebgur/SDev.Python) and
+[Kaggle account](https://www.kaggle.com/sebastiengurrieri/datasets).
 
 ## Other Tools
 
 The package contains various other tools including Black-Scholes/Bachelier formulas, Monte-Carlo simulation of vanilla prices and 
-other utilities.
+other utilities. It also features a wrapper class above Keras for easier management of trained models with their scalers,
+as well as custom callbacks and learning schedules.
+
+Jupyter notebooks of previous work are also available [github](https://github.com/sebgur/SDev.Python) (PINNs, AAD Monte-Carlo),
+waiting to be fully integrated here in a next iteration.
```

### Comparing `sdevpy-0.1.5/src/sdevpy.egg-info/SOURCES.txt` & `sdevpy-0.9.0/src/sdevpy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -22,17 +22,14 @@
 src/sdevpy/machinelearning/learningschedules.py
 src/sdevpy/machinelearning/topology.py
 src/sdevpy/maths/interpolations.py
 src/sdevpy/maths/metrics.py
 src/sdevpy/maths/optimization.py
 src/sdevpy/maths/rand.py
 src/sdevpy/projects/datafiles.py
-src/sdevpy/projects/pinns/ernst_pinns.py
-src/sdevpy/projects/pinns/pinns.py
-src/sdevpy/projects/pinns/pinns_worst_of.py
 src/sdevpy/projects/stovol/stovolgen.py
 src/sdevpy/projects/stovol/stovolplot.py
 src/sdevpy/projects/stovol/stovoltrain.py
 src/sdevpy/tools/clipboard.py
 src/sdevpy/tools/constants.py
 src/sdevpy/tools/filemanager.py
 src/sdevpy/tools/jsonmanager.py
```

