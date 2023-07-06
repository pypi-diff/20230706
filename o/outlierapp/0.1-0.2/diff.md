# Comparing `tmp/outlierapp-0.1.tar.gz` & `tmp/outlierapp-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outlierapp-0.1.tar", last modified: Wed Jul  5 12:47:17 2023, max compression
+gzip compressed data, was "outlierapp-0.2.tar", last modified: Thu Jul  6 11:49:44 2023, max compression
```

## Comparing `outlierapp-0.1.tar` & `outlierapp-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 12:47:17.193921 outlierapp-0.1/
--rw-rw-rw-   0        0        0     1026 2022-10-24 06:41:56.000000 outlierapp-0.1/LICENSE
--rw-rw-rw-   0        0        0    16140 2023-07-05 12:47:17.197916 outlierapp-0.1/PKG-INFO
--rw-rw-rw-   0        0        0    15570 2023-05-17 07:08:41.000000 outlierapp-0.1/README.md
--rw-rw-rw-   0        0        0      648 2023-07-05 12:06:58.000000 outlierapp-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 12:47:17.221922 outlierapp-0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-05 12:47:15.886944 outlierapp-0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 12:47:16.703927 outlierapp-0.1/src/outlierapp/
--rw-rw-rw-   0        0        0      161 2022-11-09 11:44:18.000000 outlierapp-0.1/src/outlierapp/__init__.py
--rw-rw-rw-   0        0        0     8115 2023-05-17 08:58:13.000000 outlierapp-0.1/src/outlierapp/anomaly_data_preprocessing.py
--rw-rw-rw-   0        0        0     5444 2023-05-17 08:58:30.000000 outlierapp-0.1/src/outlierapp/anomaly_detection.py
--rw-rw-rw-   0        0        0     1942 2023-05-15 09:46:21.000000 outlierapp-0.1/src/outlierapp/anomaly_libs.py
--rw-rw-rw-   0        0        0    15810 2023-07-05 12:13:02.000000 outlierapp-0.1/src/outlierapp/anomaly_main.py
--rw-rw-rw-   0        0        0     3363 2023-05-17 08:59:21.000000 outlierapp-0.1/src/outlierapp/anomaly_models.py
-drwxrwxrwx   0        0        0        0 2023-07-05 12:47:17.108914 outlierapp-0.1/src/outlierapp.egg-info/
--rw-rw-rw-   0        0        0    16140 2023-07-05 12:47:15.000000 outlierapp-0.1/src/outlierapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-07-05 12:47:15.000000 outlierapp-0.1/src/outlierapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 12:47:15.000000 outlierapp-0.1/src/outlierapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-05 12:47:15.000000 outlierapp-0.1/src/outlierapp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 11:49:44.143428 outlierapp-0.2/
+-rw-rw-rw-   0        0        0     1026 2022-10-24 06:41:56.000000 outlierapp-0.2/LICENSE
+-rw-rw-rw-   0        0        0    16140 2023-07-06 11:49:44.157459 outlierapp-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    15570 2023-05-17 07:08:41.000000 outlierapp-0.2/README.md
+-rw-rw-rw-   0        0        0      648 2023-07-06 11:48:36.000000 outlierapp-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 11:49:44.191409 outlierapp-0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 11:49:42.603430 outlierapp-0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 11:49:43.567410 outlierapp-0.2/src/outlierapp/
+-rw-rw-rw-   0        0        0      161 2022-11-09 11:44:18.000000 outlierapp-0.2/src/outlierapp/__init__.py
+-rw-rw-rw-   0        0        0     8115 2023-05-17 08:58:13.000000 outlierapp-0.2/src/outlierapp/anomaly_data_preprocessing.py
+-rw-rw-rw-   0        0        0     5444 2023-05-17 08:58:30.000000 outlierapp-0.2/src/outlierapp/anomaly_detection.py
+-rw-rw-rw-   0        0        0     1942 2023-05-15 09:46:21.000000 outlierapp-0.2/src/outlierapp/anomaly_libs.py
+-rw-rw-rw-   0        0        0    15811 2023-07-06 11:48:38.000000 outlierapp-0.2/src/outlierapp/anomaly_main.py
+-rw-rw-rw-   0        0        0     3363 2023-05-17 08:59:21.000000 outlierapp-0.2/src/outlierapp/anomaly_models.py
+drwxrwxrwx   0        0        0        0 2023-07-06 11:49:44.011399 outlierapp-0.2/src/outlierapp.egg-info/
+-rw-rw-rw-   0        0        0    16140 2023-07-06 11:49:42.000000 outlierapp-0.2/src/outlierapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-07-06 11:49:42.000000 outlierapp-0.2/src/outlierapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 11:49:42.000000 outlierapp-0.2/src/outlierapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-06 11:49:42.000000 outlierapp-0.2/src/outlierapp.egg-info/top_level.txt
```

### Comparing `outlierapp-0.1/LICENSE` & `outlierapp-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `outlierapp-0.1/PKG-INFO` & `outlierapp-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outlierapp
-Version: 0.1
+Version: 0.2
 Summary: Anomaly Detection package
 Author-email: Volvo <chatterjeedevosmita267@gmail.com>
 Project-URL: Homepage, https://github.com/devosmitachatterjee2018/AnomalyDetectionApp
 Project-URL: Bug Tracker, https://github.com/devosmitachatterjee2018/AnomalyDetectionApp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `outlierapp-0.1/README.md` & `outlierapp-0.2/README.md`

 * *Files identical despite different names*

### Comparing `outlierapp-0.1/pyproject.toml` & `outlierapp-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "outlierapp"
-version = "0.1"
+version = "0.2"
 authors = [
   { name="Volvo", email="chatterjeedevosmita267@gmail.com" },
 ]
 description = "Anomaly Detection package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `outlierapp-0.1/src/outlierapp/anomaly_data_preprocessing.py` & `outlierapp-0.2/src/outlierapp/anomaly_data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `outlierapp-0.1/src/outlierapp/anomaly_detection.py` & `outlierapp-0.2/src/outlierapp/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `outlierapp-0.1/src/outlierapp/anomaly_libs.py` & `outlierapp-0.2/src/outlierapp/anomaly_libs.py`

 * *Files identical despite different names*

