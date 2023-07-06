# Comparing `tmp/grassmanntn-1.1.5.tar.gz` & `tmp/grassmanntn-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grassmanntn-1.1.5.tar", last modified: Wed Jul  5 09:18:35 2023, max compression
+gzip compressed data, was "grassmanntn-1.1.6.tar", last modified: Thu Jul  6 07:03:14 2023, max compression
```

## Comparing `grassmanntn-1.1.5.tar` & `grassmanntn-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-05 09:18:35.077997 grassmanntn-1.1.5/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.1.5/LICENSE.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-05 09:18:35.077997 grassmanntn-1.1.5/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.1.5/README.md
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-05 09:18:35.077997 grassmanntn-1.1.5/grassmanntn/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109541 2023-07-05 09:17:07.000000 grassmanntn-1.1.5/grassmanntn/__init__.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.1.5/grassmanntn/example.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132605 2023-07-05 06:56:28.000000 grassmanntn-1.1.5/grassmanntn/gauge2d.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.1.5/grassmanntn/param.py
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-05 09:18:35.077997 grassmanntn-1.1.5/grassmanntn.egg-info/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-05 09:18:35.000000 grassmanntn-1.1.5/grassmanntn.egg-info/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-05 09:18:35.000000 grassmanntn-1.1.5/grassmanntn.egg-info/SOURCES.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-05 09:18:35.000000 grassmanntn-1.1.5/grassmanntn.egg-info/dependency_links.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-05 09:18:35.000000 grassmanntn-1.1.5/grassmanntn.egg-info/requires.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-05 09:18:35.000000 grassmanntn-1.1.5/grassmanntn.egg-info/top_level.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-05 09:18:35.077997 grassmanntn-1.1.5/setup.cfg
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-05 09:18:09.000000 grassmanntn-1.1.5/setup.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 07:03:14.215202 grassmanntn-1.1.6/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.1.6/LICENSE.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-06 07:03:14.215202 grassmanntn-1.1.6/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.1.6/README.md
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 07:03:14.215202 grassmanntn-1.1.6/grassmanntn/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109679 2023-07-06 06:54:32.000000 grassmanntn-1.1.6/grassmanntn/__init__.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.1.6/grassmanntn/example.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132605 2023-07-05 06:56:28.000000 grassmanntn-1.1.6/grassmanntn/gauge2d.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.1.6/grassmanntn/param.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 07:03:14.215202 grassmanntn-1.1.6/grassmanntn.egg-info/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-06 07:03:14.000000 grassmanntn-1.1.6/grassmanntn.egg-info/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-06 07:03:14.000000 grassmanntn-1.1.6/grassmanntn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-06 07:03:14.000000 grassmanntn-1.1.6/grassmanntn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-06 07:03:14.000000 grassmanntn-1.1.6/grassmanntn.egg-info/requires.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-06 07:03:14.000000 grassmanntn-1.1.6/grassmanntn.egg-info/top_level.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-06 07:03:14.215202 grassmanntn-1.1.6/setup.cfg
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-06 07:03:04.000000 grassmanntn-1.1.6/setup.py
```

### Comparing `grassmanntn-1.1.5/LICENSE.txt` & `grassmanntn-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.5/PKG-INFO` & `grassmanntn-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.1.5
+Version: 1.1.6
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_115.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_116.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.1.5/README.md` & `grassmanntn-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.5/grassmanntn/__init__.py` & `grassmanntn-1.1.6/grassmanntn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -504,18 +504,18 @@
         if target not in format_type:
             error("Error[dense.force_format]: Unrecognized target format.")
         if target != self.format :
             return self.switch_format(save_memory=True)
         else :
             return self.copy()
 
-    def join_legs(self,string_inp,make_format='standard',intermediate_stat=(-1,1),save_memory=False):
+    def join_legs(self,string_inp,make_format='standard',intermediate_stat=None,save_memory=False):
         return join_legs(self,string_inp,make_format,intermediate_stat,save_memory)
 
