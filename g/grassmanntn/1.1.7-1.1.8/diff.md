# Comparing `tmp/grassmanntn-1.1.7.tar.gz` & `tmp/grassmanntn-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grassmanntn-1.1.7.tar", last modified: Thu Jul  6 08:32:28 2023, max compression
+gzip compressed data, was "grassmanntn-1.1.8.tar", last modified: Thu Jul  6 09:06:54 2023, max compression
```

## Comparing `grassmanntn-1.1.7.tar` & `grassmanntn-1.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 08:32:28.014474 grassmanntn-1.1.7/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.1.7/LICENSE.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-06 08:32:28.014474 grassmanntn-1.1.7/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.1.7/README.md
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 08:32:28.014474 grassmanntn-1.1.7/grassmanntn/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109907 2023-07-06 08:25:35.000000 grassmanntn-1.1.7/grassmanntn/__init__.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.1.7/grassmanntn/example.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132605 2023-07-05 06:56:28.000000 grassmanntn-1.1.7/grassmanntn/gauge2d.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.1.7/grassmanntn/param.py
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 08:32:28.014474 grassmanntn-1.1.7/grassmanntn.egg-info/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-06 08:32:27.000000 grassmanntn-1.1.7/grassmanntn.egg-info/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-06 08:32:27.000000 grassmanntn-1.1.7/grassmanntn.egg-info/SOURCES.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-06 08:32:27.000000 grassmanntn-1.1.7/grassmanntn.egg-info/dependency_links.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-06 08:32:27.000000 grassmanntn-1.1.7/grassmanntn.egg-info/requires.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-06 08:32:27.000000 grassmanntn-1.1.7/grassmanntn.egg-info/top_level.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-06 08:32:28.014474 grassmanntn-1.1.7/setup.cfg
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-06 08:32:13.000000 grassmanntn-1.1.7/setup.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 09:06:54.738019 grassmanntn-1.1.8/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.1.8/LICENSE.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-06 09:06:54.738019 grassmanntn-1.1.8/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.1.8/README.md
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 09:06:54.738019 grassmanntn-1.1.8/grassmanntn/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109895 2023-07-06 09:00:33.000000 grassmanntn-1.1.8/grassmanntn/__init__.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.1.8/grassmanntn/example.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132605 2023-07-06 08:59:36.000000 grassmanntn-1.1.8/grassmanntn/gauge2d.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.1.8/grassmanntn/param.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-06 09:06:54.738019 grassmanntn-1.1.8/grassmanntn.egg-info/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-06 09:06:54.000000 grassmanntn-1.1.8/grassmanntn.egg-info/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-06 09:06:54.000000 grassmanntn-1.1.8/grassmanntn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-06 09:06:54.000000 grassmanntn-1.1.8/grassmanntn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-06 09:06:54.000000 grassmanntn-1.1.8/grassmanntn.egg-info/requires.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-06 09:06:54.000000 grassmanntn-1.1.8/grassmanntn.egg-info/top_level.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-06 09:06:54.738019 grassmanntn-1.1.8/setup.cfg
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-06 09:06:20.000000 grassmanntn-1.1.8/setup.py
```

### Comparing `grassmanntn-1.1.7/LICENSE.txt` & `grassmanntn-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.7/PKG-INFO` & `grassmanntn-1.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.1.7
+Version: 1.1.8
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_117.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_118.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.1.7/README.md` & `grassmanntn-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.7/grassmanntn/__init__.py` & `grassmanntn-1.1.8/grassmanntn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import sys
 import gc
 import tracemalloc
 import os
 from datetime import datetime
 
 hybrid_symbol = "*"
-separator_list = ("|",":",";",",","."," ")
+separator_list = ("|",":",";",",",".")
 number_character = ("0","1","2","3","4","5","6","7","8","9")
 
 skip_parity_blocking_check = False
 skip_power_of_two_check = False
 allowed_stat = (0,1,-1,hybrid_symbol)
 fermi_type = (1,-1)
 bose_type = (0,hybrid_symbol)
