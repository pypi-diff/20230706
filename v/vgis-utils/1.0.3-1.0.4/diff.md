# Comparing `tmp/vgis_utils-1.0.3.tar.gz` & `tmp/vgis_utils-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgis_utils-1.0.3.tar", last modified: Tue Jun 27 08:48:40 2023, max compression
+gzip compressed data, was "dist\vgis_utils-1.0.4.tar", last modified: Thu Jul  6 02:12:37 2023, max compression
```

## Comparing `vgis_utils-1.0.3.tar` & `vgis_utils-1.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 08:48:40.005745 vgis_utils-1.0.3/
--rw-rw-rw-   0        0        0     1034 2023-06-27 08:48:40.004746 vgis_utils-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-06-27 08:16:30.000000 vgis_utils-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 08:48:40.005745 vgis_utils-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2174 2023-06-27 08:42:14.000000 vgis_utils-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.964749 vgis_utils-1.0.3/vgis_utils/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.3/vgis_utils/__init__.py
--rw-rw-rw-   0        0        0     1423 2023-06-27 07:36:52.000000 vgis_utils-1.0.3/vgis_utils/commonTools.py
--rw-rw-rw-   0        0        0      985 2023-06-27 06:28:07.000000 vgis_utils-1.0.3/vgis_utils/iteratorTools.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.977748 vgis_utils-1.0.3/vgis_utils/vgis_datetime/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.3/vgis_utils/vgis_datetime/__init__.py
--rw-rw-rw-   0        0        0     7416 2023-06-27 07:32:12.000000 vgis_utils-1.0.3/vgis_utils/vgis_datetime/datetimeTools.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.980747 vgis_utils-1.0.3/vgis_utils/vgis_file/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.3/vgis_utils/vgis_file/__init__.py
--rw-rw-rw-   0        0        0     8353 2023-06-27 08:29:36.000000 vgis_utils-1.0.3/vgis_utils/vgis_file/fileTools.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.983747 vgis_utils-1.0.3/vgis_utils/vgis_http/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.3/vgis_utils/vgis_http/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-06-27 06:17:10.000000 vgis_utils-1.0.3/vgis_utils/vgis_http/httpTools.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.986746 vgis_utils-1.0.3/vgis_utils/vgis_image/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.3/vgis_utils/vgis_image/__init__.py
--rw-rw-rw-   0        0        0     4672 2023-06-27 08:29:35.000000 vgis_utils-1.0.3/vgis_utils/vgis_image/imageTools.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.991748 vgis_utils-1.0.3/vgis_utils/vgis_list/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.3/vgis_utils/vgis_list/__init__.py
--rw-rw-rw-   0        0        0     2498 2023-06-27 06:37:50.000000 vgis_utils-1.0.3/vgis_utils/vgis_list/listTools.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.995772 vgis_utils-1.0.3/vgis_utils/vgis_money/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.3/vgis_utils/vgis_money/__init__.py
--rw-rw-rw-   0        0        0    13669 2023-06-27 08:26:45.000000 vgis_utils-1.0.3/vgis_utils/vgis_money/moneyTools.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.998772 vgis_utils-1.0.3/vgis_utils/vgis_string/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.3/vgis_utils/vgis_string/__init__.py
--rw-rw-rw-   0        0        0     1436 2023-06-27 06:19:39.000000 vgis_utils-1.0.3/vgis_utils/vgis_string/stringTools.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:48:40.002767 vgis_utils-1.0.3/vgis_utils/vgis_video/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.3/vgis_utils/vgis_video/__init__.py
--rw-rw-rw-   0        0        0    10161 2023-06-27 08:48:22.000000 vgis_utils-1.0.3/vgis_utils/vgis_video/videoTools.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:48:39.973749 vgis_utils-1.0.3/vgis_utils.egg-info/
--rw-rw-rw-   0        0        0     1034 2023-06-27 08:48:39.000000 vgis_utils-1.0.3/vgis_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      827 2023-06-27 08:48:39.000000 vgis_utils-1.0.3/vgis_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 08:48:39.000000 vgis_utils-1.0.3/vgis_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-27 08:48:39.000000 vgis_utils-1.0.3/vgis_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-27 08:48:39.000000 vgis_utils-1.0.3/vgis_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.660843 vgis_utils-1.0.4/
+-rw-rw-rw-   0        0        0     1034 2023-07-06 02:12:37.660843 vgis_utils-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-06-27 08:16:30.000000 vgis_utils-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 02:12:37.660843 vgis_utils-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2188 2023-07-06 02:10:46.000000 vgis_utils-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.618844 vgis_utils-1.0.4/vgis_utils/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.4/vgis_utils/__init__.py
+-rw-rw-rw-   0        0        0     1423 2023-06-27 07:36:52.000000 vgis_utils-1.0.4/vgis_utils/commonTools.py
+-rw-rw-rw-   0        0        0      985 2023-06-27 06:28:07.000000 vgis_utils-1.0.4/vgis_utils/iteratorTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.631845 vgis_utils-1.0.4/vgis_utils/vgis_datetime/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.4/vgis_utils/vgis_datetime/__init__.py
+-rw-rw-rw-   0        0        0     7455 2023-07-06 02:03:14.000000 vgis_utils-1.0.4/vgis_utils/vgis_datetime/datetimeTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.634843 vgis_utils-1.0.4/vgis_utils/vgis_file/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.4/vgis_utils/vgis_file/__init__.py
+-rw-rw-rw-   0        0        0     8364 2023-07-06 02:09:51.000000 vgis_utils-1.0.4/vgis_utils/vgis_file/fileTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.638844 vgis_utils-1.0.4/vgis_utils/vgis_http/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.4/vgis_utils/vgis_http/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-06-27 06:17:10.000000 vgis_utils-1.0.4/vgis_utils/vgis_http/httpTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.643846 vgis_utils-1.0.4/vgis_utils/vgis_image/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.4/vgis_utils/vgis_image/__init__.py
+-rw-rw-rw-   0        0        0     4672 2023-06-27 08:29:35.000000 vgis_utils-1.0.4/vgis_utils/vgis_image/imageTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.647845 vgis_utils-1.0.4/vgis_utils/vgis_list/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.4/vgis_utils/vgis_list/__init__.py
+-rw-rw-rw-   0        0        0     2498 2023-06-27 06:37:50.000000 vgis_utils-1.0.4/vgis_utils/vgis_list/listTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.651845 vgis_utils-1.0.4/vgis_utils/vgis_money/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.4/vgis_utils/vgis_money/__init__.py
+-rw-rw-rw-   0        0        0    13680 2023-07-06 02:10:11.000000 vgis_utils-1.0.4/vgis_utils/vgis_money/moneyTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.654845 vgis_utils-1.0.4/vgis_utils/vgis_string/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.4/vgis_utils/vgis_string/__init__.py
+-rw-rw-rw-   0        0        0     2077 2023-07-05 05:40:47.000000 vgis_utils-1.0.4/vgis_utils/vgis_string/stringTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.658843 vgis_utils-1.0.4/vgis_utils/vgis_video/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.4/vgis_utils/vgis_video/__init__.py
+-rw-rw-rw-   0        0        0    10161 2023-06-27 08:48:22.000000 vgis_utils-1.0.4/vgis_utils/vgis_video/videoTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.628845 vgis_utils-1.0.4/vgis_utils.egg-info/
+-rw-rw-rw-   0        0        0     1034 2023-07-06 02:12:37.000000 vgis_utils-1.0.4/vgis_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      827 2023-07-06 02:12:37.000000 vgis_utils-1.0.4/vgis_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 02:12:37.000000 vgis_utils-1.0.4/vgis_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-06 02:12:37.000000 vgis_utils-1.0.4/vgis_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-06 02:12:37.000000 vgis_utils-1.0.4/vgis_utils.egg-info/top_level.txt
```

### Comparing `vgis_utils-1.0.3/PKG-INFO` & `vgis_utils-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis_utils
-Version: 1.0.3
+Version: 1.0.4
 Summary: A libary for common operator
 Home-page: https://github.com/gisfanmachel/vgisUtils
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis common lib
```

### Comparing `vgis_utils-1.0.3/setup.py` & `vgis_utils-1.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     name="vgis_utils",  # Required 项目名称
-    version="1.0.3",  # Required 发布版本号
+    version="1.0.4",  # Required 发布版本号
     description="A libary for common operator",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/vgisUtils",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
