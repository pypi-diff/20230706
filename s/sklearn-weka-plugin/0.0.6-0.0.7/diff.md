# Comparing `tmp/sklearn-weka-plugin-0.0.6.tar.gz` & `tmp/sklearn-weka-plugin-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn-weka-plugin-0.0.6.tar", last modified: Mon Apr 25 22:33:17 2022, max compression
+gzip compressed data, was "sklearn-weka-plugin-0.0.7.tar", last modified: Thu Jul  6 20:57:40 2023, max compression
```

## Comparing `sklearn-weka-plugin-0.0.6.tar` & `sklearn-weka-plugin-0.0.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2022-04-25 22:33:17.701199 sklearn-weka-plugin-0.0.6/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      685 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/.gitignore
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1732 2022-04-25 22:32:37.000000 sklearn-weka-plugin-0.0.6/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      367 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    35149 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/LICENSE
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2744 2022-04-25 22:33:17.701199 sklearn-weka-plugin-0.0.6/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5003 2022-01-09 22:03:06.000000 sklearn-weka-plugin-0.0.6/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1085 2022-03-31 22:30:00.000000 sklearn-weka-plugin-0.0.6/RELEASE.md
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2022-04-25 22:33:17.697199 sklearn-weka-plugin-0.0.6/doc/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6835 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/doc/Makefile
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6494 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/doc/make.bat
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2022-04-25 22:33:17.697199 sklearn-weka-plugin-0.0.6/doc/source/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2022-04-25 22:33:17.697199 sklearn-weka-plugin-0.0.6/doc/source/_static/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    17064 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/doc/source/_static/logo.jpg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6763 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/doc/source/_static/logo.pdf
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6017 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/doc/source/_static/logo.png
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3236 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/doc/source/_static/logo.svg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8474 2022-04-25 22:31:31.000000 sklearn-weka-plugin-0.0.6/doc/source/conf.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6513 2022-03-31 22:18:00.000000 sklearn-weka-plugin-0.0.6/doc/source/examples.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1165 2021-12-17 03:59:39.000000 sklearn-weka-plugin-0.0.6/doc/source/index.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      768 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/doc/source/install.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       52 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/doc/source/modules.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      621 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/doc/source/sklweka.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       81 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/requirements.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2022-04-25 22:33:17.701199 sklearn-weka-plugin-0.0.6/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1173 2022-04-25 22:31:31.000000 sklearn-weka-plugin-0.0.6/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2022-04-25 22:33:17.697199 sklearn-weka-plugin-0.0.6/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2022-04-25 22:33:17.701199 sklearn-weka-plugin-0.0.6/src/sklearn_weka_plugin.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2744 2022-04-25 22:33:17.000000 sklearn-weka-plugin-0.0.6/src/sklearn_weka_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      810 2022-04-25 22:33:17.000000 sklearn-weka-plugin-0.0.6/src/sklearn_weka_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2022-04-25 22:33:17.000000 sklearn-weka-plugin-0.0.6/src/sklearn_weka_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       42 2022-04-25 22:33:17.000000 sklearn-weka-plugin-0.0.6/src/sklearn_weka_plugin.egg-info/requires.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        8 2022-04-25 22:33:17.000000 sklearn-weka-plugin-0.0.6/src/sklearn_weka_plugin.egg-info/top_level.txt
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2022-04-25 22:33:17.701199 sklearn-weka-plugin-0.0.6/src/sklweka/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/src/sklweka/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    10381 2022-04-25 22:03:28.000000 sklearn-weka-plugin-0.0.6/src/sklweka/classifiers.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7806 2022-04-25 22:03:28.000000 sklearn-weka-plugin-0.0.6/src/sklweka/clusters.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1631 2021-10-31 20:00:50.000000 sklearn-weka-plugin-0.0.6/src/sklweka/datagenerators.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    15063 2022-04-25 22:03:28.000000 sklearn-weka-plugin-0.0.6/src/sklweka/dataset.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       28 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/src/sklweka/jvm.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       33 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.6/src/sklweka/packages.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    13350 2022-04-25 22:30:16.000000 sklearn-weka-plugin-0.0.6/src/sklweka/preprocessing.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 20:57:40.796982 sklearn-weka-plugin-0.0.7/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      685 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/.gitignore
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2429 2023-07-06 20:55:03.000000 sklearn-weka-plugin-0.0.7/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      367 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    35149 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/LICENSE
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3441 2023-07-06 20:57:40.796982 sklearn-weka-plugin-0.0.7/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5003 2022-01-09 22:03:06.000000 sklearn-weka-plugin-0.0.7/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1085 2022-03-31 22:30:00.000000 sklearn-weka-plugin-0.0.7/RELEASE.md
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 20:57:40.792982 sklearn-weka-plugin-0.0.7/doc/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6835 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/Makefile
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6494 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/make.bat
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 20:57:40.792982 sklearn-weka-plugin-0.0.7/doc/source/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 20:57:40.792982 sklearn-weka-plugin-0.0.7/doc/source/_static/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    17064 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/source/_static/logo.jpg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6763 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/source/_static/logo.pdf
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6017 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/source/_static/logo.png
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3236 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/source/_static/logo.svg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8474 2023-07-06 20:55:03.000000 sklearn-weka-plugin-0.0.7/doc/source/conf.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6513 2022-03-31 22:18:00.000000 sklearn-weka-plugin-0.0.7/doc/source/examples.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1165 2021-12-17 03:59:39.000000 sklearn-weka-plugin-0.0.7/doc/source/index.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      768 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/source/install.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       52 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/source/modules.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      621 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/doc/source/sklweka.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       81 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/requirements.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-07-06 20:57:40.796982 sklearn-weka-plugin-0.0.7/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1173 2023-07-06 20:55:03.000000 sklearn-weka-plugin-0.0.7/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 20:57:40.792982 sklearn-weka-plugin-0.0.7/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 20:57:40.796982 sklearn-weka-plugin-0.0.7/src/sklearn_weka_plugin.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3441 2023-07-06 20:57:40.000000 sklearn-weka-plugin-0.0.7/src/sklearn_weka_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      810 2023-07-06 20:57:40.000000 sklearn-weka-plugin-0.0.7/src/sklearn_weka_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-07-06 20:57:40.000000 sklearn-weka-plugin-0.0.7/src/sklearn_weka_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       42 2023-07-06 20:57:40.000000 sklearn-weka-plugin-0.0.7/src/sklearn_weka_plugin.egg-info/requires.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        8 2023-07-06 20:57:40.000000 sklearn-weka-plugin-0.0.7/src/sklearn_weka_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 20:57:40.796982 sklearn-weka-plugin-0.0.7/src/sklweka/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/src/sklweka/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    11541 2023-07-06 20:41:56.000000 sklearn-weka-plugin-0.0.7/src/sklweka/classifiers.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8229 2023-06-19 21:09:04.000000 sklearn-weka-plugin-0.0.7/src/sklweka/clusters.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1631 2021-10-31 20:00:50.000000 sklearn-weka-plugin-0.0.7/src/sklweka/datagenerators.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    15246 2023-07-06 20:51:41.000000 sklearn-weka-plugin-0.0.7/src/sklweka/dataset.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       28 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/src/sklweka/jvm.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       33 2021-08-14 06:43:54.000000 sklearn-weka-plugin-0.0.7/src/sklweka/packages.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    13140 2023-06-19 20:45:11.000000 sklearn-weka-plugin-0.0.7/src/sklweka/preprocessing.py
```

### Comparing `sklearn-weka-plugin-0.0.6/.gitignore` & `sklearn-weka-plugin-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.6/CHANGES.rst` & `sklearn-weka-plugin-0.0.7/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 Changelog
 =========
 
