# Comparing `tmp/pycrawlers-1.0.0.tar.gz` & `tmp/pycrawlers-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrawlers-1.0.0.tar", last modified: Wed Jul  5 05:39:39 2023, max compression
+gzip compressed data, was "pycrawlers-1.0.1.tar", last modified: Thu Jul  6 02:08:03 2023, max compression
```

## Comparing `pycrawlers-1.0.0.tar` & `pycrawlers-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-05 05:39:39.899920 pycrawlers-1.0.0/
--rw-r--r--   0 bo         (501) staff       (20)    11357 2022-08-16 07:24:33.000000 pycrawlers-1.0.0/LICENSE
--rw-r--r--   0 bo         (501) staff       (20)     2948 2023-07-05 05:39:39.899780 pycrawlers-1.0.0/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)     2491 2023-06-30 09:56:53.000000 pycrawlers-1.0.0/README.md
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-05 05:39:39.896185 pycrawlers-1.0.0/other/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:58:18.000000 pycrawlers-1.0.0/other/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)      745 2022-08-17 09:04:51.000000 pycrawlers-1.0.0/other/dw_hg.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-05 05:39:39.896375 pycrawlers-1.0.0/pycrawlers/
--rw-r--r--   0 bo         (501) staff       (20)      232 2023-06-30 09:44:44.000000 pycrawlers-1.0.0/pycrawlers/__init__.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-05 05:39:39.897535 pycrawlers-1.0.0/pycrawlers/common/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:44:00.000000 pycrawlers-1.0.0/pycrawlers/common/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     2644 2023-06-21 08:33:43.000000 pycrawlers-1.0.0/pycrawlers/common/default_data.py
--rw-r--r--   0 bo         (501) staff       (20)     5356 2023-07-05 03:46:40.000000 pycrawlers-1.0.0/pycrawlers/common/tools.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-05 05:39:39.898027 pycrawlers-1.0.0/pycrawlers/huggingfaces/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 08:04:35.000000 pycrawlers-1.0.0/pycrawlers/huggingfaces/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     5106 2023-07-05 03:33:48.000000 pycrawlers-1.0.0/pycrawlers/huggingfaces/download.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-05 05:39:39.899258 pycrawlers-1.0.0/pycrawlers/websites/
--rw-r--r--   0 bo         (501) staff       (20)       75 2023-06-25 03:29:06.000000 pycrawlers-1.0.0/pycrawlers/websites/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     2239 2023-06-25 05:57:32.000000 pycrawlers-1.0.0/pycrawlers/websites/get_web_page.py
--rw-r--r--   0 bo         (501) staff       (20)     3607 2023-06-30 07:03:43.000000 pycrawlers-1.0.0/pycrawlers/websites/get_web_page_id.py
--rw-r--r--   0 bo         (501) staff       (20)      882 2023-06-30 09:44:44.000000 pycrawlers-1.0.0/pycrawlers/websites/get_websites.py
--rw-r--r--   0 bo         (501) staff       (20)      568 2023-06-30 07:15:34.000000 pycrawlers-1.0.0/pycrawlers/websites/url_filters.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-05 05:39:39.896964 pycrawlers-1.0.0/pycrawlers.egg-info/
--rw-r--r--   0 bo         (501) staff       (20)     2948 2023-07-05 05:39:39.000000 pycrawlers-1.0.0/pycrawlers.egg-info/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      592 2023-07-05 05:39:39.000000 pycrawlers-1.0.0/pycrawlers.egg-info/SOURCES.txt
--rw-r--r--   0 bo         (501) staff       (20)        1 2023-07-05 05:39:39.000000 pycrawlers-1.0.0/pycrawlers.egg-info/dependency_links.txt
--rw-r--r--   0 bo         (501) staff       (20)       71 2023-07-05 05:39:39.000000 pycrawlers-1.0.0/pycrawlers.egg-info/requires.txt
--rw-r--r--   0 bo         (501) staff       (20)       17 2023-07-05 05:39:39.000000 pycrawlers-1.0.0/pycrawlers.egg-info/top_level.txt
--rw-r--r--   0 bo         (501) staff       (20)       38 2023-07-05 05:39:39.899961 pycrawlers-1.0.0/setup.cfg
--rw-r--r--   0 bo         (501) staff       (20)      907 2023-07-05 03:49:19.000000 pycrawlers-1.0.0/setup.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:08:03.844231 pycrawlers-1.0.1/
+-rw-r--r--   0 bo         (501) staff       (20)    11357 2022-08-16 07:24:33.000000 pycrawlers-1.0.1/LICENSE
+-rw-r--r--   0 bo         (501) staff       (20)     3013 2023-07-06 02:08:03.844115 pycrawlers-1.0.1/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)     2556 2023-07-05 06:09:58.000000 pycrawlers-1.0.1/README.md
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:08:03.842321 pycrawlers-1.0.1/other/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:58:18.000000 pycrawlers-1.0.1/other/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)      745 2022-08-17 09:04:51.000000 pycrawlers-1.0.1/other/dw_hg.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:08:03.842420 pycrawlers-1.0.1/pycrawlers/
+-rw-r--r--   0 bo         (501) staff       (20)      232 2023-06-30 09:44:44.000000 pycrawlers-1.0.1/pycrawlers/__init__.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:08:03.843240 pycrawlers-1.0.1/pycrawlers/common/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:44:00.000000 pycrawlers-1.0.1/pycrawlers/common/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2644 2023-06-21 08:33:43.000000 pycrawlers-1.0.1/pycrawlers/common/default_data.py
+-rw-r--r--   0 bo         (501) staff       (20)     5392 2023-07-06 02:07:03.000000 pycrawlers-1.0.1/pycrawlers/common/tools.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:08:03.843444 pycrawlers-1.0.1/pycrawlers/huggingfaces/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 08:04:35.000000 pycrawlers-1.0.1/pycrawlers/huggingfaces/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     5106 2023-07-05 03:33:48.000000 pycrawlers-1.0.1/pycrawlers/huggingfaces/download.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:08:03.843958 pycrawlers-1.0.1/pycrawlers/websites/
+-rw-r--r--   0 bo         (501) staff       (20)       75 2023-06-25 03:29:06.000000 pycrawlers-1.0.1/pycrawlers/websites/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2239 2023-06-25 05:57:32.000000 pycrawlers-1.0.1/pycrawlers/websites/get_web_page.py
+-rw-r--r--   0 bo         (501) staff       (20)     3607 2023-06-30 07:03:43.000000 pycrawlers-1.0.1/pycrawlers/websites/get_web_page_id.py
+-rw-r--r--   0 bo         (501) staff       (20)      882 2023-06-30 09:44:44.000000 pycrawlers-1.0.1/pycrawlers/websites/get_websites.py
+-rw-r--r--   0 bo         (501) staff       (20)      568 2023-06-30 07:15:34.000000 pycrawlers-1.0.1/pycrawlers/websites/url_filters.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-07-06 02:08:03.842916 pycrawlers-1.0.1/pycrawlers.egg-info/
+-rw-r--r--   0 bo         (501) staff       (20)     3013 2023-07-06 02:08:03.000000 pycrawlers-1.0.1/pycrawlers.egg-info/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)      592 2023-07-06 02:08:03.000000 pycrawlers-1.0.1/pycrawlers.egg-info/SOURCES.txt
+-rw-r--r--   0 bo         (501) staff       (20)        1 2023-07-06 02:08:03.000000 pycrawlers-1.0.1/pycrawlers.egg-info/dependency_links.txt
+-rw-r--r--   0 bo         (501) staff       (20)       71 2023-07-06 02:08:03.000000 pycrawlers-1.0.1/pycrawlers.egg-info/requires.txt
+-rw-r--r--   0 bo         (501) staff       (20)       17 2023-07-06 02:08:03.000000 pycrawlers-1.0.1/pycrawlers.egg-info/top_level.txt
+-rw-r--r--   0 bo         (501) staff       (20)       38 2023-07-06 02:08:03.844268 pycrawlers-1.0.1/setup.cfg
+-rw-r--r--   0 bo         (501) staff       (20)      907 2023-07-06 02:07:54.000000 pycrawlers-1.0.1/setup.py
```

### Comparing `pycrawlers-1.0.0/LICENSE` & `pycrawlers-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.0/PKG-INFO` & `pycrawlers-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrawlers
-Version: 1.0.0
+Version: 1.0.1
 Summary: A collection of Crawlers
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -54,15 +54,16 @@
     # 2.1 使用默认保存位置（'./'）
     hg.get_batch_data(urls)
     
     # 2.2 自定义保存地址
     # hg.get_batch_data(urls, paths)
 
 ### 2.  通用抓取网页
