# Comparing `tmp/fauxioapi-0.1.5.tar.gz` & `tmp/fauxioapi-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fauxioapi-0.1.5.tar", last modified: Mon Dec 20 14:39:36 2021, max compression
+gzip compressed data, was "dist/fauxioapi-0.1.6.tar", last modified: Thu Jul  6 13:15:59 2023, max compression
```

## Comparing `fauxioapi-0.1.5.tar` & `fauxioapi-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxrwsr-x   0 jbeidler  (1855) emis-hpc (54388)        0 2021-12-20 14:39:36.000000 fauxioapi-0.1.5/
--rw-rw-r--   0 jbeidler  (1855) emis-hpc (54388)      659 2021-12-20 14:39:28.000000 fauxioapi-0.1.5/setup.py
-drwxrwsr-x   0 jbeidler  (1855) emis-hpc (54388)        0 2021-12-20 14:39:36.000000 fauxioapi-0.1.5/fauxioapi.egg-info/
--rw-rw-r--   0 jbeidler  (1855) emis-hpc (54388)      227 2021-12-20 14:39:36.000000 fauxioapi-0.1.5/fauxioapi.egg-info/SOURCES.txt
--rw-rw-r--   0 jbeidler  (1855) emis-hpc (54388)     2501 2021-12-20 14:39:36.000000 fauxioapi-0.1.5/fauxioapi.egg-info/PKG-INFO
--rw-rw-r--   0 jbeidler  (1855) emis-hpc (54388)        1 2021-12-20 14:39:36.000000 fauxioapi-0.1.5/fauxioapi.egg-info/dependency_links.txt
--rw-rw-r--   0 jbeidler  (1855) emis-hpc (54388)       10 2021-12-20 14:39:36.000000 fauxioapi-0.1.5/fauxioapi.egg-info/top_level.txt
--rw-rw-r--   0 jbeidler  (1855) emis-hpc (54388)       27 2021-12-20 14:39:36.000000 fauxioapi-0.1.5/fauxioapi.egg-info/requires.txt
--rw-rw-r--   0 jbeidler  (1855) emis-hpc (54388)     2501 2021-12-20 14:39:36.000000 fauxioapi-0.1.5/PKG-INFO
-drwxrwsr-x   0 jbeidler  (1855) emis-hpc (54388)        0 2021-12-20 14:39:36.000000 fauxioapi-0.1.5/fauxioapi/
--rw-rw-r--   0 jbeidler  (1855) emis-hpc (54388)       83 2021-12-16 14:51:55.000000 fauxioapi-0.1.5/fauxioapi/__init__.py
--rw-rw-r--   0 jbeidler  (1855) emis-hpc (54388)     9477 2021-12-18 18:26:46.000000 fauxioapi-0.1.5/fauxioapi/fauxioapi.py
--rw-rw-r--   0 jbeidler  (1855) emis-hpc (54388)       38 2021-12-20 14:39:36.000000 fauxioapi-0.1.5/setup.cfg
--rw-rw-r--   0 jbeidler  (1855) emis-hpc (54388)     1897 2021-12-18 18:35:41.000000 fauxioapi-0.1.5/README.md
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-07-06 13:15:59.000000 fauxioapi-0.1.6/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      849 2023-07-06 13:15:42.000000 fauxioapi-0.1.6/setup.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2501 2023-07-06 13:15:59.000000 fauxioapi-0.1.6/PKG-INFO
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)       38 2023-07-06 13:15:59.000000 fauxioapi-0.1.6/setup.cfg
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     1897 2021-12-18 18:35:41.000000 fauxioapi-0.1.6/README.md
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-07-06 13:15:59.000000 fauxioapi-0.1.6/scripts/
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     1842 2021-12-20 14:35:35.000000 fauxioapi-0.1.6/scripts/gen_grid_shape.py
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     8484 2021-12-20 14:37:31.000000 fauxioapi-0.1.6/scripts/regrid.py
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-07-06 13:15:59.000000 fauxioapi-0.1.6/src/
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-07-06 13:15:59.000000 fauxioapi-0.1.6/src/fauxioapi.egg-info/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      331 2023-07-06 13:15:57.000000 fauxioapi-0.1.6/src/fauxioapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2501 2023-07-06 13:15:57.000000 fauxioapi-0.1.6/src/fauxioapi.egg-info/PKG-INFO
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)        1 2023-07-06 13:15:57.000000 fauxioapi-0.1.6/src/fauxioapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)       10 2023-07-06 13:15:57.000000 fauxioapi-0.1.6/src/fauxioapi.egg-info/top_level.txt
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)       44 2023-07-06 13:15:57.000000 fauxioapi-0.1.6/src/fauxioapi.egg-info/requires.txt
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-07-06 13:15:59.000000 fauxioapi-0.1.6/src/fauxioapi/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)       83 2021-12-16 14:51:55.000000 fauxioapi-0.1.6/src/fauxioapi/__init__.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     9477 2021-12-18 18:26:46.000000 fauxioapi-0.1.6/src/fauxioapi/fauxioapi.py
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-07-06 13:15:59.000000 fauxioapi-0.1.6/src/fauxioapi/data/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      542 2021-12-20 14:34:45.000000 fauxioapi-0.1.6/src/fauxioapi/data/griddesc.txt
```

### Comparing `fauxioapi-0.1.5/setup.py` & `fauxioapi-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from setuptools import setup, find_packages, Extension
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
     name="fauxioapi",
