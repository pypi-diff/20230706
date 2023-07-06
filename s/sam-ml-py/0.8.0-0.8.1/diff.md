# Comparing `tmp/sam_ml-py-0.8.0.tar.gz` & `tmp/sam_ml-py-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sam_ml-py-0.8.0.tar", last modified: Wed Jul  5 08:58:33 2023, max compression
+gzip compressed data, was "sam_ml-py-0.8.1.tar", last modified: Wed Jul  5 18:02:38 2023, max compression
```

## Comparing `sam_ml-py-0.8.0.tar` & `sam_ml-py-0.8.1.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:33.790266 sam_ml-py-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-05 08:58:33.790266 sam_ml-py-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:33.778266 sam_ml-py-0.8.0/sam_ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:33.778266 sam_ml-py-0.8.0/sam_ml/config/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/config/global_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/config/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:33.782266 sam_ml-py-0.8.0/sam_ml/data/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/data/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/data/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/data/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/data/scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/data/synthetic_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:33.786266 sam_ml-py-0.8.0/sam_ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/AdaBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/BaggingClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/BernoulliNB.py
--rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/ClassifierTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/DecisionTreeClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/ExtraTreesClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/GaussianNB.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/GaussianProcessClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/GradientBoostingMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/KNeighborsClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/LinearDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/LinearSupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/LogisticRegression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/MLPClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/QuadraticDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/RandomForestClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/SupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/XGBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22829 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/main_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/main_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/main_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:33.790266 sam_ml-py-0.8.0/sam_ml_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-05 08:58:33.000000 sam_ml-py-0.8.0/sam_ml_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-05 08:58:33.000000 sam_ml-py-0.8.0/sam_ml_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:58:33.000000 sam_ml-py-0.8.0/sam_ml_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-05 08:58:33.000000 sam_ml-py-0.8.0/sam_ml_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 08:58:33.000000 sam_ml-py-0.8.0/sam_ml_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-05 08:58:33.790266 sam_ml-py-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:33.790266 sam_ml-py-0.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/test/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:38.007584 sam_ml-py-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-05 18:02:38.007584 sam_ml-py-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:38.003584 sam_ml-py-0.8.1/sam_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:38.003584 sam_ml-py-0.8.1/sam_ml/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/config/global_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/config/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:38.003584 sam_ml-py-0.8.1/sam_ml/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/data/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/data/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/data/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/data/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/data/synthetic_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:38.007584 sam_ml-py-0.8.1/sam_ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/AdaBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/BaggingClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/BernoulliNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/ClassifierTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/DecisionTreeClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/ExtraTreesClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/GaussianNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/GaussianProcessClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/GradientBoostingMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/KNeighborsClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/LinearDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/LinearSupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/LogisticRegression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/MLPClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/QuadraticDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/RandomForestClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/SupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/XGBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/main_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/main_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/main_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:38.007584 sam_ml-py-0.8.1/sam_ml_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-05 18:02:37.000000 sam_ml-py-0.8.1/sam_ml_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-05 18:02:37.000000 sam_ml-py-0.8.1/sam_ml_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:02:37.000000 sam_ml-py-0.8.1/sam_ml_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-05 18:02:37.000000 sam_ml-py-0.8.1/sam_ml_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 18:02:37.000000 sam_ml-py-0.8.1/sam_ml_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-05 18:02:38.007584 sam_ml-py-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:38.007584 sam_ml-py-0.8.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/test/test_CTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/test/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/test/test_pipeline.py
```

### Comparing `sam_ml-py-0.8.0/LICENSE` & `sam_ml-py-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/PKG-INFO` & `sam_ml-py-0.8.1/sam_ml_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sam_ml-py
-Version: 0.8.0
+Name: sam-ml-py
+Version: 0.8.1
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: with_swig
@@ -46,14 +46,16 @@
 
 1. install the package to your activated virtual environment *(python version 3.10 and higher is needed)*
 
 ```
 pip install sam-ml-py
 ```
 
+## start using it
+
 2. now you can import the package, e.g.:
 
 ```
 from sam_ml.models import RFC
 
 RandomForestClassifier = RFC()
 ```
```

### Comparing `sam_ml-py-0.8.0/README.md` & `sam_ml-py-0.8.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
 1. install the package to your activated virtual environment *(python version 3.10 and higher is needed)*
 
 ```
 pip install sam-ml-py
 ```
 