@@ -1836,15 +1836,15 @@
 
     if this_format=='matrix':
         return Obj.switch_format(save_memory=True)
     
     if this_encoder == 'parity-preserving':
         #force convert to standard
         Obj = Obj.switch_encoder(save_memory=True)
-        
+
     return Obj
     
 def get_group_info(grouping_string, ungroup_stat, ungroup_shape):
     #print("original string:",grouping_string)
     formatted_string = grouping_string
     
     # check the string format --------------------------------------------------------
```

### Comparing `grassmanntn-1.1.7/grassmanntn/example.py` & `grassmanntn-1.1.8/grassmanntn/example.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.7/grassmanntn/gauge2d.py` & `grassmanntn-1.1.8/grassmanntn/gauge2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1020,74 +1020,74 @@
 
     # μ = 1 ===========================================================================
 
     step = 1
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Qp = gtn.einsum('IJKLijkl -> JKLijkl I',B)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    cQp = Qp.hconjugate("abcdefg x")
+    cQp = Qp.hconjugate("abcdefg|x")
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Mp = gtn.einsum('I abcdefg,abcdefg J -> IJ',cQp,Qp)
     
     del Qp, cQp
     gc.collect()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Qm = gtn.einsum('IJKLijkl -> K IJLijkl',B)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    cQm = Qm.hconjugate("x abcdefg")
+    cQm = Qm.hconjugate("x|abcdefg")
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Mm = gtn.einsum('I abcdefg,abcdefg J -> IJ',Qm,cQm)
 
     del Qm, cQm
     gc.collect()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    Up, Λp, cUp = Mp.eig("I J",cutoff)
-    Um, Λm, cUm = Mm.eig("I J",cutoff)
+    Up, Λp, cUp = Mp.eig("I|J",cutoff)
+    Um, Λm, cUm = Mm.eig("I|J",cutoff)
 
     if Λp.shape[0] < Λm.shape[0] :
         U1 = Up.copy()
         cU1 = cUp.copy()
     else:
         U1 = Um.copy()
         cU1 = cUm.copy()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     B = gtn.einsum('IA,IJKLijkl->AJKLijkl',U1,B)
-    B = gtn.einsum('CK,AJKLijkl->AJCLijkl',U1.hconjugate('I J'),B)
+    B = gtn.einsum('CK,AJKLijkl->AJCLijkl',U1.hconjugate('I|J'),B)
 
     if not mute:
         gtn.clear_progress()
         U1.info("U1")
 
     # μ = 2 ===========================================================================
     
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Qp = gtn.einsum('IJKLijkl -> IKLijkl J',B)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    cQp = Qp.hconjugate("abcdefg x")
+    cQp = Qp.hconjugate("abcdefg|x")
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Mp = gtn.einsum('I abcdefg,abcdefg J -> IJ',cQp,Qp)
     
     del Qp, cQp
     gc.collect()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Qm = gtn.einsum('IJKLijkl -> L IJKijkl',B)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    cQm = Qm.hconjugate("x abcdefg")
+    cQm = Qm.hconjugate("x|abcdefg")
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Mm = gtn.einsum('I abcdefg,abcdefg J -> IJ',Qm,cQm)
     del Qm, cQm
     gc.collect()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    Up, Λp, cUp = Mp.eig("I J",cutoff)
-    Um, Λm, cUm = Mm.eig("I J",cutoff)
+    Up, Λp, cUp = Mp.eig("I|J",cutoff)
+    Um, Λm, cUm = Mm.eig("I|J",cutoff)
 
     if Λp.shape[0] < Λm.shape[0] :
         U2 = Up.copy()
         cU2 = cUp.copy()
     else:
         U2 = Um.copy()
         cU2 = cUm.copy()
