# Comparing `tmp/kyqacommon-1.0.5.tar.gz` & `tmp/kyqacommon-1.0.706.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kyqacommon-1.0.5.tar", last modified: Wed May 31 08:00:11 2023, max compression
+gzip compressed data, was "kyqacommon-1.0.706.tar", last modified: Thu Jul  6 07:56:01 2023, max compression
```

## Comparing `kyqacommon-1.0.5.tar` & `kyqacommon-1.0.706.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 08:00:11.530852 kyqacommon-1.0.5/
--rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 kyqacommon-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      442 2023-05-31 08:00:11.530852 kyqacommon-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       67 2022-07-28 10:32:06.000000 kyqacommon-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 08:00:11.521597 kyqacommon-1.0.5/kyqacommon/
--rw-rw-rw-   0        0        0       67 2022-07-28 10:07:15.000000 kyqacommon-1.0.5/kyqacommon/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-02-16 08:19:41.000000 kyqacommon-1.0.5/kyqacommon/getLogger.py
--rw-rw-rw-   0        0        0     3075 2023-02-14 06:27:53.000000 kyqacommon-1.0.5/kyqacommon/minio_handld.py
--rw-rw-rw-   0        0        0     2126 2022-10-12 06:55:19.000000 kyqacommon-1.0.5/kyqacommon/uiCommonMethod.py
-drwxrwxrwx   0        0        0        0 2023-05-31 08:00:11.528853 kyqacommon-1.0.5/kyqacommon.egg-info/
--rw-rw-rw-   0        0        0      442 2023-05-31 08:00:11.000000 kyqacommon-1.0.5/kyqacommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-05-31 08:00:11.000000 kyqacommon-1.0.5/kyqacommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 08:00:11.000000 kyqacommon-1.0.5/kyqacommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-31 08:00:11.000000 kyqacommon-1.0.5/kyqacommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-31 08:00:11.531853 kyqacommon-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      905 2023-05-31 07:59:50.000000 kyqacommon-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:56:01.093958 kyqacommon-1.0.706/
+-rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 kyqacommon-1.0.706/LICENSE
+-rw-rw-rw-   0        0        0      444 2023-07-06 07:56:01.093958 kyqacommon-1.0.706/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2022-07-28 10:32:06.000000 kyqacommon-1.0.706/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 07:56:01.073104 kyqacommon-1.0.706/kyqacommon/
+-rw-rw-rw-   0        0        0       67 2022-07-28 10:07:15.000000 kyqacommon-1.0.706/kyqacommon/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-02-16 08:19:41.000000 kyqacommon-1.0.706/kyqacommon/getLogger.py
+-rw-rw-rw-   0        0        0     3075 2023-02-14 06:27:53.000000 kyqacommon-1.0.706/kyqacommon/minio_handld.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:56:01.091958 kyqacommon-1.0.706/kyqacommon/tools/
+-rw-rw-rw-   0        0        0        0 2023-07-06 07:45:55.000000 kyqacommon-1.0.706/kyqacommon/tools/__init__.py
+-rw-rw-rw-   0        0        0     6283 2023-07-06 07:49:19.000000 kyqacommon-1.0.706/kyqacommon/tools/cpu_ssh.py
+-rw-rw-rw-   0        0        0     3404 2023-07-06 07:49:19.000000 kyqacommon-1.0.706/kyqacommon/tools/dataBase.py
+-rw-rw-rw-   0        0        0      444 2023-07-06 07:49:19.000000 kyqacommon-1.0.706/kyqacommon/tools/loading_ly.py
+-rw-rw-rw-   0        0        0     2126 2022-10-12 06:55:19.000000 kyqacommon-1.0.706/kyqacommon/uiCommonMethod.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:56:01.083953 kyqacommon-1.0.706/kyqacommon.egg-info/
+-rw-rw-rw-   0        0        0      444 2023-07-06 07:56:00.000000 kyqacommon-1.0.706/kyqacommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-07-06 07:56:00.000000 kyqacommon-1.0.706/kyqacommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 07:56:00.000000 kyqacommon-1.0.706/kyqacommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-06 07:56:00.000000 kyqacommon-1.0.706/kyqacommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-06 07:56:00.000000 kyqacommon-1.0.706/kyqacommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-06 07:56:01.094958 kyqacommon-1.0.706/setup.cfg
+-rw-rw-rw-   0        0        0     1001 2023-07-06 07:54:03.000000 kyqacommon-1.0.706/setup.py
```

### Comparing `kyqacommon-1.0.5/LICENSE` & `kyqacommon-1.0.706/LICENSE`

 * *Files identical despite different names*

### Comparing `kyqacommon-1.0.5/kyqacommon/getLogger.py` & `kyqacommon-1.0.706/kyqacommon/getLogger.py`

 * *Files identical despite different names*

### Comparing `kyqacommon-1.0.5/kyqacommon/minio_handld.py` & `kyqacommon-1.0.706/kyqacommon/minio_handld.py`

 * *Files identical despite different names*

### Comparing `kyqacommon-1.0.5/kyqacommon/uiCommonMethod.py` & `kyqacommon-1.0.706/kyqacommon/uiCommonMethod.py`

 * *Files identical despite different names*

### Comparing `kyqacommon-1.0.5/setup.py` & `kyqacommon-1.0.706/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kyqacommon",  # 包名
-    version="1.0.5",  # 包版本号，便于维护版本
+    version="1.0.706",  # 包版本号，便于维护版本
     author="lyl",  # 作者
     author_email="lyulei66@163.com",  # 联系方式
     description="kyqacommon",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
+    install_requires = ["minio==7.1.13","pymysql==1.0.3","progress==1.6","paramiko==3.2.0"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',  # 对python的最低版本要求
 )
```

