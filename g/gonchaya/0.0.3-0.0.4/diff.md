# Comparing `tmp/gonchaya-0.0.3.tar.gz` & `tmp/gonchaya-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gonchaya-0.0.3.tar", last modified: Thu Jul  6 10:57:28 2023, max compression
+gzip compressed data, was "gonchaya-0.0.4.tar", last modified: Thu Jul  6 18:26:23 2023, max compression
```

## Comparing `gonchaya-0.0.3.tar` & `gonchaya-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 padla     (1000) padla     (1000)        0 2023-07-06 10:57:28.943678 gonchaya-0.0.3/
--rw-rw-r--   0 padla     (1000) padla     (1000)      760 2023-07-06 10:57:28.943678 gonchaya-0.0.3/PKG-INFO
--rw-rw-r--   0 padla     (1000) padla     (1000)      166 2023-07-03 12:14:18.000000 gonchaya-0.0.3/README.md
-drwxrwxr-x   0 padla     (1000) padla     (1000)        0 2023-07-06 10:57:28.943678 gonchaya-0.0.3/gonchaya/
--rw-rw-r--   0 padla     (1000) padla     (1000)     1135 2023-07-06 05:44:50.000000 gonchaya-0.0.3/gonchaya/__init__.py
--rw-rw-r--   0 padla     (1000) padla     (1000)       14 2023-07-04 07:05:52.000000 gonchaya-0.0.3/gonchaya/__main__.py
--rw-rw-r--   0 padla     (1000) padla     (1000)     5685 2023-07-06 05:49:48.000000 gonchaya-0.0.3/gonchaya/not_implemented.py
-drwxrwxr-x   0 padla     (1000) padla     (1000)        0 2023-07-06 10:57:28.943678 gonchaya-0.0.3/gonchaya.egg-info/
--rw-rw-r--   0 padla     (1000) padla     (1000)      760 2023-07-06 10:57:28.000000 gonchaya-0.0.3/gonchaya.egg-info/PKG-INFO
--rw-rw-r--   0 padla     (1000) padla     (1000)      257 2023-07-06 10:57:28.000000 gonchaya-0.0.3/gonchaya.egg-info/SOURCES.txt
--rw-rw-r--   0 padla     (1000) padla     (1000)        1 2023-07-06 10:57:28.000000 gonchaya-0.0.3/gonchaya.egg-info/dependency_links.txt
--rw-rw-r--   0 padla     (1000) padla     (1000)       17 2023-07-06 10:57:28.000000 gonchaya-0.0.3/gonchaya.egg-info/requires.txt
--rw-rw-r--   0 padla     (1000) padla     (1000)        9 2023-07-06 10:57:28.000000 gonchaya-0.0.3/gonchaya.egg-info/top_level.txt
--rw-rw-r--   0 padla     (1000) padla     (1000)       38 2023-07-06 10:57:28.943678 gonchaya-0.0.3/setup.cfg
--rw-rw-r--   0 padla     (1000) padla     (1000)      770 2023-07-06 06:37:20.000000 gonchaya-0.0.3/setup.py
+drwxrwxr-x   0 padla     (1000) padla     (1000)        0 2023-07-06 18:26:23.127226 gonchaya-0.0.4/
+-rw-rw-r--   0 padla     (1000) padla     (1000)      746 2023-07-06 18:26:23.127226 gonchaya-0.0.4/PKG-INFO
+-rw-rw-r--   0 padla     (1000) padla     (1000)      166 2023-07-03 12:14:18.000000 gonchaya-0.0.4/README.md
+drwxrwxr-x   0 padla     (1000) padla     (1000)        0 2023-07-06 18:26:23.127226 gonchaya-0.0.4/gonchaya/
+-rw-rw-r--   0 padla     (1000) padla     (1000)     1134 2023-07-06 18:24:58.000000 gonchaya-0.0.4/gonchaya/__init__.py
+-rw-rw-r--   0 padla     (1000) padla     (1000)       14 2023-07-04 07:05:52.000000 gonchaya-0.0.4/gonchaya/__main__.py
+drwxrwxr-x   0 padla     (1000) padla     (1000)        0 2023-07-06 18:26:23.127226 gonchaya-0.0.4/gonchaya.egg-info/
+-rw-rw-r--   0 padla     (1000) padla     (1000)      746 2023-07-06 18:26:23.000000 gonchaya-0.0.4/gonchaya.egg-info/PKG-INFO
+-rw-rw-r--   0 padla     (1000) padla     (1000)      229 2023-07-06 18:26:23.000000 gonchaya-0.0.4/gonchaya.egg-info/SOURCES.txt
+-rw-rw-r--   0 padla     (1000) padla     (1000)        1 2023-07-06 18:26:23.000000 gonchaya-0.0.4/gonchaya.egg-info/dependency_links.txt
+-rw-rw-r--   0 padla     (1000) padla     (1000)       17 2023-07-06 18:26:23.000000 gonchaya-0.0.4/gonchaya.egg-info/requires.txt
+-rw-rw-r--   0 padla     (1000) padla     (1000)        9 2023-07-06 18:26:23.000000 gonchaya-0.0.4/gonchaya.egg-info/top_level.txt
+-rw-rw-r--   0 padla     (1000) padla     (1000)       38 2023-07-06 18:26:23.127226 gonchaya-0.0.4/setup.cfg
+-rw-rw-r--   0 padla     (1000) padla     (1000)      756 2023-07-06 18:22:24.000000 gonchaya-0.0.4/setup.py
```

### Comparing `gonchaya-0.0.3/PKG-INFO` & `gonchaya-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gonchaya
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data Science tools
 Home-page: https://github.com/Alexander-Firsov/gonchaya
 Author: Alexander Firsov aka gonchaya aka padla
 Author-email: gonchaya@gifara.ru