@@ -48,10 +48,10 @@
 
     keywords="utils,setuptools,development",  # Optional 搜索关键字
 
     packages=find_packages(),  # Required
 
     python_requires=">=3.7, <4",  # python 版本要求
 
-    install_requires=["opencv-python","Pillow","numpy"],  # Optional 第三方依赖库
+    install_requires=["opencv-python", "Pillow", "numpy", "loguru"],  # Optional 第三方依赖库
 
-)
+)
```

### Comparing `vgis_utils-1.0.3/vgis_utils/commonTools.py` & `vgis_utils-1.0.4/vgis_utils/commonTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.3/vgis_utils/iteratorTools.py` & `vgis_utils-1.0.4/vgis_utils/iteratorTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.3/vgis_utils/vgis_datetime/datetimeTools.py` & `vgis_utils-1.0.4/vgis_utils/vgis_datetime/datetimeTools.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 @Description: 
 @ Software: PyCharm
 ===================================
 """
 import datetime
 import re
 
-from commonTools import CommonHelper
+# 需要引用最顶层的
+from vgis_utils.commonTools import CommonHelper
 
 
 class DateTimeHelper:
     def __init__(self):
         pass
 
     @staticmethod
```

### Comparing `vgis_utils-1.0.3/vgis_utils/vgis_file/fileTools.py` & `vgis_utils-1.0.4/vgis_utils/vgis_file/fileTools.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ===================================
 """
 import json
 import os
 import shutil
 import zipfile
 
