# Comparing `tmp/psychopy-phidgets-0.2.1.tar.gz` & `tmp/psychopy-phidgets-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\psychopy-phidgets-0.2.1.tar", last modified: Wed Jul  5 21:03:16 2023, max compression
+gzip compressed data, was "dist\psychopy-phidgets-0.2.2.tar", last modified: Wed Jul  5 21:27:29 2023, max compression
```

## Comparing `psychopy-phidgets-0.2.1.tar` & `psychopy-phidgets-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 21:03:16.140901 psychopy-phidgets-0.2.1/
--rw-rw-rw-   0        0        0    35823 2023-01-07 04:09:42.000000 psychopy-phidgets-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      211 2023-01-07 05:12:31.000000 psychopy-phidgets-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      482 2023-07-05 21:03:16.140901 psychopy-phidgets-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      140 2023-01-07 04:23:08.000000 psychopy-phidgets-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 21:03:16.130927 psychopy-phidgets-0.2.1/psychopy_phidgets/
--rw-rw-rw-   0        0        0      101 2023-07-05 20:38:09.000000 psychopy-phidgets-0.2.1/psychopy_phidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 21:03:16.138906 psychopy-phidgets-0.2.1/psychopy_phidgets/component/
--rw-rw-rw-   0        0        0        0 2023-01-07 06:01:44.000000 psychopy-phidgets-0.2.1/psychopy_phidgets/component/__init__.py
--rw-rw-rw-   0        0        0     6423 2023-07-05 20:54:04.000000 psychopy-phidgets-0.2.1/psychopy_phidgets/component/phidgets.py
--rw-rw-rw-   0        0        0     2726 2023-01-07 21:32:46.000000 psychopy-phidgets-0.2.1/psychopy_phidgets/phidgets.py
-drwxrwxrwx   0        0        0        0 2023-07-05 21:03:16.137909 psychopy-phidgets-0.2.1/psychopy_phidgets.egg-info/
--rw-rw-rw-   0        0        0      482 2023-07-05 21:03:16.000000 psychopy-phidgets-0.2.1/psychopy_phidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-07-05 21:03:16.000000 psychopy-phidgets-0.2.1/psychopy_phidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 21:03:16.000000 psychopy-phidgets-0.2.1/psychopy_phidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      184 2023-07-05 21:03:16.000000 psychopy-phidgets-0.2.1/psychopy_phidgets.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-01-07 04:39:59.000000 psychopy-phidgets-0.2.1/psychopy_phidgets.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-05 21:03:16.000000 psychopy-phidgets-0.2.1/psychopy_phidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-05 21:03:16.000000 psychopy-phidgets-0.2.1/psychopy_phidgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 21:03:16.140901 psychopy-phidgets-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1178 2023-07-05 20:58:16.000000 psychopy-phidgets-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 21:27:21.266151 psychopy-phidgets-0.2.2/
+-rw-rw-rw-   0        0        0    35823 2023-01-07 04:09:42.000000 psychopy-phidgets-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      148 2023-07-05 21:27:20.000000 psychopy-phidgets-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      482 2023-07-05 21:27:29.597910 psychopy-phidgets-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      140 2023-01-07 04:23:08.000000 psychopy-phidgets-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 21:27:21.256178 psychopy-phidgets-0.2.2/psychopy_phidgets/
+-rw-rw-rw-   0        0        0      101 2023-07-05 20:38:09.000000 psychopy-phidgets-0.2.2/psychopy_phidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 21:27:21.261164 psychopy-phidgets-0.2.2/psychopy_phidgets/component/
+-rw-rw-rw-   0        0        0        0 2023-01-07 06:01:44.000000 psychopy-phidgets-0.2.2/psychopy_phidgets/component/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 21:27:21.263159 psychopy-phidgets-0.2.2/psychopy_phidgets/component/classic/
+-rw-rw-rw-   0        0        0     6096 2022-06-01 16:19:48.000000 psychopy-phidgets-0.2.2/psychopy_phidgets/component/classic/phidgets.png
+-rw-rw-rw-   0        0        0    14287 2022-06-01 16:19:54.000000 psychopy-phidgets-0.2.2/psychopy_phidgets/component/classic/phidgets@2x.png
+drwxrwxrwx   0        0        0        0 2023-07-05 21:27:21.264156 psychopy-phidgets-0.2.2/psychopy_phidgets/component/dark/
+-rw-rw-rw-   0        0        0     6096 2022-06-01 16:19:48.000000 psychopy-phidgets-0.2.2/psychopy_phidgets/component/dark/phidgets.png
+-rw-rw-rw-   0        0        0    14287 2022-06-01 16:19:54.000000 psychopy-phidgets-0.2.2/psychopy_phidgets/component/dark/phidgets@2x.png
+drwxrwxrwx   0        0        0        0 2023-07-05 21:27:21.265154 psychopy-phidgets-0.2.2/psychopy_phidgets/component/light/
+-rw-rw-rw-   0        0        0     6096 2022-06-01 16:19:48.000000 psychopy-phidgets-0.2.2/psychopy_phidgets/component/light/phidgets.png
+-rw-rw-rw-   0        0        0    14287 2022-06-01 16:19:54.000000 psychopy-phidgets-0.2.2/psychopy_phidgets/component/light/phidgets@2x.png
+-rw-rw-rw-   0        0        0     6423 2023-07-05 20:54:04.000000 psychopy-phidgets-0.2.2/psychopy_phidgets/component/phidgets.py
+-rw-rw-rw-   0        0        0     2726 2023-01-07 21:32:46.000000 psychopy-phidgets-0.2.2/psychopy_phidgets/phidgets.py
+drwxrwxrwx   0        0        0        0 2023-07-05 21:27:29.594917 psychopy-phidgets-0.2.2/psychopy_phidgets.egg-info/
+-rw-rw-rw-   0        0        0      482 2023-07-05 21:27:29.000000 psychopy-phidgets-0.2.2/psychopy_phidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      719 2023-07-05 21:27:29.000000 psychopy-phidgets-0.2.2/psychopy_phidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 21:27:29.000000 psychopy-phidgets-0.2.2/psychopy_phidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      184 2023-07-05 21:27:29.000000 psychopy-phidgets-0.2.2/psychopy_phidgets.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-05 21:27:21.000000 psychopy-phidgets-0.2.2/psychopy_phidgets.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-07-05 21:27:29.000000 psychopy-phidgets-0.2.2/psychopy_phidgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 21:27:29.597910 psychopy-phidgets-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-07-05 21:13:42.000000 psychopy-phidgets-0.2.2/setup.py
```

### Comparing `psychopy-phidgets-0.2.1/LICENSE` & `psychopy-phidgets-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `psychopy-phidgets-0.2.1/psychopy_phidgets/component/phidgets.py` & `psychopy-phidgets-0.2.2/psychopy_phidgets/component/phidgets.py`

 * *Files identical despite different names*