+## start using it
+
 2. now you can import the package, e.g.:
 
 ```
 from sam_ml.models import RFC
 
 RandomForestClassifier = RFC()
 ```
```

### Comparing `sam_ml-py-0.8.0/sam_ml/config/logging.py` & `sam_ml-py-0.8.1/sam_ml/config/logging.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/data/embeddings.py` & `sam_ml-py-0.8.1/sam_ml/data/embeddings.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/data/feature_selection.py` & `sam_ml-py-0.8.1/sam_ml/data/feature_selection.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/data/sampling.py` & `sam_ml-py-0.8.1/sam_ml/data/sampling.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/data/scaler.py` & `sam_ml-py-0.8.1/sam_ml/data/scaler.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/data/synthetic_data.py` & `sam_ml-py-0.8.1/sam_ml/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/AdaBoostClassifier.py` & `sam_ml-py-0.8.1/sam_ml/models/AdaBoostClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/BaggingClassifier.py` & `sam_ml-py-0.8.1/sam_ml/models/BaggingClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/BernoulliNB.py` & `sam_ml-py-0.8.1/sam_ml/models/BernoulliNB.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/ClassifierTest.py` & `sam_ml-py-0.8.1/sam_ml/models/ClassifierTest.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import pygame
 from pkg_resources import resource_filename
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.linear_model import LogisticRegression
 from tqdm.auto import tqdm
 
-from sam_ml.config import setup_logger
+from sam_ml.config import get_sound_on, setup_logger
 from sam_ml.data import Embeddings_builder, Sampler, Scaler, Selector
 
 from .AdaBoostClassifier import ABC
 from .BaggingClassifier import BC
 from .BernoulliNB import BNB
 from .DecisionTreeClassifier import DTC
 from .ExtraTreesClassifier import ETC
@@ -191,18 +191,45 @@
             print(f"Cannot find model combination '{kind}' --> using all models")
             models = self.model_combs("all")
 
         return models
 
     def __finish_sound(self):
         """ little function to play a microwave sound """
