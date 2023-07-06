# Comparing `tmp/gonchaya-0.0.1.tar.gz` & `tmp/gonchaya-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gonchaya-0.0.1.tar", last modified: Mon Jul  3 22:23:17 2023, max compression
+gzip compressed data, was "gonchaya-0.0.2.tar", last modified: Thu Jul  6 06:26:10 2023, max compression
```

## Comparing `gonchaya-0.0.1.tar` & `gonchaya-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxr-x   0 padla     (1000) padla     (1000)        0 2023-07-03 22:23:17.178970 gonchaya-0.0.1/
--rw-rw-r--   0 padla     (1000) padla     (1000)      664 2023-07-03 22:23:17.178970 gonchaya-0.0.1/PKG-INFO
--rw-rw-r--   0 padla     (1000) padla     (1000)      166 2023-07-03 12:14:18.000000 gonchaya-0.0.1/README.md
-drwxrwxr-x   0 padla     (1000) padla     (1000)        0 2023-07-03 22:23:17.178970 gonchaya-0.0.1/gonchaya/
--rw-rw-r--   0 padla     (1000) padla     (1000)      477 2023-07-03 13:01:13.000000 gonchaya-0.0.1/gonchaya/_init_.py
--rwxrwxr-x   0 padla     (1000) padla     (1000)     6848 2023-07-03 13:14:58.000000 gonchaya-0.0.1/gonchaya/gonchaya.py
-drwxrwxr-x   0 padla     (1000) padla     (1000)        0 2023-07-03 22:23:17.178970 gonchaya-0.0.1/gonchaya.egg-info/
--rw-rw-r--   0 padla     (1000) padla     (1000)      664 2023-07-03 22:23:17.000000 gonchaya-0.0.1/gonchaya.egg-info/PKG-INFO
--rw-rw-r--   0 padla     (1000) padla     (1000)      227 2023-07-03 22:23:17.000000 gonchaya-0.0.1/gonchaya.egg-info/SOURCES.txt
--rw-rw-r--   0 padla     (1000) padla     (1000)        1 2023-07-03 22:23:17.000000 gonchaya-0.0.1/gonchaya.egg-info/dependency_links.txt
--rw-rw-r--   0 padla     (1000) padla     (1000)       17 2023-07-03 22:23:17.000000 gonchaya-0.0.1/gonchaya.egg-info/requires.txt
--rw-rw-r--   0 padla     (1000) padla     (1000)        9 2023-07-03 22:23:17.000000 gonchaya-0.0.1/gonchaya.egg-info/top_level.txt
--rw-rw-r--   0 padla     (1000) padla     (1000)       38 2023-07-03 22:23:17.178970 gonchaya-0.0.1/setup.cfg
--rw-rw-r--   0 padla     (1000) padla     (1000)      642 2023-07-03 22:23:13.000000 gonchaya-0.0.1/setup.py
+drwxrwxr-x   0 padla     (1000) padla     (1000)        0 2023-07-06 06:26:10.899522 gonchaya-0.0.2/
+-rw-rw-r--   0 padla     (1000) padla     (1000)      704 2023-07-06 06:26:10.899522 gonchaya-0.0.2/PKG-INFO
+-rw-rw-r--   0 padla     (1000) padla     (1000)      166 2023-07-03 12:14:18.000000 gonchaya-0.0.2/README.md
+drwxrwxr-x   0 padla     (1000) padla     (1000)        0 2023-07-06 06:26:10.899522 gonchaya-0.0.2/gonchaya/
+-rwxrwxr-x   0 padla     (1000) padla     (1000)      343 2023-07-06 03:21:37.000000 gonchaya-0.0.2/gonchaya/debug.py
+drwxrwxr-x   0 padla     (1000) padla     (1000)        0 2023-07-06 06:26:10.899522 gonchaya-0.0.2/gonchaya.egg-info/
+-rw-rw-r--   0 padla     (1000) padla     (1000)      704 2023-07-06 06:26:10.000000 gonchaya-0.0.2/gonchaya.egg-info/PKG-INFO
+-rw-rw-r--   0 padla     (1000) padla     (1000)      205 2023-07-06 06:26:10.000000 gonchaya-0.0.2/gonchaya.egg-info/SOURCES.txt
+-rw-rw-r--   0 padla     (1000) padla     (1000)        1 2023-07-06 06:26:10.000000 gonchaya-0.0.2/gonchaya.egg-info/dependency_links.txt
+-rw-rw-r--   0 padla     (1000) padla     (1000)       17 2023-07-06 06:26:10.000000 gonchaya-0.0.2/gonchaya.egg-info/requires.txt
+-rw-rw-r--   0 padla     (1000) padla     (1000)        9 2023-07-06 06:26:10.000000 gonchaya-0.0.2/gonchaya.egg-info/top_level.txt
+-rw-rw-r--   0 padla     (1000) padla     (1000)       38 2023-07-06 06:26:10.899522 gonchaya-0.0.2/setup.cfg
+-rw-rw-r--   0 padla     (1000) padla     (1000)      716 2023-07-06 06:17:05.000000 gonchaya-0.0.2/setup.py
```

### Comparing `gonchaya-0.0.1/PKG-INFO` & `gonchaya-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gonchaya
-Version: 0.0.1
+Version: 0.0.2
 Summary: Data Science tools
 Home-page: UNKNOWN
 Author: Alexander Firsov aka gonchaya aka padla
 Author-email: gonchaya@gifara.ru
 License: UNKNOWN
 Description: # gonchaya
         a set of additional tools for the Data Science course  
@@ -12,9 +12,10 @@
         
         
 Keywords: example python
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: Russian
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `gonchaya-0.0.1/gonchaya.egg-info/PKG-INFO` & `gonchaya-0.0.2/gonchaya.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gonchaya
-Version: 0.0.1
+Version: 0.0.2
 Summary: Data Science tools
 Home-page: UNKNOWN
 Author: Alexander Firsov aka gonchaya aka padla
 Author-email: gonchaya@gifara.ru
 License: UNKNOWN
 Description: # gonchaya
         a set of additional tools for the Data Science course  
@@ -12,9 +12,10 @@
         
         
 Keywords: example python
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: Russian
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `gonchaya-0.0.1/setup.py` & `gonchaya-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='gonchaya',
-  version='0.0.1',
+  version='0.0.2',
   author='Alexander Firsov aka gonchaya aka padla',
   author_email='gonchaya@gifara.ru',
-
+  License='BSD License (BSD-3-Clause)',
   description='Data Science tools',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=['gonchaya'],
   install_requires=['requests>=2.25.1'],
   classifiers=[
     'Programming Language :: Python :: 3.11',
     'License :: OSI Approved :: BSD License',
-    'Operating System :: OS Independent'
+    'Operating System :: OS Independent',
+    'Natural Language :: Russian'
   ],
   keywords='example python',
   python_requires='>=3.8'
 )
```