+0.0.7 (2023-07-07)
+------------------
+
+- `WekaEstimator` (module `sklweka.classifiers`) now has a custom `score` method that
+  distinguishes between classification and regression to return the correct score.
+- renamed `data` to `X` and `targets` to `y`, since some sklearn schemes use named arguments
+- added dummy argument `sample_weight=None` to `fit`, `score` and `fit_predict` methods
+- fixed: when supplying Classifier or JBObject instead of classname/options, classname/options
+  now get determined automatically
+- method `to_instance` (module: `sklweka.dataset`) now performs correct missing value check
+- method `to_nominal_labels` (module: `sklweka.dataset`) generates nicer labels now
+
+
 0.0.6 (2022-04-26)
 ------------------
 
 - `WekaEstimator` (module `sklweka.classifiers`) and `WekaCluster` (module `sklweka.clusters`)
   now allow specifying how many labels a particular nominal attribute or class attribute has
   (to avoid error message like `Cannot handle unary class attribute!` if there is only one
   label present in a particular split)
```

### Comparing `sklearn-weka-plugin-0.0.6/LICENSE` & `sklearn-weka-plugin-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.6/PKG-INFO` & `sklearn-weka-plugin-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-weka-plugin
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library for making Weka algorithms available within scikit-learn. Relies on the python-weka-wrapper3 library.
 Home-page: https://github.com/fracpete/sklearn-weka-plugin
 Author: Peter "fracpete" Reutemann
 Author-email: sklweka@fracpete.org
 License: GNU General Public License version 3.0 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,27 @@
 Examples can be found at:
 
 https://github.com/fracpete/sklearn-weka-plugin-examples
 
 Changelog
 =========
 
