# Comparing `tmp/grassmanntn-1.1.8.tar.gz` & `tmp/grassmanntn-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grassmanntn-1.1.8.tar", last modified: Thu Jul  6 09:06:54 2023, max compression
+gzip compressed data, was "grassmanntn-1.1.9.tar", last modified: Thu Jul  6 09:28:13 2023, max compression
```

## Comparing `grassmanntn-1.1.8.tar` & `grassmanntn-1.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 09:06:54.738019 grassmanntn-1.1.8/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.1.8/LICENSE.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-06 09:06:54.738019 grassmanntn-1.1.8/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.1.8/README.md
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 09:06:54.738019 grassmanntn-1.1.8/grassmanntn/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109895 2023-07-06 09:00:33.000000 grassmanntn-1.1.8/grassmanntn/__init__.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.1.8/grassmanntn/example.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132605 2023-07-06 08:59:36.000000 grassmanntn-1.1.8/grassmanntn/gauge2d.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.1.8/grassmanntn/param.py
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 09:06:54.738019 grassmanntn-1.1.8/grassmanntn.egg-info/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-06 09:06:54.000000 grassmanntn-1.1.8/grassmanntn.egg-info/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-06 09:06:54.000000 grassmanntn-1.1.8/grassmanntn.egg-info/SOURCES.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-06 09:06:54.000000 grassmanntn-1.1.8/grassmanntn.egg-info/dependency_links.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-06 09:06:54.000000 grassmanntn-1.1.8/grassmanntn.egg-info/requires.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-06 09:06:54.000000 grassmanntn-1.1.8/grassmanntn.egg-info/top_level.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-06 09:06:54.738019 grassmanntn-1.1.8/setup.cfg
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-06 09:06:20.000000 grassmanntn-1.1.8/setup.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 09:28:13.364647 grassmanntn-1.1.9/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.1.9/LICENSE.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-06 09:28:13.364647 grassmanntn-1.1.9/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.1.9/README.md
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 09:28:13.364647 grassmanntn-1.1.9/grassmanntn/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109895 2023-07-06 09:24:54.000000 grassmanntn-1.1.9/grassmanntn/__init__.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.1.9/grassmanntn/example.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132605 2023-07-06 08:59:36.000000 grassmanntn-1.1.9/grassmanntn/gauge2d.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.1.9/grassmanntn/param.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 09:28:13.364647 grassmanntn-1.1.9/grassmanntn.egg-info/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-06 09:28:13.000000 grassmanntn-1.1.9/grassmanntn.egg-info/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-06 09:28:13.000000 grassmanntn-1.1.9/grassmanntn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-06 09:28:13.000000 grassmanntn-1.1.9/grassmanntn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-06 09:28:13.000000 grassmanntn-1.1.9/grassmanntn.egg-info/requires.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-06 09:28:13.000000 grassmanntn-1.1.9/grassmanntn.egg-info/top_level.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-06 09:28:13.364647 grassmanntn-1.1.9/setup.cfg
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-06 09:27:31.000000 grassmanntn-1.1.9/setup.py
```

### Comparing `grassmanntn-1.1.8/LICENSE.txt` & `grassmanntn-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.8/PKG-INFO` & `grassmanntn-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.1.8
+Version: 1.1.9
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_118.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_119.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.1.8/README.md` & `grassmanntn-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.8/grassmanntn/__init__.py` & `grassmanntn-1.1.9/grassmanntn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2184,15 +2184,15 @@
     # check if Obj.statistics or final_statistics is weird or not
     for stat in Obj.statistics:
         if(stat not in allowed_stat):
             error("Error[svd]: The input object contains illegal statistics. (0, 1, -1, or "+hybrid_symbol+" only)")
 
     if string.count("(")==string.count(")") and string.count("(")>0:
         string = string.replace(" ","")
-        string = string.replace(")("," ")
+        string = string.replace(")(","|")
         if string.count("(")>1 or string.count(")")<1:
             error("Error[svd]: Parentheses don't match")
         string = string.replace(")","")
         string = string.replace("(","")
 
     partition_count = 0
     for partition in separator_list:
@@ -2528,15 +2528,15 @@
     # check if Obj.statistics or final_statistics is weird or not
     for stat in Obj.statistics:
         if(stat not in allowed_stat):
             error("Error[eig]: The input object contains illegal statistics. (0, 1, -1, or "+hybrid_symbol+" only)")
 
     if string.count("(")==string.count(")") and string.count("(")>0:
         string = string.replace(" ","")
-        string = string.replace(")("," ")
+        string = string.replace(")(","|")
         if string.count("(")>1 or string.count(")")<1:
             error("Error[eig]: Parentheses don't match")
         string = string.replace(")","")
         string = string.replace("(","")
 
     partition_count = 0
     for partition in separator_list:
@@ -2735,15 +2735,15 @@
     s00 = time.time()
     progress_space() # << Don't remove this. This is for the show_progress!
 
     string = denumerate(string)
     
     if string.count("(")==string.count(")") and string.count("(")>0:
         string = string.replace(" ","")
-        string = string.replace(")("," ")
+        string = string.replace(")(","|")
         if string.count("(")>1 or string.count(")")<1:
             error("Error[hconjugate]: Parentheses don't match")
         string = string.replace(")","")
         string = string.replace("(","")
 
 
     # the string is of the form aaaa|bbb
```

### Comparing `grassmanntn-1.1.8/grassmanntn/example.py` & `grassmanntn-1.1.9/grassmanntn/example.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.8/grassmanntn/gauge2d.py` & `grassmanntn-1.1.9/grassmanntn/gauge2d.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.8/grassmanntn/param.py` & `grassmanntn-1.1.9/grassmanntn/param.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.8/grassmanntn.egg-info/PKG-INFO` & `grassmanntn-1.1.9/grassmanntn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.1.8
+Version: 1.1.9
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_118.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_119.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.1.8/setup.py` & `grassmanntn-1.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'grassmanntn',         # How you named your package folder (MyLib)
   packages = ['grassmanntn'],   # Chose the same as "name"
-  version = '1.1.8',      # Start with a small number and increase it with every change you make
+  version = '1.1.9',      # Start with a small number and increase it with every change you make
   license='Apache',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'a Python library for Grassmann tensor network computation',   # Give a short description about your library
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Atis Yosprakob',                   # Type in your name
   author_email = 'yosprakob2@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/ayosprakob/grassmanntn',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_118.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_119.tar.gz',    # I explain this later on
   keywords = ['physics', 'lattice', 'gauge theory', 'tensor network', 'grassmann'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'sparse',
           'opt_einsum',
       ],
   classifiers=[
```

