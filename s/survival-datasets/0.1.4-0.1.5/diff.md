# Comparing `tmp/survival-datasets-0.1.4.tar.gz` & `tmp/survival-datasets-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survival-datasets-0.1.4.tar", last modified: Fri Mar 31 14:05:25 2023, max compression
+gzip compressed data, was "survival-datasets-0.1.5.tar", last modified: Thu Jul  6 13:01:45 2023, max compression
```

## Comparing `survival-datasets-0.1.4.tar` & `survival-datasets-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 14:05:25.089850 survival-datasets-0.1.4/
--rw-rw-rw-   0        0        0     1091 2023-03-31 10:01:14.000000 survival-datasets-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       32 2023-03-31 13:23:48.000000 survival-datasets-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2597 2023-03-31 14:05:25.089555 survival-datasets-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1626 2023-03-31 14:04:52.000000 survival-datasets-0.1.4/README.md
--rw-rw-rw-   0        0        0       99 2023-03-31 10:01:14.000000 survival-datasets-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-31 14:05:25.090846 survival-datasets-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1439 2023-03-31 14:05:02.000000 survival-datasets-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 14:05:25.052068 survival-datasets-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-03-31 14:05:25.075068 survival-datasets-0.1.4/src/survdata/
--rw-rw-rw-   0        0        0        0 2023-03-31 13:06:46.000000 survival-datasets-0.1.4/src/survdata/__init__.py
--rw-rw-rw-   0        0        0     3265 2023-03-31 13:27:46.000000 survival-datasets-0.1.4/src/survdata/datasets.py
--rw-rw-rw-   0        0        0    63362 2023-03-10 09:44:42.000000 survival-datasets-0.1.4/src/survdata/metabric.feather
--rw-rw-rw-   0        0        0   396119 2023-03-20 13:22:25.000000 survival-datasets-0.1.4/src/survdata/seer.csv
--rw-rw-rw-   0        0        0   318058 2023-03-10 09:44:42.000000 survival-datasets-0.1.4/src/survdata/support.feather
-drwxrwxrwx   0        0        0        0 2023-03-31 14:05:25.084844 survival-datasets-0.1.4/src/survival_datasets.egg-info/
--rw-rw-rw-   0        0        0     2597 2023-03-31 14:05:24.000000 survival-datasets-0.1.4/src/survival_datasets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-03-31 14:05:24.000000 survival-datasets-0.1.4/src/survival_datasets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 14:05:24.000000 survival-datasets-0.1.4/src/survival_datasets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-03-31 14:05:24.000000 survival-datasets-0.1.4/src/survival_datasets.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-31 14:05:24.000000 survival-datasets-0.1.4/src/survival_datasets.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-31 14:05:25.086846 survival-datasets-0.1.4/tests/
--rw-rw-rw-   0        0        0     1182 2023-03-31 13:14:30.000000 survival-datasets-0.1.4/tests/test_data_loader.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:45.198299 survival-datasets-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-03-31 10:01:14.000000 survival-datasets-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-03-31 13:23:48.000000 survival-datasets-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2597 2023-07-06 13:01:45.197776 survival-datasets-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1626 2023-03-31 14:07:52.000000 survival-datasets-0.1.5/README.md
+-rw-rw-rw-   0        0        0       99 2023-03-31 10:01:14.000000 survival-datasets-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 13:01:45.198979 survival-datasets-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1429 2023-07-06 12:56:42.000000 survival-datasets-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:45.165050 survival-datasets-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:45.184049 survival-datasets-0.1.5/src/survdata/
+-rw-rw-rw-   0        0        0        0 2023-03-31 13:06:46.000000 survival-datasets-0.1.5/src/survdata/__init__.py
+-rw-rw-rw-   0        0        0     3265 2023-03-31 14:12:14.000000 survival-datasets-0.1.5/src/survdata/datasets.py
+-rw-rw-rw-   0        0        0    63362 2023-03-10 09:44:42.000000 survival-datasets-0.1.5/src/survdata/metabric.feather
+-rw-rw-rw-   0        0        0   396119 2023-03-20 13:22:25.000000 survival-datasets-0.1.5/src/survdata/seer.csv
+-rw-rw-rw-   0        0        0   318058 2023-03-10 09:44:42.000000 survival-datasets-0.1.5/src/survdata/support.feather
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:45.195426 survival-datasets-0.1.5/src/survival_datasets.egg-info/
+-rw-rw-rw-   0        0        0     2597 2023-07-06 13:01:45.000000 survival-datasets-0.1.5/src/survival_datasets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-07-06 13:01:45.000000 survival-datasets-0.1.5/src/survival_datasets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 13:01:45.000000 survival-datasets-0.1.5/src/survival_datasets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-06 13:01:45.000000 survival-datasets-0.1.5/src/survival_datasets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 13:01:45.000000 survival-datasets-0.1.5/src/survival_datasets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:45.196601 survival-datasets-0.1.5/tests/
+-rw-rw-rw-   0        0        0     1182 2023-03-31 13:14:30.000000 survival-datasets-0.1.5/tests/test_data_loader.py
```

### Comparing `survival-datasets-0.1.4/LICENSE` & `survival-datasets-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `survival-datasets-0.1.4/PKG-INFO` & `survival-datasets-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survival-datasets
-Version: 0.1.4
+Version: 0.1.5
 Summary: Data loader for common datasets in Survival Analysis.
 Home-page: https://github.com/thecml/survival-datasets
 Author: Christian Marius Lillelund
 Author-email: chr1000@gmail.com
 Keywords: Survival Analysis,Datasets
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `survival-datasets-0.1.4/README.md` & `survival-datasets-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `survival-datasets-0.1.4/setup.py` & `survival-datasets-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'survival-datasets', 
-    version = '0.1.4',
+    version = '0.1.5',
     description = 'Data loader for common datasets in Survival Analysis.',
     packages = find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     author = 'Christian Marius Lillelund',
     author_email = 'chr1000@gmail.com',
     
@@ -27,17 +27,17 @@
         'Intended Audience :: Science/Research',
         'Intended Audience :: Education',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Operating System :: OS Independent',
     ],
     
     install_requires = [
-        'scikit-survival ~= 0.17.2',
-        'pandas ~= 1.4.3',
-        'numpy ~= 1.22.4',
-        'shap ~= 0.41.0',
-        'pyarrow ~= 11.0.0',
+        'scikit-survival ~= 0.17',
+        'pandas ~= 1.4',
+        'numpy ~= 1.22',
+        'shap ~= 0.41',
+        'pyarrow ~= 11.0',
     ],
     
     keywords = ['Survival Analysis', 'Datasets'],
     
 )
```

