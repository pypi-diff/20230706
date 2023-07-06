# Comparing `tmp/grassmanntn-1.1.6.tar.gz` & `tmp/grassmanntn-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grassmanntn-1.1.6.tar", last modified: Thu Jul  6 07:03:14 2023, max compression
+gzip compressed data, was "grassmanntn-1.1.7.tar", last modified: Thu Jul  6 08:32:28 2023, max compression
```

## Comparing `grassmanntn-1.1.6.tar` & `grassmanntn-1.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 07:03:14.215202 grassmanntn-1.1.6/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.1.6/LICENSE.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-06 07:03:14.215202 grassmanntn-1.1.6/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.1.6/README.md
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 07:03:14.215202 grassmanntn-1.1.6/grassmanntn/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109679 2023-07-06 06:54:32.000000 grassmanntn-1.1.6/grassmanntn/__init__.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.1.6/grassmanntn/example.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132605 2023-07-05 06:56:28.000000 grassmanntn-1.1.6/grassmanntn/gauge2d.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.1.6/grassmanntn/param.py
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 07:03:14.215202 grassmanntn-1.1.6/grassmanntn.egg-info/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-06 07:03:14.000000 grassmanntn-1.1.6/grassmanntn.egg-info/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-06 07:03:14.000000 grassmanntn-1.1.6/grassmanntn.egg-info/SOURCES.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-06 07:03:14.000000 grassmanntn-1.1.6/grassmanntn.egg-info/dependency_links.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-06 07:03:14.000000 grassmanntn-1.1.6/grassmanntn.egg-info/requires.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-06 07:03:14.000000 grassmanntn-1.1.6/grassmanntn.egg-info/top_level.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-06 07:03:14.215202 grassmanntn-1.1.6/setup.cfg
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-06 07:03:04.000000 grassmanntn-1.1.6/setup.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 08:32:28.014474 grassmanntn-1.1.7/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.1.7/LICENSE.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-06 08:32:28.014474 grassmanntn-1.1.7/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.1.7/README.md
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 08:32:28.014474 grassmanntn-1.1.7/grassmanntn/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109907 2023-07-06 08:25:35.000000 grassmanntn-1.1.7/grassmanntn/__init__.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.1.7/grassmanntn/example.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132605 2023-07-05 06:56:28.000000 grassmanntn-1.1.7/grassmanntn/gauge2d.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.1.7/grassmanntn/param.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 08:32:28.014474 grassmanntn-1.1.7/grassmanntn.egg-info/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-06 08:32:27.000000 grassmanntn-1.1.7/grassmanntn.egg-info/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-06 08:32:27.000000 grassmanntn-1.1.7/grassmanntn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-06 08:32:27.000000 grassmanntn-1.1.7/grassmanntn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-06 08:32:27.000000 grassmanntn-1.1.7/grassmanntn.egg-info/requires.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-06 08:32:27.000000 grassmanntn-1.1.7/grassmanntn.egg-info/top_level.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-06 08:32:28.014474 grassmanntn-1.1.7/setup.cfg
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-06 08:32:13.000000 grassmanntn-1.1.7/setup.py
```

### Comparing `grassmanntn-1.1.6/LICENSE.txt` & `grassmanntn-1.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.6/PKG-INFO` & `grassmanntn-1.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.1.6
+Version: 1.1.7
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_116.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_117.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.1.6/README.md` & `grassmanntn-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.6/grassmanntn/__init__.py` & `grassmanntn-1.1.7/grassmanntn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1787,15 +1787,17 @@
     Obj.statistics = new_stats
     
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00)
     #===============================================================================#
     #   Step 4: Switch encoder                                                      #
     #===============================================================================#
     
-    Obj = Obj.switch_encoder(save_memory=True)
+    if this_encoder == 'parity-preserving':
+        #force convert to standard
+        Obj = Obj.switch_encoder(save_memory=True)
     
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00)
     #===============================================================================#
     #   Step 3: Switch format if this_format='matrix'                               #
     #===============================================================================#
     
     if this_format == 'matrix':
@@ -1831,14 +1833,18 @@
     
     clear_progress()
     tab_up()
 
     if this_format=='matrix':
         return Obj.switch_format(save_memory=True)
     
+    if this_encoder == 'parity-preserving':
+        #force convert to standard
+        Obj = Obj.switch_encoder(save_memory=True)
+        
     return Obj
     
 def get_group_info(grouping_string, ungroup_stat, ungroup_shape):
     #print("original string:",grouping_string)
     formatted_string = grouping_string
     
     # check the string format --------------------------------------------------------
```

### Comparing `grassmanntn-1.1.6/grassmanntn/example.py` & `grassmanntn-1.1.7/grassmanntn/example.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.6/grassmanntn/gauge2d.py` & `grassmanntn-1.1.7/grassmanntn/gauge2d.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.6/grassmanntn/param.py` & `grassmanntn-1.1.7/grassmanntn/param.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.6/grassmanntn.egg-info/PKG-INFO` & `grassmanntn-1.1.7/grassmanntn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.1.6
+Version: 1.1.7
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_116.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_117.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.1.6/setup.py` & `grassmanntn-1.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'grassmanntn',         # How you named your package folder (MyLib)
   packages = ['grassmanntn'],   # Chose the same as "name"
-  version = '1.1.6',      # Start with a small number and increase it with every change you make
+  version = '1.1.7',      # Start with a small number and increase it with every change you make
   license='Apache',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'a Python library for Grassmann tensor network computation',   # Give a short description about your library
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Atis Yosprakob',                   # Type in your name
   author_email = 'yosprakob2@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/ayosprakob/grassmanntn',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_116.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_117.tar.gz',    # I explain this later on
   keywords = ['physics', 'lattice', 'gauge theory', 'tensor network', 'grassmann'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'sparse',
           'opt_einsum',
       ],
   classifiers=[
```