-    def split_legs(self,string_inp,final_stat,final_shape,intermediate_stat=(-1,1),save_memory=False):
+    def split_legs(self,string_inp,final_stat,final_shape,intermediate_stat=None,save_memory=False):
         return split_legs(self,string_inp,final_stat,final_shape,intermediate_stat,save_memory)
 
     def hconjugate(self,input_string,save_memory=False):
         return hconjugate(self,input_string,save_memory)
 
     def svd(self,string_inp,cutoff=None,save_memory=False):
         return svd(self,string_inp,cutoff,save_memory)
@@ -761,18 +761,18 @@
         if target not in format_type:
             error("Error[sparse.force_format]: Unrecognized target format.")
         if target != self.format :
             return self.switch_format()
         else :
             return self.copy()
 
-    def join_legs(self,string_inp,make_format='standard',intermediate_stat=(-1,1),save_memory=False):
+    def join_legs(self,string_inp,make_format='standard',intermediate_stat=None,save_memory=False):
         return join_legs(self,string_inp,make_format,intermediate_stat,save_memory)
 
-    def split_legs(self,string_inp,final_stat,final_shape,intermediate_stat=(-1,1),save_memory=False):
+    def split_legs(self,string_inp,final_stat,final_shape,intermediate_stat=None,save_memory=False):
         return split_legs(self,string_inp,final_stat,final_shape,intermediate_stat,save_memory)
 
     def hconjugate(self,input_string,save_memory=False):
         return hconjugate(self,input_string,save_memory)
 
     def svd(self,string_inp,cutoff=None,save_memory=False):
         return svd(self,string_inp,cutoff,save_memory)
@@ -1628,15 +1628,15 @@
         else:
             return np.array(ret).flatten()[0]
 
 ####################################################
 ##                     Reshape                    ##
 ####################################################
 
-def join_legs(InpObj,string_inp,make_format='standard',intermediate_stat=(-1,1),save_memory=False):
+def join_legs(InpObj,string_inp,make_format='standard',intermediate_stat=None,save_memory=False):
 
     process_name = "join_legs"
     process_length = 6
     process_color="green"
     step = 1
     s00 = time.time()
     progress_space() # << Don't remove this. This is for the show_progress!
@@ -1738,15 +1738,15 @@
     Obj.statistics = final_stats
     
     clear_progress()
     tab_up()
 
     return Obj
     
-def split_legs(InpObj,string_inp,final_stat,final_shape,intermediate_stat=(-1,1),save_memory=False):
+def split_legs(InpObj,string_inp,final_stat,final_shape,intermediate_stat=None,save_memory=False):
 
     process_name = "split_legs"
     process_length = 6
     process_color="green"
     step = 1
     s00 = time.time()
     progress_space() # << Don't remove this. This is for the show_progress!
@@ -2345,17 +2345,17 @@
     Vind   = new_ind1 + "("+Vind+")"
     Ustats = tuple(Ustats + [-Λstatleft])
     Vstats = tuple([-Λstatright] + Vstats)
     Ushape = tuple(Ushape + [dΛ])
     Vshape = tuple([dΛ] + Vshape)
     
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00) #6
-    U = U.split_legs(Uind,Ustats,Ushape,save_memory=True)
+    U = U.split_legs(Uind,Ustats,Ushape,intermediate_stat=(-1,1),save_memory=True)
     Λ = Λ.switch_encoder(save_memory=True)
-    V = V.split_legs(Vind,Vstats,Vshape,save_memory=True)
+    V = V.split_legs(Vind,Vstats,Vshape,intermediate_stat=(-1,1),save_memory=True)
     
     if(this_format == 'standard'):
         U = U.switch_format(save_memory=True)
         Λ = Λ.switch_format(save_memory=True)
         V = V.switch_format(save_memory=True)
 
     if(this_encoder == 'parity-preserving'):
