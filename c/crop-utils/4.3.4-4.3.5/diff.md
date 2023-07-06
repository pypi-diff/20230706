# Comparing `tmp/crop_utils-4.3.4.tar.gz` & `tmp/crop_utils-4.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crop_utils-4.3.4.tar", last modified: Mon Jun 12 03:13:51 2023, max compression
+gzip compressed data, was "crop_utils-4.3.5.tar", last modified: Thu Jul  6 09:27:45 2023, max compression
```

## Comparing `crop_utils-4.3.4.tar` & `crop_utils-4.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 03:13:51.868327 crop_utils-4.3.4/
--rw-rw-rw-   0        0        0     1091 2021-10-21 02:22:48.000000 crop_utils-4.3.4/LICENSE
--rw-rw-rw-   0        0        0       52 2021-10-21 06:40:49.000000 crop_utils-4.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1997 2023-06-12 03:13:51.865323 crop_utils-4.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      910 2023-06-09 03:37:04.000000 crop_utils-4.3.4/README.md
--rw-rw-rw-   0        0        0      108 2021-10-20 10:50:24.000000 crop_utils-4.3.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 03:13:51.868327 crop_utils-4.3.4/setup.cfg
--rw-rw-rw-   0        0        0      894 2023-06-12 03:13:50.000000 crop_utils-4.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:13:51.843318 crop_utils-4.3.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 03:13:51.857324 crop_utils-4.3.4/src/crop_utils/
--rw-rw-rw-   0        0        0        4 2021-10-21 03:45:02.000000 crop_utils-4.3.4/src/crop_utils/__init__.py
--rw-rw-rw-   0        0        0     2157 2023-06-06 03:35:58.000000 crop_utils-4.3.4/src/crop_utils/html_slot_config.py
--rw-rw-rw-   0        0        0    63534 2023-06-07 06:16:06.000000 crop_utils-4.3.4/src/crop_utils/image.py
--rw-rw-rw-   0        0        0    43292 2023-06-09 03:36:10.000000 crop_utils-4.3.4/src/crop_utils/img_crop.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:13:51.864320 crop_utils-4.3.4/src/crop_utils.egg-info/
--rw-rw-rw-   0        0        0     1997 2023-06-12 03:13:51.000000 crop_utils-4.3.4/src/crop_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-06-12 03:13:51.000000 crop_utils-4.3.4/src/crop_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 03:13:51.000000 crop_utils-4.3.4/src/crop_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-12 03:13:51.000000 crop_utils-4.3.4/src/crop_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 09:27:45.061596 crop_utils-4.3.5/
+-rw-rw-rw-   0        0        0     1091 2021-10-21 02:22:48.000000 crop_utils-4.3.5/LICENSE
+-rw-rw-rw-   0        0        0       52 2021-10-21 06:40:49.000000 crop_utils-4.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2016 2023-07-06 09:27:45.060595 crop_utils-4.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2023-06-12 03:15:02.000000 crop_utils-4.3.5/README.md
+-rw-rw-rw-   0        0        0      108 2021-10-20 10:50:24.000000 crop_utils-4.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 09:27:45.061596 crop_utils-4.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      913 2023-07-06 09:27:35.000000 crop_utils-4.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 09:27:45.032605 crop_utils-4.3.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 09:27:45.049594 crop_utils-4.3.5/src/crop_utils/
+-rw-rw-rw-   0        0        0        4 2021-10-21 03:45:02.000000 crop_utils-4.3.5/src/crop_utils/__init__.py
+-rw-rw-rw-   0        0        0     2157 2023-06-06 03:35:58.000000 crop_utils-4.3.5/src/crop_utils/html_slot_config.py
+-rw-rw-rw-   0        0        0    63534 2023-06-07 06:16:06.000000 crop_utils-4.3.5/src/crop_utils/image.py
+-rw-rw-rw-   0        0        0    43480 2023-07-06 08:56:09.000000 crop_utils-4.3.5/src/crop_utils/img_crop.py
+drwxrwxrwx   0        0        0        0 2023-07-06 09:27:45.059599 crop_utils-4.3.5/src/crop_utils.egg-info/
+-rw-rw-rw-   0        0        0     2016 2023-07-06 09:27:44.000000 crop_utils-4.3.5/src/crop_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-07-06 09:27:44.000000 crop_utils-4.3.5/src/crop_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 09:27:44.000000 crop_utils-4.3.5/src/crop_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-06 09:27:44.000000 crop_utils-4.3.5/src/crop_utils.egg-info/top_level.txt
```

### Comparing `crop_utils-4.3.4/LICENSE` & `crop_utils-4.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.4/PKG-INFO` & `crop_utils-4.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: crop_utils
-Version: 4.3.4
-Summary: 鞋类ai识别
+Version: 4.3.5
+Summary: 鞋类ai识别;裁剪边距计算
 Home-page: http://git.chaomy.com/libo/ecpro-utils.git
 Author: libo
 Author-email: 6878595@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: 为了区分3.0与4.0版本，同时资源图与详情页也共用的一套裁剪逻辑代码。
         