### Comparing `survival-datasets-0.1.4/src/survdata/datasets.py` & `survival-datasets-0.1.5/src/survdata/datasets.py`

 * *Files identical despite different names*

### Comparing `survival-datasets-0.1.4/src/survdata/metabric.feather` & `survival-datasets-0.1.5/src/survdata/metabric.feather`

 * *Files identical despite different names*

### Comparing `survival-datasets-0.1.4/src/survdata/seer.csv` & `survival-datasets-0.1.5/src/survdata/seer.csv`

 * *Files identical despite different names*

### Comparing `survival-datasets-0.1.4/src/survdata/support.feather` & `survival-datasets-0.1.5/src/survdata/support.feather`

 * *Files identical despite different names*

### Comparing `survival-datasets-0.1.4/src/survival_datasets.egg-info/PKG-INFO` & `survival-datasets-0.1.5/src/survival_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survival-datasets
-Version: 0.1.4
+Version: 0.1.5
 Summary: Data loader for common datasets in Survival Analysis.
 Home-page: https://github.com/thecml/survival-datasets
 Author: Christian Marius Lillelund
 Author-email: chr1000@gmail.com
 Keywords: Survival Analysis,Datasets
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `survival-datasets-0.1.4/tests/test_data_loader.py` & `survival-datasets-0.1.5/tests/test_data_loader.py`

 * *Files identical despite different names*