-from commonTools import CommonHelper
+from vgis_utils.commonTools import CommonHelper
 
 
 class FileHelper:
     # 初始化
     def __init__(self):
         pass
```

### Comparing `vgis_utils-1.0.3/vgis_utils/vgis_http/httpTools.py` & `vgis_utils-1.0.4/vgis_utils/vgis_http/httpTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.3/vgis_utils/vgis_image/imageTools.py` & `vgis_utils-1.0.4/vgis_utils/vgis_image/imageTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.3/vgis_utils/vgis_list/listTools.py` & `vgis_utils-1.0.4/vgis_utils/vgis_list/listTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.3/vgis_utils/vgis_money/moneyTools.py` & `vgis_utils-1.0.4/vgis_utils/vgis_money/moneyTools.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # @File    : moneyTools.py
 # @Descr   : 
 # @Software: PyCharm
 import re
 
 import requests
 
-from vgis_string.stringTools import StringHelper
+from vgis_utils.vgis_string.stringTools import StringHelper
 
 
 class MoneyHelper:
     def __int__(self):
         pass
 
     @staticmethod
```

### Comparing `vgis_utils-1.0.3/vgis_utils/vgis_string/stringTools.py` & `vgis_utils-1.0.4/vgis_utils/vgis_string/stringTools.py`

 * *Files 26% similar despite different names*

```diff
@@ -42,12 +42,27 @@
     def get_cn_in_str(input_str):
         str_result = re.findall("[\u4e00-\u9fa5]", input_str)
         str_return = ""
         for one in str_result:
             str_return = str_return + one
         return str_return
 
-    # 获取两个字符串中间的字符串
+
     @staticmethod
+    # 获取两个字符串中间的字符串
     def get_str_btw(s, f, b):
         par = s.partition(f)
-        return (par[2].partition(b))[0][:]
+        return (par[2].partition(b))[0][:]
+
+    @staticmethod
+    # 去掉字符串里的\x开头的特殊字符
+    def handle_x_str(content):
+        # 使用unicode-escape编码集，将unicode内存编码值直接存储，并替换空白字符
+        content = content.encode('unicode_escape').decode('utf-8').replace(' ', '')
+        # 利用正则匹配\x开头的特殊字符
+        result = re.findall(r'\\x[a-f0-9]{2}', content)
+        for x in result:
+            # 替换找的的特殊字符
+            content = content.replace(x, '')
+        # 最后再解码
+        content = content.encode('utf-8').decode('unicode_escape')
+        return content
```

### Comparing `vgis_utils-1.0.3/vgis_utils/vgis_video/videoTools.py` & `vgis_utils-1.0.4/vgis_utils/vgis_video/videoTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.3/vgis_utils.egg-info/PKG-INFO` & `vgis_utils-1.0.4/vgis_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis-utils
-Version: 1.0.3
+Version: 1.0.4
 Summary: A libary for common operator
 Home-page: https://github.com/gisfanmachel/vgisUtils
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis common lib
```

### Comparing `vgis_utils-1.0.3/vgis_utils.egg-info/SOURCES.txt` & `vgis_utils-1.0.4/vgis_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