@@ -1122,34 +1122,34 @@
 
     # μ = 1 ===========================================================================
 
     step = 1
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Qp = gtn.einsum('IJKLijkl,km -> JKLjklm Ii',B,δ)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    cQp = Qp.hconjugate("JKLjklm Ii")
+    cQp = Qp.hconjugate("JKLjklm|Ii")
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Mp = gtn.einsum('Ii abcdefg,abcdefg Jj -> IiJj',cQp,Qp)
     
     del Qp, cQp
     gc.collect()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Qm = gtn.einsum('IJKLijkl,km -> Kk IJLijlm',B,δ)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    cQm = Qm.hconjugate("Kk IJLijlm")
+    cQm = Qm.hconjugate("Kk|IJLijlm")
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Mm = gtn.einsum('Ii abcdefg,abcdefg Jj -> IiJj',Qm,cQm)
 
     del Qm, cQm
     gc.collect()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    Up, Λp, cUp = Mp.eig("Ii Jj",cutoff)
-    Um, Λm, cUm = Mm.eig("Ii Jj",cutoff)
+    Up, Λp, cUp = Mp.eig("Ii|Jj",cutoff)
+    Um, Λm, cUm = Mm.eig("Ii|Jj",cutoff)
 
     if Λp.shape[0] < Λm.shape[0] :
         U1 = Up.copy()
     else:
         U1 = Um.copy()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
@@ -1161,34 +1161,34 @@
 
 
     # μ = 2 ===========================================================================
     
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Qp = gtn.einsum('IJKLijkl,lm -> IKLiklm Jj',B,δ)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    cQp = Qp.hconjugate("JKLjklm Ii")
+    cQp = Qp.hconjugate("JKLjklm|Ii")
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Mp = gtn.einsum('Ii abcdefg,abcdefg Jj -> IiJj',cQp,Qp)
     
     del Qp, cQp
     gc.collect()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Qm = gtn.einsum('IJKLijkl,lm -> Ll IJKijkm',B,δ)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    cQm = Qm.hconjugate("Kk IJLijlm")
+    cQm = Qm.hconjugate("Kk|IJLijlm")
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Mm = gtn.einsum('Ii abcdefg,abcdefg Jj -> IiJj',Qm,cQm)
 
     del Qm, cQm
     gc.collect()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    Up, Λp, cUp = Mp.eig("Ii Jj",cutoff)
-    Um, Λm, cUm = Mm.eig("Ii Jj",cutoff)
+    Up, Λp, cUp = Mp.eig("Ii|Jj",cutoff)
+    Um, Λm, cUm = Mm.eig("Ii|Jj",cutoff)
 
     if Λp.shape[0] < Λm.shape[0] :
         U2 = Up.copy()
     else:
         U2 = Um.copy()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
@@ -1199,81 +1199,81 @@
         U2.info("U2")
 
     # μ = 3 ===========================================================================
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Qp = gtn.einsum('IJKLijkl,im -> JKLjklm Ii',B,δ)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    cQp = Qp.hconjugate("JKLjklm Ii")
+    cQp = Qp.hconjugate("JKLjklm|Ii")
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Mp = gtn.einsum('Ii abcdefg,abcdefg Jj -> IiJj',cQp,Qp)
     
     del Qp, cQp
     gc.collect()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Qm = gtn.einsum('IJKLijkl,im -> Kk IJLijlm',B,δ)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    cQm = Qm.hconjugate("Kk IJLijlm")
+    cQm = Qm.hconjugate("Kk|IJLijlm")
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Mm = gtn.einsum('Ii abcdefg,abcdefg Jj -> IiJj',Qm,cQm)
 
     del Qm, cQm
     gc.collect()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    Up, Λp, cUp = Mp.eig("Ii Jj",cutoff)
