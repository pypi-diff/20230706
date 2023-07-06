# Comparing `tmp/pycrawlers-1.0.1.tar.gz` & `tmp/pycrawlers-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrawlers-1.0.1.tar", last modified: Thu Jul  6 02:08:03 2023, max compression
+gzip compressed data, was "pycrawlers-1.0.2.tar", last modified: Thu Jul  6 02:16:35 2023, max compression
```

## Comparing `pycrawlers-1.0.1.tar` & `pycrawlers-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:08:03.844231 pycrawlers-1.0.1/
--rw-r--r--   0 bo         (501) staff       (20)    11357 2022-08-16 07:24:33.000000 pycrawlers-1.0.1/LICENSE
--rw-r--r--   0 bo         (501) staff       (20)     3013 2023-07-06 02:08:03.844115 pycrawlers-1.0.1/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)     2556 2023-07-05 06:09:58.000000 pycrawlers-1.0.1/README.md
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:08:03.842321 pycrawlers-1.0.1/other/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:58:18.000000 pycrawlers-1.0.1/other/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)      745 2022-08-17 09:04:51.000000 pycrawlers-1.0.1/other/dw_hg.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:08:03.842420 pycrawlers-1.0.1/pycrawlers/
--rw-r--r--   0 bo         (501) staff       (20)      232 2023-06-30 09:44:44.000000 pycrawlers-1.0.1/pycrawlers/__init__.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:08:03.843240 pycrawlers-1.0.1/pycrawlers/common/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:44:00.000000 pycrawlers-1.0.1/pycrawlers/common/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     2644 2023-06-21 08:33:43.000000 pycrawlers-1.0.1/pycrawlers/common/default_data.py
--rw-r--r--   0 bo         (501) staff       (20)     5392 2023-07-06 02:07:03.000000 pycrawlers-1.0.1/pycrawlers/common/tools.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:08:03.843444 pycrawlers-1.0.1/pycrawlers/huggingfaces/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 08:04:35.000000 pycrawlers-1.0.1/pycrawlers/huggingfaces/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     5106 2023-07-05 03:33:48.000000 pycrawlers-1.0.1/pycrawlers/huggingfaces/download.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:08:03.843958 pycrawlers-1.0.1/pycrawlers/websites/
--rw-r--r--   0 bo         (501) staff       (20)       75 2023-06-25 03:29:06.000000 pycrawlers-1.0.1/pycrawlers/websites/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     2239 2023-06-25 05:57:32.000000 pycrawlers-1.0.1/pycrawlers/websites/get_web_page.py
--rw-r--r--   0 bo         (501) staff       (20)     3607 2023-06-30 07:03:43.000000 pycrawlers-1.0.1/pycrawlers/websites/get_web_page_id.py
--rw-r--r--   0 bo         (501) staff       (20)      882 2023-06-30 09:44:44.000000 pycrawlers-1.0.1/pycrawlers/websites/get_websites.py
--rw-r--r--   0 bo         (501) staff       (20)      568 2023-06-30 07:15:34.000000 pycrawlers-1.0.1/pycrawlers/websites/url_filters.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:08:03.842916 pycrawlers-1.0.1/pycrawlers.egg-info/
--rw-r--r--   0 bo         (501) staff       (20)     3013 2023-07-06 02:08:03.000000 pycrawlers-1.0.1/pycrawlers.egg-info/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      592 2023-07-06 02:08:03.000000 pycrawlers-1.0.1/pycrawlers.egg-info/SOURCES.txt
--rw-r--r--   0 bo         (501) staff       (20)        1 2023-07-06 02:08:03.000000 pycrawlers-1.0.1/pycrawlers.egg-info/dependency_links.txt
--rw-r--r--   0 bo         (501) staff       (20)       71 2023-07-06 02:08:03.000000 pycrawlers-1.0.1/pycrawlers.egg-info/requires.txt
--rw-r--r--   0 bo         (501) staff       (20)       17 2023-07-06 02:08:03.000000 pycrawlers-1.0.1/pycrawlers.egg-info/top_level.txt
--rw-r--r--   0 bo         (501) staff       (20)       38 2023-07-06 02:08:03.844268 pycrawlers-1.0.1/setup.cfg
--rw-r--r--   0 bo         (501) staff       (20)      907 2023-07-06 02:07:54.000000 pycrawlers-1.0.1/setup.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:16:35.163493 pycrawlers-1.0.2/
+-rw-r--r--   0 bo         (501) staff       (20)    11357 2022-08-16 07:24:33.000000 pycrawlers-1.0.2/LICENSE
+-rw-r--r--   0 bo         (501) staff       (20)     3013 2023-07-06 02:16:35.163352 pycrawlers-1.0.2/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)     2556 2023-07-05 06:09:58.000000 pycrawlers-1.0.2/README.md
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:16:35.159719 pycrawlers-1.0.2/other/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:58:18.000000 pycrawlers-1.0.2/other/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)      745 2022-08-17 09:04:51.000000 pycrawlers-1.0.2/other/dw_hg.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:16:35.159915 pycrawlers-1.0.2/pycrawlers/
+-rw-r--r--   0 bo         (501) staff       (20)      232 2023-06-30 09:44:44.000000 pycrawlers-1.0.2/pycrawlers/__init__.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:16:35.161035 pycrawlers-1.0.2/pycrawlers/common/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:44:00.000000 pycrawlers-1.0.2/pycrawlers/common/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2644 2023-06-21 08:33:43.000000 pycrawlers-1.0.2/pycrawlers/common/default_data.py
+-rw-r--r--   0 bo         (501) staff       (20)     5392 2023-07-06 02:07:03.000000 pycrawlers-1.0.2/pycrawlers/common/tools.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:16:35.161412 pycrawlers-1.0.2/pycrawlers/huggingfaces/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 08:04:35.000000 pycrawlers-1.0.2/pycrawlers/huggingfaces/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     5132 2023-07-06 02:16:23.000000 pycrawlers-1.0.2/pycrawlers/huggingfaces/download.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:16:35.162856 pycrawlers-1.0.2/pycrawlers/websites/
+-rw-r--r--   0 bo         (501) staff       (20)       75 2023-06-25 03:29:06.000000 pycrawlers-1.0.2/pycrawlers/websites/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2239 2023-06-25 05:57:32.000000 pycrawlers-1.0.2/pycrawlers/websites/get_web_page.py
+-rw-r--r--   0 bo         (501) staff       (20)     3607 2023-06-30 07:03:43.000000 pycrawlers-1.0.2/pycrawlers/websites/get_web_page_id.py
+-rw-r--r--   0 bo         (501) staff       (20)      882 2023-06-30 09:44:44.000000 pycrawlers-1.0.2/pycrawlers/websites/get_websites.py
+-rw-r--r--   0 bo         (501) staff       (20)      568 2023-06-30 07:15:34.000000 pycrawlers-1.0.2/pycrawlers/websites/url_filters.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:16:35.160539 pycrawlers-1.0.2/pycrawlers.egg-info/
+-rw-r--r--   0 bo         (501) staff       (20)     3013 2023-07-06 02:16:34.000000 pycrawlers-1.0.2/pycrawlers.egg-info/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)      592 2023-07-06 02:16:35.000000 pycrawlers-1.0.2/pycrawlers.egg-info/SOURCES.txt
+-rw-r--r--   0 bo         (501) staff       (20)        1 2023-07-06 02:16:34.000000 pycrawlers-1.0.2/pycrawlers.egg-info/dependency_links.txt
+-rw-r--r--   0 bo         (501) staff       (20)       71 2023-07-06 02:16:35.000000 pycrawlers-1.0.2/pycrawlers.egg-info/requires.txt
+-rw-r--r--   0 bo         (501) staff       (20)       17 2023-07-06 02:16:35.000000 pycrawlers-1.0.2/pycrawlers.egg-info/top_level.txt
+-rw-r--r--   0 bo         (501) staff       (20)       38 2023-07-06 02:16:35.163533 pycrawlers-1.0.2/setup.cfg
+-rw-r--r--   0 bo         (501) staff       (20)      907 2023-07-06 02:16:23.000000 pycrawlers-1.0.2/setup.py
```

### Comparing `pycrawlers-1.0.1/LICENSE` & `pycrawlers-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.1/PKG-INFO` & `pycrawlers-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrawlers
-Version: 1.0.1
+Version: 1.0.2
 Summary: A collection of Crawlers
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pycrawlers-1.0.1/README.md` & `pycrawlers-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.1/other/dw_hg.py` & `pycrawlers-1.0.2/other/dw_hg.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.1/pycrawlers/common/default_data.py` & `pycrawlers-1.0.2/pycrawlers/common/default_data.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.1/pycrawlers/common/tools.py` & `pycrawlers-1.0.2/pycrawlers/common/tools.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.1/pycrawlers/huggingfaces/download.py` & `pycrawlers-1.0.2/pycrawlers/huggingfaces/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: UTF-8 -*-
 # @Time : 2022/8/17 15:38 
 # @Author : 刘洪波
 
 """
 获取hugging face 模型
 """
