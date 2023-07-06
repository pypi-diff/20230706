# Comparing `tmp/bitbucket-pipes-toolkit-3.3.0.tar.gz` & `tmp/bitbucket-pipes-toolkit-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bitbucket-pipes-toolkit-3.3.0.tar", last modified: Tue Jun 27 08:33:46 2023, max compression
+gzip compressed data, was "dist/bitbucket-pipes-toolkit-3.3.1.tar", last modified: Thu Jul  6 10:48:34 2023, max compression
```

## Comparing `bitbucket-pipes-toolkit-3.3.0.tar` & `bitbucket-pipes-toolkit-3.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/
--rw-r--r--   0 root         (0) root         (0)     1973 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-06-27 08:33:27.000000 bitbucket-pipes-toolkit-3.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-06-27 08:33:27.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6851 2023-06-27 08:33:27.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)    14341 2023-06-27 08:33:27.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/core.py
--rw-rw-rw-   0 root         (0) root         (0)     5811 2023-06-27 08:33:27.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     3106 2023-06-27 08:33:27.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1973 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      426 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 08:33:46.000000 bitbucket-pipes-toolkit-3.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      742 2023-06-27 08:33:27.000000 bitbucket-pipes-toolkit-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-07-06 10:48:20.000000 bitbucket-pipes-toolkit-3.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-06 10:48:20.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6851 2023-07-06 10:48:20.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)    14341 2023-07-06 10:48:20.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     5811 2023-07-06 10:48:20.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3106 2023-07-06 10:48:20.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      426 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      742 2023-07-06 10:48:20.000000 bitbucket-pipes-toolkit-3.3.1/setup.py
```

### Comparing `bitbucket-pipes-toolkit-3.3.0/PKG-INFO` & `bitbucket-pipes-toolkit-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitbucket-pipes-toolkit
-Version: 3.3.0
+Version: 3.3.1
 Summary: This package contains various helpers for developing bitbucket pipelines pipes
 Home-page: https://bitbucket.org/bitbucketpipelines/bitbucket-pipes-toolkit
 Author: Atlassian
 Author-email: bitbucketci-team@atlassian.com
 License: UNKNOWN
 Description: Bitbucket Pipes Toolkit
         =========
```

### Comparing `bitbucket-pipes-toolkit-3.3.0/README.md` & `bitbucket-pipes-toolkit-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/annotations.py` & `bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/annotations.py`

 * *Files identical despite different names*

### Comparing `bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/core.py` & `bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/core.py`

 * *Files identical despite different names*

### Comparing `bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/helpers.py` & `bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/helpers.py`

 * *Files identical despite different names*

### Comparing `bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit/test.py` & `bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/test.py`

 * *Files identical despite different names*

### Comparing `bitbucket-pipes-toolkit-3.3.0/bitbucket_pipes_toolkit.egg-info/PKG-INFO` & `bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitbucket-pipes-toolkit
-Version: 3.3.0
+Version: 3.3.1
 Summary: This package contains various helpers for developing bitbucket pipelines pipes
 Home-page: https://bitbucket.org/bitbucketpipelines/bitbucket-pipes-toolkit
 Author: Atlassian
 Author-email: bitbucketci-team@atlassian.com
 License: UNKNOWN
 Description: Bitbucket Pipes Toolkit
         =========
```

### Comparing `bitbucket-pipes-toolkit-3.3.0/setup.py` & `bitbucket-pipes-toolkit-3.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='bitbucket-pipes-toolkit',
-    version='3.3.0',
+    version='3.3.1',
     packages=['bitbucket_pipes_toolkit', ],
     url='https://bitbucket.org/bitbucketpipelines/bitbucket-pipes-toolkit',
     author='Atlassian',
     author_email='bitbucketci-team@atlassian.com',
     description='This package contains various helpers for developing bitbucket pipelines pipes',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