@@ -74,14 +74,14 @@
         
         
         
         # 安装
         
         
         
-        pip install crop-utils==4.3.3 -i  https://pypi.python.org/simple/
+        pip install crop-utils==4.3.4 -i  https://pypi.python.org/simple/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `crop_utils-4.3.4/README.md` & `crop_utils-4.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -65,8 +65,8 @@
 
 
 
 # 安装
 
 
 
-pip install crop-utils==4.3.3 -i  https://pypi.python.org/simple/
+pip install crop-utils==4.3.4 -i  https://pypi.python.org/simple/
```

### Comparing `crop_utils-4.3.4/setup.py` & `crop_utils-4.3.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="crop_utils",  # 包名称
-    version="4.3.4",  # 版本号
+    version="4.3.5",  # 版本号
     author="libo",
     author_email="6878595@qq.com",
-    description="鞋类ai识别",
+    description="鞋类ai识别;裁剪边距计算",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://git.chaomy.com/libo/ecpro-utils.git",
     project_urls={
         "Bug Tracker": "https://github.com/pypa/sampleproject/issues",
     },
     classifiers=[
```

### Comparing `crop_utils-4.3.4/src/crop_utils/html_slot_config.py` & `crop_utils-4.3.5/src/crop_utils/html_slot_config.py`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.4/src/crop_utils/image.py` & `crop_utils-4.3.5/src/crop_utils/image.py`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.4/src/crop_utils/img_crop.py` & `crop_utils-4.3.5/src/crop_utils/img_crop.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,14 +231,18 @@
             padding_left, padding_right = float(crop_parameter.get(LEFT, 0)) / slot_width, float(
                 crop_parameter.get(RIGHT, 0)) / slot_width
             padding_top, padding_bottom = float(crop_parameter.get(TOP, 0)) / slot_height, float(
                 crop_parameter.get(BOTTOM, 0)) / slot_height
 
         x1 = max(left - padding_left, 0)
         x2 = min(right + padding_right, 1)
+
+        padding_top = (bottom - top) / (1 - padding_top - padding_bottom) * padding_top
+        padding_bottom = (bottom - top) / (1 - padding_top - padding_bottom) * padding_bottom
+
         y1 = max(top - padding_top, 0)
         y2 = min(bottom + padding_bottom, 1)
 
         expand_y1 = top - padding_top
         expand_y2 = bottom + padding_bottom
 
         self.si.get_top_and_bottom_padding(top, padding_top, bottom, padding_bottom)
```

### Comparing `crop_utils-4.3.4/src/crop_utils.egg-info/PKG-INFO` & `crop_utils-4.3.5/src/crop_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: crop-utils
-Version: 4.3.4
-Summary: 鞋类ai识别
+Version: 4.3.5
+Summary: 鞋类ai识别;裁剪边距计算
 Home-page: http://git.chaomy.com/libo/ecpro-utils.git
 Author: libo
 Author-email: 6878595@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: 为了区分3.0与4.0版本，同时资源图与详情页也共用的一套裁剪逻辑代码。
         
@@ -74,14 +74,14 @@
         
         
         
         # 安装
         
         
         
-        pip install crop-utils==4.3.3 -i  https://pypi.python.org/simple/
+        pip install crop-utils==4.3.4 -i  https://pypi.python.org/simple/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