+0.0.7 (2023-07-07)
+------------------
+
+- `WekaEstimator` (module `sklweka.classifiers`) now has a custom `score` method that
+  distinguishes between classification and regression to return the correct score.
+- renamed `data` to `X` and `targets` to `y`, since some sklearn schemes use named arguments
+- added dummy argument `sample_weight=None` to `fit`, `score` and `fit_predict` methods
+- fixed: when supplying Classifier or JBObject instead of classname/options, classname/options
+  now get determined automatically
+- method `to_instance` (module: `sklweka.dataset`) now performs correct missing value check
+- method `to_nominal_labels` (module: `sklweka.dataset`) generates nicer labels now
+
+
 0.0.6 (2022-04-26)
 ------------------
 
 - `WekaEstimator` (module `sklweka.classifiers`) and `WekaCluster` (module `sklweka.clusters`)
   now allow specifying how many labels a particular nominal attribute or class attribute has
   (to avoid error message like `Cannot handle unary class attribute!` if there is only one
   label present in a particular split)
```

### Comparing `sklearn-weka-plugin-0.0.6/README.md` & `sklearn-weka-plugin-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.6/RELEASE.md` & `sklearn-weka-plugin-0.0.7/RELEASE.md`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.6/doc/Makefile` & `sklearn-weka-plugin-0.0.7/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.6/doc/make.bat` & `sklearn-weka-plugin-0.0.7/doc/make.bat`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.6/doc/source/_static/logo.jpg` & `sklearn-weka-plugin-0.0.7/doc/source/_static/logo.jpg`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.6/doc/source/_static/logo.pdf` & `sklearn-weka-plugin-0.0.7/doc/source/_static/logo.pdf`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.6/doc/source/_static/logo.png` & `sklearn-weka-plugin-0.0.7/doc/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.6/doc/source/_static/logo.svg` & `sklearn-weka-plugin-0.0.7/doc/source/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.6/doc/source/conf.py` & `sklearn-weka-plugin-0.0.7/doc/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,24 +42,24 @@
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'sklearn-weka-plugin'
-copyright = u'2021-2022, Peter "fracpete" Reutemann'
+copyright = u'2021-2023, Peter "fracpete" Reutemann'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '0.0.6'
+version = '0.0.7'
 # The full version, including alpha/beta/rc tags.