-可以抓取那些反爬不厉害的网站
+可以抓取那些反爬不厉害的网站。
+注意：需安装 mongodb，数据将会存储在 mongodb里
 
 #### 2.1  简单使用
 
 
     from pycrawlers import crawl_website
 
     mongo_host = ''
```

### Comparing `pycrawlers-1.0.0/README.md` & `pycrawlers-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     # 2.1 使用默认保存位置（'./'）
     hg.get_batch_data(urls)
     
     # 2.2 自定义保存地址
     # hg.get_batch_data(urls, paths)
 
 ### 2.  通用抓取网页
-可以抓取那些反爬不厉害的网站
+可以抓取那些反爬不厉害的网站。
+注意：需安装 mongodb，数据将会存储在 mongodb里
 
 #### 2.1  简单使用
 
 
     from pycrawlers import crawl_website
 
     mongo_host = ''
```

### Comparing `pycrawlers-1.0.0/other/dw_hg.py` & `pycrawlers-1.0.1/other/dw_hg.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.0/pycrawlers/common/default_data.py` & `pycrawlers-1.0.1/pycrawlers/common/default_data.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.0/pycrawlers/common/tools.py` & `pycrawlers-1.0.1/pycrawlers/common/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     resp_ = get_data()
     total_ = int(resp_.headers.get('content-length', 0))
     if file_size < total_:
         file_op = 'wb'
         if file_size:
             headers['Range'] = f'bytes={file_size}-'
             file_op = 'ab'
