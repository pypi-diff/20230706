# Comparing `tmp/h5coro-0.0.4.tar.gz` & `tmp/h5coro-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5coro-0.0.4.tar", last modified: Fri Jun 30 18:17:09 2023, max compression
+gzip compressed data, was "h5coro-0.0.5.tar", last modified: Thu Jul  6 14:03:10 2023, max compression
```

## Comparing `h5coro-0.0.4.tar` & `h5coro-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-06-30 18:17:09.790831 h5coro-0.0.4/
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     3078 2023-06-27 11:55:04.000000 h5coro-0.0.4/.gitignore
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     1511 2023-06-27 11:55:04.000000 h5coro-0.0.4/LICENSE
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      150 2023-06-27 11:55:04.000000 h5coro-0.0.4/MANIFEST.in
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      572 2023-06-30 18:17:09.790831 h5coro-0.0.4/PKG-INFO
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       55 2023-06-27 11:55:04.000000 h5coro-0.0.4/README.md
-drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-06-30 18:17:09.786831 h5coro-0.0.4/data/
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      338 2023-06-27 19:37:14.000000 h5coro-0.0.4/data/grandmesa.geojson
-drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-06-30 18:17:09.786831 h5coro-0.0.4/h5coro/
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      194 2023-06-27 11:55:04.000000 h5coro-0.0.4/h5coro/__init__.py
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      229 2023-06-27 13:23:23.000000 h5coro-0.0.4/h5coro/filedriver.py
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)    93760 2023-06-29 19:02:55.000000 h5coro-0.0.4/h5coro/h5coro.py
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     1941 2023-06-27 19:47:55.000000 h5coro-0.0.4/h5coro/s3driver.py
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      319 2023-06-27 11:55:04.000000 h5coro-0.0.4/h5coro/version.py
-drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-06-30 18:17:09.790831 h5coro-0.0.4/h5coro.egg-info/
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      572 2023-06-30 18:17:09.000000 h5coro-0.0.4/h5coro.egg-info/PKG-INFO
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      437 2023-06-30 18:17:09.000000 h5coro-0.0.4/h5coro.egg-info/SOURCES.txt
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)        1 2023-06-30 18:17:09.000000 h5coro-0.0.4/h5coro.egg-info/dependency_links.txt
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       12 2023-06-30 18:17:09.000000 h5coro-0.0.4/h5coro.egg-info/requires.txt
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       13 2023-06-30 18:17:09.000000 h5coro-0.0.4/h5coro.egg-info/top_level.txt
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      134 2023-06-27 13:30:21.000000 h5coro-0.0.4/pytest.ini
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       11 2023-06-27 13:24:47.000000 h5coro-0.0.4/requirements.txt
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       38 2023-06-30 18:17:09.790831 h5coro-0.0.4/setup.cfg
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     1169 2023-06-27 13:13:35.000000 h5coro-0.0.4/setup.py
-drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-06-30 18:17:09.790831 h5coro-0.0.4/utils/
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     3189 2023-06-27 20:18:26.000000 h5coro-0.0.4/utils/read_variable.py
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     7347 2023-06-29 20:21:49.000000 h5coro-0.0.4/utils/subset_atl03.py
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     5127 2023-06-28 18:01:05.000000 h5coro-0.0.4/utils/subset_atl06.py
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)    10271 2023-06-28 15:45:48.000000 h5coro-0.0.4/utils/utils.py
--rw-rw-r--   0 jswinski  (1001) jswinski  (1001)        7 2023-06-30 17:20:52.000000 h5coro-0.0.4/version.txt
+drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-07-06 14:03:10.450705 h5coro-0.0.5/
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     3078 2023-06-27 11:55:04.000000 h5coro-0.0.5/.gitignore
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     1511 2023-06-27 11:55:04.000000 h5coro-0.0.5/LICENSE
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      150 2023-06-27 11:55:04.000000 h5coro-0.0.5/MANIFEST.in
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      572 2023-07-06 14:03:10.450705 h5coro-0.0.5/PKG-INFO
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)    13802 2023-07-05 20:41:02.000000 h5coro-0.0.5/README.md
+drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-07-06 14:03:10.446705 h5coro-0.0.5/data/
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      338 2023-06-27 19:37:14.000000 h5coro-0.0.5/data/grandmesa.geojson
+drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-07-06 14:03:10.450705 h5coro-0.0.5/h5coro/
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      194 2023-06-27 11:55:04.000000 h5coro-0.0.5/h5coro/__init__.py
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      229 2023-06-27 13:23:23.000000 h5coro-0.0.5/h5coro/filedriver.py
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)    93760 2023-07-05 20:38:28.000000 h5coro-0.0.5/h5coro/h5coro.py
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     2059 2023-07-05 20:54:12.000000 h5coro-0.0.5/h5coro/s3driver.py
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      319 2023-06-27 11:55:04.000000 h5coro-0.0.5/h5coro/version.py
+drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-07-06 14:03:10.450705 h5coro-0.0.5/h5coro.egg-info/
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      572 2023-07-06 14:03:10.000000 h5coro-0.0.5/h5coro.egg-info/PKG-INFO
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      437 2023-07-06 14:03:10.000000 h5coro-0.0.5/h5coro.egg-info/SOURCES.txt
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)        1 2023-07-06 14:03:10.000000 h5coro-0.0.5/h5coro.egg-info/dependency_links.txt
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       12 2023-07-06 14:03:10.000000 h5coro-0.0.5/h5coro.egg-info/requires.txt
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       13 2023-07-06 14:03:10.000000 h5coro-0.0.5/h5coro.egg-info/top_level.txt
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)      134 2023-06-27 13:30:21.000000 h5coro-0.0.5/pytest.ini
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       11 2023-06-27 13:24:47.000000 h5coro-0.0.5/requirements.txt
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)       38 2023-07-06 14:03:10.450705 h5coro-0.0.5/setup.cfg
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     1078 2023-07-03 19:56:10.000000 h5coro-0.0.5/setup.py
+drwxrwxr-x   0 jswinski  (1001) jswinski  (1001)        0 2023-07-06 14:03:10.450705 h5coro-0.0.5/utils/
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     3380 2023-07-06 12:51:32.000000 h5coro-0.0.5/utils/read_variable.py
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     7347 2023-06-29 20:21:49.000000 h5coro-0.0.5/utils/subset_atl03.py
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)     5127 2023-06-28 18:01:05.000000 h5coro-0.0.5/utils/subset_atl06.py
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)    10271 2023-07-05 20:48:46.000000 h5coro-0.0.5/utils/utils.py
+-rw-rw-r--   0 jswinski  (1001) jswinski  (1001)        7 2023-07-06 13:57:02.000000 h5coro-0.0.5/version.txt
```

### Comparing `h5coro-0.0.4/.gitignore` & `h5coro-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `h5coro-0.0.4/LICENSE` & `h5coro-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `h5coro-0.0.4/PKG-INFO` & `h5coro-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5coro
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for reading HDF5 data from S3
 Home-page: https://github.com/ICESat2-SlideRule/h5coro/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `h5coro-0.0.4/h5coro/h5coro.py` & `h5coro-0.0.5/h5coro/h5coro.py`

 * *Files identical despite different names*

