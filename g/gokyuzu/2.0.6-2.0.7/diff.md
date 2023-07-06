# Comparing `tmp/gokyuzu-2.0.6.tar.gz` & `tmp/gokyuzu-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gokyuzu-2.0.6.tar", last modified: Thu Jul  6 18:14:58 2023, max compression
+gzip compressed data, was "gokyuzu-2.0.7.tar", last modified: Thu Jul  6 18:42:11 2023, max compression
```

## Comparing `gokyuzu-2.0.6.tar` & `gokyuzu-2.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-06 18:14:58.568746 gokyuzu-2.0.6/
--rw-r--r--   0 kilic      (501) staff       (20)       50 2023-07-03 19:01:04.000000 gokyuzu-2.0.6/LICENSE
--rw-r--r--   0 kilic      (501) staff       (20)     6440 2023-07-06 18:14:58.568632 gokyuzu-2.0.6/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)     5652 2023-07-03 19:01:58.000000 gokyuzu-2.0.6/README.md
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-06 18:14:58.566396 gokyuzu-2.0.6/gokyuzu/
--rw-r--r--   0 kilic      (501) staff       (20)     8595 2023-07-03 19:01:04.000000 gokyuzu-2.0.6/gokyuzu/BlueskyEndpoints.py
--rw-r--r--   0 kilic      (501) staff       (20)      688 2023-07-03 19:01:04.000000 gokyuzu-2.0.6/gokyuzu/BlueskyHelper.py
--rw-r--r--   0 kilic      (501) staff       (20)      247 2023-07-03 19:01:04.000000 gokyuzu-2.0.6/gokyuzu/BlueskyRecords.py
--rw-r--r--   0 kilic      (501) staff       (20)     4014 2023-07-03 19:01:04.000000 gokyuzu-2.0.6/gokyuzu/BlueskySession.py
--rw-r--r--   0 kilic      (501) staff       (20)    33711 2023-07-06 18:14:31.000000 gokyuzu-2.0.6/gokyuzu/__init__.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-06 18:14:58.568055 gokyuzu-2.0.6/gokyuzu.egg-info/
--rw-r--r--   0 kilic      (501) staff       (20)     6440 2023-07-06 18:14:58.000000 gokyuzu-2.0.6/gokyuzu.egg-info/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)      357 2023-07-06 18:14:58.000000 gokyuzu-2.0.6/gokyuzu.egg-info/SOURCES.txt
--rw-r--r--   0 kilic      (501) staff       (20)        1 2023-07-06 18:14:58.000000 gokyuzu-2.0.6/gokyuzu.egg-info/dependency_links.txt
--rw-r--r--   0 kilic      (501) staff       (20)       17 2023-07-06 18:14:58.000000 gokyuzu-2.0.6/gokyuzu.egg-info/requires.txt
--rw-r--r--   0 kilic      (501) staff       (20)       14 2023-07-06 18:14:58.000000 gokyuzu-2.0.6/gokyuzu.egg-info/top_level.txt
--rw-r--r--   0 kilic      (501) staff       (20)      475 2023-07-06 18:14:41.000000 gokyuzu-2.0.6/pyproject.toml
--rw-r--r--   0 kilic      (501) staff       (20)       38 2023-07-06 18:14:58.568785 gokyuzu-2.0.6/setup.cfg
--rw-r--r--   0 kilic      (501) staff       (20)     1041 2023-07-06 18:14:46.000000 gokyuzu-2.0.6/setup.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-06 18:14:58.568290 gokyuzu-2.0.6/tests/
--rw-r--r--   0 kilic      (501) staff       (20)        0 2023-07-03 19:01:04.000000 gokyuzu-2.0.6/tests/__init__.py
--rw-r--r--   0 kilic      (501) staff       (20)     5440 2023-07-03 19:01:04.000000 gokyuzu-2.0.6/tests/test_main.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-06 18:42:11.803141 gokyuzu-2.0.7/
+-rw-r--r--   0 kilic      (501) staff       (20)       50 2023-07-03 19:01:04.000000 gokyuzu-2.0.7/LICENSE
+-rw-r--r--   0 kilic      (501) staff       (20)     6440 2023-07-06 18:42:11.803028 gokyuzu-2.0.7/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)     5652 2023-07-03 19:01:58.000000 gokyuzu-2.0.7/README.md
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-06 18:42:11.801412 gokyuzu-2.0.7/gokyuzu/
+-rw-r--r--   0 kilic      (501) staff       (20)     8595 2023-07-03 19:01:04.000000 gokyuzu-2.0.7/gokyuzu/BlueskyEndpoints.py
+-rw-r--r--   0 kilic      (501) staff       (20)      688 2023-07-03 19:01:04.000000 gokyuzu-2.0.7/gokyuzu/BlueskyHelper.py
+-rw-r--r--   0 kilic      (501) staff       (20)      247 2023-07-03 19:01:04.000000 gokyuzu-2.0.7/gokyuzu/BlueskyRecords.py
+-rw-r--r--   0 kilic      (501) staff       (20)     4014 2023-07-03 19:01:04.000000 gokyuzu-2.0.7/gokyuzu/BlueskySession.py
+-rw-r--r--   0 kilic      (501) staff       (20)    33919 2023-07-06 18:40:53.000000 gokyuzu-2.0.7/gokyuzu/__init__.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-06 18:42:11.802487 gokyuzu-2.0.7/gokyuzu.egg-info/
+-rw-r--r--   0 kilic      (501) staff       (20)     6440 2023-07-06 18:42:11.000000 gokyuzu-2.0.7/gokyuzu.egg-info/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)      357 2023-07-06 18:42:11.000000 gokyuzu-2.0.7/gokyuzu.egg-info/SOURCES.txt
+-rw-r--r--   0 kilic      (501) staff       (20)        1 2023-07-06 18:42:11.000000 gokyuzu-2.0.7/gokyuzu.egg-info/dependency_links.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       17 2023-07-06 18:42:11.000000 gokyuzu-2.0.7/gokyuzu.egg-info/requires.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       14 2023-07-06 18:42:11.000000 gokyuzu-2.0.7/gokyuzu.egg-info/top_level.txt
+-rw-r--r--   0 kilic      (501) staff       (20)      475 2023-07-06 18:40:19.000000 gokyuzu-2.0.7/pyproject.toml
+-rw-r--r--   0 kilic      (501) staff       (20)       38 2023-07-06 18:42:11.803177 gokyuzu-2.0.7/setup.cfg
+-rw-r--r--   0 kilic      (501) staff       (20)     1041 2023-07-06 18:40:22.000000 gokyuzu-2.0.7/setup.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-06 18:42:11.802705 gokyuzu-2.0.7/tests/
+-rw-r--r--   0 kilic      (501) staff       (20)        0 2023-07-03 19:01:04.000000 gokyuzu-2.0.7/tests/__init__.py
+-rw-r--r--   0 kilic      (501) staff       (20)     5440 2023-07-03 19:01:04.000000 gokyuzu-2.0.7/tests/test_main.py
```

### Comparing `gokyuzu-2.0.6/PKG-INFO` & `gokyuzu-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 2.0.6
+Version: 2.0.7
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gokyuzu-2.0.6/README.md` & `gokyuzu-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gokyuzu-2.0.6/gokyuzu/BlueskyEndpoints.py` & `gokyuzu-2.0.7/gokyuzu/BlueskyEndpoints.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-2.0.6/gokyuzu/BlueskyHelper.py` & `gokyuzu-2.0.7/gokyuzu/BlueskyHelper.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-2.0.6/gokyuzu/BlueskySession.py` & `gokyuzu-2.0.7/gokyuzu/BlueskySession.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-2.0.6/gokyuzu/__init__.py` & `gokyuzu-2.0.7/gokyuzu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -853,19 +853,27 @@
         for follow in follows:
             if follow["handle"] not in follow_list:
                 follow_list[follow["handle"]] = follow
         return follow_list
     
     def merge_unique_lists(self, first_list, second_list):
         merged_list = {}