-release = '0.0.6'
+release = '0.0.7'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `sklearn-weka-plugin-0.0.6/doc/source/examples.rst` & `sklearn-weka-plugin-0.0.7/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.6/doc/source/index.rst` & `sklearn-weka-plugin-0.0.7/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.6/doc/source/install.rst` & `sklearn-weka-plugin-0.0.7/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.6/doc/source/sklweka.rst` & `sklearn-weka-plugin-0.0.7/doc/source/sklweka.rst`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.6/setup.py` & `sklearn-weka-plugin-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     license='GNU General Public License version 3.0 (GPLv3)',
     package_dir={
         '': 'src'
     },
     packages=[
         "sklweka",
     ],
-    version="0.0.6",
+    version="0.0.7",
     author='Peter "fracpete" Reutemann',
     author_email='sklweka@fracpete.org',
     install_requires=[
         "numpy",
         "python-weka-wrapper3>=0.2.5",
         "sklearn",
     ],
```

### Comparing `sklearn-weka-plugin-0.0.6/src/sklearn_weka_plugin.egg-info/PKG-INFO` & `sklearn-weka-plugin-0.0.7/src/sklearn_weka_plugin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-weka-plugin
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library for making Weka algorithms available within scikit-learn. Relies on the python-weka-wrapper3 library.
 Home-page: https://github.com/fracpete/sklearn-weka-plugin
 Author: Peter "fracpete" Reutemann
 Author-email: sklweka@fracpete.org
 License: GNU General Public License version 3.0 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,27 @@
 Examples can be found at:
 
 https://github.com/fracpete/sklearn-weka-plugin-examples
 
 Changelog
 =========
 
+0.0.7 (2023-07-07)
+------------------
+
+- `WekaEstimator` (module `sklweka.classifiers`) now has a custom `score` method that
+  distinguishes between classification and regression to return the correct score.
+- renamed `data` to `X` and `targets` to `y`, since some sklearn schemes use named arguments
+- added dummy argument `sample_weight=None` to `fit`, `score` and `fit_predict` methods
+- fixed: when supplying Classifier or JBObject instead of classname/options, classname/options
+  now get determined automatically
+- method `to_instance` (module: `sklweka.dataset`) now performs correct missing value check
+- method `to_nominal_labels` (module: `sklweka.dataset`) generates nicer labels now
+
+
 0.0.6 (2022-04-26)
 ------------------
 
 - `WekaEstimator` (module `sklweka.classifiers`) and `WekaCluster` (module `sklweka.clusters`)
   now allow specifying how many labels a particular nominal attribute or class attribute has
   (to avoid error message like `Cannot handle unary class attribute!` if there is only one
   label present in a particular split)
```

### Comparing `sklearn-weka-plugin-0.0.6/src/sklearn_weka_plugin.egg-info/SOURCES.txt` & `sklearn-weka-plugin-0.0.7/src/sklearn_weka_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.6/src/sklweka/classifiers.py` & `sklearn-weka-plugin-0.0.7/src/sklweka/classifiers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 from numpy import ndarray
 from sklearn.base import BaseEstimator, ClassifierMixin, RegressorMixin
 from sklearn.utils.validation import check_X_y, check_array, check_is_fitted
+from sklearn.metrics import accuracy_score, r2_score
 from sklweka.preprocessing import to_nominal_attributes, to_nominal_labels
 from weka.classifiers import Classifier
 from weka.core.classes import is_instance_of, OptionHandler
 from weka.core.dataset import missing_value
 from weka.core.serialization import deepcopy
 from sklweka.dataset import to_instances, to_instance
 
@@ -57,16 +58,16 @@
             raise Exception("Java object does not implement weka.classifiers.Classifier!")
 
         super(WekaEstimator, self).__init__(_jobject)
         self._classifier = Classifier(jobject=_jobject)
         self.header_ = None
         self.classes_ = None
         # the following references are required for get_params/set_params
-        self._classname = classname
-        self._options = options
+        self._classname = classname if (classname is not None) else self._classifier.classname
+        self._options = options if (options is not None) else self._classifier.options
         self._nominal_input_vars = nominal_input_vars
         self._nominal_output_var = nominal_output_var
         self._num_nominal_input_labels = num_nominal_input_labels
         self._num_nominal_output_labels = num_nominal_output_labels
 
     @property
     def classifier(self):