+import random
 import os
 import time
 from lxml import etree
 from pycrawlers.common.default_data import headers
 from pycrawlers.common.tools import requests_session
 from pycrawlers.common.tools import DealException
 from pycrawlers.common.tools import download
@@ -109,15 +110,15 @@
 
     def get_files(self, file_names, file_urls, files_path):
         for name, part_url in zip(file_names, file_urls):
             if name in part_url:
                 url = self.base_url + part_url
                 save_file_path = files_path + name
                 download(url, save_file_path, headers, read_timeout=60, file_size=self.get_file_size(save_file_path))
-                time.sleep(0.5)
+                time.sleep(random.random())
 
     @staticmethod
     def count_info(success_urls, fail_urls):
         print(f'程序执行统计：')
         print(f'a. 成功{str(len(success_urls))}个')
         print(f'b. 失败{str(len(fail_urls))}个')
         print(f'c. 成功的URL：{"，".join(success_urls)}')
```

### Comparing `pycrawlers-1.0.1/pycrawlers/websites/get_web_page.py` & `pycrawlers-1.0.2/pycrawlers/websites/get_web_page.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.1/pycrawlers/websites/get_web_page_id.py` & `pycrawlers-1.0.2/pycrawlers/websites/get_web_page_id.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.1/pycrawlers/websites/get_websites.py` & `pycrawlers-1.0.2/pycrawlers/websites/get_websites.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.1/pycrawlers/websites/url_filters.py` & `pycrawlers-1.0.2/pycrawlers/websites/url_filters.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.1/pycrawlers.egg-info/PKG-INFO` & `pycrawlers-1.0.2/pycrawlers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrawlers
-Version: 1.0.1
+Version: 1.0.2
 Summary: A collection of Crawlers
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pycrawlers-1.0.1/pycrawlers.egg-info/SOURCES.txt` & `pycrawlers-1.0.2/pycrawlers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.1/setup.py` & `pycrawlers-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pycrawlers',
-    version='1.0.1',
+    version='1.0.2',
     packages=setuptools.find_packages(),
     url='https://gitee.com/maxbanana',
     license='Apache',
     author='hongbo liu',
     author_email='782027465@qq.com',
     description='A collection of Crawlers',
     long_description=long_description,
```