### Comparing `h5coro-0.0.4/h5coro/s3driver.py` & `h5coro-0.0.5/h5coro/s3driver.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,17 +25,19 @@
     #######################
     def __init__(self, resource, credentials):
 
         # construct path to resource
         self.resourcePath = list(filter(('').__ne__, resource.split('/')))
 
         # apply credentials is supplied
-        if  "aws_access_key_id" in credentials and \
-            "aws_secret_access_key" in credentials and \
-            "aws_session_token" in credentials:
+        if "profile" in credentials:
+            self.session = boto3.Session(profile_name=credentials["profile"])
+        elif "aws_access_key_id" in credentials and \
+             "aws_secret_access_key" in credentials and \
+             "aws_session_token" in credentials:
             self.session = boto3.Session(aws_access_key_id=credentials["aws_access_key_id"],
                                          aws_secret_access_key=credentials["aws_secret_access_key"],
                                          aws_session_token=credentials["aws_session_token"])
         elif len(credentials) == 0:
             self.session = boto3.Session()
         else:
             raise FatalError('invalid credential keys provided, looking for: aws_access_key_id, aws_secret_access_key, and aws_session_token')
```

### Comparing `h5coro-0.0.4/h5coro.egg-info/PKG-INFO` & `h5coro-0.0.5/h5coro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5coro
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for reading HDF5 data from S3
 Home-page: https://github.com/ICESat2-SlideRule/h5coro/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `h5coro-0.0.4/setup.py` & `h5coro-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,17 +11,14 @@
 
 # get version
 with open('version.txt') as fh:
     version = fh.read().strip()
     if version[0] == 'v':
         version = version[1:]
 