@@ -84,81 +85,103 @@
         Returns the underlying dataset header, if any.
 
         :return: the dataset structure
         :rtype: Instances
         """
         return self.header_
 
-    def fit(self, data, targets):
+    def fit(self, X, y, sample_weight=None):
         """
         Trains the estimator.
 
-        :param data: the input variables as matrix, array-like of shape (n_samples, n_features)
-        :type data: ndarray
-        :param targets: the class attribute column, array-like of shape (n_samples,)
-        :type targets: ndarray
+        :param X: the input variables as matrix, array-like of shape (n_samples, n_features)
+        :type X: ndarray
+        :param y: the class attribute column, array-like of shape (n_samples,)
+        :type y: ndarray
+        :param sample_weight: Sample weights. If None, then samples are equally weighted. TODO Currently ignored.
+        :type sample_weight: array-like of shape (n_samples,), default=None
         :return: itself
         :rtype: WekaEstimator
         """
-        data, targets = check_X_y(data, y=targets, dtype=None)
+        X, y = check_X_y(X, y=y, dtype=None)
         if self._nominal_input_vars is not None:
-            data = to_nominal_attributes(data, self._nominal_input_vars)
+            X = to_nominal_attributes(X, self._nominal_input_vars)
         if self._nominal_output_var is not None:
-            targets = to_nominal_labels(targets)
-        d = to_instances(data, targets,
+            y = to_nominal_labels(y)
+        d = to_instances(X, y,
                          num_nominal_labels=self._num_nominal_input_labels,
                          num_class_labels=self._num_nominal_output_labels)
         self._classifier.build_classifier(d)
         self.header_ = d.template_instances(d, 0)
         if d.class_attribute.is_nominal:
             self.classes_ = d.class_attribute.values
         else:
             self.classes_ = None
         return self
 
-    def predict(self, data):
+    def predict(self, X):
         """
         Performs predictions with the trained classifier.
 
-        :param data: the data matrix to generate predictions for, array-like of shape (n_samples, n_features)
-        :type data: ndarray
+        :param X: the data matrix to generate predictions for, array-like of shape (n_samples, n_features)
+        :type X: ndarray
         :return: the score (or scores)
         :rtype: ndarray
         """
         check_is_fitted(self)
         if self._nominal_input_vars is not None:
-            data = to_nominal_attributes(data, self._nominal_input_vars)
-        data = check_array(data, dtype=None)
+            X = to_nominal_attributes(X, self._nominal_input_vars)
+        X = check_array(X, dtype=None)
         result = []
-        for d in data:
-            inst = to_instance(self.header_, d, missing_value())
+        for d in X:
+            inst = to_instance(self.header_, d, y=missing_value())
             if self.header_.class_attribute.is_nominal:
                 result.append(self.header_.class_attribute.value(int(self._classifier.classify_instance(inst))))
             else:
                 result.append(self._classifier.classify_instance(inst))
         return np.array(result)
 
-    def predict_proba(self, data):
+    def predict_proba(self, X):
         """
         Performs predictions and returns class probabilities.
 
-        :param data: the data matrix to generate predictions for, array-like of shape (n_samples, n_features)
-        :type data: ndarray
+        :param X: the data matrix to generate predictions for, array-like of shape (n_samples, n_features)
+        :type X: ndarray
         :return: the probabilities
         """
         check_is_fitted(self)
         if self._nominal_input_vars is not None:
-            data = to_nominal_attributes(data, self._nominal_input_vars)
-        data = check_array(data, dtype=None)
+            X = to_nominal_attributes(X, self._nominal_input_vars)
+        X = check_array(X, dtype=None)
         result = []
-        for d in data:
-            inst = to_instance(self.header_, d, missing_value())
+        for d in X:
+            inst = to_instance(self.header_, d, y=missing_value())
             result.append(self._classifier.distribution_for_instance(inst))
         return np.array(result)
 
+    def score(self, X, y, sample_weight=None):
+        """
+        Classification: return the mean accuracy on the given test data and labels.
+        Regression: return the coefficient of determination of the prediction.
+
+        :param X: the input variables as matrix, array-like of shape (n_samples, n_features)
+        :type X: ndarray
+        :param y: the class attribute column, array-like of shape (n_samples,)
+        :type y: ndarray
+        :param sample_weight: Sample weights. If None, then samples are equally weighted.
+        :type sample_weight: array-like of shape (n_samples,), default=None
+        :return: the score
+        :rtype: float
+        """
+        y_pred = self.predict(X)
+        if self._nominal_output_var:
+            return accuracy_score(y, y_pred, sample_weight=sample_weight)
+        else:
+            return r2_score(y, y_pred, sample_weight=sample_weight)
+
     def get_params(self, deep=True):
         """
         Returns the parameters for this classifier, basically classname and options list.
 
         :param deep: ignored
         :type deep: bool
         :return: the dictionary with options
