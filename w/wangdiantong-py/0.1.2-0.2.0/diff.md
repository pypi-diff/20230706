# Comparing `tmp/wangdiantong-py-0.1.2.tar.gz` & `tmp/wangdiantong-py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wangdiantong-py-0.1.2.tar", last modified: Wed Aug 19 07:36:05 2020, max compression
+gzip compressed data, was "wangdiantong-py-0.2.0.tar", last modified: Thu Jul  6 09:43:02 2023, max compression
```

## Comparing `wangdiantong-py-0.1.2.tar` & `wangdiantong-py-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 youngtwain   (501) staff       (20)        0 2020-08-19 07:36:05.000000 wangdiantong-py-0.1.2/
--rw-r--r--   0 youngtwain   (501) staff       (20)      128 2020-08-19 07:30:03.000000 wangdiantong-py-0.1.2/MANIFEST.in
--rw-r--r--   0 youngtwain   (501) staff       (20)      778 2020-08-19 07:36:05.000000 wangdiantong-py-0.1.2/PKG-INFO
--rw-r--r--   0 youngtwain   (501) staff       (20)      757 2020-08-19 07:12:40.000000 wangdiantong-py-0.1.2/README.md
--rw-r--r--   0 youngtwain   (501) staff       (20)      286 2020-08-19 07:36:05.000000 wangdiantong-py-0.1.2/setup.cfg
--rw-r--r--   0 youngtwain   (501) staff       (20)     2332 2020-08-19 07:34:13.000000 wangdiantong-py-0.1.2/setup.py
-drwxr-xr-x   0 youngtwain   (501) staff       (20)        0 2020-08-19 07:36:05.000000 wangdiantong-py-0.1.2/wangdiantong/
--rw-r--r--   0 youngtwain   (501) staff       (20)      209 2020-08-19 07:35:58.000000 wangdiantong-py-0.1.2/wangdiantong/__init__.py
-drwxr-xr-x   0 youngtwain   (501) staff       (20)        0 2020-08-19 07:36:05.000000 wangdiantong-py-0.1.2/wangdiantong/api/
--rw-r--r--   0 youngtwain   (501) staff       (20)      266 2020-08-19 06:44:35.000000 wangdiantong-py-0.1.2/wangdiantong/api/__init__.py
--rw-r--r--   0 youngtwain   (501) staff       (20)      868 2020-08-19 06:44:35.000000 wangdiantong-py-0.1.2/wangdiantong/api/base.py
--rw-r--r--   0 youngtwain   (501) staff       (20)     8229 2020-08-19 06:44:35.000000 wangdiantong-py-0.1.2/wangdiantong/api/goods.py
--rw-r--r--   0 youngtwain   (501) staff       (20)     1766 2020-08-19 06:44:35.000000 wangdiantong-py-0.1.2/wangdiantong/api/logistics.py
--rw-r--r--   0 youngtwain   (501) staff       (20)     5022 2020-08-19 06:44:35.000000 wangdiantong-py-0.1.2/wangdiantong/api/order.py
--rw-r--r--   0 youngtwain   (501) staff       (20)     3112 2020-08-19 06:44:35.000000 wangdiantong-py-0.1.2/wangdiantong/api/stocks.py
-drwxr-xr-x   0 youngtwain   (501) staff       (20)        0 2020-08-19 07:36:05.000000 wangdiantong-py-0.1.2/wangdiantong/client/
--rw-r--r--   0 youngtwain   (501) staff       (20)      574 2020-08-19 06:44:35.000000 wangdiantong-py-0.1.2/wangdiantong/client/__init__.py
--rw-r--r--   0 youngtwain   (501) staff       (20)     3197 2020-08-19 06:44:35.000000 wangdiantong-py-0.1.2/wangdiantong/client/base.py
--rw-r--r--   0 youngtwain   (501) staff       (20)      502 2020-08-19 06:44:35.000000 wangdiantong-py-0.1.2/wangdiantong/settings.py
--rw-r--r--   0 youngtwain   (501) staff       (20)     1972 2020-08-19 06:44:35.000000 wangdiantong-py-0.1.2/wangdiantong/utils.py
-drwxr-xr-x   0 youngtwain   (501) staff       (20)        0 2020-08-19 07:36:05.000000 wangdiantong-py-0.1.2/wangdiantong_py.egg-info/
--rw-r--r--   0 youngtwain   (501) staff       (20)      778 2020-08-19 07:36:05.000000 wangdiantong-py-0.1.2/wangdiantong_py.egg-info/PKG-INFO
--rw-r--r--   0 youngtwain   (501) staff       (20)      609 2020-08-19 07:36:05.000000 wangdiantong-py-0.1.2/wangdiantong_py.egg-info/SOURCES.txt
--rw-r--r--   0 youngtwain   (501) staff       (20)        1 2020-08-19 07:36:05.000000 wangdiantong-py-0.1.2/wangdiantong_py.egg-info/dependency_links.txt
--rw-r--r--   0 youngtwain   (501) staff       (20)       20 2020-08-19 07:36:05.000000 wangdiantong-py-0.1.2/wangdiantong_py.egg-info/entry_points.txt
--rw-r--r--   0 youngtwain   (501) staff       (20)        1 2020-08-19 06:53:48.000000 wangdiantong-py-0.1.2/wangdiantong_py.egg-info/not-zip-safe
--rw-r--r--   0 youngtwain   (501) staff       (20)       38 2020-08-19 07:36:05.000000 wangdiantong-py-0.1.2/wangdiantong_py.egg-info/requires.txt
--rw-r--r--   0 youngtwain   (501) staff       (20)       13 2020-08-19 07:36:05.000000 wangdiantong-py-0.1.2/wangdiantong_py.egg-info/top_level.txt
+drwxr-xr-x   0 xoss      (1000) xoss      (1000)        0 2023-07-06 09:43:02.773772 wangdiantong-py-0.2.0/
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)     1068 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/LICENSE
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)      128 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/MANIFEST.in
+-rw-r--r--   0 xoss      (1000) xoss      (1000)      744 2023-07-06 09:43:02.773772 wangdiantong-py-0.2.0/PKG-INFO
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)      757 2023-07-06 09:41:26.000000 wangdiantong-py-0.2.0/README.md
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)      286 2023-07-06 09:43:02.773772 wangdiantong-py-0.2.0/setup.cfg
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)     2332 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/setup.py
+drwxr-xr-x   0 xoss      (1000) xoss      (1000)        0 2023-07-06 09:43:02.769773 wangdiantong-py-0.2.0/wangdiantong/
+-rw-r--r--   0 xoss      (1000) xoss      (1000)      212 2023-07-06 09:40:58.000000 wangdiantong-py-0.2.0/wangdiantong/__init__.py
+drwxr-xr-x   0 xoss      (1000) xoss      (1000)        0 2023-07-06 09:43:02.773772 wangdiantong-py-0.2.0/wangdiantong/api/
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)      266 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/wangdiantong/api/__init__.py
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)      868 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/wangdiantong/api/base.py
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)     8229 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/wangdiantong/api/goods.py
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)     1766 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/wangdiantong/api/logistics.py
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)     5022 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/wangdiantong/api/order.py
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)     3112 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/wangdiantong/api/stocks.py
+drwxr-xr-x   0 xoss      (1000) xoss      (1000)        0 2023-07-06 09:43:02.773772 wangdiantong-py-0.2.0/wangdiantong/client/
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)      574 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/wangdiantong/client/__init__.py
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)     3197 2023-07-06 09:16:39.000000 wangdiantong-py-0.2.0/wangdiantong/client/base.py
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)      502 2023-07-06 09:37:41.000000 wangdiantong-py-0.2.0/wangdiantong/settings.py
+-rw-rw-r--   0 xoss      (1000) xoss      (1000)     1972 2023-07-06 09:31:27.000000 wangdiantong-py-0.2.0/wangdiantong/utils.py
+drwxr-xr-x   0 xoss      (1000) xoss      (1000)        0 2023-07-06 09:43:02.773772 wangdiantong-py-0.2.0/wangdiantong_py.egg-info/
+-rw-r--r--   0 xoss      (1000) xoss      (1000)      744 2023-07-06 09:43:02.000000 wangdiantong-py-0.2.0/wangdiantong_py.egg-info/PKG-INFO
+-rw-r--r--   0 xoss      (1000) xoss      (1000)      575 2023-07-06 09:43:02.000000 wangdiantong-py-0.2.0/wangdiantong_py.egg-info/SOURCES.txt
+-rw-r--r--   0 xoss      (1000) xoss      (1000)        1 2023-07-06 09:43:02.000000 wangdiantong-py-0.2.0/wangdiantong_py.egg-info/dependency_links.txt
+-rw-r--r--   0 xoss      (1000) xoss      (1000)        1 2023-07-06 09:43:02.000000 wangdiantong-py-0.2.0/wangdiantong_py.egg-info/not-zip-safe
+-rw-r--r--   0 xoss      (1000) xoss      (1000)       38 2023-07-06 09:43:02.000000 wangdiantong-py-0.2.0/wangdiantong_py.egg-info/requires.txt
+-rw-r--r--   0 xoss      (1000) xoss      (1000)       13 2023-07-06 09:43:02.000000 wangdiantong-py-0.2.0/wangdiantong_py.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wangdiantong-py-0.1.2/PKG-INFO` & `wangdiantong-py-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: wangdiantong-py
-Version: 0.1.2
+Version: 0.2.0
 Summary: wangdiantong python openapi
 Home-page: https://github.com/AoAoStudio/wangdiantong-py
 Author: Ranger Huang
 Author-email: ranger_huang@yeah.net
