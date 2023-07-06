# Comparing `tmp/py-datalab-0.1.0.tar.gz` & `tmp/py-datalab-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-datalab-0.1.0.tar", last modified: Thu Jul  6 10:31:37 2023, max compression
+gzip compressed data, was "py-datalab-0.1.1.tar", last modified: Thu Jul  6 10:45:56 2023, max compression
```

## Comparing `py-datalab-0.1.0.tar` & `py-datalab-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 10:31:37.788787 py-datalab-0.1.0/
--rw-rw-rw-   0        0        0     1085 2023-06-20 10:54:28.000000 py-datalab-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1018 2023-07-06 10:31:37.787788 py-datalab-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2437 2023-07-03 12:36:33.000000 py-datalab-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 10:31:37.760656 py-datalab-0.1.0/bin/
-drwxrwxrwx   0        0        0        0 2023-07-06 10:31:37.786787 py-datalab-0.1.0/bin/py_datalab.egg-info/
--rw-rw-rw-   0        0        0     1018 2023-07-06 10:31:37.000000 py-datalab-0.1.0/bin/py_datalab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-07-06 10:31:37.000000 py-datalab-0.1.0/bin/py_datalab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 10:31:37.000000 py-datalab-0.1.0/bin/py_datalab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 10:31:37.000000 py-datalab-0.1.0/bin/py_datalab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 10:31:37.788787 py-datalab-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1248 2023-07-06 10:21:36.000000 py-datalab-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:45:56.201971 py-datalab-0.1.1/
+-rw-rw-rw-   0        0        0     1085 2023-06-20 10:54:28.000000 py-datalab-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1018 2023-07-06 10:45:56.200464 py-datalab-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2437 2023-07-03 12:36:33.000000 py-datalab-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 10:45:56.177962 py-datalab-0.1.1/datalab/
+drwxrwxrwx   0        0        0        0 2023-07-06 10:45:56.198458 py-datalab-0.1.1/datalab/py_datalab.egg-info/
+-rw-rw-rw-   0        0        0     1018 2023-07-06 10:45:56.000000 py-datalab-0.1.1/datalab/py_datalab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-07-06 10:45:56.000000 py-datalab-0.1.1/datalab/py_datalab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 10:45:56.000000 py-datalab-0.1.1/datalab/py_datalab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 10:45:56.000000 py-datalab-0.1.1/datalab/py_datalab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 10:45:56.201971 py-datalab-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1256 2023-07-06 10:45:49.000000 py-datalab-0.1.1/setup.py
```

### Comparing `py-datalab-0.1.0/LICENSE` & `py-datalab-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-datalab-0.1.0/PKG-INFO` & `py-datalab-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-datalab
-Version: 0.1.0
+Version: 0.1.1
 Summary: This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 Home-page: https://github.com/matuszen/Python-DataLab
 Author: Mateusz Nowak
 Author-email: mateusz.nowak.pol@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py-datalab-0.1.0/README.md` & `py-datalab-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `py-datalab-0.1.0/bin/py_datalab.egg-info/PKG-INFO` & `py-datalab-0.1.1/datalab/py_datalab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-datalab
-Version: 0.1.0
+Version: 0.1.1
 Summary: This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 Home-page: https://github.com/matuszen/Python-DataLab
 Author: Mateusz Nowak
 Author-email: mateusz.nowak.pol@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py-datalab-0.1.0/setup.py` & `py-datalab-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from setuptools import setup, find_packages
 
 if sys.version_info < (3, 6):
     sys.exit("Sorry, Python < 3.6 is not supported")
 
 setup(
     name="py-datalab",
-    version="0.1.0",
+    version="0.1.1",
     author="Mateusz Nowak",
     author_email="mateusz.nowak.pol@gmail.com",
     description="This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.",
     url="https://github.com/matuszen/Python-DataLab",
-    packages=find_packages(where="bin"),
-    package_dir={"": "bin"},
+    packages=find_packages(where="datalab"),
+    package_dir={"": "datalab"},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

