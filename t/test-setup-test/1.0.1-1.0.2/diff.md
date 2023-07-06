# Comparing `tmp/test_setup_test-1.0.1.tar.gz` & `tmp/test_setup_test-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_setup_test-1.0.1.tar", last modified: Thu Jul  6 11:49:15 2023, max compression
+gzip compressed data, was "test_setup_test-1.0.2.tar", last modified: Thu Jul  6 11:50:07 2023, max compression
```

## Comparing `test_setup_test-1.0.1.tar` & `test_setup_test-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-06 11:49:15.466583 test_setup_test-1.0.1/
--rw-rw-r--   0 divy      (1000) divy      (1000)     1022 2023-07-06 11:49:15.466583 test_setup_test-1.0.1/PKG-INFO
--rw-rw-r--   0 divy      (1000) divy      (1000)       95 2023-07-05 11:00:27.000000 test_setup_test-1.0.1/README.md
--rw-rw-r--   0 divy      (1000) divy      (1000)       38 2023-07-06 11:49:15.466583 test_setup_test-1.0.1/setup.cfg
--rw-rw-r--   0 divy      (1000) divy      (1000)      968 2023-07-06 11:49:03.000000 test_setup_test-1.0.1/setup.py
-drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-06 11:49:15.466583 test_setup_test-1.0.1/test_setup_test.egg-info/
--rw-rw-r--   0 divy      (1000) divy      (1000)     1022 2023-07-06 11:49:15.000000 test_setup_test-1.0.1/test_setup_test.egg-info/PKG-INFO
--rw-rw-r--   0 divy      (1000) divy      (1000)      174 2023-07-06 11:49:15.000000 test_setup_test-1.0.1/test_setup_test.egg-info/SOURCES.txt
--rw-rw-r--   0 divy      (1000) divy      (1000)        1 2023-07-06 11:49:15.000000 test_setup_test-1.0.1/test_setup_test.egg-info/dependency_links.txt
--rw-rw-r--   0 divy      (1000) divy      (1000)        1 2023-07-06 11:49:15.000000 test_setup_test-1.0.1/test_setup_test.egg-info/top_level.txt
+drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-06 11:50:07.103019 test_setup_test-1.0.2/
+-rw-rw-r--   0 divy      (1000) divy      (1000)      999 2023-07-06 11:50:07.103019 test_setup_test-1.0.2/PKG-INFO
+-rw-rw-r--   0 divy      (1000) divy      (1000)       95 2023-07-05 11:00:27.000000 test_setup_test-1.0.2/README.md
+-rw-rw-r--   0 divy      (1000) divy      (1000)       38 2023-07-06 11:50:07.103019 test_setup_test-1.0.2/setup.cfg
+-rw-rw-r--   0 divy      (1000) divy      (1000)      989 2023-07-06 11:50:04.000000 test_setup_test-1.0.2/setup.py
+drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-06 11:50:07.099031 test_setup_test-1.0.2/test_setup_test.egg-info/
+-rw-rw-r--   0 divy      (1000) divy      (1000)      999 2023-07-06 11:50:07.000000 test_setup_test-1.0.2/test_setup_test.egg-info/PKG-INFO
+-rw-rw-r--   0 divy      (1000) divy      (1000)      174 2023-07-06 11:50:07.000000 test_setup_test-1.0.2/test_setup_test.egg-info/SOURCES.txt
+-rw-rw-r--   0 divy      (1000) divy      (1000)        1 2023-07-06 11:50:07.000000 test_setup_test-1.0.2/test_setup_test.egg-info/dependency_links.txt
+-rw-rw-r--   0 divy      (1000) divy      (1000)        1 2023-07-06 11:50:07.000000 test_setup_test-1.0.2/test_setup_test.egg-info/top_level.txt
```

### Comparing `test_setup_test-1.0.1/PKG-INFO` & `test_setup_test-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: test_setup_test
-Version: 1.0.1
+Version: 1.0.2
 Summary: utils_bs_test
 Home-page: UNKNOWN
 Author: Divy TEST
 Author-email: divy.jain@bombaysoftwares.com
-Maintainer: Divy TEST1
 License: MIT
 Project-URL: Bug Tracker, https://github.com/abc
 Project-URL: Source Code, https://github.com/abc
 Project-URL: Documentation, https://github.com/abc
 Description: # Your Package
         
         Your Package Description
```

### Comparing `test_setup_test-1.0.1/setup.py` & `test_setup_test-1.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # setup.py
 from setuptools import setup
 
 setup(
     name='test_setup_test',
-    version='1.0.1',
+    version='1.0.2',
     author='Divy TEST',
     author_email='divy.jain@bombaysoftwares.com',
     description='utils_bs_test',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    maintainer='Divy TEST1',
+    maintainers=['Maintainer 1', 'Maintainer 2'],
 
     license='MIT',
     project_urls={
         "Bug Tracker": "https://github.com/abc",
         "Source Code": "https://github.com/abc",
         "Documentation": "https://github.com/abc"
     },
```

### Comparing `test_setup_test-1.0.1/test_setup_test.egg-info/PKG-INFO` & `test_setup_test-1.0.2/test_setup_test.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: test-setup-test
-Version: 1.0.1
+Version: 1.0.2
 Summary: utils_bs_test
 Home-page: UNKNOWN
 Author: Divy TEST
 Author-email: divy.jain@bombaysoftwares.com
-Maintainer: Divy TEST1
 License: MIT
 Project-URL: Bug Tracker, https://github.com/abc
 Project-URL: Source Code, https://github.com/abc
 Project-URL: Documentation, https://github.com/abc
 Description: # Your Package
         
         Your Package Description
```

