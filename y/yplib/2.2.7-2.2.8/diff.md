# Comparing `tmp/yplib-2.2.7.tar.gz` & `tmp/yplib-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.2.7.tar", last modified: Thu Jul  6 00:43:32 2023, max compression
+gzip compressed data, was "dist\yplib-2.2.8.tar", last modified: Thu Jul  6 06:13:25 2023, max compression
```

## Comparing `yplib-2.2.7.tar` & `yplib-2.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 00:43:32.091759 yplib-2.2.7/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.2.7/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-06 00:43:32.091759 yplib-2.2.7/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.2.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 00:43:32.091759 yplib-2.2.7/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-06 00:43:20.000000 yplib-2.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:43:32.088528 yplib-2.2.7/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.2.7/yplib/__init__.py
--rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.2.7/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.2.7/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.2.7/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.2.7/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.2.7/yplib/http_util.py
--rw-rw-rw-   0        0        0    32405 2023-07-06 00:43:07.000000 yplib-2.2.7/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.2.7/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.2.7/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.2.7/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.2.7/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:43:32.091257 yplib-2.2.7/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-06 00:43:32.000000 yplib-2.2.7/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-06 00:43:32.000000 yplib-2.2.7/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 00:43:32.000000 yplib-2.2.7/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 00:43:32.000000 yplib-2.2.7/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 06:13:25.993117 yplib-2.2.8/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.2.8/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-06 06:13:25.993117 yplib-2.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.2.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 06:13:25.993117 yplib-2.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-06 06:12:38.000000 yplib-2.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:13:25.987672 yplib-2.2.8/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.2.8/yplib/__init__.py
+-rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.2.8/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.2.8/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.2.8/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.2.8/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.2.8/yplib/http_util.py
+-rw-rw-rw-   0        0        0    32397 2023-07-06 06:10:01.000000 yplib-2.2.8/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.2.8/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.2.8/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.2.8/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.2.8/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:13:25.993117 yplib-2.2.8/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-06 06:13:25.000000 yplib-2.2.8/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-06 06:13:25.000000 yplib-2.2.8/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 06:13:25.000000 yplib-2.2.8/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 06:13:25.000000 yplib-2.2.8/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.2.7/LICENSE` & `yplib-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.2.7/setup.py` & `yplib-2.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.2.7",
+  version="2.2.8",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.2.7/yplib/__init__.py` & `yplib-2.2.8/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.7/yplib/chart.py` & `yplib-2.2.8/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.7/yplib/chart_html.py` & `yplib-2.2.8/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.7/yplib/db.py` & `yplib-2.2.8/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.7/yplib/file.py` & `yplib-2.2.8/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.7/yplib/http_util.py` & `yplib-2.2.8/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.7/yplib/index.py` & `yplib-2.2.8/yplib/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -552,15 +552,15 @@
             continue
         elif end_flag is not None and end_flag:
             # 有结束标记位参数,并且,已经走到了结束标记位
             continue
         c += 1
         data_list.append(line)
     # 有行分隔符
-    if sep_line is not None or sep_line_contain is not None or sep_line_prefix is not None or sep_line_suffix is not None:
+    if len(list(filter(lambda x: x is not None, [sep_line, sep_line_contain, sep_line_prefix, sep_line_suffix]))):
         r_list = []
         t_l = []
         for d_o in data_list:
             n_l_f = False
             # 这一行, 等于 sep_line
             if sep_line is not None and d_o == sep_line:
                 n_l_f = True
```

### Comparing `yplib-2.2.7/yplib/mail.py` & `yplib-2.2.8/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.7/yplib/mail_html.py` & `yplib-2.2.8/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.7/yplib/markdown.py` & `yplib-2.2.8/yplib/markdown.py`

 * *Files identical despite different names*