-    version="0.1.5",
-    packages = find_packages(),
+    version="0.1.6",
+    packages=find_packages(where='src'),
+    package_dir={'': 'src'},
     python_requires='>=3.5',
-    setup_requires=['numpy>=1.16','netCDF4>=1.2.9'],
-    install_requires=['numpy>=1.16','netCDF4>=1.2.9'],
+    setup_requires=['numpy>=1.16,<=1.24.3','netCDF4>=1.2.9,<=1.5.8'],
+    install_requires=['numpy>=1.16,<=1.24.3','netCDF4>=1.2.9,<=1.5.8'],
+    scripts=['scripts/gen_grid_shape.py','scripts/regrid.py'],
+    package_data={'fauxioapi': ['data/griddesc.txt']},
     url="https://github.com/jlbeidler/fauxioapi",
     author_email='james.beidler@gmail.com',
     description="A simple module reproducing limited I/O API functions",
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

### Comparing `fauxioapi-0.1.5/fauxioapi.egg-info/PKG-INFO` & `fauxioapi-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fauxioapi
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple module reproducing limited I/O API functions
 Home-page: https://github.com/jlbeidler/fauxioapi
 Author-email: james.beidler@gmail.com
 License: UNKNOWN
 Description: # fauxioapi 
         A simple approximation of a limited set of functions from the I/O API targeted at gridded atmospheric emissions QA in a netCDF container such as those created by SMOKE for CMAQ
```

### Comparing `fauxioapi-0.1.5/PKG-INFO` & `fauxioapi-0.1.6/src/fauxioapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fauxioapi
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple module reproducing limited I/O API functions
 Home-page: https://github.com/jlbeidler/fauxioapi
 Author-email: james.beidler@gmail.com
 License: UNKNOWN
 Description: # fauxioapi 
         A simple approximation of a limited set of functions from the I/O API targeted at gridded atmospheric emissions QA in a netCDF container such as those created by SMOKE for CMAQ
```

### Comparing `fauxioapi-0.1.5/fauxioapi/fauxioapi.py` & `fauxioapi-0.1.6/src/fauxioapi/fauxioapi.py`

 * *Files identical despite different names*

### Comparing `fauxioapi-0.1.5/README.md` & `fauxioapi-0.1.6/README.md`

 * *Files identical despite different names*

