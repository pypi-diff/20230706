# Comparing `tmp/vgis_utils-1.0.4.tar.gz` & `tmp/vgis_utils-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgis_utils-1.0.4.tar", last modified: Thu Jul  6 02:12:37 2023, max compression
+gzip compressed data, was "dist\vgis_utils-1.0.5.tar", last modified: Thu Jul  6 03:48:08 2023, max compression
```

## Comparing `vgis_utils-1.0.4.tar` & `vgis_utils-1.0.5.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.660843 vgis_utils-1.0.4/
--rw-rw-rw-   0        0        0     1034 2023-07-06 02:12:37.660843 vgis_utils-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-06-27 08:16:30.000000 vgis_utils-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 02:12:37.660843 vgis_utils-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2188 2023-07-06 02:10:46.000000 vgis_utils-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.618844 vgis_utils-1.0.4/vgis_utils/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.4/vgis_utils/__init__.py
--rw-rw-rw-   0        0        0     1423 2023-06-27 07:36:52.000000 vgis_utils-1.0.4/vgis_utils/commonTools.py
--rw-rw-rw-   0        0        0      985 2023-06-27 06:28:07.000000 vgis_utils-1.0.4/vgis_utils/iteratorTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.631845 vgis_utils-1.0.4/vgis_utils/vgis_datetime/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.4/vgis_utils/vgis_datetime/__init__.py
--rw-rw-rw-   0        0        0     7455 2023-07-06 02:03:14.000000 vgis_utils-1.0.4/vgis_utils/vgis_datetime/datetimeTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.634843 vgis_utils-1.0.4/vgis_utils/vgis_file/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.4/vgis_utils/vgis_file/__init__.py
--rw-rw-rw-   0        0        0     8364 2023-07-06 02:09:51.000000 vgis_utils-1.0.4/vgis_utils/vgis_file/fileTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.638844 vgis_utils-1.0.4/vgis_utils/vgis_http/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.4/vgis_utils/vgis_http/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-06-27 06:17:10.000000 vgis_utils-1.0.4/vgis_utils/vgis_http/httpTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.643846 vgis_utils-1.0.4/vgis_utils/vgis_image/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.4/vgis_utils/vgis_image/__init__.py
--rw-rw-rw-   0        0        0     4672 2023-06-27 08:29:35.000000 vgis_utils-1.0.4/vgis_utils/vgis_image/imageTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.647845 vgis_utils-1.0.4/vgis_utils/vgis_list/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.4/vgis_utils/vgis_list/__init__.py
--rw-rw-rw-   0        0        0     2498 2023-06-27 06:37:50.000000 vgis_utils-1.0.4/vgis_utils/vgis_list/listTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.651845 vgis_utils-1.0.4/vgis_utils/vgis_money/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.4/vgis_utils/vgis_money/__init__.py
--rw-rw-rw-   0        0        0    13680 2023-07-06 02:10:11.000000 vgis_utils-1.0.4/vgis_utils/vgis_money/moneyTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.654845 vgis_utils-1.0.4/vgis_utils/vgis_string/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.4/vgis_utils/vgis_string/__init__.py
--rw-rw-rw-   0        0        0     2077 2023-07-05 05:40:47.000000 vgis_utils-1.0.4/vgis_utils/vgis_string/stringTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.658843 vgis_utils-1.0.4/vgis_utils/vgis_video/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.4/vgis_utils/vgis_video/__init__.py
--rw-rw-rw-   0        0        0    10161 2023-06-27 08:48:22.000000 vgis_utils-1.0.4/vgis_utils/vgis_video/videoTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:12:37.628845 vgis_utils-1.0.4/vgis_utils.egg-info/
--rw-rw-rw-   0        0        0     1034 2023-07-06 02:12:37.000000 vgis_utils-1.0.4/vgis_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      827 2023-07-06 02:12:37.000000 vgis_utils-1.0.4/vgis_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 02:12:37.000000 vgis_utils-1.0.4/vgis_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-06 02:12:37.000000 vgis_utils-1.0.4/vgis_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-06 02:12:37.000000 vgis_utils-1.0.4/vgis_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 03:48:08.027413 vgis_utils-1.0.5/
+-rw-rw-rw-   0        0        0     1034 2023-07-06 03:48:08.024412 vgis_utils-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 03:48:08.027413 vgis_utils-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2188 2023-07-06 03:43:35.000000 vgis_utils-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:48:06.943416 vgis_utils-1.0.5/vgis_utils/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/__init__.py
+-rw-rw-rw-   0        0        0     1423 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/commonTools.py
+-rw-rw-rw-   0        0        0      985 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/iteratorTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:48:07.097413 vgis_utils-1.0.5/vgis_utils/vgis_datetime/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/vgis_datetime/__init__.py
+-rw-rw-rw-   0        0        0     8186 2023-07-06 03:43:12.000000 vgis_utils-1.0.5/vgis_utils/vgis_datetime/datetimeTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:48:07.231413 vgis_utils-1.0.5/vgis_utils/vgis_file/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/vgis_file/__init__.py
+-rw-rw-rw-   0        0        0     8364 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/vgis_file/fileTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:48:07.370411 vgis_utils-1.0.5/vgis_utils/vgis_http/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/vgis_http/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/vgis_http/httpTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:48:07.501412 vgis_utils-1.0.5/vgis_utils/vgis_image/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/vgis_image/__init__.py
+-rw-rw-rw-   0        0        0     4672 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/vgis_image/imageTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:48:07.634413 vgis_utils-1.0.5/vgis_utils/vgis_list/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/vgis_list/__init__.py
+-rw-rw-rw-   0        0        0     2498 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/vgis_list/listTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:48:07.770413 vgis_utils-1.0.5/vgis_utils/vgis_money/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/vgis_money/__init__.py
+-rw-rw-rw-   0        0        0    13680 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/vgis_money/moneyTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:48:07.835412 vgis_utils-1.0.5/vgis_utils/vgis_string/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/vgis_string/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:48:07.957414 vgis_utils-1.0.5/vgis_utils/vgis_video/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/vgis_video/__init__.py
+-rw-rw-rw-   0        0        0    10161 2023-07-06 02:41:01.000000 vgis_utils-1.0.5/vgis_utils/vgis_video/videoTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:48:07.026414 vgis_utils-1.0.5/vgis_utils.egg-info/
+-rw-rw-rw-   0        0        0     1034 2023-07-06 03:48:06.000000 vgis_utils-1.0.5/vgis_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      789 2023-07-06 03:48:06.000000 vgis_utils-1.0.5/vgis_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 03:48:06.000000 vgis_utils-1.0.5/vgis_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-06 03:48:06.000000 vgis_utils-1.0.5/vgis_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-06 03:48:06.000000 vgis_utils-1.0.5/vgis_utils.egg-info/top_level.txt
```

### Comparing `vgis_utils-1.0.4/PKG-INFO` & `vgis_utils-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis_utils
-Version: 1.0.4
+Version: 1.0.5
 Summary: A libary for common operator
 Home-page: https://github.com/gisfanmachel/vgisUtils
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis common lib
```

### Comparing `vgis_utils-1.0.4/setup.py` & `vgis_utils-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     name="vgis_utils",  # Required 项目名称
-    version="1.0.4",  # Required 发布版本号
+    version="1.0.5",  # Required 发布版本号
     description="A libary for common operator",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/vgisUtils",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
