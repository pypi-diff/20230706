# Comparing `tmp/visionner-0.0.6.tar.gz` & `tmp/visionner-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionner-0.0.6.tar", last modified: Thu Jul  6 16:01:37 2023, max compression
+gzip compressed data, was "visionner-0.0.7.tar", last modified: Thu Jul  6 16:39:34 2023, max compression
```

## Comparing `visionner-0.0.6.tar` & `visionner-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 16:01:37.265162 visionner-0.0.6/
--rw-rw-rw-   0        0        0      381 2023-07-06 16:01:37.264170 visionner-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1335 2023-07-06 15:56:16.000000 visionner-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 16:01:37.266145 visionner-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-07-06 16:00:54.000000 visionner-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:01:37.227142 visionner-0.0.6/visionner/
--rw-rw-rw-   0        0        0       28 2023-07-06 15:56:16.000000 visionner-0.0.6/visionner/__init__.py
--rw-rw-rw-   0        0        0     5717 2023-07-06 15:56:16.000000 visionner-0.0.6/visionner/core.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:01:37.262142 visionner-0.0.6/visionner.egg-info/
--rw-rw-rw-   0        0        0      381 2023-07-06 16:01:37.000000 visionner-0.0.6/visionner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-07-06 16:01:37.000000 visionner-0.0.6/visionner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 16:01:37.000000 visionner-0.0.6/visionner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-06 16:01:37.000000 visionner-0.0.6/visionner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-06 16:01:37.000000 visionner-0.0.6/visionner.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 16:39:34.384928 visionner-0.0.7/
+-rw-rw-rw-   0        0        0     1906 2023-07-06 16:39:34.383929 visionner-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1335 2023-07-06 15:56:16.000000 visionner-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 16:39:34.384928 visionner-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2023-07-06 16:39:15.000000 visionner-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:39:34.361939 visionner-0.0.7/visionner/
+-rw-rw-rw-   0        0        0       28 2023-07-06 15:56:16.000000 visionner-0.0.7/visionner/__init__.py
+-rw-rw-rw-   0        0        0     5717 2023-07-06 15:56:16.000000 visionner-0.0.7/visionner/core.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:39:34.382933 visionner-0.0.7/visionner.egg-info/
+-rw-rw-rw-   0        0        0     1906 2023-07-06 16:39:34.000000 visionner-0.0.7/visionner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-07-06 16:39:34.000000 visionner-0.0.7/visionner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 16:39:34.000000 visionner-0.0.7/visionner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-06 16:39:34.000000 visionner-0.0.7/visionner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-06 16:39:34.000000 visionner-0.0.7/visionner.egg-info/top_level.txt
```

### Comparing `visionner-0.0.6/README.md` & `visionner-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `visionner-0.0.6/setup.py` & `visionner-0.0.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6' 
-DESCRIPTION = 'manipulate your image dataset easly'
+VERSION = '0.0.7' 
+DESCRIPTION = "Turn raw image dataset into numpy array ; more suitable for deep learning tasks"
 
 setup(
         name="visionner", 
         version=VERSION,
         author="charles TCHANAKE",
-        author_email="<youremail@email.com>",
+        author_email="datadevfernolf@gmail.com",
+        url="https://github.com/charleslf2/visionner",
         description=DESCRIPTION,
-        #long_description=LONG_DESCRIPTION,
+        long_description_content_type="text/markdown",
+        long_description=open("README.md","r",encoding="utf-8").read(),
         packages=find_packages(),
         install_requires=["numpy","opencv-python",
                           "matplotlib","rich"],  
-        keywords=['python'],
+        keywords=["Computer-vision",
+        "preprocessing","Images","Dataset","visionner"],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Programming Language :: Python :: 3",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
         ]
 )
```

### Comparing `visionner-0.0.6/visionner/core.py` & `visionner-0.0.7/visionner/core.py`

 * *Files identical despite different names*