### Comparing `outlierapp-0.1/src/outlierapp/anomaly_main.py` & `outlierapp-0.2/src/outlierapp/anomaly_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
         #user_choice = input("Do you wish to change suggested best parameters (Y/N): ")
         #if user_choice.casefold() == 'y':
         #    self.dbscan_eps, self.dbscan_n_samples, self.thyme_boost_p, self.ocsvm_kernel, self.ocsvm_nu, self.lof_alg, self.lof_contamination = self.user_parameters()
         #else:
         #    self.dbscan_eps, self.dbscan_n_samples, self.thyme_boost_p, self.ocsvm_kernel, self.ocsvm_nu, self.lof_alg, self.lof_contamination = self.find_parameters()
 
-        self.dbscan_eps, self.dbscan_n_samples, self.thyme_boost_p, self.ocsvm_kernel, self.ocsvm_nu, self.lof_alg, self.lof_contamination = self.find_parameters()
+        #self.dbscan_eps, self.dbscan_n_samples, self.thyme_boost_p, self.ocsvm_kernel, self.ocsvm_nu, self.lof_alg, self.lof_contamination = self.find_parameters()
 
         parameters = {
             "id":self.id_column, 
             "time_column":self.time_column, 
             "models":self.models, 
             "threshold":self.threshold, 
             "eps":self.dbscan_eps,
```

### Comparing `outlierapp-0.1/src/outlierapp/anomaly_models.py` & `outlierapp-0.2/src/outlierapp/anomaly_models.py`

 * *Files identical despite different names*

### Comparing `outlierapp-0.1/src/outlierapp.egg-info/PKG-INFO` & `outlierapp-0.2/src/outlierapp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outlierapp
-Version: 0.1
+Version: 0.2
 Summary: Anomaly Detection package
 Author-email: Volvo <chatterjeedevosmita267@gmail.com>
 Project-URL: Homepage, https://github.com/devosmitachatterjee2018/AnomalyDetectionApp
 Project-URL: Bug Tracker, https://github.com/devosmitachatterjee2018/AnomalyDetectionApp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