```

### Comparing `sklearn-weka-plugin-0.0.6/src/sklweka/clusters.py` & `sklearn-weka-plugin-0.0.7/src/sklweka/clusters.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,16 +48,16 @@
         if not is_instance_of(_jobject, "weka.clusterers.Clusterer"):
             raise Exception("Java object does not implement weka.clusterers.Clusterer!")
 
         super(WekaCluster, self).__init__(_jobject)
         self._cluster = Clusterer(jobject=_jobject)
         self.header_ = None
         # the following references are required for get_params/set_params
-        self._classname = classname
-        self._options = options
+        self._classname = classname if (classname is not None) else self._cluster.classname
+        self._options = options if (options is not None) else self._cluster.options
         self._nominal_input_vars = nominal_input_vars
         self._num_nominal_input_labels = num_nominal_input_labels
 
     @property
     def cluster(self):
         """
         Returns the underlying cluster object, if any.
@@ -73,65 +73,69 @@
         Returns the underlying dataset header, if any.
 
         :return: the dataset structure
         :rtype: Instances
         """
         return self.header_
 
-    def fit(self, data, targets=None):
+    def fit(self, X, y=None, sample_weight=None):
         """
         Trains the cluster.
 
-        :param data: the input variables as matrix, array-like of shape (n_samples, n_features)
-        :type data: ndarray
-        :param targets: ignored
-        :type targets: ndarray
+        :param X: the input variables as matrix, array-like of shape (n_samples, n_features)
+        :type X: ndarray
+        :param y: ignored
+        :type y: ndarray
+        :param sample_weight: Sample weights. If None, then samples are equally weighted. TODO Currently ignored.
+        :type sample_weight: array-like of shape (n_samples,), default=None
         :return: the cluster
         :rtype: WekaCluster
         """
         if self._nominal_input_vars is not None:
-            data = to_nominal_attributes(data, self._nominal_input_vars)
-        d = to_instances(data, num_nominal_labels=self._num_nominal_input_labels)
+            X = to_nominal_attributes(X, self._nominal_input_vars)
+        d = to_instances(X, num_nominal_labels=self._num_nominal_input_labels)
         self._cluster.build_clusterer(d)
         self.header_ = d.template_instances(d, 0)
         return self
 
-    def predict(self, data, targets=None):
+    def predict(self, X, y=None):
         """
         Predicts cluster labels.
 
-        :param data: the input variables as matrix, array-like of shape (n_samples, n_features)
-        :type data: ndarray
-        :param targets: ignored
-        :type targets: ndarray
+        :param X: the input variables as matrix, array-like of shape (n_samples, n_features)
+        :type X: ndarray
+        :param y: ignored
+        :type y: ndarray
         :return: the cluster labels (of type int)
         :rtype: ndarray
         """
         check_is_fitted(self)
         if self._nominal_input_vars is not None:
-            data = to_nominal_attributes(data, self._nominal_input_vars)
+            X = to_nominal_attributes(X, self._nominal_input_vars)
         result = []
-        for d in data:
+        for d in X:
             inst = to_instance(self.header_, d)
             result.append(int(self._cluster.cluster_instance(inst)))
         return np.array(result)
 