-# list of all utility scripts to be included with package
-scripts=[]
-
 setup(
     name='h5coro',
     author='SlideRule Developers',
     description='Python package for reading HDF5 data from S3',
     long_description_content_type="text/markdown",
     url='https://github.com/ICESat2-SlideRule/h5coro/',
     license='BSD 3-Clause',
@@ -32,9 +29,8 @@
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.11',
     ],
     packages=find_packages(),
     version=version,
     install_requires=install_requires,
-    scripts=scripts,
 )
```

### Comparing `h5coro-0.0.4/utils/read_variable.py` & `h5coro-0.0.5/utils/read_variable.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 ###############################################################################
 # COMMAND LINE ARGUMENTS
 ###############################################################################
 
 parser = argparse.ArgumentParser(description="""Subset ATL06 granules""")
 parser.add_argument('--granule','-g', type=str, default="/data/ATLAS/ATL03_20181017222812_02950102_005_01.h5")
 parser.add_argument('--variables','-x', nargs='+', type=str, default=["/gt2l/heights/h_ph"])
+parser.add_argument('--profile','-p', type=str, default="default")
 parser.add_argument('--driver','-d', type=str, default="file") # s3
 parser.add_argument('--checkErrors','-e', action='store_true', default=False)
 parser.add_argument('--verbose','-v', action='store_true', default=False)
 parser.add_argument('--enableAttributes','-a', action='store_true', default=False)
 parser.add_argument('--slice','-s', nargs=2, type=int, default=[0,10])
 args,_ = parser.parse_known_args()
 
@@ -53,11 +54,14 @@
 else:
     args.driver = None
 
 ###############################################################################
 # MAIN
 ###############################################################################
 
-h5coro.config(errorChecking=args.checkErrors, verbose=args.verbose, enableAttributes=args.enableAttributes, logLevel=logging.INFO)
-h5obj = h5coro.H5Coro(args.granule, args.driver, datasets=args.variables, block=False)
-for variable in h5obj:
-    print(f'{variable}: {h5obj[variable][args.slice[0]:args.slice[1]]}')
+try:
+    h5coro.config(errorChecking=args.checkErrors, verbose=args.verbose, enableAttributes=args.enableAttributes, logLevel=logging.INFO)
+    h5obj = h5coro.H5Coro(args.granule, args.driver, datasets=args.variables, block=False, credentials={"profile":args.profile})
+    for variable in h5obj:
+        print(f'{variable}: {h5obj[variable][args.slice[0]:args.slice[1]]}')
+except Exception as e:
+    print(f'{e.__class__.__name__}: {e}')
```

### Comparing `h5coro-0.0.4/utils/subset_atl03.py` & `h5coro-0.0.5/utils/subset_atl03.py`

 * *Files identical despite different names*

### Comparing `h5coro-0.0.4/utils/subset_atl06.py` & `h5coro-0.0.5/utils/subset_atl06.py`

 * *Files identical despite different names*

### Comparing `h5coro-0.0.4/utils/utils.py` & `h5coro-0.0.5/utils/utils.py`

 * *Files identical despite different names*

