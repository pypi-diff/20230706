# Comparing `tmp/gaussFilter-1.0.0.tar.gz` & `tmp/gaussFilter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaussFilter-1.0.0.tar", last modified: Thu Jul  6 18:28:59 2023, max compression
+gzip compressed data, was "gaussFilter-1.0.1.tar", last modified: Thu Jul  6 19:03:46 2023, max compression
```

## Comparing `gaussFilter-1.0.0.tar` & `gaussFilter-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 divagar    (501) staff       (20)        0 2023-07-06 18:28:59.883691 gaussFilter-1.0.0/
--rw-r--r--   0 divagar    (501) staff       (20)     1065 2023-07-06 18:06:32.000000 gaussFilter-1.0.0/LICENSE
--rw-r--r--   0 divagar    (501) staff       (20)     1264 2023-07-06 18:28:59.883750 gaussFilter-1.0.0/PKG-INFO
--rw-r--r--   0 divagar    (501) staff       (20)      966 2023-07-06 18:26:31.000000 gaussFilter-1.0.0/README.md
-drwxr-xr-x   0 divagar    (501) staff       (20)        0 2023-07-06 18:28:59.883591 gaussFilter-1.0.0/gaussFilter.egg-info/
--rw-r--r--   0 divagar    (501) staff       (20)     1264 2023-07-06 18:28:59.000000 gaussFilter-1.0.0/gaussFilter.egg-info/PKG-INFO
--rw-r--r--   0 divagar    (501) staff       (20)      216 2023-07-06 18:28:59.000000 gaussFilter-1.0.0/gaussFilter.egg-info/SOURCES.txt
--rw-r--r--   0 divagar    (501) staff       (20)        1 2023-07-06 18:28:59.000000 gaussFilter-1.0.0/gaussFilter.egg-info/dependency_links.txt
--rw-r--r--   0 divagar    (501) staff       (20)       20 2023-07-06 18:28:59.000000 gaussFilter-1.0.0/gaussFilter.egg-info/requires.txt
--rw-r--r--   0 divagar    (501) staff       (20)        1 2023-07-06 18:28:59.000000 gaussFilter-1.0.0/gaussFilter.egg-info/top_level.txt
--rw-r--r--   0 divagar    (501) staff       (20)      207 2023-07-06 18:27:24.000000 gaussFilter-1.0.0/pyproject.toml
--rw-r--r--   0 divagar    (501) staff       (20)      461 2023-07-06 18:28:59.883988 gaussFilter-1.0.0/setup.cfg
+drwxr-xr-x   0 divagar    (501) staff       (20)        0 2023-07-06 19:03:46.722786 gaussFilter-1.0.1/
+-rw-r--r--   0 divagar    (501) staff       (20)     1065 2023-07-06 18:06:32.000000 gaussFilter-1.0.1/LICENSE
+-rw-r--r--   0 divagar    (501) staff       (20)     1260 2023-07-06 19:03:46.722880 gaussFilter-1.0.1/PKG-INFO
+-rw-r--r--   0 divagar    (501) staff       (20)      962 2023-07-06 18:57:20.000000 gaussFilter-1.0.1/README.md
+drwxr-xr-x   0 divagar    (501) staff       (20)        0 2023-07-06 19:03:46.721642 gaussFilter-1.0.1/gaussFilter/
+-rw-r--r--   0 divagar    (501) staff       (20)      118 2023-07-06 18:07:26.000000 gaussFilter-1.0.1/gaussFilter/__init__.py
+-rw-r--r--   0 divagar    (501) staff       (20)     1531 2023-07-06 18:01:46.000000 gaussFilter-1.0.1/gaussFilter/gaussFilter.py
+drwxr-xr-x   0 divagar    (501) staff       (20)        0 2023-07-06 19:03:46.722638 gaussFilter-1.0.1/gaussFilter.egg-info/
+-rw-r--r--   0 divagar    (501) staff       (20)     1260 2023-07-06 19:03:46.000000 gaussFilter-1.0.1/gaussFilter.egg-info/PKG-INFO
+-rw-r--r--   0 divagar    (501) staff       (20)      267 2023-07-06 19:03:46.000000 gaussFilter-1.0.1/gaussFilter.egg-info/SOURCES.txt
+-rw-r--r--   0 divagar    (501) staff       (20)        1 2023-07-06 19:03:46.000000 gaussFilter-1.0.1/gaussFilter.egg-info/dependency_links.txt
+-rw-r--r--   0 divagar    (501) staff       (20)       20 2023-07-06 19:03:46.000000 gaussFilter-1.0.1/gaussFilter.egg-info/requires.txt
+-rw-r--r--   0 divagar    (501) staff       (20)       12 2023-07-06 19:03:46.000000 gaussFilter-1.0.1/gaussFilter.egg-info/top_level.txt
+-rw-r--r--   0 divagar    (501) staff       (20)      207 2023-07-06 18:27:24.000000 gaussFilter-1.0.1/pyproject.toml
+-rw-r--r--   0 divagar    (501) staff       (20)      461 2023-07-06 19:03:46.723237 gaussFilter-1.0.1/setup.cfg
```

### Comparing `gaussFilter-1.0.0/LICENSE` & `gaussFilter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gaussFilter-1.0.0/PKG-INFO` & `gaussFilter-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaussFilter
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for applying Gaussian filter to images
 Home-page: https://github.com/divagarn/gaussFilter.git
 Author: Divagar N
 Author-email: divagar2kn@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,15 +22,15 @@
 ```
 
 
 ## Usage
 
 ```python
 import cv2
-from src.gaussFilter import apply_gaussian_filter
+from gaussFilter import apply_gaussian_filter
 
 # Load an image
 image = cv2.imread('path/to/your/image.jpg')
 
 # Apply the Gaussian filter with desired sigma and kernel size
 filtered_image = apply_gaussian_filter(image, sigma=1.5, kernel_size=5)
```

### Comparing `gaussFilter-1.0.0/README.md` & `gaussFilter-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ```
 
 
 ## Usage
 
 ```python
 import cv2
-from src.gaussFilter import apply_gaussian_filter
+from gaussFilter import apply_gaussian_filter
 
 # Load an image
 image = cv2.imread('path/to/your/image.jpg')
 
 # Apply the Gaussian filter with desired sigma and kernel size
 filtered_image = apply_gaussian_filter(image, sigma=1.5, kernel_size=5)
```

### Comparing `gaussFilter-1.0.0/gaussFilter.egg-info/PKG-INFO` & `gaussFilter-1.0.1/gaussFilter.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaussFilter
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for applying Gaussian filter to images
 Home-page: https://github.com/divagarn/gaussFilter.git
 Author: Divagar N
 Author-email: divagar2kn@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,15 +22,15 @@
 ```
 
 
 ## Usage
 
 ```python
 import cv2
-from src.gaussFilter import apply_gaussian_filter
+from gaussFilter import apply_gaussian_filter
 
 # Load an image
 image = cv2.imread('path/to/your/image.jpg')
 
 # Apply the Gaussian filter with desired sigma and kernel size
 filtered_image = apply_gaussian_filter(image, sigma=1.5, kernel_size=5)
```

