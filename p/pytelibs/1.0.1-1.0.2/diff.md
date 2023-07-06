# Comparing `tmp/pytelibs-1.0.1.tar.gz` & `tmp/pytelibs-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytelibs-1.0.1.tar", last modified: Thu Jul  6 18:13:14 2023, max compression
+gzip compressed data, was "pytelibs-1.0.2.tar", last modified: Thu Jul  6 19:23:49 2023, max compression
```

## Comparing `pytelibs-1.0.1.tar` & `pytelibs-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:13:14.787966 pytelibs-1.0.1/
--rw-r--r--   0 root         (0) root         (0)    34523 2023-07-06 17:18:01.000000 pytelibs-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      466 2023-07-06 18:13:14.787966 pytelibs-1.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:13:14.747966 pytelibs-1.0.1/pytelibs/
--rw-r--r--   0 root         (0) root         (0)      337 2023-07-06 18:11:33.000000 pytelibs-1.0.1/pytelibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:13:14.787966 pytelibs-1.0.1/pytelibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      466 2023-07-06 18:13:14.000000 pytelibs-1.0.1/pytelibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      196 2023-07-06 18:13:14.000000 pytelibs-1.0.1/pytelibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 18:13:14.000000 pytelibs-1.0.1/pytelibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-06 18:13:14.000000 pytelibs-1.0.1/pytelibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-06 18:13:14.000000 pytelibs-1.0.1/pytelibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 18:13:14.797966 pytelibs-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      817 2023-07-06 18:08:03.000000 pytelibs-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:23:49.687965 pytelibs-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-07-06 17:18:01.000000 pytelibs-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      547 2023-07-06 19:23:49.687965 pytelibs-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-06 18:38:25.000000 pytelibs-1.0.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:23:49.647965 pytelibs-1.0.2/pytelibs/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-07-06 19:17:03.000000 pytelibs-1.0.2/pytelibs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      943 2023-07-06 18:54:53.000000 pytelibs-1.0.2/pytelibs/_journal.py
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-06 19:21:16.000000 pytelibs-1.0.2/pytelibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:23:49.677965 pytelibs-1.0.2/pytelibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      547 2023-07-06 19:23:49.000000 pytelibs-1.0.2/pytelibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      248 2023-07-06 19:23:49.000000 pytelibs-1.0.2/pytelibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 19:23:49.000000 pytelibs-1.0.2/pytelibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-06 19:23:49.000000 pytelibs-1.0.2/pytelibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-06 19:23:49.000000 pytelibs-1.0.2/pytelibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 19:23:49.687965 pytelibs-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      923 2023-07-06 19:23:14.000000 pytelibs-1.0.2/setup.py
```

### Comparing `pytelibs-1.0.1/LICENSE` & `pytelibs-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytelibs-1.0.1/setup.py` & `pytelibs-1.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from setuptools import setup, find_packages
-import codecs
+from pytelibs import __version__
 import os
+import re
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-with codecs.open(os.path.join(here, ".github/README.md"), encoding="utf-8") as fh:
-    long_description = "\\n" + fh.read()
+with open(os.path.join(here, "README.rst"), encoding="utf-8") as rd:
+    long_description = rd.read()
 
 setup(
     name="pytelibs",
-    version='1.0.1',
+    version=__version__,
     author="Unknown",
     author_email="unknownkz@outlook.co.id",
-    description="KASTA ID #PYTEL",
+    description="Client library for Pytel. @kastaid",
     url="https://github.com/kastaid/pytelibs",
+    license="AGPL",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['pyrogram'],
+    install_requires=['pyrogram', 'tgcrypto'],
     keywords=['pypi', 'pytelibs', 'python', 'pyrogram', 'telebot'],
     classifiers=[
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
     ]
 )
+
```