-    Um, Λm, cUm = Mm.eig("Ii Jj",cutoff)
+    Up, Λp, cUp = Mp.eig("Ii|Jj",cutoff)
+    Um, Λm, cUm = Mm.eig("Ii|Jj",cutoff)
 
     if Λp.shape[0] < Λm.shape[0] :
         U3 = Up.copy()
     else:
         U3 = Um.copy()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    Bfin = gtn.einsum('ABKLkl,CKk->ABCLl',Bfin,U3.hconjugate('ij k'))
+    Bfin = gtn.einsum('ABKLkl,CKk->ABCLl',Bfin,U3.hconjugate('ij|k'))
     
     if not mute:
         gtn.clear_progress()
         U3.info("U3")
 
 
     # μ = 4 ===========================================================================
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Qp = gtn.einsum('IJKLijkl,jm -> IKLiklm Jj',B,δ)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    cQp = Qp.hconjugate("JKLjklm Ii")
+    cQp = Qp.hconjugate("JKLjklm|Ii")
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Mp = gtn.einsum('Ii abcdefg,abcdefg Jj -> IiJj',cQp,Qp)
     
     del Qp, cQp
     gc.collect()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Qm = gtn.einsum('IJKLijkl,jm -> Ll IJKijkm',B,δ)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    cQm = Qm.hconjugate("Kk IJLijlm")
+    cQm = Qm.hconjugate("Kk|IJLijlm")
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Mm = gtn.einsum('Ii abcdefg,abcdefg Jj -> IiJj',Qm,cQm)
 
     del Qm, cQm
     gc.collect()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    Up, Λp, cUp = Mp.eig("Ii Jj",cutoff)
-    Um, Λm, cUm = Mm.eig("Ii Jj",cutoff)
+    Up, Λp, cUp = Mp.eig("Ii|Jj",cutoff)
+    Um, Λm, cUm = Mm.eig("Ii|Jj",cutoff)
 
     if Λp.shape[0] < Λm.shape[0] :
         U4 = Up.copy()
     else:
         U4 = Um.copy()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    Bfin = gtn.einsum('ABCLl,DLl->ABCD',Bfin,U4.hconjugate('ij k'))
+    Bfin = gtn.einsum('ABCLl,DLl->ABCD',Bfin,U4.hconjugate('ij|k'))
     gtn.clear_progress()
     gtn.tab_up()
     
     if not mute:
         U1.info("U4")
         Bfin.info("B (compressed)")
 
@@ -1295,17 +1295,17 @@
     δ = gtn.sparse(δ,statistics=(0,0))
 
     if not mute:
         A.info("A (uncompressed)")
 
     step = 1
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    Ix = gtn.einsum('KXj,XjI->KIj',U1.hconjugate('ij k'),U3)
+    Ix = gtn.einsum('KXj,XjI->KIj',U1.hconjugate('ij|k'),U3)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    Iy = gtn.einsum('LYj,YjJ->LJj',U2.hconjugate('ij k'),U4)
+    Iy = gtn.einsum('LYj,YjJ->LJj',U2.hconjugate('ij|k'),U4)
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Afin = gtn.einsum('ijkl,KIl,LJk,km,ln->IJKLijklmn',A,Ix,Iy,δ,δ)
     gtn.clear_progress()
     gtn.tab_up()
 
     if not mute:
@@ -1325,74 +1325,74 @@
     step = 1
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Txp = gtn.einsum('IJKLijklmn -> JKLjklmn Ii',T)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Txm = gtn.einsum('IJKLijklmn -> Kk IJLijlmn',T)
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    cTxp = Txp.hconjugate('abcdefgh xy')
+    cTxp = Txp.hconjugate('abcdefgh|xy')
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    cTxm = Txm.hconjugate('xy abcdefgh')
+    cTxm = Txm.hconjugate('xy|abcdefgh')
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Mp = gtn.einsum('Ii abcdefgh, abcdefgh Jj -> IiJj',cTxp,Txp)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Mm = gtn.einsum('Ii abcdefgh, abcdefgh Jj -> IiJj',Txm,cTxm)
 
     del Txp, Txm, cTxp, cTxm
     gc.collect()
 
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    Up, Λp, cUp = Mp.eig("Ii Jj",cutoff)
-    Um, Λm, cUm = Mm.eig("Ii Jj",cutoff)
+    Up, Λp, cUp = Mp.eig("Ii|Jj",cutoff)
+    Um, Λm, cUm = Mm.eig("Ii|Jj",cutoff)
 
     if Λp.shape[0] < Λm.shape[0] :
         U = Up.copy()
     else:
         U = Um.copy()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
 