+        time.sleep(random.random())
         resp = get_data()
         total = int(resp.headers.get('content-length', 0))
         with open(fname, file_op) as file, tqdm(
             desc=fname,
             total=total,
             unit='iB',
             unit_scale=True,
```

### Comparing `pycrawlers-1.0.0/pycrawlers/huggingfaces/download.py` & `pycrawlers-1.0.1/pycrawlers/huggingfaces/download.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.0/pycrawlers/websites/get_web_page.py` & `pycrawlers-1.0.1/pycrawlers/websites/get_web_page.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.0/pycrawlers/websites/get_web_page_id.py` & `pycrawlers-1.0.1/pycrawlers/websites/get_web_page_id.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.0/pycrawlers/websites/get_websites.py` & `pycrawlers-1.0.1/pycrawlers/websites/get_websites.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.0/pycrawlers/websites/url_filters.py` & `pycrawlers-1.0.1/pycrawlers/websites/url_filters.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.0/pycrawlers.egg-info/PKG-INFO` & `pycrawlers-1.0.1/pycrawlers.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrawlers
-Version: 1.0.0
+Version: 1.0.1
 Summary: A collection of Crawlers
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -54,15 +54,16 @@
     # 2.1 使用默认保存位置（'./'）
     hg.get_batch_data(urls)
     
     # 2.2 自定义保存地址
     # hg.get_batch_data(urls, paths)
 
 ### 2.  通用抓取网页
-可以抓取那些反爬不厉害的网站
+可以抓取那些反爬不厉害的网站。
+注意：需安装 mongodb，数据将会存储在 mongodb里
 
 #### 2.1  简单使用
 
 
     from pycrawlers import crawl_website
 
     mongo_host = ''
```

### Comparing `pycrawlers-1.0.0/pycrawlers.egg-info/SOURCES.txt` & `pycrawlers-1.0.1/pycrawlers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycrawlers-1.0.0/setup.py` & `pycrawlers-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pycrawlers',
-    version='1.0.0',
+    version='1.0.1',
     packages=setuptools.find_packages(),
     url='https://gitee.com/maxbanana',
     license='Apache',
     author='hongbo liu',
     author_email='782027465@qq.com',
     description='A collection of Crawlers',
     long_description=long_description,
```

