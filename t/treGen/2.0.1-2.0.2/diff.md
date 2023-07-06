# Comparing `tmp/treGen-2.0.1.tar.gz` & `tmp/treGen-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treGen-2.0.1.tar", last modified: Thu Jul  6 18:43:02 2023, max compression
+gzip compressed data, was "treGen-2.0.2.tar", last modified: Thu Jul  6 18:44:56 2023, max compression
```

## Comparing `treGen-2.0.1.tar` & `treGen-2.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:02.639622 treGen-2.0.1/
--rw-rw-rw-   0        0        0      172 2023-07-06 18:04:58.000000 treGen-2.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1099 2023-07-06 16:52:25.000000 treGen-2.0.1/LICENSE
--rw-rw-rw-   0        0        0       25 2023-07-06 18:04:52.000000 treGen-2.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3369 2023-07-06 18:43:02.638585 treGen-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1853 2023-07-06 18:08:26.000000 treGen-2.0.1/README.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 18:43:02.639622 treGen-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-07-06 18:42:57.000000 treGen-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:02.605824 treGen-2.0.1/src/
--rw-rw-rw-   0        0        0      128 2023-07-06 17:56:41.000000 treGen-2.0.1/src/tree.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:02.615588 treGen-2.0.1/src/treeGen/
--rw-rw-rw-   0        0        0      129 2023-07-06 18:27:50.000000 treGen-2.0.1/src/treeGen/__init__.py
--rw-rw-rw-   0        0        0     1421 2023-07-06 17:58:35.000000 treGen-2.0.1/src/treeGen/cli.py
--rw-rw-rw-   0        0        0     2658 2023-07-06 16:58:32.000000 treGen-2.0.1/src/treeGen/treeGen.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:02.626588 treGen-2.0.1/treGen.egg-info/
--rw-rw-rw-   0        0        0     3369 2023-07-06 18:43:02.000000 treGen-2.0.1/treGen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-07-06 18:43:02.000000 treGen-2.0.1/treGen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 18:43:02.000000 treGen-2.0.1/treGen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 18:43:02.000000 treGen-2.0.1/treGen.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:02.636932 treGen-2.0.1/treeGen.egg-info/
--rw-rw-rw-   0        0        0      255 2023-07-06 18:30:12.000000 treGen-2.0.1/treeGen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 18:30:12.000000 treGen-2.0.1/treeGen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 18:30:12.000000 treGen-2.0.1/treeGen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 18:44:56.627858 treGen-2.0.2/
+-rw-rw-rw-   0        0        0      172 2023-07-06 18:04:58.000000 treGen-2.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1099 2023-07-06 16:52:25.000000 treGen-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-07-06 18:04:52.000000 treGen-2.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3410 2023-07-06 18:44:56.627858 treGen-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1853 2023-07-06 18:08:26.000000 treGen-2.0.2/README.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 18:44:56.629851 treGen-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-07-06 18:44:51.000000 treGen-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:44:56.603849 treGen-2.0.2/src/
+-rw-rw-rw-   0        0        0      128 2023-07-06 17:56:41.000000 treGen-2.0.2/src/tree.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:44:56.609848 treGen-2.0.2/src/treeGen/
+-rw-rw-rw-   0        0        0      129 2023-07-06 18:27:50.000000 treGen-2.0.2/src/treeGen/__init__.py
+-rw-rw-rw-   0        0        0     1421 2023-07-06 17:58:35.000000 treGen-2.0.2/src/treeGen/cli.py
+-rw-rw-rw-   0        0        0     2658 2023-07-06 16:58:32.000000 treGen-2.0.2/src/treeGen/treeGen.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:44:56.619859 treGen-2.0.2/treGen.egg-info/
+-rw-rw-rw-   0        0        0     3410 2023-07-06 18:44:56.000000 treGen-2.0.2/treGen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-07-06 18:44:56.000000 treGen-2.0.2/treGen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 18:44:56.000000 treGen-2.0.2/treGen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 18:44:56.000000 treGen-2.0.2/treGen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 18:44:56.625858 treGen-2.0.2/treeGen.egg-info/
+-rw-rw-rw-   0        0        0      255 2023-07-06 18:30:12.000000 treGen-2.0.2/treeGen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 18:30:12.000000 treGen-2.0.2/treeGen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 18:30:12.000000 treGen-2.0.2/treeGen.egg-info/top_level.txt
```

### Comparing `treGen-2.0.1/LICENSE` & `treGen-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `treGen-2.0.1/PKG-INFO` & `treGen-2.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: treGen
-Version: 2.0.1
+Version: 2.0.2
 Summary: A simple Directory Tree Generator
 Home-page: https://github.com/JRS296/Directory-Tree
 Author: Jonathan Rufus Samuel
 Author-email: jrsstudios@skiff.com
 License: MIT
 Description: # Directory-Tree
         Simple Python CLI App to generate a directory tree for a given path
@@ -82,7 +82,8 @@
 Keywords: tree-generator
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
```

### Comparing `treGen-2.0.1/README.txt` & `treGen-2.0.2/README.txt`

 * *Files identical despite different names*

### Comparing `treGen-2.0.1/setup.py` & `treGen-2.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,19 @@
   "Operating System :: OS Independent",
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='treGen',
-  version='2.0.1',
+  version='2.0.2',
   description='A simple Directory Tree Generator',
   readme='README.MD',
   long_description=open('README.md').read(),
+  long_description_content_type='text/markdown',
   url='https://github.com/JRS296/Directory-Tree',  
   author='Jonathan Rufus Samuel',
   author_email='jrsstudios@skiff.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='tree-generator', 
   packages=find_packages(),
```

### Comparing `treGen-2.0.1/src/treeGen/cli.py` & `treGen-2.0.2/src/treeGen/cli.py`

 * *Files identical despite different names*

### Comparing `treGen-2.0.1/src/treeGen/treeGen.py` & `treGen-2.0.2/src/treeGen/treeGen.py`

 * *Files identical despite different names*

### Comparing `treGen-2.0.1/treGen.egg-info/PKG-INFO` & `treGen-2.0.2/treGen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: treGen
-Version: 2.0.1
+Version: 2.0.2
 Summary: A simple Directory Tree Generator
 Home-page: https://github.com/JRS296/Directory-Tree
 Author: Jonathan Rufus Samuel
 Author-email: jrsstudios@skiff.com
 License: MIT
 Description: # Directory-Tree
         Simple Python CLI App to generate a directory tree for a given path
@@ -82,7 +82,8 @@
 Keywords: tree-generator
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
```