-    def fit_predict(self, data, targets=None):
+    def fit_predict(self, X, y=None, sample_weight=None):
         """
         Trains the cluster and returns the cluster labels.
 
-        :param data: the input variables as matrix, array-like of shape (n_samples, n_features)
-        :type data: ndarray
-        :param targets: ignored
-        :type targets: ndarray
+        :param X: the input variables as matrix, array-like of shape (n_samples, n_features)
+        :type X: ndarray
+        :param y: ignored
+        :type y: ndarray
+        :param sample_weight: Sample weights. If None, then samples are equally weighted. TODO Currently ignored.
+        :type sample_weight: array-like of shape (n_samples,), default=None
         :return: the cluster labels (of type int)
         :rtype: ndarray
         """
-        self.fit(data)
-        return self.predict(data)
+        self.fit(X)
+        return self.predict(X)
 
     def get_params(self, deep=True):
         """
         Returns the parameters for this cluster, basically classname and options list.
 
         :param deep: ignored
         :type deep: bool
```

### Comparing `sklearn-weka-plugin-0.0.6/src/sklweka/datagenerators.py` & `sklearn-weka-plugin-0.0.7/src/sklweka/datagenerators.py`

 * *Files identical despite different names*

### Comparing `sklearn-weka-plugin-0.0.6/src/sklweka/dataset.py` & `sklearn-weka-plugin-0.0.7/src/sklweka/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 from scipy.io.arff import loadarff
 from weka.core.dataset import Instances, Instance, Attribute
 from datetime import datetime
 from weka.core.dataset import missing_value
 from weka.core.converters import loader_for_file, Loader
 import numpy as np
 from numpy import ndarray
@@ -100,15 +101,21 @@
     Turns the numeric column vector into a string vector.
 
     :param y: the vector to convert
     :type y: list or ndarray
     :return: the converted vector
     :rtype: ndarray
     """
-    return np.array(["_" + str(x) for x in y])
+    result = []
+    for item in y:
+        if isinstance(item, np.bytes_):
+            result.append("_" + item.astype(str))
+        else:
+            result.append("_" + str(item))
+    return result
 
 
 def split_off_class(data, class_index):
     """
     Splits off the class attribute from the data matrix.
     The class index can either be a 0-based int or a 1-based string
     (first,second,last,last-1 are accepted as well).
@@ -399,15 +406,16 @@
             values.append(header.attribute(i).index_of(str(x[i])))
         elif header.attribute(i).is_numeric:
             values.append(x[i])
         else:
             raise Exception("Unsupported attribute type for column %d: %s" % ((i+1), header.attribute(i).type_str()))
 
     if y is not None and header.has_class():
-        if y == missing_value():
+        # missing value?
+        if math.isnan(y):
             values.append(missing_value())
         elif header.class_attribute.is_nominal:
             values.append(header.class_attribute.index_of(str(y)))
         elif header.class_attribute.is_numeric:
             values.append(y)
         else:
             raise Exception("Unsupported attribute type for class attribute: %s" % header.class_attribute.type_str())
```

### Comparing `sklearn-weka-plugin-0.0.6/src/sklweka/preprocessing.py` & `sklearn-weka-plugin-0.0.7/src/sklweka/preprocessing.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,59 +75,59 @@
         Returns the underlying dataset header, if any.
 
         :return: the dataset structure
         :rtype: Instances
         """
         return self.header_
 
-    def fit(self, data, targets):
+    def fit(self, X, y):
         """
         Trains the estimator.
 
-        :param data: the input variables as matrix, array-like of shape (n_samples, n_features)
-        :type data: ndarray
-        :param targets: the optional class attribute column, array-like of shape (n_samples,)
-        :type targets: ndarray
+        :param X: the input variables as matrix, array-like of shape (n_samples, n_features)
+        :type X: ndarray
+        :param y: the optional class attribute column, array-like of shape (n_samples,)
+        :type y: ndarray
         :return: itself
         :rtype: WekaTransformer
         """