-License: UNKNOWN
-Description: UNKNOWN
 Keywords: wangdiantong
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
```

### Comparing `wangdiantong-py-0.1.2/README.md` & `wangdiantong-py-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.1.2/setup.py` & `wangdiantong-py-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.1.2/wangdiantong/api/base.py` & `wangdiantong-py-0.2.0/wangdiantong/api/base.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.1.2/wangdiantong/api/goods.py` & `wangdiantong-py-0.2.0/wangdiantong/api/goods.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.1.2/wangdiantong/api/logistics.py` & `wangdiantong-py-0.2.0/wangdiantong/api/logistics.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.1.2/wangdiantong/api/order.py` & `wangdiantong-py-0.2.0/wangdiantong/api/order.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.1.2/wangdiantong/api/stocks.py` & `wangdiantong-py-0.2.0/wangdiantong/api/stocks.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.1.2/wangdiantong/client/__init__.py` & `wangdiantong-py-0.2.0/wangdiantong/client/__init__.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.1.2/wangdiantong/client/base.py` & `wangdiantong-py-0.2.0/wangdiantong/client/base.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.1.2/wangdiantong/utils.py` & `wangdiantong-py-0.2.0/wangdiantong/utils.py`

 * *Files identical despite different names*

### Comparing `wangdiantong-py-0.1.2/wangdiantong_py.egg-info/PKG-INFO` & `wangdiantong-py-0.2.0/wangdiantong_py.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: wangdiantong-py
-Version: 0.1.2
+Version: 0.2.0
 Summary: wangdiantong python openapi
 Home-page: https://github.com/AoAoStudio/wangdiantong-py
 Author: Ranger Huang
 Author-email: ranger_huang@yeah.net
-License: UNKNOWN
-Description: UNKNOWN
 Keywords: wangdiantong
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
```

### Comparing `wangdiantong-py-0.1.2/wangdiantong_py.egg-info/SOURCES.txt` & `wangdiantong-py-0.2.0/wangdiantong_py.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 wangdiantong/__init__.py
 wangdiantong/settings.py
 wangdiantong/utils.py
@@ -12,11 +13,10 @@
 wangdiantong/api/order.py
 wangdiantong/api/stocks.py
 wangdiantong/client/__init__.py
 wangdiantong/client/base.py
 wangdiantong_py.egg-info/PKG-INFO
 wangdiantong_py.egg-info/SOURCES.txt
 wangdiantong_py.egg-info/dependency_links.txt
-wangdiantong_py.egg-info/entry_points.txt
 wangdiantong_py.egg-info/not-zip-safe
 wangdiantong_py.egg-info/requires.txt
 wangdiantong_py.egg-info/top_level.txt
```

