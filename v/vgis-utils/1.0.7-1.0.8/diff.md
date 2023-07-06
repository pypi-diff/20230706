# Comparing `tmp/vgis_utils-1.0.7.tar.gz` & `tmp/vgis_utils-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgis_utils-1.0.7.tar", last modified: Thu Jul  6 06:59:58 2023, max compression
+gzip compressed data, was "dist\vgis_utils-1.0.8.tar", last modified: Thu Jul  6 07:12:14 2023, max compression
```

## Comparing `vgis_utils-1.0.7.tar` & `vgis_utils-1.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.666406 vgis_utils-1.0.7/
--rw-rw-rw-   0        0        0     1034 2023-07-06 06:59:58.664404 vgis_utils-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 06:59:58.667405 vgis_utils-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2188 2023-07-06 06:59:27.000000 vgis_utils-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.319407 vgis_utils-1.0.7/vgis_utils/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/__init__.py
--rw-rw-rw-   0        0        0     1423 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/commonTools.py
--rw-rw-rw-   0        0        0      985 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/iteratorTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.368407 vgis_utils-1.0.7/vgis_utils/vgis_datetime/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_datetime/__init__.py
--rw-rw-rw-   0        0        0     8245 2023-07-06 06:58:50.000000 vgis_utils-1.0.7/vgis_utils/vgis_datetime/datetimeTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.459405 vgis_utils-1.0.7/vgis_utils/vgis_file/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_file/__init__.py
--rw-rw-rw-   0        0        0     8364 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_file/fileTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.506409 vgis_utils-1.0.7/vgis_utils/vgis_http/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_http/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_http/httpTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.529407 vgis_utils-1.0.7/vgis_utils/vgis_image/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_image/__init__.py
--rw-rw-rw-   0        0        0     4672 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_image/imageTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.554404 vgis_utils-1.0.7/vgis_utils/vgis_list/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_list/__init__.py
--rw-rw-rw-   0        0        0     2498 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_list/listTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.574406 vgis_utils-1.0.7/vgis_utils/vgis_money/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_money/__init__.py
--rw-rw-rw-   0        0        0    13680 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_money/moneyTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.602407 vgis_utils-1.0.7/vgis_utils/vgis_string/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_string/__init__.py
--rw-rw-rw-   0        0        0     2599 2023-07-06 04:09:42.000000 vgis_utils-1.0.7/vgis_utils/vgis_string/stringTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.654404 vgis_utils-1.0.7/vgis_utils/vgis_video/
--rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_video/__init__.py
--rw-rw-rw-   0        0        0    10161 2023-07-06 02:41:01.000000 vgis_utils-1.0.7/vgis_utils/vgis_video/videoTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:59:58.351405 vgis_utils-1.0.7/vgis_utils.egg-info/
--rw-rw-rw-   0        0        0     1034 2023-07-06 06:59:58.000000 vgis_utils-1.0.7/vgis_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      827 2023-07-06 06:59:58.000000 vgis_utils-1.0.7/vgis_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 06:59:58.000000 vgis_utils-1.0.7/vgis_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-06 06:59:58.000000 vgis_utils-1.0.7/vgis_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-06 06:59:58.000000 vgis_utils-1.0.7/vgis_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.495675 vgis_utils-1.0.8/
+-rw-rw-rw-   0        0        0     1034 2023-07-06 07:12:14.494671 vgis_utils-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-06-27 08:16:30.000000 vgis_utils-1.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 07:12:14.495675 vgis_utils-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2200 2023-07-06 07:10:53.000000 vgis_utils-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.462638 vgis_utils-1.0.8/vgis_utils/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.8/vgis_utils/__init__.py
+-rw-rw-rw-   0        0        0     1423 2023-06-27 07:36:52.000000 vgis_utils-1.0.8/vgis_utils/commonTools.py
+-rw-rw-rw-   0        0        0      985 2023-06-27 06:28:07.000000 vgis_utils-1.0.8/vgis_utils/iteratorTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.473639 vgis_utils-1.0.8/vgis_utils/vgis_datetime/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.8/vgis_utils/vgis_datetime/__init__.py
+-rw-rw-rw-   0        0        0     8245 2023-07-06 07:08:32.000000 vgis_utils-1.0.8/vgis_utils/vgis_datetime/datetimeTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.475650 vgis_utils-1.0.8/vgis_utils/vgis_file/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.8/vgis_utils/vgis_file/__init__.py
+-rw-rw-rw-   0        0        0     8364 2023-07-06 02:09:51.000000 vgis_utils-1.0.8/vgis_utils/vgis_file/fileTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.478639 vgis_utils-1.0.8/vgis_utils/vgis_http/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.8/vgis_utils/vgis_http/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-06-27 06:17:10.000000 vgis_utils-1.0.8/vgis_utils/vgis_http/httpTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.481639 vgis_utils-1.0.8/vgis_utils/vgis_image/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.8/vgis_utils/vgis_image/__init__.py
+-rw-rw-rw-   0        0        0     4672 2023-06-27 08:29:35.000000 vgis_utils-1.0.8/vgis_utils/vgis_image/imageTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.484638 vgis_utils-1.0.8/vgis_utils/vgis_list/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.8/vgis_utils/vgis_list/__init__.py
+-rw-rw-rw-   0        0        0     2498 2023-06-27 06:37:50.000000 vgis_utils-1.0.8/vgis_utils/vgis_list/listTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.487638 vgis_utils-1.0.8/vgis_utils/vgis_money/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.8/vgis_utils/vgis_money/__init__.py
+-rw-rw-rw-   0        0        0    13680 2023-07-06 02:10:11.000000 vgis_utils-1.0.8/vgis_utils/vgis_money/moneyTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.490665 vgis_utils-1.0.8/vgis_utils/vgis_string/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.8/vgis_utils/vgis_string/__init__.py
+-rw-rw-rw-   0        0        0     3238 2023-07-06 07:09:21.000000 vgis_utils-1.0.8/vgis_utils/vgis_string/stringTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.493640 vgis_utils-1.0.8/vgis_utils/vgis_video/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.8/vgis_utils/vgis_video/__init__.py
+-rw-rw-rw-   0        0        0    10161 2023-06-27 08:48:22.000000 vgis_utils-1.0.8/vgis_utils/vgis_video/videoTools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.470640 vgis_utils-1.0.8/vgis_utils.egg-info/
+-rw-rw-rw-   0        0        0     1034 2023-07-06 07:12:14.000000 vgis_utils-1.0.8/vgis_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      827 2023-07-06 07:12:14.000000 vgis_utils-1.0.8/vgis_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 07:12:14.000000 vgis_utils-1.0.8/vgis_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-07-06 07:12:14.000000 vgis_utils-1.0.8/vgis_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-06 07:12:14.000000 vgis_utils-1.0.8/vgis_utils.egg-info/top_level.txt
```

### Comparing `vgis_utils-1.0.7/PKG-INFO` & `vgis_utils-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis_utils
-Version: 1.0.7
+Version: 1.0.8
 Summary: A libary for common operator
 Home-page: https://github.com/gisfanmachel/vgisUtils
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis common lib
```

### Comparing `vgis_utils-1.0.7/setup.py` & `vgis_utils-1.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     name="vgis_utils",  # Required 项目名称
-    version="1.0.7",  # Required 发布版本号
+    version="1.0.8",  # Required 发布版本号
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
 
