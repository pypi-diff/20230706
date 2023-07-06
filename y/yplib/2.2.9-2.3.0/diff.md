# Comparing `tmp/yplib-2.2.9.tar.gz` & `tmp/yplib-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.2.9.tar", last modified: Thu Jul  6 06:32:15 2023, max compression
+gzip compressed data, was "dist\yplib-2.3.0.tar", last modified: Thu Jul  6 08:19:19 2023, max compression
```

## Comparing `yplib-2.2.9.tar` & `yplib-2.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 06:32:15.897072 yplib-2.2.9/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.2.9/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-06 06:32:15.897072 yplib-2.2.9/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.2.9/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 06:32:15.897072 yplib-2.2.9/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-06 06:30:43.000000 yplib-2.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:32:15.893083 yplib-2.2.9/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.2.9/yplib/__init__.py
--rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.2.9/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.2.9/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.2.9/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.2.9/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.2.9/yplib/http_util.py
--rw-rw-rw-   0        0        0    32765 2023-07-06 06:29:57.000000 yplib-2.2.9/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.2.9/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.2.9/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.2.9/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.2.9/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:32:15.896370 yplib-2.2.9/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-06 06:32:15.000000 yplib-2.2.9/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-06 06:32:15.000000 yplib-2.2.9/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 06:32:15.000000 yplib-2.2.9/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 06:32:15.000000 yplib-2.2.9/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 08:19:19.883493 yplib-2.3.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.0/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-06 08:19:19.883493 yplib-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 08:19:19.884174 yplib-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-06 08:19:00.000000 yplib-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:19:19.880391 yplib-2.3.0/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.0/yplib/__init__.py
+-rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.3.0/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.0/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.3.0/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.0/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.0/yplib/http_util.py
+-rw-rw-rw-   0        0        0    32812 2023-07-06 08:18:01.000000 yplib-2.3.0/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.0/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.0/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.0/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.0/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:19:19.882772 yplib-2.3.0/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-06 08:19:19.000000 yplib-2.3.0/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-06 08:19:19.000000 yplib-2.3.0/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 08:19:19.000000 yplib-2.3.0/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 08:19:19.000000 yplib-2.3.0/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.2.9/LICENSE` & `yplib-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.2.9/setup.py` & `yplib-2.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.2.9",
+  version="2.3.0",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.2.9/yplib/__init__.py` & `yplib-2.3.0/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.9/yplib/chart.py` & `yplib-2.3.0/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.9/yplib/chart_html.py` & `yplib-2.3.0/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.9/yplib/db.py` & `yplib-2.3.0/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.9/yplib/file.py` & `yplib-2.3.0/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.9/yplib/http_util.py` & `yplib-2.3.0/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.9/yplib/index.py` & `yplib-2.3.0/yplib/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,16 +33,18 @@
     d = ''
     for one in l:
         if can_use_json(one):
             o = json.dumps(one)
         else:
             o = str(one)
         if o != '':
-            d = d + ' ' + o
-    lo = datetime.today().strftime('%Y-%m-%d %H:%M:%S') + d if time_prefix else d
+            if len(d):
+                d += ' '
+            d += o
+    lo = datetime.today().strftime('%Y-%m-%d %H:%M:%S') + ' ' + d if time_prefix else d
     print(lo)
     return lo
 
 
 # 将 log 数据, 写入到文件
 def to_log_file(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
                 a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20='', time_prefix=True):
```

### Comparing `yplib-2.2.9/yplib/mail.py` & `yplib-2.3.0/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.9/yplib/mail_html.py` & `yplib-2.3.0/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.2.9/yplib/markdown.py` & `yplib-2.3.0/yplib/markdown.py`

 * *Files identical despite different names*