-    Tfin = gtn.einsum('IJKLijklmn,IiA,CKk->ACJLjlmn',T,U,U.hconjugate('ij k'))
+    Tfin = gtn.einsum('IJKLijklmn,IiA,CKk->ACJLjlmn',T,U,U.hconjugate('ij|k'))
 
     if not mute:
         Tfin.info("T (x-compression)")
 
     # y direction =====================================================================
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Typ = gtn.einsum('IKJLjlmn -> IKLlmn Jj',Tfin)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Tym = gtn.einsum('IKJLjlmn -> Ll IKJjmn',Tfin)
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    cTyp = Typ.hconjugate('abcdef xy')
+    cTyp = Typ.hconjugate('abcdef|xy')
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    cTym = Tym.hconjugate('xy abcdef')
+    cTym = Tym.hconjugate('xy|abcdef')
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Mp = gtn.einsum('Ii abcdef, abcdef Jj -> IiJj',cTyp,Typ)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Mm = gtn.einsum('Ii abcdef, abcdef Jj -> IiJj',Tym,cTym)
 
     del Typ, Tym, cTyp, cTym
     gc.collect()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    Up, Λp, cUp = Mp.eig("Ii Jj",cutoff)
-    Um, Λm, cUm = Mm.eig("Ii Jj",cutoff)
+    Up, Λp, cUp = Mp.eig("Ii|Jj",cutoff)
+    Um, Λm, cUm = Mm.eig("Ii|Jj",cutoff)
 
     if Λp.shape[0] < Λm.shape[0] :
         U = Up.copy()
     else:
         U = Um.copy()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
-    Tfin = gtn.einsum('ACJLjlmn,JjB,DLl->ABCDmn',Tfin,U,U.hconjugate('ij k'))
+    Tfin = gtn.einsum('ACJLjlmn,JjB,DLl->ABCDmn',Tfin,U,U.hconjugate('ij|k'))
     gtn.clear_progress()
     gtn.tab_up()
 
     if not mute:
         Tfin.info("T (y-compression)")
 
     return Tfin
@@ -1472,16 +1472,16 @@
     #===============================================================================#
     #   Step 1: Rearrange the tensor legs in two ways                               #
     #===============================================================================#
     
     T1 = gtn.einsum('ijkl->jkli',T)
     T2 = gtn.einsum('ijkl->klij',T)
 
-    U1,S1,V1 = T1.svd('ab cd',dcut)
-    U2,S2,V2 = T2.svd('ab cd',dcut)
+    U1,S1,V1 = T1.svd('ab|cd',dcut)
+    U2,S2,V2 = T2.svd('ab|cd',dcut)
 
     #
     #                             j                                     j
     #                             ↑                                     ↑
     #        j                    ↑                                     ↑
     #        ↑              k → →(U1)                                 (V2)→ → i
     #        ↑                      ↘                                 ↗
@@ -1562,16 +1562,16 @@
 
     if intermediate_dcut==None:
         intermediate_dcut=dcut
 
     T1 = gtn.einsum("ijkl->li jk",T1)
     T2 = gtn.einsum("ijkl->li jk",T2)
 