-License: BSD License (BSD-3-Clause)
+License: BSD-3-Clause
 Description: # gonchaya
         a set of additional tools for the Data Science course  
         набор дополнительных инструментов для курса Data Science  
         
         
 Keywords: example python
 Platform: UNKNOWN
```

### Comparing `gonchaya-0.0.3/gonchaya/__init__.py` & `gonchaya-0.0.4/gonchaya/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,8 +23,7 @@
     import time
     import math  # математические операции типа логарифмов
     import re  # работа с регулярными выражениями
     import matplotlib.pyplot as plt  # базовая работа с графиками
     import pandas as pd  # работа с датафреймами
     from IPython.display import display, Markdown  # Для вывода форматированного текста в jupyter notebooks
     import seaborn as sns
-
```

### Comparing `gonchaya-0.0.3/gonchaya.egg-info/PKG-INFO` & `gonchaya-0.0.4/gonchaya.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gonchaya
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data Science tools
 Home-page: https://github.com/Alexander-Firsov/gonchaya
 Author: Alexander Firsov aka gonchaya aka padla
 Author-email: gonchaya@gifara.ru
-License: BSD License (BSD-3-Clause)
+License: BSD-3-Clause
 Description: # gonchaya
         a set of additional tools for the Data Science course  
         набор дополнительных инструментов для курса Data Science  
         
         
 Keywords: example python
 Platform: UNKNOWN
```

### Comparing `gonchaya-0.0.3/setup.py` & `gonchaya-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='gonchaya',
-  version='0.0.3',
+  version='0.0.4',
   author='Alexander Firsov aka gonchaya aka padla',
   author_email='gonchaya@gifara.ru',
   url='https://github.com/Alexander-Firsov/gonchaya',
-  license='BSD License (BSD-3-Clause)',
+  license='BSD-3-Clause',
   description='Data Science tools',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=['gonchaya'],
   install_requires=['requests>=2.25.1'],
   classifiers=[
     'Programming Language :: Python :: 3.11',
```

