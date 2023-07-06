# Comparing `tmp/yplib-2.2.8.tar.gz` & `tmp/yplib-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.2.8.tar", last modified: Thu Jul  6 06:13:25 2023, max compression
+gzip compressed data, was "dist\yplib-2.2.9.tar", last modified: Thu Jul  6 06:32:15 2023, max compression
```

## Comparing `yplib-2.2.8.tar` & `yplib-2.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 06:13:25.993117 yplib-2.2.8/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.2.8/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-06 06:13:25.993117 yplib-2.2.8/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.2.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 06:13:25.993117 yplib-2.2.8/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-06 06:12:38.000000 yplib-2.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:13:25.987672 yplib-2.2.8/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.2.8/yplib/__init__.py
--rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.2.8/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.2.8/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.2.8/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.2.8/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.2.8/yplib/http_util.py
--rw-rw-rw-   0        0        0    32397 2023-07-06 06:10:01.000000 yplib-2.2.8/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.2.8/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.2.8/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.2.8/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.2.8/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:13:25.993117 yplib-2.2.8/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-06 06:13:25.000000 yplib-2.2.8/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-06 06:13:25.000000 yplib-2.2.8/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 06:13:25.000000 yplib-2.2.8/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 06:13:25.000000 yplib-2.2.8/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 06:32:15.897072 yplib-2.2.9/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.2.9/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-06 06:32:15.897072 yplib-2.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 06:32:15.897072 yplib-2.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-06 06:30:43.000000 yplib-2.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:32:15.893083 yplib-2.2.9/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.2.9/yplib/__init__.py
+-rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.2.9/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.2.9/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.2.9/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.2.9/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.2.9/yplib/http_util.py
+-rw-rw-rw-   0        0        0    32765 2023-07-06 06:29:57.000000 yplib-2.2.9/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.2.9/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.2.9/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.2.9/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.2.9/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:32:15.896370 yplib-2.2.9/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-06 06:32:15.000000 yplib-2.2.9/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-06 06:32:15.000000 yplib-2.2.9/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 06:32:15.000000 yplib-2.2.9/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 06:32:15.000000 yplib-2.2.9/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.2.8/LICENSE` & `yplib-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.2.8/setup.py` & `yplib-2.2.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.2.8",
+  version="2.2.9",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.2.8/yplib/__init__.py` & `yplib-2.2.9/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.8/yplib/chart.py` & `yplib-2.2.9/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.8/yplib/chart_html.py` & `yplib-2.2.9/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.8/yplib/db.py` & `yplib-2.2.9/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.8/yplib/file.py` & `yplib-2.2.9/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.8/yplib/http_util.py` & `yplib-2.2.9/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.8/yplib/index.py` & `yplib-2.2.9/yplib/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -490,32 +490,34 @@
 def to_list_from_txt_with_blank_row(file_name='a.txt'):
     return to_list_from_txt(file_name, sep_line='')
 
 
 # 将 txt 文件转化成 list 的方法
 # 当读取 txt 之类的文件的时候
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
-# sep : 是否对每一行进行分割,如果存在这个字段,就分割
-# sep_line : 这一行是一个分隔符, 返回的是一个 list(list)
-# sep_line_contain : 这一行是一个分隔符,包含这个行分隔符的做分割, 返回的是一个 list(list)
-# sep_line_prefix : 这一行是一个分隔符,以这个分隔符作为前缀的, 返回的是一个 list(list)
-# sep_line_suffix : 这一行是一个分隔符,以这个分隔符作为后缀的, 返回的是一个 list(list)
-# sep_all : 将文件转化成一个字符串,然后对这个字符串,再次总体分割
-# start_index : 从这个地方开始读取,从1开始标号 , 包含这一行
-# start_line :  从这个地方开始读取,从第一行开始找到这个字符串开始标记 , 包含这一行
-# end_index :   读取到这个地方结束,从1开始标号 , 不包含这一行
-# end_line :    读取到这个地方结束,从第一行开始找到这个字符串开始标记 , 不包含这一行
-# count :       读取指定的行数
+# sep               : 是否对每一行进行分割,如果存在这个字段,就分割
+# sep_line          : 这一行是一个分隔符, 返回的是一个 list(list)
+# sep_line_contain  : 这一行是一个分隔符,包含这个行分隔符的做分割, 返回的是一个 list(list)
+# sep_line_prefix   : 这一行是一个分隔符,以这个分隔符作为前缀的, 返回的是一个 list(list)
+# sep_line_suffix   : 这一行是一个分隔符,以这个分隔符作为后缀的, 返回的是一个 list(list)
+# sep_all           : 将文件转化成一个字符串,然后对这个字符串,再次总体分割
+# join              : 针对 list(list) 转化成 list(str) 类型的数据
+# start_index       : 从这个地方开始读取,从1开始标号 , 包含这一行
+# start_line        : 从这个地方开始读取,从第一行开始找到这个字符串开始标记 , 包含这一行
+# end_index         : 读取到这个地方结束,从1开始标号 , 不包含这一行
+# end_line          : 读取到这个地方结束,从第一行开始找到这个字符串开始标记 , 不包含这一行
+# count             : 读取指定的行数
 def to_list_from_txt(file_name='a.txt',
                      sep=None,
                      sep_line=None,
                      sep_line_contain=None,
                      sep_line_prefix=None,
                      sep_line_suffix=None,
                      sep_all=None,
+                     join=None,
                      start_index=None,
                      start_line=None,
                      end_index=None,
                      end_line=None,
                      count=None):
     if file_is_empty(file_name=file_name):
         return []
@@ -551,15 +553,18 @@
             # 有开始标记位参数,并且,还没有走到开始标记位
             continue
         elif end_flag is not None and end_flag:
             # 有结束标记位参数,并且,已经走到了结束标记位
             continue
         c += 1
         data_list.append(line)
-    # 有行分隔符
+    if sep_all is not None:
+        # 全部划分, 重新分割成 list(str)
+        data_list = ''.join(data_list).split(str(sep_all))
+    # 有行分隔符, 将会把 list(str) 转化成 list(list)
     if len(list(filter(lambda x: x is not None, [sep_line, sep_line_contain, sep_line_prefix, sep_line_suffix]))):
         r_list = []
         t_l = []
         for d_o in data_list:
             n_l_f = False
             # 这一行, 等于 sep_line
             if sep_line is not None and d_o == sep_line:
@@ -581,30 +586,30 @@
                     r_list.append(t_l)
                 t_l = []
             elif len(d_o):
                 t_l.append(d_o)
         if len(t_l):
             r_list.append(t_l)
         data_list = r_list
-    if sep_all is not None:
-        data_list = ''.join(data_list).split(str(sep_all))
     # 对这个 list 进行行内再次分割
     if sep is not None:
         r_list = []
         for line in data_list:
             # list(str) 情况
             if isinstance(line, str):
                 r_list.append(line.split(str(sep)))
             # list(list) 情况
             elif isinstance(line, list):
                 a_list = []
                 for o_line in line:
                     a_list.append(o_line.split(str(sep)))
                 r_list.append(a_list)
         data_list = r_list
+    if join is not None:
+        data_list = list(map(lambda x: str(join).join(x), data_list))
     return data_list
 
 
 # 读取文件中的数据,返回一个 str
 def to_str_from_file(file_name='a.txt',
                      str_join='',
                      start_index=None,
```

### Comparing `yplib-2.2.8/yplib/mail.py` & `yplib-2.2.9/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.8/yplib/mail_html.py` & `yplib-2.2.9/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.8/yplib/markdown.py` & `yplib-2.2.9/yplib/markdown.py`

 * *Files identical despite different names*