+        if len(first_list) == 0 and len(second_list) == 0:
+            return merged_list
+        
+        if len(first_list) == 0:
+            return second_list
+        elif len(second_list) == 0:
+            return first_list
+        
         for item in first_list:
-            merged_list[item["handle"]] = item
+            merged_list[item] = item
         for item in second_list:
-            if item["handle"] not in merged_list.keys():
-                merged_list[item["handle"]] = item
+            if item not in merged_list.keys():
+                merged_list[item] = item
         return merged_list
     
     def exclude_users(self, follow_list: dict, exluded_users):
         for handle in exluded_users:
             if handle in follow_list.keys():
                 follow_list.pop(handle)
         return follow_list
```

### Comparing `gokyuzu-2.0.6/gokyuzu.egg-info/PKG-INFO` & `gokyuzu-2.0.7/gokyuzu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 2.0.6
+Version: 2.0.7
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gokyuzu-2.0.6/setup.py` & `gokyuzu-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gokyuzu',
-    version='2.0.6',
+    version='2.0.7',
     description='bsky.social client library',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Muhammed Kılıç',
     author_email='muhammeddkilicc@gmail.com',
     url='https://github.com/kiliczsh/gokyuzu',
     packages=find_packages(),
```

### Comparing `gokyuzu-2.0.6/tests/test_main.py` & `gokyuzu-2.0.7/tests/test_main.py`

 * *Files identical despite different names*