-    install_requires=["opencv-python", "Pillow", "numpy", "loguru"],  # Optional 第三方依赖库
+    install_requires=["opencv-python", "Pillow", "numpy", "loguru", "pypinyin"],  # Optional 第三方依赖库
 
 )
```

### Comparing `vgis_utils-1.0.7/vgis_utils/commonTools.py` & `vgis_utils-1.0.8/vgis_utils/commonTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.7/vgis_utils/iteratorTools.py` & `vgis_utils-1.0.8/vgis_utils/iteratorTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.7/vgis_utils/vgis_datetime/datetimeTools.py` & `vgis_utils-1.0.8/vgis_utils/vgis_datetime/datetimeTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.7/vgis_utils/vgis_file/fileTools.py` & `vgis_utils-1.0.8/vgis_utils/vgis_file/fileTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.7/vgis_utils/vgis_http/httpTools.py` & `vgis_utils-1.0.8/vgis_utils/vgis_http/httpTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.7/vgis_utils/vgis_image/imageTools.py` & `vgis_utils-1.0.8/vgis_utils/vgis_image/imageTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.7/vgis_utils/vgis_list/listTools.py` & `vgis_utils-1.0.8/vgis_utils/vgis_list/listTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.7/vgis_utils/vgis_money/moneyTools.py` & `vgis_utils-1.0.8/vgis_utils/vgis_money/moneyTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.7/vgis_utils/vgis_string/stringTools.py` & `vgis_utils-1.0.8/vgis_utils/vgis_string/stringTools.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,11 +74,25 @@
         for replace in replace_list:
             input_str = input_str.replace(replace.get("hanzi"), replace.get("pinyin"))
         if len(re.findall("[\u4e00-\u9fa5]", input_str)) == 0:
             return input_str
         else:
             StringHelper.convert_hanzi_to_pinyin_in_str(input_str)
 
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
+
 if __name__ == '__main__':
     input_str = "中故宫eee中工"
     input_str = StringHelper.convert_hanzi_to_pinyin_in_str(input_str)
     print(input_str)
```

### Comparing `vgis_utils-1.0.7/vgis_utils/vgis_video/videoTools.py` & `vgis_utils-1.0.8/vgis_utils/vgis_video/videoTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.7/vgis_utils.egg-info/PKG-INFO` & `vgis_utils-1.0.8/vgis_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis-utils
-Version: 1.0.7
+Version: 1.0.8
 Summary: A libary for common operator
 Home-page: https://github.com/gisfanmachel/vgisUtils
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis common lib
```

### Comparing `vgis_utils-1.0.7/vgis_utils.egg-info/SOURCES.txt` & `vgis_utils-1.0.8/vgis_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