```

### Comparing `vgis_utils-1.0.4/vgis_utils/commonTools.py` & `vgis_utils-1.0.5/vgis_utils/commonTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.4/vgis_utils/iteratorTools.py` & `vgis_utils-1.0.5/vgis_utils/iteratorTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.4/vgis_utils/vgis_datetime/datetimeTools.py` & `vgis_utils-1.0.5/vgis_utils/vgis_datetime/datetimeTools.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @Date: Create in 2021/1/25 16:36
 @Description: 
 @ Software: PyCharm
 ===================================
 """
 import datetime
 import re
-
+import time
 # 需要引用最顶层的
 from vgis_utils.commonTools import CommonHelper
 
 
 class DateTimeHelper:
     def __init__(self):
         pass
@@ -187,8 +187,26 @@
         # print(is_date_type)
 
         return is_date_type
 
     @staticmethod
     # 根据时间戳（到毫秒）获取uuid
     def get_uuid():
-        return datetime.datetime.now().strftime('%Y%m%d%H%M%S%f')
+        return datetime.datetime.now().strftime('%Y%m%d%H%M%S%f')
+
+    @staticmethod
+    # 字符串转换为时间数字
+    def string2time_stamp(str_value):
+
+        try:
+            d = datetime.datetime.strptime(str_value, "%Y-%m-%d %H:%M:%S.%f")
+            t = d.timetuple()
+            time_stamp = int(time.mktime(t))
+            time_stamp = float(str(time_stamp) + str("%06d" % d.microsecond)) / 1000000
+            return time_stamp
+        except ValueError as e:
+            print(e)
+            d = datetime.datetime.strptime(str_value, "%Y-%m-%d %H:%M:%S")
+            t = d.timetuple()
+            time_stamp = int(time.mktime(t))
+            time_stamp = float(str(time_stamp) + str("%06d" % d.microsecond)) / 1000000
+            return time_stamp
```

### Comparing `vgis_utils-1.0.4/vgis_utils/vgis_file/fileTools.py` & `vgis_utils-1.0.5/vgis_utils/vgis_file/fileTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.4/vgis_utils/vgis_http/httpTools.py` & `vgis_utils-1.0.5/vgis_utils/vgis_http/httpTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.4/vgis_utils/vgis_image/imageTools.py` & `vgis_utils-1.0.5/vgis_utils/vgis_image/imageTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.4/vgis_utils/vgis_list/listTools.py` & `vgis_utils-1.0.5/vgis_utils/vgis_list/listTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.4/vgis_utils/vgis_money/moneyTools.py` & `vgis_utils-1.0.5/vgis_utils/vgis_money/moneyTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.4/vgis_utils/vgis_video/videoTools.py` & `vgis_utils-1.0.5/vgis_utils/vgis_video/videoTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.4/vgis_utils.egg-info/PKG-INFO` & `vgis_utils-1.0.5/vgis_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis-utils
-Version: 1.0.4
+Version: 1.0.5
 Summary: A libary for common operator
 Home-page: https://github.com/gisfanmachel/vgisUtils
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis common lib
```

### Comparing `vgis_utils-1.0.4/vgis_utils.egg-info/SOURCES.txt` & `vgis_utils-1.0.5/vgis_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,10 +17,9 @@
 vgis_utils/vgis_image/__init__.py
 vgis_utils/vgis_image/imageTools.py
 vgis_utils/vgis_list/__init__.py
 vgis_utils/vgis_list/listTools.py
 vgis_utils/vgis_money/__init__.py
 vgis_utils/vgis_money/moneyTools.py
 vgis_utils/vgis_string/__init__.py
-vgis_utils/vgis_string/stringTools.py
 vgis_utils/vgis_video/__init__.py
 vgis_utils/vgis_video/videoTools.py
```

