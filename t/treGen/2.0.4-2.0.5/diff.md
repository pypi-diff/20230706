# Comparing `tmp/treGen-2.0.4.tar.gz` & `tmp/treGen-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treGen-2.0.4.tar", last modified: Thu Jul  6 18:50:22 2023, max compression
+gzip compressed data, was "treGen-2.0.5.tar", last modified: Thu Jul  6 18:51:54 2023, max compression
```

## Comparing `treGen-2.0.4.tar` & `treGen-2.0.5.tar`

### file list

```diff
@@ -1,23 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 18:50:22.485192 treGen-2.0.4/
--rw-rw-rw-   0        0        0      172 2023-07-06 18:04:58.000000 treGen-2.0.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1099 2023-07-06 16:52:25.000000 treGen-2.0.4/LICENSE
--rw-rw-rw-   0        0        0       25 2023-07-06 18:04:52.000000 treGen-2.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      591 2023-07-06 18:50:22.484190 treGen-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2093 2023-07-06 17:19:43.000000 treGen-2.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 18:50:22.486188 treGen-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0      757 2023-07-06 18:50:19.000000 treGen-2.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:50:22.458190 treGen-2.0.4/src/
--rw-rw-rw-   0        0        0      128 2023-07-06 17:56:41.000000 treGen-2.0.4/src/tree.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:50:22.465192 treGen-2.0.4/src/treeGen/
--rw-rw-rw-   0        0        0      129 2023-07-06 18:27:50.000000 treGen-2.0.4/src/treeGen/__init__.py
--rw-rw-rw-   0        0        0     1421 2023-07-06 17:58:35.000000 treGen-2.0.4/src/treeGen/cli.py
--rw-rw-rw-   0        0        0     2658 2023-07-06 16:58:32.000000 treGen-2.0.4/src/treeGen/treeGen.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:50:22.473198 treGen-2.0.4/treGen.egg-info/
--rw-rw-rw-   0        0        0      591 2023-07-06 18:50:22.000000 treGen-2.0.4/treGen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-07-06 18:50:22.000000 treGen-2.0.4/treGen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 18:50:22.000000 treGen-2.0.4/treGen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 18:50:22.000000 treGen-2.0.4/treGen.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-06 18:50:22.482191 treGen-2.0.4/treeGen.egg-info/
--rw-rw-rw-   0        0        0      255 2023-07-06 18:30:12.000000 treGen-2.0.4/treeGen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 18:30:12.000000 treGen-2.0.4/treeGen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 18:30:12.000000 treGen-2.0.4/treeGen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 18:51:54.893319 treGen-2.0.5/
+-rw-rw-rw-   0        0        0      172 2023-07-06 18:04:58.000000 treGen-2.0.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1099 2023-07-06 16:52:25.000000 treGen-2.0.5/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-07-06 18:04:52.000000 treGen-2.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3410 2023-07-06 18:51:54.891312 treGen-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2093 2023-07-06 17:19:43.000000 treGen-2.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 18:51:54.893319 treGen-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-07-06 18:51:51.000000 treGen-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:51:54.871309 treGen-2.0.5/src/
+-rw-rw-rw-   0        0        0      128 2023-07-06 17:56:41.000000 treGen-2.0.5/src/tree.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:51:54.882328 treGen-2.0.5/src/treeGen/
+-rw-rw-rw-   0        0        0      129 2023-07-06 18:27:50.000000 treGen-2.0.5/src/treeGen/__init__.py
+-rw-rw-rw-   0        0        0     1421 2023-07-06 17:58:35.000000 treGen-2.0.5/src/treeGen/cli.py
+-rw-rw-rw-   0        0        0     2658 2023-07-06 16:58:32.000000 treGen-2.0.5/src/treeGen/treeGen.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:51:54.889444 treGen-2.0.5/treGen.egg-info/
+-rw-rw-rw-   0        0        0     3410 2023-07-06 18:51:54.000000 treGen-2.0.5/treGen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-07-06 18:51:54.000000 treGen-2.0.5/treGen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 18:51:54.000000 treGen-2.0.5/treGen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 18:51:54.000000 treGen-2.0.5/treGen.egg-info/top_level.txt
```

### Comparing `treGen-2.0.4/LICENSE` & `treGen-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `treGen-2.0.4/PKG-INFO` & `treGen-2.0.5/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,26 @@
-Metadata-Version: 2.1
-Name: treGen
-Version: 2.0.4
-Summary: A simple Directory Tree Generator
-Home-page: https://github.com/JRS296/Directory-Tree
-Author: Jonathan Rufus Samuel
-Author-email: jrsstudios@skiff.com
-License: MIT
-Description: README.MD
-Keywords: tree-generator
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Education
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
+from setuptools import setup, find_packages
+ 
+classifiers = [
+  'Development Status :: 5 - Production/Stable',
+  'Intended Audience :: Education',
+  "Operating System :: OS Independent",
+  'License :: OSI Approved :: MIT License',
+  'Programming Language :: Python :: 3'
+]
+ 
+setup(
+  name='treGen',
+  version='2.0.5',
+  description='A simple Directory Tree Generator',
+  readme='README.MD',
+  long_description=open('README.MD').read(),
+  long_description_content_type='text/markdown',
+  url='https://github.com/JRS296/Directory-Tree',  
+  author='Jonathan Rufus Samuel',
+  author_email='jrsstudios@skiff.com',
+  license='MIT', 
+  classifiers=classifiers,
+  keywords='tree-generator', 
+  packages=find_packages(),
+  install_requires=[''] 
+)
```

### Comparing `treGen-2.0.4/README.md` & `treGen-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `treGen-2.0.4/src/treeGen/cli.py` & `treGen-2.0.5/src/treeGen/cli.py`

 * *Files identical despite different names*

### Comparing `treGen-2.0.4/src/treeGen/treeGen.py` & `treGen-2.0.5/src/treeGen/treeGen.py`

 * *Files identical despite different names*

