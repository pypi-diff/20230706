# Comparing `tmp/datawhispers-0.2.8.7.tar.gz` & `tmp/datawhispers-0.2.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawhispers-0.2.8.7.tar", last modified: Thu Jul  6 08:40:24 2023, max compression
+gzip compressed data, was "datawhispers-0.2.8.8.tar", last modified: Thu Jul  6 08:53:23 2023, max compression
```

## Comparing `datawhispers-0.2.8.7.tar` & `datawhispers-0.2.8.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-06 08:40:24.080672 datawhispers-0.2.8.7/
--rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.8.7/LICENSE
--rw-r--r--   0 german     (501) staff       (20)     2340 2023-07-06 08:40:24.080537 datawhispers-0.2.8.7/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)     1218 2023-07-05 20:19:46.000000 datawhispers-0.2.8.7/README.md
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-06 08:40:24.079685 datawhispers-0.2.8.7/datawhispers/
--rw-r--r--   0 german     (501) staff       (20)      111 2023-07-03 08:22:12.000000 datawhispers-0.2.8.7/datawhispers/__init__.py
--rw-r--r--   0 german     (501) staff       (20)    11593 2023-07-05 19:23:07.000000 datawhispers-0.2.8.7/datawhispers/advancedProg.py
--rw-r--r--   0 german     (501) staff       (20)    17824 2023-07-05 13:05:34.000000 datawhispers-0.2.8.7/datawhispers/datavis.py
--rw-r--r--   0 german     (501) staff       (20)        0 2023-07-03 08:22:31.000000 datawhispers-0.2.8.7/datawhispers/mathFuncs.py
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-06 08:40:24.080291 datawhispers-0.2.8.7/datawhispers.egg-info/
--rw-r--r--   0 german     (501) staff       (20)     2340 2023-07-06 08:40:24.000000 datawhispers-0.2.8.7/datawhispers.egg-info/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      309 2023-07-06 08:40:24.000000 datawhispers-0.2.8.7/datawhispers.egg-info/SOURCES.txt
--rw-r--r--   0 german     (501) staff       (20)        1 2023-07-06 08:40:24.000000 datawhispers-0.2.8.7/datawhispers.egg-info/dependency_links.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-06 08:40:24.000000 datawhispers-0.2.8.7/datawhispers.egg-info/requires.txt
--rw-r--r--   0 german     (501) staff       (20)       13 2023-07-06 08:40:24.000000 datawhispers-0.2.8.7/datawhispers.egg-info/top_level.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-06 08:40:24.080724 datawhispers-0.2.8.7/setup.cfg
--rw-r--r--   0 german     (501) staff       (20)     2297 2023-07-06 08:40:12.000000 datawhispers-0.2.8.7/setup.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-06 08:53:23.592875 datawhispers-0.2.8.8/
+-rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.8.8/LICENSE
+-rw-r--r--   0 german     (501) staff       (20)     2340 2023-07-06 08:53:23.592761 datawhispers-0.2.8.8/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)     1218 2023-07-05 20:19:46.000000 datawhispers-0.2.8.8/README.md
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-06 08:53:23.591924 datawhispers-0.2.8.8/datawhispers/
+-rw-r--r--   0 german     (501) staff       (20)      111 2023-07-03 08:22:12.000000 datawhispers-0.2.8.8/datawhispers/__init__.py
+-rw-r--r--   0 german     (501) staff       (20)    11593 2023-07-05 19:23:07.000000 datawhispers-0.2.8.8/datawhispers/advancedProg.py
+-rw-r--r--   0 german     (501) staff       (20)    17824 2023-07-05 13:05:34.000000 datawhispers-0.2.8.8/datawhispers/datavis.py
+-rw-r--r--   0 german     (501) staff       (20)        0 2023-07-03 08:22:31.000000 datawhispers-0.2.8.8/datawhispers/mathFuncs.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-06 08:53:23.592546 datawhispers-0.2.8.8/datawhispers.egg-info/
+-rw-r--r--   0 german     (501) staff       (20)     2340 2023-07-06 08:53:23.000000 datawhispers-0.2.8.8/datawhispers.egg-info/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)      309 2023-07-06 08:53:23.000000 datawhispers-0.2.8.8/datawhispers.egg-info/SOURCES.txt
+-rw-r--r--   0 german     (501) staff       (20)        1 2023-07-06 08:53:23.000000 datawhispers-0.2.8.8/datawhispers.egg-info/dependency_links.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-06 08:53:23.000000 datawhispers-0.2.8.8/datawhispers.egg-info/requires.txt
+-rw-r--r--   0 german     (501) staff       (20)       13 2023-07-06 08:53:23.000000 datawhispers-0.2.8.8/datawhispers.egg-info/top_level.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-06 08:53:23.592917 datawhispers-0.2.8.8/setup.cfg
+-rw-r--r--   0 german     (501) staff       (20)     2297 2023-07-06 08:53:11.000000 datawhispers-0.2.8.8/setup.py
```

### Comparing `datawhispers-0.2.8.7/LICENSE` & `datawhispers-0.2.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.8.7/PKG-INFO` & `datawhispers-0.2.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.8.7
+Version: 0.2.8.8
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
```

### Comparing `datawhispers-0.2.8.7/README.md` & `datawhispers-0.2.8.8/README.md`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.8.7/datawhispers/advancedProg.py` & `datawhispers-0.2.8.8/datawhispers/advancedProg.py`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.8.7/datawhispers/datavis.py` & `datawhispers-0.2.8.8/datawhispers/datavis.py`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.8.7/datawhispers.egg-info/PKG-INFO` & `datawhispers-0.2.8.8/datawhispers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.8.7
+Version: 0.2.8.8
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
```

### Comparing `datawhispers-0.2.8.7/setup.py` & `datawhispers-0.2.8.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'datawhispers',         # How you named your package folder (MyLib)
   packages = ["datawhispers"],   # Chose the same as "name"
-  version = "0.2.8.7",      # Start with a small number and increase it with every change you make
+  version = "0.2.8.8",      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation',   # Give a short description about your library
   author = 'German Paul',                   # Type in your name
   author_email = 'motets-rosiest-0r@icloud.com',      # Type in your E-Mail
   url = 'https://github.com/GermanPaul12/datawhispers',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Python3', 'Data Visualisation', 'Statistical Analysis', "Regression", "Advanced Programming"],   # Keywords that define your package best
```

