# Comparing `tmp/treGen-2.0.5.tar.gz` & `tmp/treGen-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treGen-2.0.5.tar", last modified: Thu Jul  6 18:51:54 2023, max compression
+gzip compressed data, was "treGen-2.1.0.tar", last modified: Thu Jul  6 19:26:45 2023, max compression
```

## Comparing `treGen-2.0.5.tar` & `treGen-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 18:51:54.893319 treGen-2.0.5/
--rw-rw-rw-   0        0        0      172 2023-07-06 18:04:58.000000 treGen-2.0.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1099 2023-07-06 16:52:25.000000 treGen-2.0.5/LICENSE
--rw-rw-rw-   0        0        0       25 2023-07-06 18:04:52.000000 treGen-2.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3410 2023-07-06 18:51:54.891312 treGen-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2093 2023-07-06 17:19:43.000000 treGen-2.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 18:51:54.893319 treGen-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-07-06 18:51:51.000000 treGen-2.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:51:54.871309 treGen-2.0.5/src/
--rw-rw-rw-   0        0        0      128 2023-07-06 17:56:41.000000 treGen-2.0.5/src/tree.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:51:54.882328 treGen-2.0.5/src/treeGen/
--rw-rw-rw-   0        0        0      129 2023-07-06 18:27:50.000000 treGen-2.0.5/src/treeGen/__init__.py
--rw-rw-rw-   0        0        0     1421 2023-07-06 17:58:35.000000 treGen-2.0.5/src/treeGen/cli.py
--rw-rw-rw-   0        0        0     2658 2023-07-06 16:58:32.000000 treGen-2.0.5/src/treeGen/treeGen.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:51:54.889444 treGen-2.0.5/treGen.egg-info/
--rw-rw-rw-   0        0        0     3410 2023-07-06 18:51:54.000000 treGen-2.0.5/treGen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-07-06 18:51:54.000000 treGen-2.0.5/treGen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 18:51:54.000000 treGen-2.0.5/treGen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 18:51:54.000000 treGen-2.0.5/treGen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 19:26:45.831757 treGen-2.1.0/
+-rw-rw-rw-   0        0        0      172 2023-07-06 18:04:58.000000 treGen-2.1.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1099 2023-07-06 16:52:25.000000 treGen-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-07-06 18:04:52.000000 treGen-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      591 2023-07-06 19:26:45.830845 treGen-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2093 2023-07-06 17:19:43.000000 treGen-2.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 19:26:45.832451 treGen-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      869 2023-07-06 19:26:43.000000 treGen-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 19:26:45.807473 treGen-2.1.0/src/
+-rw-rw-rw-   0        0        0      140 2023-07-06 19:24:39.000000 treGen-2.1.0/src/__main__.py
+-rw-rw-rw-   0        0        0      128 2023-07-06 17:56:41.000000 treGen-2.1.0/src/tree.py
+drwxrwxrwx   0        0        0        0 2023-07-06 19:26:45.815451 treGen-2.1.0/src/treeGen/
+-rw-rw-rw-   0        0        0       62 2023-07-06 19:18:21.000000 treGen-2.1.0/src/treeGen/__init__.py
+-rw-rw-rw-   0        0        0     1421 2023-07-06 17:58:35.000000 treGen-2.1.0/src/treeGen/cli.py
+-rw-rw-rw-   0        0        0     2658 2023-07-06 16:58:32.000000 treGen-2.1.0/src/treeGen/treeGen.py
+drwxrwxrwx   0        0        0        0 2023-07-06 19:26:45.828451 treGen-2.1.0/treGen.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-07-06 19:26:45.000000 treGen-2.1.0/treGen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-06 19:26:45.000000 treGen-2.1.0/treGen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 19:26:45.000000 treGen-2.1.0/treGen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-06 19:26:45.000000 treGen-2.1.0/treGen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 19:26:45.000000 treGen-2.1.0/treGen.egg-info/top_level.txt
```

### Comparing `treGen-2.0.5/LICENSE` & `treGen-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `treGen-2.0.5/README.md` & `treGen-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `treGen-2.0.5/setup.py` & `treGen-2.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,20 +6,24 @@
   "Operating System :: OS Independent",
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='treGen',
-  version='2.0.5',
+  version='2.1.0',
   description='A simple Directory Tree Generator',
   readme='README.MD',
-  long_description=open('README.MD').read(),
+  long_description='README.MD', #open('README.MD').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/JRS296/Directory-Tree',  
+  entry_points='''
+        [console_scripts]
+        treGen=src.__main__:main
+    ''',
   author='Jonathan Rufus Samuel',
   author_email='jrsstudios@skiff.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='tree-generator', 
   packages=find_packages(),
   install_requires=['']
```

### Comparing `treGen-2.0.5/src/treeGen/cli.py` & `treGen-2.1.0/src/treeGen/cli.py`

 * *Files identical despite different names*

### Comparing `treGen-2.0.5/src/treeGen/treeGen.py` & `treGen-2.1.0/src/treeGen/treeGen.py`

 * *Files identical despite different names*

