# Comparing `tmp/vgis_utils-1.0.6.tar.gz` & `tmp/vgis_utils-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgis_utils-1.0.6.tar", last modified: Thu Jul  6 04:14:07 2023, max compression
+gzip compressed data, was "dist\vgis_utils-1.0.7.tar", last modified: Thu Jul  6 06:59:58 2023, max compression
```

## Comparing `vgis_utils-1.0.6.tar` & `vgis_utils-1.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 04:14:07.900315 vgis_utils-1.0.6/
--rw-rw-rw-   0        0        0     1034 2023-07-06 04:14:07.898312 vgis_utils-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 04:14:07.900315 vgis_utils-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2188 2023-07-06 04:13:15.000000 vgis_utils-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:14:07.731312 vgis_utils-1.0.6/vgis_utils/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/__init__.py
--rw-rw-rw-   0        0        0     1423 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/commonTools.py
--rw-rw-rw-   0        0        0      985 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/iteratorTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:14:07.770312 vgis_utils-1.0.6/vgis_utils/vgis_datetime/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/vgis_datetime/__init__.py
--rw-rw-rw-   0        0        0     8230 2023-07-06 04:11:27.000000 vgis_utils-1.0.6/vgis_utils/vgis_datetime/datetimeTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:14:07.787314 vgis_utils-1.0.6/vgis_utils/vgis_file/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/vgis_file/__init__.py
--rw-rw-rw-   0        0        0     8364 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/vgis_file/fileTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:14:07.805315 vgis_utils-1.0.6/vgis_utils/vgis_http/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/vgis_http/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/vgis_http/httpTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:14:07.823318 vgis_utils-1.0.6/vgis_utils/vgis_image/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/vgis_image/__init__.py
--rw-rw-rw-   0        0        0     4672 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/vgis_image/imageTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:14:07.840314 vgis_utils-1.0.6/vgis_utils/vgis_list/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/vgis_list/__init__.py
--rw-rw-rw-   0        0        0     2498 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/vgis_list/listTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:14:07.856329 vgis_utils-1.0.6/vgis_utils/vgis_money/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/vgis_money/__init__.py
--rw-rw-rw-   0        0        0    13680 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/vgis_money/moneyTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:14:07.872315 vgis_utils-1.0.6/vgis_utils/vgis_string/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/vgis_string/__init__.py
--rw-rw-rw-   0        0        0     2599 2023-07-06 04:09:42.000000 vgis_utils-1.0.6/vgis_utils/vgis_string/stringTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:14:07.889316 vgis_utils-1.0.6/vgis_utils/vgis_video/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/vgis_video/__init__.py
--rw-rw-rw-   0        0        0    10161 2023-07-06 02:41:01.000000 vgis_utils-1.0.6/vgis_utils/vgis_video/videoTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:14:07.758316 vgis_utils-1.0.6/vgis_utils.egg-info/
--rw-rw-rw-   0        0        0     1034 2023-07-06 04:14:07.000000 vgis_utils-1.0.6/vgis_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      827 2023-07-06 04:14:07.000000 vgis_utils-1.0.6/vgis_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 04:14:07.000000 vgis_utils-1.0.6/vgis_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-06 04:14:07.000000 vgis_utils-1.0.6/vgis_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-06 04:14:07.000000 vgis_utils-1.0.6/vgis_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.666406 vgis_utils-1.0.7/
+-rw-rw-rw-   0        0        0     1034 2023-07-06 06:59:58.664404 vgis_utils-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 06:59:58.667405 vgis_utils-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2188 2023-07-06 06:59:27.000000 vgis_utils-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.319407 vgis_utils-1.0.7/vgis_utils/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/__init__.py
+-rw-rw-rw-   0        0        0     1423 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/commonTools.py
+-rw-rw-rw-   0        0        0      985 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/iteratorTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.368407 vgis_utils-1.0.7/vgis_utils/vgis_datetime/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_datetime/__init__.py
+-rw-rw-rw-   0        0        0     8245 2023-07-06 06:58:50.000000 vgis_utils-1.0.7/vgis_utils/vgis_datetime/datetimeTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.459405 vgis_utils-1.0.7/vgis_utils/vgis_file/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_file/__init__.py
+-rw-rw-rw-   0        0        0     8364 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_file/fileTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.506409 vgis_utils-1.0.7/vgis_utils/vgis_http/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_http/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_http/httpTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.529407 vgis_utils-1.0.7/vgis_utils/vgis_image/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_image/__init__.py
+-rw-rw-rw-   0        0        0     4672 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_image/imageTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.554404 vgis_utils-1.0.7/vgis_utils/vgis_list/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_list/__init__.py
+-rw-rw-rw-   0        0        0     2498 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_list/listTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.574406 vgis_utils-1.0.7/vgis_utils/vgis_money/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_money/__init__.py
+-rw-rw-rw-   0        0        0    13680 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_money/moneyTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.602407 vgis_utils-1.0.7/vgis_utils/vgis_string/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_string/__init__.py
+-rw-rw-rw-   0        0        0     2599 2023-07-06 04:09:42.000000 vgis_utils-1.0.7/vgis_utils/vgis_string/stringTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.654404 vgis_utils-1.0.7/vgis_utils/vgis_video/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_video/__init__.py
+-rw-rw-rw-   0        0        0    10161 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_video/videoTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.351405 vgis_utils-1.0.7/vgis_utils.egg-info/
+-rw-rw-rw-   0        0        0     1034 2023-07-06 06:59:58.000000 vgis_utils-1.0.7/vgis_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      827 2023-07-06 06:59:58.000000 vgis_utils-1.0.7/vgis_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 06:59:58.000000 vgis_utils-1.0.7/vgis_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-06 06:59:58.000000 vgis_utils-1.0.7/vgis_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-06 06:59:58.000000 vgis_utils-1.0.7/vgis_utils.egg-info/top_level.txt
```

### Comparing `vgis_utils-1.0.6/PKG-INFO` & `vgis_utils-1.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis_utils
-Version: 1.0.6
+Version: 1.0.7
 Summary: A libary for common operator
 Home-page: https://github.com/gisfanmachel/vgisUtils
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis common lib
```

### Comparing `vgis_utils-1.0.6/setup.py` & `vgis_utils-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     name="vgis_utils",  # Required 项目名称
-    version="1.0.6",  # Required 发布版本号
+    version="1.0.7",  # Required 发布版本号
     description="A libary for common operator",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/vgisUtils",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
