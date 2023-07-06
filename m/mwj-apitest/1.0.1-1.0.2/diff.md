# Comparing `tmp/mwj-apitest-1.0.1.tar.gz` & `tmp/mwj-apitest-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwj-apitest-1.0.1.tar", last modified: Wed May 31 11:12:34 2023, max compression
+gzip compressed data, was "mwj-apitest-1.0.2.tar", last modified: Thu Jul  6 10:09:36 2023, max compression
```

## Comparing `mwj-apitest-1.0.1.tar` & `mwj-apitest-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 11:12:34.726054 mwj-apitest-1.0.1/
--rw-rw-rw-   0        0        0     1091 2023-05-31 08:57:31.000000 mwj-apitest-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       34 2023-05-31 08:08:20.000000 mwj-apitest-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      565 2023-05-31 11:12:34.725079 mwj-apitest-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       81 2023-05-31 11:03:33.000000 mwj-apitest-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 11:12:34.715319 mwj-apitest-1.0.1/mwjApiTest/
--rw-rw-rw-   0        0        0      215 2023-05-31 09:41:04.000000 mwj-apitest-1.0.1/mwjApiTest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 11:12:34.716295 mwj-apitest-1.0.1/mwjApiTest/core/
--rw-rw-rw-   0        0        0      190 2023-05-31 08:48:04.000000 mwj-apitest-1.0.1/mwjApiTest/core/__init__.py
--rw-rw-rw-   0        0        0     1140 2023-05-31 11:08:47.000000 mwj-apitest-1.0.1/mwjApiTest/manage.py
-drwxrwxrwx   0        0        0        0 2023-05-31 11:12:34.716295 mwj-apitest-1.0.1/mwjApiTest/utils/
--rw-rw-rw-   0        0        0      190 2023-05-31 08:48:04.000000 mwj-apitest-1.0.1/mwjApiTest/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 11:12:34.724103 mwj-apitest-1.0.1/mwj_apitest.egg-info/
--rw-rw-rw-   0        0        0      565 2023-05-31 11:12:34.000000 mwj-apitest-1.0.1/mwj_apitest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-05-31 11:12:34.000000 mwj-apitest-1.0.1/mwj_apitest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 11:12:34.000000 mwj-apitest-1.0.1/mwj_apitest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-31 11:12:34.000000 mwj-apitest-1.0.1/mwj_apitest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-05-31 11:12:34.000000 mwj-apitest-1.0.1/mwj_apitest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 11:12:34.726054 mwj-apitest-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1482 2023-05-31 11:08:47.000000 mwj-apitest-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:09:36.532032 mwj-apitest-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-31 08:57:31.000000 mwj-apitest-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-05-31 08:08:20.000000 mwj-apitest-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      630 2023-07-06 10:09:36.531091 mwj-apitest-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2023-07-06 09:33:36.000000 mwj-apitest-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 10:09:36.512745 mwj-apitest-1.0.2/mwjApiTest/
+-rw-rw-rw-   0        0        0      215 2023-05-31 09:41:04.000000 mwj-apitest-1.0.2/mwjApiTest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:09:36.513742 mwj-apitest-1.0.2/mwjApiTest/core/
+-rw-rw-rw-   0        0        0      190 2023-05-31 08:48:04.000000 mwj-apitest-1.0.2/mwjApiTest/core/__init__.py
+-rw-rw-rw-   0        0        0     1140 2023-05-31 11:08:47.000000 mwj-apitest-1.0.2/mwjApiTest/manage.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:09:36.514739 mwj-apitest-1.0.2/mwjApiTest/utils/
+-rw-rw-rw-   0        0        0      190 2023-05-31 08:48:04.000000 mwj-apitest-1.0.2/mwjApiTest/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:09:36.528761 mwj-apitest-1.0.2/mwj_apitest.egg-info/
+-rw-rw-rw-   0        0        0      630 2023-07-06 10:09:36.000000 mwj-apitest-1.0.2/mwj_apitest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-07-06 10:09:36.000000 mwj-apitest-1.0.2/mwj_apitest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 10:09:36.000000 mwj-apitest-1.0.2/mwj_apitest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-06 10:09:36.000000 mwj-apitest-1.0.2/mwj_apitest.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-07-06 10:09:36.000000 mwj-apitest-1.0.2/mwj_apitest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 10:09:36.532032 mwj-apitest-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1516 2023-07-06 09:33:06.000000 mwj-apitest-1.0.2/setup.py
```

### Comparing `mwj-apitest-1.0.1/LICENSE` & `mwj-apitest-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.0.1/mwjApiTest/manage.py` & `mwj-apitest-1.0.2/mwjApiTest/manage.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.0.1/setup.py` & `mwj-apitest-1.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mwj-apitest",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.0.1",  # 包版本号，便于维护版本,保证每次发布都是版本都是唯一的
+    version="1.0.2",  # 包版本号，便于维护版本,保证每次发布都是版本都是唯一的
     author="梦无矶小仔",  # 作者，可以写自己的姓名
     author_email="Lvan826199@163.com",  # 作者联系方式，可写自己的邮箱地址
-    description="A small example package",  # 包的简述
+    description="An execution engine for the interface automation platform",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/Lvan826199/mwjApiTest",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
     entry_points={
         "console_scripts" : ['mwjApiTest = mwjApiTest.manage:main']
     }, #安装成功后，在命令行输入mwjApiTest 就相当于执行了mwjApiTest.manage.py中的main了
```