### Comparing `psychopy-phidgets-0.2.1/psychopy_phidgets/phidgets.py` & `psychopy-phidgets-0.2.2/psychopy_phidgets/phidgets.py`

 * *Files identical despite different names*

### Comparing `psychopy-phidgets-0.2.1/setup.py` & `psychopy-phidgets-0.2.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup
 setup(name='psychopy-phidgets',
-    version='0.2.1',
+    version='0.2.2',
     description='Psychopy plugin providing support for Phidgets',
     long_description='',
     url='https://github.com/maqadri/psychopy-phidgets',
     author='Muhammad A. J. Qadri',
     author_email='mqadri@holycross.edu',
     license='GPL3',
     classifiers=[
@@ -16,14 +16,13 @@
     ],
     keywords='psychopy phidgets',
     packages=['psychopy_phidgets',
               'psychopy_phidgets.component',
               'psychopy_phidgets.component.light',
               'psychopy_phidgets.component.dark',
               'psychopy_phidgets.component.classic'],
-    install_requires=['psychopy'],
     include_package_data=True,
     entry_points={
         'psychopy.hardware': ['PhidgetOutputComponent = psychopy_phidgets:PhidgetOutputComponent'],
         'psychopy.experiment.components': ['PhidgetRelayComponent = psychopy_phidgets:PhidgetRelayComponent']
     },
     zip_safe=False)
```

