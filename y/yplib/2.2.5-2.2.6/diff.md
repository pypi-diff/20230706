# Comparing `tmp/yplib-2.2.5.tar.gz` & `tmp/yplib-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.2.5.tar", last modified: Wed Jul  5 01:35:47 2023, max compression
+gzip compressed data, was "dist\yplib-2.2.6.tar", last modified: Wed Jul  5 02:02:12 2023, max compression
```

## Comparing `yplib-2.2.5.tar` & `yplib-2.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 01:35:47.614213 yplib-2.2.5/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.2.5/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-05 01:35:47.613934 yplib-2.2.5/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-05 01:35:47.614714 yplib-2.2.5/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-05 01:35:36.000000 yplib-2.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 01:35:47.610281 yplib-2.2.5/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.2.5/yplib/__init__.py
--rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.2.5/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.2.5/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.2.5/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.2.5/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.2.5/yplib/http_util.py
--rw-rw-rw-   0        0        0    31084 2023-07-05 01:33:19.000000 yplib-2.2.5/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.2.5/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.2.5/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.2.5/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.2.5/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-05 01:35:47.612571 yplib-2.2.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-05 01:35:47.000000 yplib-2.2.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-05 01:35:47.000000 yplib-2.2.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 01:35:47.000000 yplib-2.2.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-05 01:35:47.000000 yplib-2.2.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 02:02:12.618293 yplib-2.2.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.2.6/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-05 02:02:12.617330 yplib-2.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-05 02:02:12.618293 yplib-2.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-05 02:01:57.000000 yplib-2.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 02:02:12.615189 yplib-2.2.6/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.2.6/yplib/__init__.py
+-rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.2.6/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.2.6/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.2.6/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.2.6/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.2.6/yplib/http_util.py
+-rw-rw-rw-   0        0        0    31348 2023-07-05 02:01:21.000000 yplib-2.2.6/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.2.6/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.2.6/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.2.6/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.2.6/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-05 02:02:12.617330 yplib-2.2.6/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-05 02:02:12.000000 yplib-2.2.6/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-05 02:02:12.000000 yplib-2.2.6/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 02:02:12.000000 yplib-2.2.6/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-05 02:02:12.000000 yplib-2.2.6/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.2.5/LICENSE` & `yplib-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.2.5/setup.py` & `yplib-2.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.2.5",
+  version="2.2.6",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.2.5/yplib/__init__.py` & `yplib-2.2.6/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.5/yplib/chart.py` & `yplib-2.2.6/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.5/yplib/chart_html.py` & `yplib-2.2.6/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.5/yplib/db.py` & `yplib-2.2.6/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.5/yplib/file.py` & `yplib-2.2.6/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.5/yplib/http_util.py` & `yplib-2.2.6/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.5/yplib/index.py` & `yplib-2.2.6/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,24 +191,28 @@
 
 def random_int_str(length=10):
     return random_str(length=length, start_str=53, end_str=62)
 
 
 # 去掉 str 中的 非数字字符, 然后, 再转化为 int
 def to_int(s):
+    if isinstance(s, int):
+        return s
     if s is None or s == '':
         return 0
     if isinstance(s, float):
         return int(s)
     s = ''.join(filter(lambda ch: ch in '0123456789', str(s)))
     return 0 if s == '' else int(s)
 
 
 # 去掉 str 中的 非数字字符, 然后, 再转化为 float
 def to_float(s):
+    if isinstance(s, float):
+        return s
     if s is None or s == '':
         return 0.0
     s = ''.join(filter(lambda ch: ch in '0123456789.', str(s)))
     return 0.0 if s == '' else float(s)
 
 
 def to_datetime(s=None, r_str=False):
@@ -503,14 +507,15 @@
                      end_line=None,
                      count=None):
     if file_is_empty(file_name=file_name):
         return []
     data_list = []
     # 普通文件的解析
     d_list = open(file_name, 'r', encoding='utf-8').readlines()
+    # 数量
     c = 0
     start_flag = None
     end_flag = None
     if start_line is not None:
         start_flag = False
     if end_line is not None:
         end_flag = False
@@ -528,16 +533,18 @@
         # 开始标记位
         if start_flag is not None and not start_flag and line.find(start_line) > -1:
             start_flag = True
         # 开始标记位
         if end_flag is not None and not end_flag and line.find(end_line) > -1:
             end_flag = True
         if start_flag is not None and not start_flag:
+            # 有开始标记位参数,并且,还没有走到开始标记位
             continue
         elif end_flag is not None and end_flag:
+            # 有结束标记位参数,并且,已经走到了结束标记位
             continue
         c += 1
         if sep is not None:
             data_list.append(line.split(str(sep)))
         else:
             data_list.append(line)
     if sep_all is not None:
```

### Comparing `yplib-2.2.5/yplib/mail.py` & `yplib-2.2.6/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.5/yplib/mail_html.py` & `yplib-2.2.6/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.5/yplib/markdown.py` & `yplib-2.2.6/yplib/markdown.py`

 * *Files identical despite different names*

