# Comparing `tmp/magic-scissors-0.0.1.tar.gz` & `tmp/magic-scissors-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magic-scissors-0.0.1.tar", last modified: Thu Jun 29 14:02:34 2023, max compression
+gzip compressed data, was "magic-scissors-0.1.0.tar", last modified: Thu Jul  6 18:10:18 2023, max compression
```

## Comparing `magic-scissors-0.0.1.tar` & `magic-scissors-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 14:02:34.845028 magic-scissors-0.0.1/
--rw-r--r--   0 james      (501) staff       (20)      357 2023-06-29 14:02:34.844899 magic-scissors-0.0.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)       17 2023-06-29 14:02:23.000000 magic-scissors-0.0.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 14:02:34.843750 magic-scissors-0.0.1/magic_scissors/
--rw-r--r--   0 james      (501) staff       (20)       22 2023-06-29 14:01:11.000000 magic-scissors-0.0.1/magic_scissors/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 14:02:34.844720 magic-scissors-0.0.1/magic_scissors.egg-info/
--rw-r--r--   0 james      (501) staff       (20)      357 2023-06-29 14:02:34.000000 magic-scissors-0.0.1/magic_scissors.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      234 2023-06-29 14:02:34.000000 magic-scissors-0.0.1/magic_scissors.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-29 14:02:34.000000 magic-scissors-0.0.1/magic_scissors.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       53 2023-06-29 14:02:34.000000 magic-scissors-0.0.1/magic_scissors.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       15 2023-06-29 14:02:34.000000 magic-scissors-0.0.1/magic_scissors.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-29 14:02:34.845068 magic-scissors-0.0.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)      973 2023-06-29 14:01:11.000000 magic-scissors-0.0.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-06 18:10:18.681136 magic-scissors-0.1.0/
+-rw-r--r--   0 james      (501) staff       (20)     2755 2023-07-06 18:10:18.680995 magic-scissors-0.1.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     2252 2023-07-06 18:09:34.000000 magic-scissors-0.1.0/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-06 18:10:18.679897 magic-scissors-0.1.0/magic_scissors/
+-rw-r--r--   0 james      (501) staff       (20)       94 2023-07-06 18:09:34.000000 magic-scissors-0.1.0/magic_scissors/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     4259 2023-07-06 18:09:34.000000 magic-scissors-0.1.0/magic_scissors/generate_image.py
+-rw-r--r--   0 james      (501) staff       (20)    16567 2023-07-06 18:09:34.000000 magic-scissors-0.1.0/magic_scissors/magic_scissors.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-06 18:10:18.680792 magic-scissors-0.1.0/magic_scissors.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2755 2023-07-06 18:10:18.000000 magic-scissors-0.1.0/magic_scissors.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      300 2023-07-06 18:10:18.000000 magic-scissors-0.1.0/magic_scissors.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-07-06 18:10:18.000000 magic-scissors-0.1.0/magic_scissors.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       70 2023-07-06 18:10:18.000000 magic-scissors-0.1.0/magic_scissors.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       15 2023-07-06 18:10:18.000000 magic-scissors-0.1.0/magic_scissors.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-07-06 18:10:18.681186 magic-scissors-0.1.0/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1164 2023-07-06 18:10:04.000000 magic-scissors-0.1.0/setup.py
```

### Comparing `magic-scissors-0.0.1/setup.py` & `magic-scissors-0.1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import setuptools
 from setuptools import find_packages
 import re
 
 with open("./magic_scissors/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
@@ -12,23 +11,26 @@
     long_description = fh.read()
 
 setuptools.setup(
     name="magic-scissors",
     version=version,
     author="Roboflow",
     author_email="support@roboflow.com",
-    description="",
+    description="Generate synthetic data for computer vision projects using copy-paste context-augmentation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=[],
+    url="https://github.com/roboflow/magic-scissors-python",
+    install_requires=[
+        "roboflow",
+        "shapely",
+    ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
 )
-
```

