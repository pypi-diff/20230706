# Comparing `tmp/pyappbundler-0.1.0.tar.gz` & `tmp/pyappbundler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyappbundler-0.1.0.tar", last modified: Thu Jul  6 08:01:59 2023, max compression
+gzip compressed data, was "pyappbundler-0.1.1.tar", last modified: Thu Jul  6 13:07:49 2023, max compression
```

## Comparing `pyappbundler-0.1.0.tar` & `pyappbundler-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 08:01:59.259277 pyappbundler-0.1.0/
--rw-rw-rw-   0        0        0     1074 2023-07-05 03:17:37.000000 pyappbundler-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      730 2023-07-06 08:01:59.258276 pyappbundler-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-05 14:55:05.000000 pyappbundler-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 08:01:59.254274 pyappbundler-0.1.0/pyappbundler/
--rw-rw-rw-   0        0        0       62 2023-07-06 07:59:09.000000 pyappbundler-0.1.0/pyappbundler/__init__.py
--rw-rw-rw-   0        0        0     2553 2023-07-06 07:59:09.000000 pyappbundler-0.1.0/pyappbundler/__main__.py
--rw-rw-rw-   0        0        0       22 2023-07-05 14:24:13.000000 pyappbundler-0.1.0/pyappbundler/_version.py
--rw-rw-rw-   0        0        0     3578 2023-07-05 16:17:12.000000 pyappbundler-0.1.0/pyappbundler/pyappbundler.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:01:59.257275 pyappbundler-0.1.0/pyappbundler/templates/
--rw-rw-rw-   0        0        0     1537 2023-07-05 15:18:33.000000 pyappbundler-0.1.0/pyappbundler/templates/iss.tmpl
-drwxrwxrwx   0        0        0        0 2023-07-06 08:01:59.257275 pyappbundler-0.1.0/pyappbundler.egg-info/
--rw-rw-rw-   0        0        0      730 2023-07-06 08:01:59.000000 pyappbundler-0.1.0/pyappbundler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-06 08:01:59.000000 pyappbundler-0.1.0/pyappbundler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 08:01:59.000000 pyappbundler-0.1.0/pyappbundler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-06 08:01:59.000000 pyappbundler-0.1.0/pyappbundler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-06 08:01:59.000000 pyappbundler-0.1.0/pyappbundler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      768 2023-07-06 07:59:09.000000 pyappbundler-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 08:01:59.259277 pyappbundler-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0       38 2023-07-05 16:21:35.000000 pyappbundler-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:07:49.282609 pyappbundler-0.1.1/
+-rw-rw-rw-   0        0        0     1074 2023-07-05 03:17:37.000000 pyappbundler-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      730 2023-07-06 13:07:49.281609 pyappbundler-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-05 14:55:05.000000 pyappbundler-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 13:07:49.277608 pyappbundler-0.1.1/pyappbundler/
+-rw-rw-rw-   0        0        0       79 2023-07-06 12:55:47.000000 pyappbundler-0.1.1/pyappbundler/__init__.py
+-rw-rw-rw-   0        0        0     2553 2023-07-06 07:59:09.000000 pyappbundler-0.1.1/pyappbundler/__main__.py
+-rw-rw-rw-   0        0        0       22 2023-07-06 12:57:54.000000 pyappbundler-0.1.1/pyappbundler/_version.py
+-rw-rw-rw-   0        0        0     3572 2023-07-06 12:57:31.000000 pyappbundler-0.1.1/pyappbundler/pyappbundler.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:07:49.281609 pyappbundler-0.1.1/pyappbundler/templates/
+-rw-rw-rw-   0        0        0     1537 2023-07-05 15:18:33.000000 pyappbundler-0.1.1/pyappbundler/templates/iss.tmpl
+drwxrwxrwx   0        0        0        0 2023-07-06 13:07:49.280608 pyappbundler-0.1.1/pyappbundler.egg-info/
+-rw-rw-rw-   0        0        0      730 2023-07-06 13:07:49.000000 pyappbundler-0.1.1/pyappbundler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-06 13:07:49.000000 pyappbundler-0.1.1/pyappbundler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 13:07:49.000000 pyappbundler-0.1.1/pyappbundler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-06 13:07:49.000000 pyappbundler-0.1.1/pyappbundler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-06 13:07:49.000000 pyappbundler-0.1.1/pyappbundler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      776 2023-07-06 12:57:21.000000 pyappbundler-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 13:07:49.282609 pyappbundler-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-07-05 16:21:35.000000 pyappbundler-0.1.1/setup.py
```

### Comparing `pyappbundler-0.1.0/LICENSE` & `pyappbundler-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyappbundler-0.1.0/PKG-INFO` & `pyappbundler-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappbundler
-Version: 0.1.0
+Version: 0.1.1
 Summary: automate bundle a Python application into a single package
 Author-email: inerject <kumbalup@gmail.com>
 Project-URL: Homepage, https://github.com/inerject/pyappbundler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `pyappbundler-0.1.0/pyappbundler/__main__.py` & `pyappbundler-0.1.1/pyappbundler/__main__.py`

 * *Files identical despite different names*

### Comparing `pyappbundler-0.1.0/pyappbundler/pyappbundler.py` & `pyappbundler-0.1.1/pyappbundler/pyappbundler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-__all__ = ('exe', 'exe_and_setup')
-
 from pathlib import Path
 import shutil
 import logging
 import subprocess
 
 import PyInstaller.__main__
 import jinja2
 
 
 def exe(
     target, *,
-    app_name, icon, dist, build,
+    app_name, icon, dist='dist', build='build',
     res_dirs: list = None, pyinst_flags: list = None,
     no_clean_dist=False,
 ):
     if not no_clean_dist:
         clean_dist(dist)
 
     build_exe(target, app_name, icon, dist, build, res_dirs, pyinst_flags)
 
 
 def exe_and_setup(
     target, *,
-    app_name, icon, app_guid, app_ver, dist, build,
+    app_name, icon, app_guid, app_ver, dist='dist', build='build',
     res_dirs: list = None, pyinst_flags: list = None,
     no_clean_dist=False,
 ):
     exe(target, app_name=app_name, icon=icon,
         dist=dist, build=build, res_dirs=res_dirs, pyinst_flags=pyinst_flags,
         no_clean_dist=no_clean_dist)
```

### Comparing `pyappbundler-0.1.0/pyappbundler/templates/iss.tmpl` & `pyappbundler-0.1.1/pyappbundler/templates/iss.tmpl`

 * *Files identical despite different names*

### Comparing `pyappbundler-0.1.0/pyappbundler.egg-info/PKG-INFO` & `pyappbundler-0.1.1/pyappbundler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappbundler
-Version: 0.1.0
+Version: 0.1.1
 Summary: automate bundle a Python application into a single package
 Author-email: inerject <kumbalup@gmail.com>
 Project-URL: Homepage, https://github.com/inerject/pyappbundler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `pyappbundler-0.1.0/pyproject.toml` & `pyappbundler-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["version"]
 dependencies = [
-    "pyinstaller>=5.13,<6",
-    "Jinja2>=3.1,<4",
+    "pyinstaller >=5.13, <6.0",
+    "Jinja2 >=3.1, <4.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/inerject/pyappbundler"
 
 [tool.setuptools.dynamic]
 version = {attr = "pyappbundler._version.__version__"}
```

