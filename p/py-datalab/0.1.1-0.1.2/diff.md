# Comparing `tmp/py-datalab-0.1.1.tar.gz` & `tmp/py-datalab-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-datalab-0.1.1.tar", last modified: Thu Jul  6 10:45:56 2023, max compression
+gzip compressed data, was "py-datalab-0.1.2.tar", last modified: Thu Jul  6 10:58:49 2023, max compression
```

## Comparing `py-datalab-0.1.1.tar` & `py-datalab-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 10:45:56.201971 py-datalab-0.1.1/
--rw-rw-rw-   0        0        0     1085 2023-06-20 10:54:28.000000 py-datalab-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1018 2023-07-06 10:45:56.200464 py-datalab-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2437 2023-07-03 12:36:33.000000 py-datalab-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 10:45:56.177962 py-datalab-0.1.1/datalab/
-drwxrwxrwx   0        0        0        0 2023-07-06 10:45:56.198458 py-datalab-0.1.1/datalab/py_datalab.egg-info/
--rw-rw-rw-   0        0        0     1018 2023-07-06 10:45:56.000000 py-datalab-0.1.1/datalab/py_datalab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-07-06 10:45:56.000000 py-datalab-0.1.1/datalab/py_datalab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 10:45:56.000000 py-datalab-0.1.1/datalab/py_datalab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 10:45:56.000000 py-datalab-0.1.1/datalab/py_datalab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 10:45:56.201971 py-datalab-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1256 2023-07-06 10:45:49.000000 py-datalab-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:58:49.860866 py-datalab-0.1.2/
+-rw-rw-rw-   0        0        0     1085 2023-06-20 10:54:28.000000 py-datalab-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1006 2023-07-06 10:58:49.859866 py-datalab-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2437 2023-07-03 12:36:33.000000 py-datalab-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 10:58:49.838832 py-datalab-0.1.2/datalab/
+-rw-rw-rw-   0        0        0    10352 2023-07-06 09:19:28.000000 py-datalab-0.1.2/datalab/Matrix.py
+-rw-rw-rw-   0        0        0     7059 2023-07-06 09:20:41.000000 py-datalab-0.1.2/datalab/Vector.py
+-rw-rw-rw-   0        0        0       58 2023-07-06 10:44:09.000000 py-datalab-0.1.2/datalab/__init__.py
+-rw-rw-rw-   0        0        0     4228 2023-07-06 08:04:25.000000 py-datalab-0.1.2/datalab/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:58:49.858866 py-datalab-0.1.2/py_datalab.egg-info/
+-rw-rw-rw-   0        0        0     1006 2023-07-06 10:58:49.000000 py-datalab-0.1.2/py_datalab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-06 10:58:49.000000 py-datalab-0.1.2/py_datalab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 10:58:49.000000 py-datalab-0.1.2/py_datalab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-06 10:58:49.000000 py-datalab-0.1.2/py_datalab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 10:58:49.861865 py-datalab-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1195 2023-07-06 10:58:47.000000 py-datalab-0.1.2/setup.py
```

### Comparing `py-datalab-0.1.1/LICENSE` & `py-datalab-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-datalab-0.1.1/PKG-INFO` & `py-datalab-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: py-datalab
-Version: 0.1.1
+Version: 0.1.2
 Summary: This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 Home-page: https://github.com/matuszen/Python-DataLab
 Author: Mateusz Nowak
 Author-email: mateusz.nowak.pol@gmail.com
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `py-datalab-0.1.1/README.md` & `py-datalab-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `py-datalab-0.1.1/datalab/py_datalab.egg-info/PKG-INFO` & `py-datalab-0.1.2/py_datalab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: py-datalab
-Version: 0.1.1
+Version: 0.1.2
 Summary: This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 Home-page: https://github.com/matuszen/Python-DataLab
 Author: Mateusz Nowak
 Author-email: mateusz.nowak.pol@gmail.com
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `py-datalab-0.1.1/setup.py` & `py-datalab-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 from setuptools import setup, find_packages
 
 if sys.version_info < (3, 6):
     sys.exit("Sorry, Python < 3.6 is not supported")
 
 setup(
     name="py-datalab",
-    version="0.1.1",
+    version="0.1.2",
     author="Mateusz Nowak",
     author_email="mateusz.nowak.pol@gmail.com",
     description="This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.",
     url="https://github.com/matuszen/Python-DataLab",
-    packages=find_packages(where="datalab"),
-    package_dir={"": "datalab"},
+    packages=find_packages(),
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