```

### Comparing `vgis_utils-1.0.6/vgis_utils/commonTools.py` & `vgis_utils-1.0.7/vgis_utils/commonTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.6/vgis_utils/iteratorTools.py` & `vgis_utils-1.0.7/vgis_utils/iteratorTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.6/vgis_utils/vgis_datetime/datetimeTools.py` & `vgis_utils-1.0.7/vgis_utils/vgis_datetime/datetimeTools.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,19 +58,19 @@
         return info_time
 
     @staticmethod
     # 将秒数转换为时分秒
     def convert_seconds(seconds):
         m, s = divmod(seconds, 60)
         h, m = divmod(m, 60)
-        result = "{}秒".format(s)
+        result = "{}秒".format(int(s))
         if m > 0:
-            result = "{}分".format(m) + result
+            result = "{}分".format(int(m)) + result
         if h > 0:
-            result = "{}时".format(m) + result
+            result = "{}时".format(int(m)) + result
         # print("程序总共耗时%02d:%02d:%02d" % (h, m, s))
         return result
 
 
 
     @staticmethod
     # 将识别字符如2月23日转换为2023-02-27,年份默认用当年
```

### Comparing `vgis_utils-1.0.6/vgis_utils/vgis_file/fileTools.py` & `vgis_utils-1.0.7/vgis_utils/vgis_file/fileTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.6/vgis_utils/vgis_http/httpTools.py` & `vgis_utils-1.0.7/vgis_utils/vgis_http/httpTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.6/vgis_utils/vgis_image/imageTools.py` & `vgis_utils-1.0.7/vgis_utils/vgis_image/imageTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.6/vgis_utils/vgis_list/listTools.py` & `vgis_utils-1.0.7/vgis_utils/vgis_list/listTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.6/vgis_utils/vgis_money/moneyTools.py` & `vgis_utils-1.0.7/vgis_utils/vgis_money/moneyTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.6/vgis_utils/vgis_string/stringTools.py` & `vgis_utils-1.0.7/vgis_utils/vgis_string/stringTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.6/vgis_utils/vgis_video/videoTools.py` & `vgis_utils-1.0.7/vgis_utils/vgis_video/videoTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.6/vgis_utils.egg-info/PKG-INFO` & `vgis_utils-1.0.7/vgis_utils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis-utils
-Version: 1.0.6
+Version: 1.0.7
 Summary: A libary for common operator
 Home-page: https://github.com/gisfanmachel/vgisUtils
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis common lib
```

### Comparing `vgis_utils-1.0.6/vgis_utils.egg-info/SOURCES.txt` & `vgis_utils-1.0.7/vgis_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