-    U1, S1, V1 = T1.svd("li jk",intermediate_dcut)
-    U2, S2, V2 = T2.svd("li jk",intermediate_dcut)
+    U1, S1, V1 = T1.svd("li|jk",intermediate_dcut)
+    U2, S2, V2 = T2.svd("li|jk",intermediate_dcut)
 
     #
     #        j                    j
     #        :                    :
     #        :                    :
     #  k --- X --- i        k --- V
     #        :                    :
@@ -1601,15 +1601,15 @@
     #  k --- M --- i        
     #        :                    
     #        :                    
     #        a                    
     #
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00)
-    U, S, V = M.svd("ai bk",intermediate_dcut)
+    U, S, V = M.svd("ai|bk",intermediate_dcut)
 
     sqrtS = gtn.sqrt(S)
     Y = gtn.einsum('abx,xc->abc',U,sqrtS)
     X = gtn.einsum('ax,xbc->abc',sqrtS,V)
 
     del U.data,S.data,V.data,sqrtS.data
     del U,S,V,sqrtS
@@ -1619,15 +1619,15 @@
     Q1 = gtn.einsum('iax,xbj->ijab',D,Y)
     Q2 = gtn.einsum('kya,ylb->abkl',X,A)
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00)
     Q = gtn.einsum('ijab,abkl->ijkl',Q1,Q2)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00)
     
-    U,S,V = Q.svd("ij kl",dcut)
+    U,S,V = Q.svd("ij|kl",dcut)
 
     sqrtS = gtn.sqrt(S)
     H = gtn.einsum('abx,xc->abc',U,sqrtS)
     G = gtn.einsum('ax,xbc->abc',sqrtS,V)
 
     del U.data,S.data,V.data,sqrtS.data
     del U,S,V,sqrtS
@@ -1783,15 +1783,15 @@
         Sx = S1.copy()
     else:
         Ux = U3.copy()
         Sx = S3.copy()
 
     if not svd_only :
         step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00) #20
-        cUx = Ux.hconjugate('ij a')
+        cUx = Ux.hconjugate('ij|a')
         #switch the i and j
         step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00)
         XX = gtn.einsum('i3 j3 ab i1 j1 -> j3 i3 ab i1 j1',XX)
         step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00)
         XX = gtn.einsum('j3 i3 ab i1 j1 -> j3 i3 ab j1 i1',XX)
 
         #=================================================================================================
@@ -1847,15 +1847,15 @@
     else:
         Uy = U4.copy()
         Sy = S4.copy()
 
 
     if not svd_only :
         step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00) #32
-        cUy = Uy.hconjugate('ij a')
+        cUy = Uy.hconjugate('ij|a')
 
         #switch the i and j
         step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00) #33
         YY = gtn.einsum('i4 j4 b a i2 j2 -> j4 i4 b a i2 j2',YY)
         step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00)
         YY = gtn.einsum('j4 i4 b a i2 j2 -> j4 i4 b a j2 i2',YY)
```

### Comparing `grassmanntn-1.1.7/grassmanntn/param.py` & `grassmanntn-1.1.8/grassmanntn/param.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.7/grassmanntn.egg-info/PKG-INFO` & `grassmanntn-1.1.8/grassmanntn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.1.7
+Version: 1.1.8
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_117.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_118.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.1.7/setup.py` & `grassmanntn-1.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'grassmanntn',         # How you named your package folder (MyLib)
   packages = ['grassmanntn'],   # Chose the same as "name"
-  version = '1.1.7',      # Start with a small number and increase it with every change you make
+  version = '1.1.8',      # Start with a small number and increase it with every change you make
   license='Apache',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'a Python library for Grassmann tensor network computation',   # Give a short description about your library
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Atis Yosprakob',                   # Type in your name
   author_email = 'yosprakob2@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/ayosprakob/grassmanntn',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_117.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_118.tar.gz',    # I explain this later on
   keywords = ['physics', 'lattice', 'gauge theory', 'tensor network', 'grassmann'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'sparse',
           'opt_einsum',
       ],
   classifiers=[
```