@@ -2688,17 +2688,17 @@
     Vind   = new_ind1 + "("+Vind+")"
     Ustats = tuple(Ustats + [-Λstatleft])
     Vstats = tuple([-Λstatright] + Vstats)
     Ushape = tuple(Ushape + [dΛ])
     Vshape = tuple([dΛ] + Vshape)
     
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00) #6
-    U = U.split_legs(Uind,Ustats,Ushape,save_memory=True)
+    U = U.split_legs(Uind,Ustats,Ushape,intermediate_stat=(-1,1),save_memory=True)
     Λ = Λ.switch_encoder(save_memory=True)
-    V = V.split_legs(Vind,Vstats,Vshape,save_memory=True)
+    V = V.split_legs(Vind,Vstats,Vshape,intermediate_stat=(-1,1),save_memory=True)
     
     if(this_format == 'standard'):
         U = U.switch_format(save_memory=True)
         Λ = Λ.switch_format(save_memory=True)
         V = V.switch_format(save_memory=True)
 
     if(this_encoder == 'parity-preserving'):
@@ -2834,15 +2834,15 @@
             if prefer != None:
                 return prefer
             else:
                 return 0
         elif(boson_count>0 and fermi_count>0):
             return hybrid_symbol
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00)
-    Obj = Obj.join_legs(join_legs_string_input,"matrix",save_memory=True)
+    Obj = Obj.join_legs(join_legs_string_input,"matrix",intermediate_stat=(-1,1),save_memory=True)
     
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00)
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
     #:::::      STEP 2 - Perform Hermitian Conjugation                                          :::::
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
 
     Obj.data = np.conjugate(oe.contract('ij->ji',Obj.data))
@@ -2894,15 +2894,15 @@
     new_stats = Vstats + Ustats
     new_shape = make_tuple(Vshape + Ushape)
     for i in range(len(new_stats)):
         if new_stats[i] in fermi_type :
             new_stats[i]*=-1
     new_stats = make_tuple(new_stats)
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00)
-    Obj = Obj.split_legs(new_ind,new_stats,new_shape,save_memory=True)
+    Obj = Obj.split_legs(new_ind,new_stats,new_shape,intermediate_stat=(-1,1),save_memory=True)
     
     #if this_type==sparse :
     #    Obj = sparse(Obj)
     if this_format!=Obj.format :
         Obj = Obj.switch_format(save_memory=True)
     if this_encoder!=Obj.encoder :
         Obj = Obj.switch_encoder(save_memory=True)
```

### Comparing `grassmanntn-1.1.5/grassmanntn/example.py` & `grassmanntn-1.1.6/grassmanntn/example.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.5/grassmanntn/gauge2d.py` & `grassmanntn-1.1.6/grassmanntn/gauge2d.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.5/grassmanntn/param.py` & `grassmanntn-1.1.6/grassmanntn/param.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.5/grassmanntn.egg-info/PKG-INFO` & `grassmanntn-1.1.6/grassmanntn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.1.5
+Version: 1.1.6
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_115.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_116.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.1.5/setup.py` & `grassmanntn-1.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'grassmanntn',         # How you named your package folder (MyLib)
   packages = ['grassmanntn'],   # Chose the same as "name"
-  version = '1.1.5',      # Start with a small number and increase it with every change you make
+  version = '1.1.6',      # Start with a small number and increase it with every change you make
   license='Apache',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'a Python library for Grassmann tensor network computation',   # Give a short description about your library
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Atis Yosprakob',                   # Type in your name
   author_email = 'yosprakob2@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/ayosprakob/grassmanntn',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_115.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_116.tar.gz',    # I explain this later on
   keywords = ['physics', 'lattice', 'gauge theory', 'tensor network', 'grassmann'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'sparse',
           'opt_einsum',
       ],
   classifiers=[
```