-        filepath = resource_filename(__name__, 'microwave_finish_sound.mp3')
-        pygame.mixer.init()
-        pygame.mixer.music.load(filepath)
-        pygame.mixer.music.play()
+        if get_sound_on():
+            filepath = resource_filename(__name__, 'microwave_finish_sound.mp3')
+            pygame.mixer.init()
+            pygame.mixer.music.load(filepath)
+            pygame.mixer.music.play()
+
+    def output_scores_as_pd(self, sort_by: Union[str, list[str]] = "index", console_out: bool = True) -> pd.DataFrame:
+        """
+        @param:
+            sorted_by:
+                'index': sort index ascending=True
+                'precision'/'recall'/'accuracy'/'train_score'/'train_time': sort by these columns ascending=False
+
+                e.g. ['precision', 'recall'] - sort first by 'precision' and then by 'recall'
+        """
+        if self.scores != {}:
+            if sort_by == "index":
+                scores = pd.DataFrame.from_dict(self.scores, orient="index").sort_index(ascending=True)
+            else:
+                scores = (
+                    pd.DataFrame.from_dict(self.scores, orient="index")
+                    .sort_values(by=sort_by, ascending=False)
+                )
+
+            if console_out:
+                print(scores)
+        else:
+            logger.warning("no scores are created -> use 'eval_models()'/'eval_models_cv()' to create scores")
+            scores = None
+
+        return scores
 
     def eval_models(
         self,
         x_train: pd.DataFrame,
         y_train: pd.Series,
         x_test: pd.DataFrame,
         y_test: pd.Series,
@@ -283,40 +310,14 @@
             self.__finish_sound()
             return self.scores
 
         except KeyboardInterrupt:
             logger.info("KeyboardInterrupt - output interim result")
             return self.scores
 
-    def output_scores_as_pd(self, sort_by: Union[str, list[str]] = "index", console_out: bool = True) -> pd.DataFrame:
-        """
-        @param:
-            sorted_by:
-                'index': sort index ascending=True
-                'precision'/'recall'/'accuracy'/'train_score'/'train_time': sort by these columns ascending=False
-
-                e.g. ['precision', 'recall'] - sort first by 'precision' and then by 'recall'
-        """
-        if self.scores != {}:
-            if sort_by == "index":
-                scores = pd.DataFrame.from_dict(self.scores, orient="index").sort_index(ascending=True)
-            else:
-                scores = (
-                    pd.DataFrame.from_dict(self.scores, orient="index")
-                    .sort_values(by=sort_by, ascending=False)
-                )
-
-            if console_out:
-                print(scores)
-        else:
-            logger.warning("no scores are created -> use 'eval_models()'/'eval_models_cv()' to create scores")
-            scores = None
-
-        return scores
-
     def find_best_model_randomCV(
         self,
         x_train: pd.DataFrame,
         y_train: pd.Series,
         x_test: pd.DataFrame,
         y_test: pd.Series,
         n_trails: int = 5,
```

### Comparing `sam_ml-py-0.8.0/sam_ml/models/DecisionTreeClassifier.py` & `sam_ml-py-0.8.1/sam_ml/models/DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/ExtraTreesClassifier.py` & `sam_ml-py-0.8.1/sam_ml/models/ExtraTreesClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/GaussianNB.py` & `sam_ml-py-0.8.1/sam_ml/models/GaussianNB.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/GaussianProcessClassifier.py` & `sam_ml-py-0.8.1/sam_ml/models/GaussianProcessClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/GradientBoostingMachine.py` & `sam_ml-py-0.8.1/sam_ml/models/GradientBoostingMachine.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,29 +33,27 @@
         grid = ConfigurationSpace(
             seed=42,
             space={
             "n_estimators": Integer("n_estimators", (20, 1500), log=True, default=100),
             "max_depth": Integer("max_depth", (1, 15), distribution=Normal(5, 3), default=3),
             "min_samples_split": Integer("min_samples_split", (2, 100), log=True, default=2),
             "min_samples_leaf": Integer("min_samples_leaf", (1, 100), log=True, default=1),
-            "max_features": Categorical("max_features", ["auto", "sqrt", "log2"], default="auto"),
+            "max_features": Categorical("max_features", [1.0, "sqrt", "log2"], default=1.0),
             "subsample": Float("subsample", (0.7, 1), default=1),
             "criterion": Categorical("criterion", ["friedman_mse", "squared_error"], default="friedman_mse"),
-            "loss": Categorical("loss", ["log_loss", "deviance"], default="log_loss"),
             "learning_rate": Float("learning_rate", (0.005, 0.3), log=True, default=0.1),
             })
         
         # workaround for now -> Problems with Normal distribution (in smac_search) (04/07/2023)
         self.smac_grid = ConfigurationSpace(
             seed=42,
             space={
             "n_estimators": Integer("n_estimators", (20, 1500), log=True, default=100),
             "max_depth": Integer("max_depth", (1, 15), default=3),
             "min_samples_split": Integer("min_samples_split", (2, 100), log=True, default=2),
             "min_samples_leaf": Integer("min_samples_leaf", (1, 100), log=True, default=1),
-            "max_features": Categorical("max_features", ["auto", "sqrt", "log2"], default="auto"),
+            "max_features": Categorical("max_features", [1.0, "sqrt", "log2"], default=1.0),
             "subsample": Float("subsample", (0.7, 1), default=1),
             "criterion": Categorical("criterion", ["friedman_mse", "squared_error"], default="friedman_mse"),
-            "loss": Categorical("loss", ["log_loss", "deviance"], default="log_loss"),
             "learning_rate": Float("learning_rate", (0.005, 0.3), log=True, default=0.1),
             })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.8.0/sam_ml/models/KNeighborsClassifier.py` & `sam_ml-py-0.8.1/sam_ml/models/KNeighborsClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/LinearDiscriminantAnalysis.py` & `sam_ml-py-0.8.1/sam_ml/models/LinearDiscriminantAnalysis.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/LinearSupportVectorClassifier.py` & `sam_ml-py-0.8.1/sam_ml/models/LinearSupportVectorClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/LogisticRegression.py` & `sam_ml-py-0.8.1/sam_ml/models/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/MLPClassifier.py` & `sam_ml-py-0.8.1/sam_ml/models/MLPClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/QuadraticDiscriminantAnalysis.py` & `sam_ml-py-0.8.1/sam_ml/models/QuadraticDiscriminantAnalysis.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/RandomForestClassifier.py` & `sam_ml-py-0.8.1/sam_ml/models/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/SupportVectorClassifier.py` & `sam_ml-py-0.8.1/sam_ml/models/SupportVectorClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/XGBoostClassifier.py` & `sam_ml-py-0.8.1/sam_ml/models/XGBoostClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/__init__.py` & `sam_ml-py-0.8.1/sam_ml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/main_classifier.py` & `sam_ml-py-0.8.1/sam_ml/models/main_classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
 
         return self.cv_scores
 
     def feature_importance(self) -> plt.show:
         """
         feature_importance() generates a matplotlib plot of the feature importance from self.model
         """
-        if not self.trained:
+        if not self.feature_names:
             logger.error("You have to first train the classifier before getting the feature importance")
             return
 
         if self.model_type == "MLPC":
             importances = [np.mean(i) for i in self.model.coefs_[0]]  # MLP Classifier
         elif self.model_type in ("DTC", "RFC", "GBM", "CBC", "ABC", "ETC", "XGBC"):
             importances = self.model.feature_importances_
```

### Comparing `sam_ml-py-0.8.0/sam_ml/models/main_model.py` & `sam_ml-py-0.8.1/sam_ml/models/main_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,19 +19,18 @@
             model_object: model with 'fit', 'predict', 'set_params', and 'get_params' method (see sklearn API)
             model_name: name of the model
             model_type: kind of estimator (e.g. 'RFC' for RandomForestClassifier)
         """
         self.model = model_object
         self.model_name = model_name
         self.model_type = model_type
-        self.trained: bool = False
         self.train_score: float = None
         self.train_time: str = None
         self.test_score: Union[float, dict[str, float]] = None
-        self.feature_names: list = None
+        self.feature_names: list = []
 
     def __repr__(self) -> str:
         return f"Model(model_object={self.model.__str__()}, model_name='{self.model_name}', model_type='{self.model_type}')"
 
     def train(self, x_train: pd.DataFrame, y_train: pd.Series, console_out: bool = True) -> tuple[float, str]:
         """
         @return:
@@ -47,16 +46,14 @@
         self.train_time = str(timedelta(seconds=int(end_time-start_time)))
 
         if console_out:
             print("Train score: ", self.train_score, " - Train time: ", self.train_time)
             
         logger.debug(f"training {self.model_name} - finished")
 
-        self.trained = True
-
         return self.train_score, self.train_time
 
     def fit(self, x_train: pd.DataFrame, y_train: pd.Series):
         self.model.fit(x_train, y_train)
         return self
 
     def predict(self, x_test: pd.DataFrame) -> list:
```

### Comparing `sam_ml-py-0.8.0/sam_ml/models/main_pipeline.py` & `sam_ml-py-0.8.1/sam_ml/models/main_pipeline.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml/models/scorer.py` & `sam_ml-py-0.8.1/sam_ml/models/scorer.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.0/sam_ml_py.egg-info/PKG-INFO` & `sam_ml-py-0.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sam-ml-py
-Version: 0.8.0
+Name: sam_ml-py
+Version: 0.8.1
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: with_swig
@@ -46,14 +46,16 @@
 
 1. install the package to your activated virtual environment *(python version 3.10 and higher is needed)*
 
 ```
 pip install sam-ml-py
 ```
 
+## start using it
+
 2. now you can import the package, e.g.:
 
 ```
 from sam_ml.models import RFC
 
 RandomForestClassifier = RFC()
 ```
```

### Comparing `sam_ml-py-0.8.0/sam_ml_py.egg-info/SOURCES.txt` & `sam_ml-py-0.8.1/sam_ml_py.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -37,8 +37,10 @@
 sam_ml/models/scorer.py
 sam_ml_py.egg-info/PKG-INFO
 sam_ml_py.egg-info/SOURCES.txt
 sam_ml_py.egg-info/dependency_links.txt
 sam_ml_py.egg-info/requires.txt
 sam_ml_py.egg-info/top_level.txt
 test/__init__.py
-test/test_models.py
+test/test_CTest.py
+test/test_classifier.py
+test/test_pipeline.py
```

### Comparing `sam_ml-py-0.8.0/setup.py` & `sam_ml-py-0.8.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="sam_ml-py",
-    version="0.8.0",
+    version="0.8.1",
     description="a library for ML programing created by Samuel Brinkmann",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.10",
     packages=find_packages(),
     package_data={},
     scripts=[],
```

### Comparing `sam_ml-py-0.8.0/test/test_models.py` & `sam_ml-py-0.8.1/test/test_pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,74 +30,70 @@
                             n_informative = 5,
                             n_redundant = 0,
                             n_classes = 3,
                             weights = [.2, .3, .8])
 X = pd.DataFrame(X, columns=["col1", "col2", "col3", "col4", "col5"])
 Y = pd.Series(Y)
 
-
-def test_classifier_train_evaluate():
+def test_pipelines_fit_evaluate():
     for classifier in MODELS:
-        classifier.train(X, Y, console_out=False)
-        classifier.evaluate(X, Y, console_out=False)
-        classifier.evaluate_score(X, Y)
-
+        model = Pipeline(model=classifier, model_name=classifier.model_name)
+        model.fit(X, Y)
+        model.evaluate(X, Y, console_out=False)
+        model.evaluate_score(X, Y)
 
 def test_pipelines_train_evaluate():
     for classifier in MODELS:
         model = Pipeline(model=classifier, model_name=classifier.model_name)
         model.train(X, Y, console_out=False)
         model.evaluate(X, Y, console_out=False)
         model.evaluate_score(X, Y)
 
-def test_classifier_crossvalidation():
-    for classifier in MODELS:
-        classifier.cross_validation(X, Y, cv_num=3)
-
 def test_pipelines_crossvalidation():
     for classifier in MODELS:
         model = Pipeline(model=classifier, model_name=classifier.model_name)
-        model.cross_validation(X, Y, cv_num=3)
-
-def test_classifier_crossvalidation_small_data():
-    for classifier in MODELS:
-        classifier.cross_validation_small_data(X, Y)
+        model.cross_validation(X, Y, cv_num=2)
 
 def test_pipelines_crossvalidation_small_data():
     for classifier in MODELS:
         model = Pipeline(model=classifier, model_name=classifier.model_name)
         model.cross_validation_small_data(X, Y)
 
-def test_classifier_randomCVsearch():
+def test_pipelines_randomCVsearch():
     for classifier in MODELS:
-        best_param, _ = classifier.randomCVsearch(X, Y, n_trails=5, cv_num=3)
+        model = Pipeline(model=classifier, model_name=classifier.model_name)
+        best_param, _ = model.randomCVsearch(X, Y, n_trails=5, cv_num=2)
         assert best_param != {}, "should always find a parameter combination"
 
-def test_pipelines_randomCVsearch():
+def test_pipelines_randomCVsearch_small_data():
     for classifier in MODELS:
         model = Pipeline(model=classifier, model_name=classifier.model_name)
-        best_param, _ = model.randomCVsearch(X, Y, n_trails=5, cv_num=3)
+        best_param, _ = model.randomCVsearch(X, Y, n_trails=5, cv_num=2, small_data_eval=True)
         assert best_param != {}, "should always find a parameter combination"
 
-def test_classifier_smac_search():
+@pytest.mark.with_swig
+def test_pipelines_smac_search():
     if SMAC_INSTALLED:
         for classifier in MODELS:
-            best_param = classifier.smac_search(X, Y, n_trails=10, cv_num=3)
+            model = Pipeline(model=classifier, model_name=classifier.model_name)
+            best_param = model.smac_search(X, Y, n_trails=5, cv_num=2)
             assert best_param != {}, "should always find a parameter combination"
     else:
         with pytest.raises(ImportError):
             for classifier in MODELS:
-                best_param = classifier.smac_search(X, Y, n_trails=10, cv_num=3)
+                model = Pipeline(model=classifier, model_name=classifier.model_name)
+                best_param = model.smac_search(X, Y, n_trails=5, cv_num=2)
                 assert best_param != {}, "should always find a parameter combination"
 
-def test_pipelines_smac_search():
+@pytest.mark.with_swig
+def test_pipelines_smac_search_small_data():
     if SMAC_INSTALLED:
         for classifier in MODELS:
             model = Pipeline(model=classifier, model_name=classifier.model_name)
-            best_param = model.smac_search(X, Y, n_trails=10, cv_num=3)
+            best_param = model.smac_search(X, Y, n_trails=5, cv_num=2, small_data_eval=True)
             assert best_param != {}, "should always find a parameter combination"
     else:
         with pytest.raises(ImportError):
             for classifier in MODELS:
                 model = Pipeline(model=classifier, model_name=classifier.model_name)
-                best_param = model.smac_search(X, Y, n_trails=10, cv_num=3)
+                best_param = model.smac_search(X, Y, n_trails=5, cv_num=2, small_data_eval=True)
                 assert best_param != {}, "should always find a parameter combination"
```

