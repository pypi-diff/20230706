# Comparing `tmp/py-datalab-0.1.6.tar.gz` & `tmp/py-datalab-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-datalab-0.1.6.tar", last modified: Thu Jul  6 12:05:45 2023, max compression
+gzip compressed data, was "py-datalab-0.1.7.tar", last modified: Thu Jul  6 12:08:38 2023, max compression
```

## Comparing `py-datalab-0.1.6.tar` & `py-datalab-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 12:05:45.245122 py-datalab-0.1.6/
--rw-rw-rw-   0        0        0     1085 2023-06-20 10:54:28.000000 py-datalab-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     1006 2023-07-06 12:05:45.244122 py-datalab-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2437 2023-07-03 12:36:33.000000 py-datalab-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 12:05:45.227863 py-datalab-0.1.6/datalab/
--rw-rw-rw-   0        0        0    10352 2023-07-06 09:19:28.000000 py-datalab-0.1.6/datalab/Matrix.py
--rw-rw-rw-   0        0        0     7059 2023-07-06 09:20:41.000000 py-datalab-0.1.6/datalab/Vector.py
--rw-rw-rw-   0        0        0       68 2023-07-06 12:05:30.000000 py-datalab-0.1.6/datalab/__init__.py
--rw-rw-rw-   0        0        0     4231 2023-07-06 12:02:49.000000 py-datalab-0.1.6/datalab/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:05:45.242122 py-datalab-0.1.6/py_datalab.egg-info/
--rw-rw-rw-   0        0        0     1006 2023-07-06 12:05:45.000000 py-datalab-0.1.6/py_datalab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-06 12:05:45.000000 py-datalab-0.1.6/py_datalab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 12:05:45.000000 py-datalab-0.1.6/py_datalab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-06 12:05:45.000000 py-datalab-0.1.6/py_datalab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 12:05:45.245122 py-datalab-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1195 2023-07-06 12:05:43.000000 py-datalab-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:08:38.218553 py-datalab-0.1.7/
+-rw-rw-rw-   0        0        0     1085 2023-06-20 10:54:28.000000 py-datalab-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     1006 2023-07-06 12:08:38.217449 py-datalab-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2437 2023-07-03 12:36:33.000000 py-datalab-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 12:08:38.203936 py-datalab-0.1.7/datalab/
+-rw-rw-rw-   0        0        0    10353 2023-07-06 12:08:16.000000 py-datalab-0.1.7/datalab/Matrix.py
+-rw-rw-rw-   0        0        0     7060 2023-07-06 12:08:19.000000 py-datalab-0.1.7/datalab/Vector.py
+-rw-rw-rw-   0        0        0       56 2023-07-06 12:08:09.000000 py-datalab-0.1.7/datalab/__init__.py
+-rw-rw-rw-   0        0        0     4231 2023-07-06 12:02:49.000000 py-datalab-0.1.7/datalab/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:08:38.216449 py-datalab-0.1.7/py_datalab.egg-info/
+-rw-rw-rw-   0        0        0     1006 2023-07-06 12:08:38.000000 py-datalab-0.1.7/py_datalab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-06 12:08:38.000000 py-datalab-0.1.7/py_datalab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 12:08:38.000000 py-datalab-0.1.7/py_datalab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-06 12:08:38.000000 py-datalab-0.1.7/py_datalab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 12:08:38.218553 py-datalab-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1195 2023-07-06 12:08:29.000000 py-datalab-0.1.7/setup.py
```

### Comparing `py-datalab-0.1.6/LICENSE` & `py-datalab-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py-datalab-0.1.6/PKG-INFO` & `py-datalab-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-datalab
-Version: 0.1.6
+Version: 0.1.7
 Summary: This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 Home-page: https://github.com/matuszen/Python-DataLab
 Author: Mateusz Nowak
 Author-email: mateusz.nowak.pol@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py-datalab-0.1.6/README.md` & `py-datalab-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `py-datalab-0.1.6/datalab/Matrix.py` & `py-datalab-0.1.7/datalab/Matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utils import *
+from .utils import *
 
 
 class Matrix:
     @overload
     def __init__(self, object: Iterable) -> None:
         pass
```

### Comparing `py-datalab-0.1.6/datalab/Vector.py` & `py-datalab-0.1.7/datalab/Vector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utils import *
+from .utils import *
 
 
 class Vector:
     @overload
     def __init__(self, object: Iterable) -> None:
         pass
```

### Comparing `py-datalab-0.1.6/datalab/utils.py` & `py-datalab-0.1.7/datalab/utils.py`

 * *Files identical despite different names*

### Comparing `py-datalab-0.1.6/py_datalab.egg-info/PKG-INFO` & `py-datalab-0.1.7/py_datalab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-datalab
-Version: 0.1.6
+Version: 0.1.7
 Summary: This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 Home-page: https://github.com/matuszen/Python-DataLab
 Author: Mateusz Nowak
 Author-email: mateusz.nowak.pol@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py-datalab-0.1.6/setup.py` & `py-datalab-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 if sys.version_info < (3, 6):
     sys.exit("Sorry, Python < 3.6 is not supported")
 
 setup(
     name="py-datalab",
-    version="0.1.6",
+    version="0.1.7",
     author="Mateusz Nowak",
     author_email="mateusz.nowak.pol@gmail.com",
     description="This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.",
     url="https://github.com/matuszen/Python-DataLab",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
```

