# Comparing `tmp/alibabacloud_dytnsapi20200217-1.0.9.tar.gz` & `tmp/alibabacloud_dytnsapi20200217-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dytnsapi20200217-1.0.9.tar", last modified: Mon Mar 21 03:12:08 2022, max compression
+gzip compressed data, was "dist/alibabacloud_dytnsapi20200217-2.0.0.tar", last modified: Thu Jul  6 06:20:10 2023, max compression
```

## Comparing `alibabacloud_dytnsapi20200217-1.0.9.tar` & `alibabacloud_dytnsapi20200217-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-21 03:12:08.000000 alibabacloud_dytnsapi20200217-1.0.9/
--rw-r--r--   0 root         (0) root         (0)      519 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2022-03-21 03:12:08.000000 alibabacloud_dytnsapi20200217-1.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-21 03:12:08.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217/
--rw-r--r--   0 root         (0) root         (0)       21 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26409 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217/client.py
--rw-r--r--   0 root         (0) root         (0)    34192 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-21 03:12:08.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-03-21 03:12:08.000000 alibabacloud_dytnsapi20200217-1.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     2238 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/alibabacloud_dytnsapi20200217/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/alibabacloud_dytnsapi20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    61761 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/alibabacloud_dytnsapi20200217/client.py
+-rw-r--r--   0 root         (0) root         (0)    90041 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/alibabacloud_dytnsapi20200217/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/alibabacloud_dytnsapi20200217.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/alibabacloud_dytnsapi20200217.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/alibabacloud_dytnsapi20200217.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/alibabacloud_dytnsapi20200217.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/alibabacloud_dytnsapi20200217.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/alibabacloud_dytnsapi20200217.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-07-06 06:20:10.000000 alibabacloud_dytnsapi20200217-2.0.0/setup.py
```

### Comparing `alibabacloud_dytnsapi20200217-1.0.9/LICENSE` & `alibabacloud_dytnsapi20200217-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dytnsapi20200217-1.0.9/PKG-INFO` & `alibabacloud_dytnsapi20200217-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dytnsapi20200217
-Version: 1.0.9
+Version: 2.0.0
 Summary: Alibaba Cloud Dytnsapi (20200217) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dytnsapi20200217-1.0.9/README-CN.md` & `alibabacloud_dytnsapi20200217-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dytnsapi20200217-1.0.9/README.md` & `alibabacloud_dytnsapi20200217-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217.egg-info/PKG-INFO` & `alibabacloud_dytnsapi20200217-2.0.0/alibabacloud_dytnsapi20200217.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dytnsapi20200217
-Version: 1.0.9
+Version: 2.0.0
 Summary: Alibaba Cloud Dytnsapi (20200217) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dytnsapi20200217-1.0.9/setup.py` & `alibabacloud_dytnsapi20200217-2.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dytnsapi20200217.
 
-Created on 21/03/2022
+Created on 06/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dytnsapi20200217"
 NAME = "alibabacloud_dytnsapi20200217" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dytnsapi (20200217) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.1, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