-        if targets is None:
-            check_array(data)
+        if y is None:
+            check_array(X)
         else:
-            check_X_y(data, targets)
-        d = to_instances(data, y=targets,
+            check_X_y(X, y)
+        d = to_instances(X, y=y,
                          num_nominal_labels=self._num_nominal_input_labels,
                          num_class_labels=self._num_nominal_output_labels)
         self.header_ = Instances.template_instances(d)
         self._filter.inputformat(d)
         self._filter.filter(d)
         return self
 
-    def transform(self, data, targets=None):
+    def transform(self, X, y=None):
         """
         Filters the data.
 
-        :param data: the data to filter, array-like of shape (n_samples, n_features)
-        :type data: ndarray
-        :param targets: the optional class attribute column, array-like of shape (n_samples,)
-        :type targets: ndarray
+        :param X: the data to filter, array-like of shape (n_samples, n_features)
+        :type X: ndarray
+        :param y: the optional class attribute column, array-like of shape (n_samples,)
+        :type y: ndarray
         :return: the filtered data, X if no targets or (X, y) if targets provided
         :rtype: ndarray or tuple
         """
         check_is_fitted(self)
-        no_targets = targets is None
+        no_targets = y is None
 
         # dummy class values necessary?
         if no_targets and self.header_.has_class():
-            targets = []
-            for i in range(data.shape[0]):
-                targets.append(missing_value())
-            targets = np.array(targets)
+            y = []
+            for i in range(X.shape[0]):
+                y.append(missing_value())
+            y = np.array(y)
 
-        d = to_instances(data, y=targets,
+        d = to_instances(X, y=y,
                          num_nominal_labels=self._num_nominal_input_labels,
                          num_class_labels=self._num_nominal_output_labels)
         d_new = self._filter.filter(d)
         X, y = to_array(d_new)
         if no_targets:
             return X
         else:
@@ -250,48 +250,48 @@
         Returns whether the output variable gets converted as well.
 
         :return: True if the output variable gets converted
         :rtype: bool
         """
         return self._input_vars
 
-    def fit(self, data, targets):
+    def fit(self, X, y):
         """
         Trains the estimator.
 
-        :param data: the input variables as matrix, array-like of shape (n_samples, n_features)
-        :type data: ndarray
-        :param targets: the optional class attribute column, array-like of shape (n_samples,)
-        :type targets: ndarray
+        :param X: the input variables as matrix, array-like of shape (n_samples, n_features)
+        :type X: ndarray
+        :param y: the optional class attribute column, array-like of shape (n_samples,)
+        :type y: ndarray
         :return: itself
         :rtype: WekaTransformer
         """
-        if targets is None:
-            check_array(data, dtype=None)
+        if y is None:
+            check_array(X, dtype=None)
         else:
-            check_X_y(data, targets, dtype=None)
+            check_X_y(X, y, dtype=None)
         self.initialized_ = True
         return self
 
-    def transform(self, data, targets=None):
+    def transform(self, X, y=None):
         """
         Filters the data.
 
-        :param data: the data to filter, array-like of shape (n_samples, n_features)
-        :type data: ndarray
-        :param targets: the optional class attribute column, array-like of shape (n_samples,)
-        :type targets: ndarray
+        :param X: the data to filter, array-like of shape (n_samples, n_features)
+        :type X: ndarray
+        :param y: the optional class attribute column, array-like of shape (n_samples,)
+        :type y: ndarray
         :return: the filtered data, X if no targets or (X, y) if targets provided
         :rtype: ndarray or tuple
         """
         check_is_fitted(self)
-        X_new = to_nominal_attributes(data, self._input_vars)
+        X_new = to_nominal_attributes(X, self._input_vars)
         y_new = None
-        if targets is not None:
-            y_new = to_nominal_labels(targets)
+        if y is not None:
+            y_new = to_nominal_labels(y)
         return X_new, y_new
 
     def get_params(self, deep=True):
         """
         Returns the parameters for this classifier, basically classname and options list.
 
         :param deep: ignored
```

